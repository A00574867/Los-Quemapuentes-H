# Código fuente del robot

**M01 Mini-sumo autónomo:** `codigo/mini-sumo/` con `main.ino`, `sensors.*`, `motors.*`, `strategy.*`, documentación de pinout.

```text
codigo/mini-sumo/
├── main.ino          # Setup general, retardo de 5 s y bucle principal (loop)
├── sensors.h         # Definición de pines y umbrales de sensores
├── sensors.cpp       # Lectura de QTR-1A (línea) y JS40F (oponente)
├── motors.h          # Prototipos de control de tracción y constantes PWM
├── motors.cpp        # Funciones de movimiento (setMotores, parar)
├── strategy.h        # Declaración de rutinas de ataque y evasión
├── strategy.cpp      # Lógica de combate y rutina inicial (ataque en arco)
└── README.md         # Documentación técnica, pinout y parada segura
```

```cpp
/*
 * Código de Minisumo Autónomo en Arduino IDE
 * 
 * Sensores de Piso (Línea blanca):
 * - QTR-1A Izquierdo: A2
 * - QTR-1A Derecho:   A1
 * 
 * Sensores de Oponente:
 * - JS40F Frontal Izquierdo: D4
 * - JS40F Frontal Derecho:   D2
 * 
 * NOTA: Los pines D0 y D1 se dejan libres para la comunicación Serial/USB,
 * ya que su uso interferiría con la carga de código en placas como Arduino Nano/Uno.
 */

// ================= PINES DE SENSORES =================
const int PIN_QTR_IZQ = A2;
const int PIN_QTR_DER = A1;

const int PIN_OPONENTE_IZQ = 4; // D4
const int PIN_OPONENTE_DER = 2; // D2

// Umbral analógico para detectar la línea blanca (0 a 1023)
// Ajustar en pruebas si la pista negra/blanca da valores intermedios
const int UMBRAL_LINEA = 500; 

// ================= PINES DE MOTORES =================
// Modificar estos pines según las conexiones a tu puente H
const int MOTOR_IZQ_IN1 = 5;
const int MOTOR_IZQ_IN2 = 6;
const int MOTOR_DER_IN3 = 9;
const int MOTOR_DER_IN4 = 10;

// Velocidades PWM (0 a 255)
const int VEL_MAX    = 255;
const int VEL_BUSCA  = 160;
const int VEL_AJUSTE = 200;

// ================= CONTROL DE MOTORES =================
void setMotores(int velIzq, int velDer) {
  // Motor Izquierdo
  if (velIzq > 0) {
    analogWrite(MOTOR_IZQ_IN1, velIzq);
    analogWrite(MOTOR_IZQ_IN2, 0);
  } else if (velIzq < 0) {
    analogWrite(MOTOR_IZQ_IN1, 0);
    analogWrite(MOTOR_IZQ_IN2, -velIzq);
  } else {
    analogWrite(MOTOR_IZQ_IN1, 0);
    analogWrite(MOTOR_IZQ_IN2, 0);
  }

  // Motor Derecho
  if (velDer > 0) {
    analogWrite(MOTOR_DER_IN3, velDer);
    analogWrite(MOTOR_DER_IN4, 0);
  } else if (velDer < 0) {
    analogWrite(MOTOR_DER_IN3, 0);
    analogWrite(MOTOR_DER_IN4, -velDer);
  } else {
    analogWrite(MOTOR_DER_IN3, 0);
    analogWrite(MOTOR_DER_IN4, 0);
  }
}

void parar() {
  setMotores(0, 0);
}

// ================= LECTURA DE SENSORES =================
// JS40F suele entregar nivel BAJO (LOW) al detectar objeto
bool detectaOponenteIzq() {
  return digitalRead(PIN_OPONENTE_IZQ) == LOW;
}

bool detectaOponenteDer() {
  return digitalRead(PIN_OPONENTE_DER) == LOW;
}

// QTR-1A entrega menor voltaje al reflejar sobre superficie blanca
bool detectaLineaIzq() {
  return analogRead(PIN_QTR_IZQ) < UMBRAL_LINEA;
}

bool detectaLineaDer() {
  return analogRead(PIN_QTR_DER) < UMBRAL_LINEA;
}

// ================= RUTINA INICIAL: ATAQUE DE ARCO =================
void ataqueDeArco() {
  // Curva cerrada rápida hacia el costado del rival
  setMotores(VEL_MAX, VEL_MAX / 2);
  delay(450);

  // Cierre de embestida en arco
  setMotores(VEL_MAX, VEL_MAX);
  delay(350);
}

// ================= SETUP =================
void setup() {
  pinMode(PIN_QTR_IZQ, INPUT);
  pinMode(PIN_QTR_DER, INPUT);

  pinMode(PIN_OPONENTE_IZQ, INPUT_PULLUP);
  pinMode(PIN_OPONENTE_DER, INPUT_PULLUP);

  pinMode(MOTOR_IZQ_IN1, OUTPUT);
  pinMode(MOTOR_IZQ_IN2, OUTPUT);
  pinMode(MOTOR_DER_IN3, OUTPUT);
  pinMode(MOTOR_DER_IN4, OUTPUT);

  parar();

  // Espera reglamentaria de 5 segundos de seguridad
  delay(5000);

  // Ejecución de la estrategia inicial
  ataqueDeArco();
}

// ================= BUCLE PRINCIPAL =================
void loop() {
  // 1. Prioridad Absoluta: Detección de Borde (Sensores QTR-1A)
  bool lineaIzq = detectaLineaIzq();
  bool lineaDer = detectaLineaDer();

  if (lineaIzq && lineaDer) {
    // Ambos detectan borde: retroceso rápido por 1 segundo
    setMotores(-VEL_MAX, -VEL_MAX);
    delay(1000);
    return;
  } 
  else if (lineaDer) {
    // Solo derecho: gira llanta izquierda hacia atrás 1s, luego avanza 1s
    setMotores(-VEL_MAX, 0);
    delay(1000);
    setMotores(VEL_MAX, VEL_MAX);
    delay(1000);
    return;
  } 
  else if (lineaIzq) {
    // Solo izquierdo: gira llanta derecha hacia atrás 1s, luego avanza 1s
    setMotores(0, -VEL_MAX);
    delay(1000);
    setMotores(VEL_MAX, VEL_MAX);
    delay(1000);
    return;
  }

  // 2. Control de Combate: Sensores JS40F
  bool opIzq = detectaOponenteIzq();
  bool opDer = detectaOponenteDer();

  if (opIzq && opDer) {
    // Ambos detectan: embestida frontal a máxima potencia
    setMotores(VEL_MAX, VEL_MAX);
  } 
  else if (opDer && !opIzq) {
    // Solo sensor derecho: gira llanta izquierda al frente para corregir
    setMotores(VEL_AJUSTE, 0);
  } 
  else if (opIzq && !opDer) {
    // Solo sensor izquierdo: gira llanta derecha al frente para corregir
    setMotores(0, VEL_AJUSTE);
  } 
  else {
    // Búsqueda y rastreo: Giro continuo en el propio eje (Spot Spin)
    setMotores(VEL_BUSCA, -VEL_BUSCA);
  }
}
```

| Periférico | Pin Arduino | Modo | Descripción |
| :--- | :--- | :--- | :--- |
| QTR-1A Izquierdo | A2 | INPUT | Sensor de piso / línea blanca analógico (< 500) |
| QTR-1A Derecho|A1|INPUT|Sensor de piso / línea blanca analógico (< 500)|
|JS40F Izquierdo|D4|INPUT_PULLUP|Detección digital de oponente (LOW activo)|
|JS40F Derecho|D2|INPUT_PULLUP|Detección digital de oponente (LOW activo)|
|Motor Izq (IN1)|D5 (PWM)|OUTPUT|Señal de avance / retroceso motor izquierdo|
|Motor Izq (IN2)|D6 (PWM)|OUTPUT|Señal de reversa / frenado motor izquierdo|
|Motor Der (IN3)|D9 (PWM)|OUTPUT|Señal de avance / retroceso motor derecho|
|Motor Der (IN4)|D10 (PWM)|OUTPUT|Señal de reversa / frenado motor derecho|
|UART / Serial|D0 / D1|N/A|Reservados exclusivamente para programación USB|

## Versiones y entorno de desarrollo
IDE: Arduino IDE 2.3+ (o Arduino CLI)

Placa / Core: Arduino AVR Boards v1.8.6 (compatible con microcontroladores ATmega328P / Nano / XMotion V3)

Librerías externas: Ninguna (implementación con registros estándar de Arduino para máxima portabilidad y velocidad de ciclo)

## Procedimiento de compilación y carga
Abrir codigo/mini-sumo/main.ino en Arduino IDE.

Seleccionar la placa correspondiente en Herramientas > Placa y el puerto COM asignado.

Compilar con Ctrl + R para verificar que no existan errores de sintaxis.

Conectar el robot por USB (con interruptor de motores apagado) y cargar el firmware con Ctrl + U.

## Procedimiento de parada segura y arranque reglamentario
Parada de emergencia: Desconectar el switch principal de potencia ubicado en el chasis para desenergizar el puente H y detener inmediatamente la tracción de los motores.

Arranque reglamentario: Al encender el circuito, el firmware ejecuta una espera obligatoria de 5 segundos (delay(5000)) con los motores detenidos antes de iniciar la rutina ataqueDeArco(), cumpliendo con la normativa de seguridad de mini-sumo.

