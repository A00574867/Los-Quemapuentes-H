---
kit: "Kaizen Dōjō 2026 — Compromiso de misión"
version_catalogo: "C2 / 1.1"
participante: "Erik Daniel Puente Hernández"
equipo: "Los Quemapuentes H"
mision: "M01"
plataforma: "Mini-sumo autónomo"
territorio_personal: "D · DOMINAR"
frontera_personal: "F1 · INTEGRAR"
validacion_docente: "PENDIENTE"
---

# Mi compromiso Kaizen · 2026

> **Mi desafío:** Armar y programar un mini sumo

## 1. Mi misión y mi frontera

- **Participante:** Erik Daniel Puente Hernández
- **Equipo:** Los Quemapuentes H
- **Plataforma:** M01 · Mini-sumo autónomo
- **Territorio personal:** D · DOMINAR
- **Frontera personal:** F1 · INTEGRAR

**Hoy todavía no puedo:**

Hacer, calibrar ni programar un mini sumo

**Al finalizar Kaizen Dōjō demostraré que puedo:**

Armar y programar un mini sumo

**La evidencia o indicador que utilizaré:**

Funcionamiento del mini sumo

**Mi motivación:**

Quiero ser capas de crear un mini sumo básico he implementar dentro de este mis conocimientos para mejorarlo

## 2. Alcances y katas seleccionados

Esta es mi propuesta individual dentro de una misión colaborativa. Cada alcance requiere evidencia de contribución propia y negociación de viabilidad.

### 1. MS05 · Integrar y calibrar sensores de borde

- **Tipo:** Preestablecido · catálogo C2
- **Territorio sugerido:** DOMINAR
- **Frontera sugerida:** F1 · INTEGRAR
- **Carta:** D2 · ROBUST ROBOT
- **Duración estimada:** 3–4 h
- **Resultado esperado / aceptación:** Detección del límite del dohyō en condiciones definidas, con umbrales trazables.
- **Recursos o prerequisitos:** Sensores de reflectancia montados y dohyō de pruebas.

**Katas elegidos**

- [ ] Registrar lecturas sobre fondo y borde en varias posiciones.
- [ ] Definir umbral e implementar detector con señal de prueba.
- [ ] Medir aciertos y falsos avisos en al menos cinco aproximaciones.

**Mi evidencia final:** _Completar al avanzar el proyecto_

**Enlaces a código/CAD/pruebas:** _Agregar enlaces relativos al repositorio_

### 2. MS03 · Integrar y verificar motorización y tracción

- **Tipo:** Preestablecido · catálogo C2
- **Territorio sugerido:** DOMINAR
- **Frontera sugerida:** F1 · INTEGRAR
- **Carta:** D1 · AUTONOMOUS SYSTEM
- **Duración estimada:** 3–4 h
- **Resultado esperado / aceptación:** Conjunto motor–driver–rueda capaz de avanzar, retroceder y girar de forma controlada.
- **Recursos o prerequisitos:** Motores y drivers compatibles, chasis y alimentación protegida.

**Katas elegidos**

- [ ] Identificar polaridad, relaciones de transmisión y límites del driver.
- [ ] Montar motor y rueda; probar sentido de giro con comandos breves.
- [ ] Comparar deslizamiento y respuesta en tres maniobras repetidas.

**Mi evidencia final:** _Completar al avanzar el proyecto_

**Enlaces a código/CAD/pruebas:** _Agregar enlaces relativos al repositorio_

### 3. MS11 · Implementar recuperación robusta ante borde o atasco

- **Tipo:** Preestablecido · catálogo C2
- **Territorio sugerido:** DOMINAR
- **Frontera sugerida:** F2 · DECIDIR
- **Carta:** D2 · ROBUST ROBOT
- **Duración estimada:** 3–4 h
- **Resultado esperado / aceptación:** Rutina de evasión prioritaria y recuperación sin salida del área en ensayos controlados.
- **Recursos o prerequisitos:** Sensores de borde y motores operativos; protecciones activas.

**Katas elegidos**

- [ ] Construir casos de borde frontal/lateral sin movimiento peligroso.
- [ ] Programar prioridad de evasión y temporizador de maniobra.
- [ ] Probar en varios ángulos de aproximación y corregir fallos.

**Mi evidencia final:** [https://docs.google.com/document/d/1VxCkeARCwehgKrcwWJjHoiACUyt3JGDWCz6tgDRHYX4/edit?tab=t.0]

**Enlaces a código/CAD/pruebas:** [https://github.com/A00574867/Los-Quemapuentes-H/blob/main/README.md]

## 3. Planeación y viabilidad

- **Alcances:** 3 de un máximo de 3
- **Katas:** 9
- **Esfuerzo técnico estimado:** 9–12 horas
- **Disponibilidad orientativa:** 8–10 horas de trabajo técnico dentro de las 15 horas presenciales.
- **Estado:** REQUIERE REVISIÓN: el máximo estimado supera 10 horas

## 4. Mi bitácora Kaizen (cinco sesiones)

| Día | Evidencia que registraré | Estado |
|---|---|---|
| D1 · Atreverse | Diagnóstico y pacto de frontera | [Finalizado] |
| D2 · Hacer | Prototipo / primera integración V1 | [Finalizado] |
| D3 · Medir | Ensayo base y ciclo Kaizen 1 | [Finalizado] |
| D4 · Iterar | Ciclo Kaizen 2 y comparación V1–Vn | [Finalizado] |
| D5 · Demostrar | Desafío, evidencia y reflexión | [Finalizado] |

## 5. Mi protocolo de mejora

### Ciclo Kaizen 1

Durante la fase de integración y validación de la tracción y maniobras de escape (metas MS03 y MS11), se presentó una anomalía crítica: una de las ruedas motrices no respondía a los comandos de movimiento en el robot integrado, a pesar de que el motor de forma aislada operaba con normalidad. Debido a las restricciones de tiempo antes de la competencia, no fue posible ejecutar una reparación a nivel de componente en la placa, por lo que el método Kepner-Tregoe se utilizó para aislar variables, plantear hipótesis fundadas y decidir el plan de contingencia más viable.

### Definición del Problema (Análisis de la Situación)
Declaración de la desviación: Una rueda del minisumo permanece inactiva al ejecutar rutinas de movimiento en el prototipo ensamblado, impidiendo la traslación y los giros controlados requeridos por las metas de motorización y evasión.
Matriz ES / NO ES (Delimitación del Problema):
- QUÉ ES: Falta de entrega de potencia y señal motriz hacia una sola rueda/actuador.
- QUÉ NO ES: Un fallo en el motor mismo (probado externamente con fuente de poder directa y funcionando con normalidad), ni un defecto en el código de control (rutinas validadas en lógica de software y simulación).
- DÓNDE ES: Localizado en la salida de potencia/control correspondiente al canal de ese motor en la placa integrada Xmotion V3.
- DÓNDE NO ES: En el cableado externo ni en los conectores (se verificó continuidad, aislamiento físico y ausencia de daños en los cables).
- CUÁNDO ES: Al enviar comandos de avance, retroceso o giro con el sistema energizado en el chasis.
- CUÁNDO NO ES: Durante las pruebas aisladas de banco del micromotor DC.
- ALCANCE: Inhabilitó la motricidad simétrica del robot, imposibilitando completar las pruebas de deslizamiento y las maniobras evasivas en ángulo en el Dohyo (katas de MS03 y MS11).

### Análisis de Causas Raíz y Factores Limitantes
Al contrastar las diferencias entre lo que "ES" y lo que "NO ES", se descartaron fallas en el actuador, el firmware y la integridad física del arnés de cables. Por lo tanto, la causa raíz más probable se focaliza internamente en la tarjeta controladora Xmotion V3:
1. Fallo en la etapa interna del driver de potencia (Puente H): Daño térmico, electrostático o sobrecorriente en uno de los MOSFETs o compuertas lógicas internas del puente H integrado asignado a ese canal específico en la Xmotion V3.
2. Defecto en la ruta de conmutación o pistas de la PCB: Posible fisura microscópica en la pista de cobre de salida del puente H, soldadura fría o daño en la resistencia/filtro de sensado de corriente de ese canal particular.
3. Restricción temporal severa: Al competir contra reloj, el equipo no dispuso del tiempo ni de la instrumentación avanzada (como estación de retrabajo de aire caliente u osciloscopio) para diagnosticar y reemplazar chips de montaje superficial (SMD) dentro de la placa.
### Análisis de Decisiones y Propuestas de Solución
Ante la imposibilidad temporal de desoldar y reparar componentes a nivel silicio en la Xmotion V3, se evaluaron tres alternativas viables para mitigar el impacto y permitir que el equipo continuará con la evaluación:

| Criterio de Decisión | Peso (1-10) | Alternativa A: Reemplazar la placa por otra idéntica | Alternativa B: Cablear un driver externo puente H puenteando señales lógicas | Alternativa C: Intentar reparación a nivel componente |
| :--- | :---: | :---: | :---: | :---: |
| Tiempo de ejecución antes del cierre de entrega | 10 | 10 (100) | 6 (60) | 2 (20) |
| Preservación del límite de volumen ($10 \times 10\,\text{cm}$) | 9 | 10 (90) | 6 (54) | 10 (90) |
| Cumplimiento de la restricción de masa ($< 500\,\text{g}$) | 9 | 10 (90) | 7 (63) | 10 (90) |
| Confiabilidad eléctrica ante vibraciones e impactos | 8 | 9 (72) | 5 (40) | 4 (32) |
| **Puntaje Ponderado Total** | | **352** | **217** | **232** |

**Decisión seleccionada (Alternativa A):** La solución óptima y viable ante el margen de tiempo disponible habría sido recurrir al cambio directo por una placa de repuesto, garantizando que el diseño mantuviera el centro de masa, la compacidad dentro de los 1010cm y el peso reglamentario menor a 500g sin añadir peso parásito por módulos auxiliares. Pero decidimos buscar otras soluciones y por ende no logramos solucionar el problema.

**Acciones preventivas futuras:**
Implementar diodos de protección externos (flyback/TVS) y fusibles rearmables (PTC) en las líneas de motor para evitar que picos de contra-fuerza electromotriz dañen los puentes H de la tarjeta durante colisiones frontales bruscas.
Diseñar un protocolo estandarizado de prueba previa con multímetro/osciloscopio en las salidas de motor antes de montar la placa de forma definitiva en el chasis.


## 6. Cierre y reflexión

**Antes no podía:** Armar un minisumo ni entender su funcionamiento

**Ahora puedo:** Armar desde cero un mini sumo y crear su lógica de funcionamiento

**Cómo lo demostré:** Creando un mini sumo desde cero 

**Qué intentaría mejorar después:** Verificar siempre el estado de los componentes antes de implementarlos y aprender más acerca del lenguaje de programación C++

---

_Documento generado localmente con el configurador Kaizen Dōjō 2026 · catálogo C2. El estudiante debe revisar y acordar con el profesor los alcances y condiciones de seguridad antes de operar robots físicos._

**Fuente de catálogo:** https://docs.google.com/spreadsheets/d/1FKxFzoyu9KJb3RlOwB609vliS5hAtmwWFu2G2zG3Ky4/edit
