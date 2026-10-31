## Mecánica y electrónica

### 1. Modelo mecánico (`modelo/`)

Para la estructura del robot se uso una base ya existente y únicamente se diseñó y fabricó una única pieza personalizada en CAD:

* **Archivo:** <img width="918" height="592" alt="CAD1" src="https://github.com/user-attachments/assets/a988ec0d-ebd9-4797-bfb8-d2764b12d443" /> <img width="1070" height="381" alt="CAD2" src="https://github.com/user-attachments/assets/5136eee6-fe15-4bfc-844d-603d857499b3" />


* **Descripción:** Chasis unibody compacto diseñado para cumplir con las dimensiones máximas reglamentarias de mini-sumo (menor a 10 × 10 cm). Integra bahía interna para batería LiPo, ranuras de montaje para micromotores con reducción, soportes frontales para 2 sensores JS40F y alojamientos inferiores a 3 mm del piso para los sensores de reflectancia QTR-1A.
* **Material / Manufactura:** Impresión 3D en filamento PLA/PETG, relleno al 40% para maximizar rigidez y resistencia al impacto frontal.

---

### 2. Conexiones eléctricas (`electrica/`)

El cableado y la distribución de señales se organizan según el siguiente esquema de interconexión:

```text
                  +---------------------------+
                  |   Batería LiPo (7.4V)     |
                  +-------------+-------------+
                                |
                         [Interruptor ON/OFF]
                                |
         +----------------------+----------------------+
         |                                             |
         v (VIN)                                       v (VCC Motor)
+--------------------------------------------------------------+
|                     Controlador XMotion V3                   |
|                                                              |
| [A2] <--- QTR-1A Izquierdo (Piso)                            |
| [A1] <--- QTR-1A Derecho   (Piso)                            |
| [D4] <--- JS40F Frontal Izq (Oponente)                       |
| [D2] <--- JS40F Frontal Der (Oponente)                       |
|                                                              |
| [D5, D6]   --------(PWM / DIR)--------> Driver / Motor Izq   |
| [D9, D10]  --------(PWM / DIR)--------> Driver / Motor Der   |
+--------------------------------------------------------------+
```
---

### 3. Lista de materiales (`bom.md`)

| Componente | Cantidad | Especificaciones / Modelo | Justificación / Decisión técnica |
| --- | --- | --- | --- |
| **Controlador** | 1 | XMotion V3 (ATmega328P) | Placa "todo en uno" con drivers integrados, tamaño reducido y peso ligero ideal para mini-sumo. |
| **Chasis** | 1 | Pieza única en PLA/PETG | Estructura unibody a medida para alojar sensores, motores y batería dentro del límite de 10x10 cm. |
| **Sensores de borde** | 2 | Pololu QTR-1A | Sensores de reflectancia infrarroja para detección precisa y de rápida respuesta de la línea blanca.|
| **Sensores de oponente** | 2 | JS40F | Sensores de distancia digitales inmunes a luz ambiente para detección frontal directa.|
| **Motores** | 2 | Micromotores N20 metálicos | Alto torque con relación de reducción adecuada para empuje y tamaño compacto.|
| **Ruedas** | 2 | Llantas de goma / silicona | Máximo coeficiente de fricción contra la superficie del dohyō para evitar deslizamiento.|
| **Batería** | 1 | LiPo 2S (7.4V, ~350-500 mAh) | Relación óptima de densidad de energía y peso para mantenerse bajo el límite de 500 g. |
| **Interruptor** | 1 | Switch deslizable 2 pines | Corte general de energía para parada de emergencia y cumplimiento de seguridad. |

