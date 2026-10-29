---
kaizen_dojo: "2026"
formato: "Entregable diario G2"
evidencia: "E3"
dia: 3
responsable_registro: "equipo"
estado: "EN_PROCESO"
fecha: "2026-10-28"
revision_docente: "PENDIENTE"
---

# E3 · Día 3 — MEDIR Y APRENDER | Kaizen 1: ensayo, hipótesis y mejora

> Se documentan las actividades reportadas por el equipo. La compilación satisfactoria no demuestra por sí sola el funcionamiento físico del robot. No se registran como realizadas pruebas ni mediciones que no fueron proporcionadas.

## 0 · Contexto de investigación de hoy

**Fecha/equipo/misión:** 2026-10-28 / Los Quemapuentes-H / M01 · Mini-sumo autónomo con XMotion V3.

**Dōjō exacto:** pendiente de registrar.

**Versión de partida:** integración física de conexiones realizada durante el Día 2; commit o etiqueta V1 pendiente de incorporar.

**Protocolo E2:** [`../../pruebas/protocolo.md`](../../pruebas/protocolo.md). Contenido y actualización pendientes de verificar.

## 1 · Ruta del Día 3 (180 min)

Los intervalos corresponden a la planeación del formato; no se registraron tiempos reales por actividad.

| Actividad | Minutos | Evidencia a registrar |
|---|---:|---|
| Analizar un fallo real / demostración | 0–15 | Se presentó una dificultad para incorporar la biblioteca XMotion en Arduino mediante el archivo ZIP. Se resolvió utilizando una copia previamente instalada y extraída de la biblioteca. El mensaje exacto del error y las capturas quedan pendientes de incorporar. |
| Diseño del experimento | 15–40 | Se modificó el diseño de la carcasa superior en SolidWorks para preparar su impresión. Debido a que las impresoras 3D estaban ocupadas, se optó por elaborar una representación física en cartón con las medidas del diseño. Esta representación permite revisar el espacio y ajuste, pero no valida la resistencia de la pieza impresa. |
| Diagnóstico del prototipo V1 | 40–80 | Erik verificó el estado de las conexiones. A00574867 realizó una soldadura para alargar un cable de un motor. Se identificó además un bloqueo en el entorno de programación relacionado con la incorporación de la biblioteca. No se documentaron mediciones eléctricas ni una prueba discriminante formal. |
| Kaizen 1: cambio técnico | 80–125 | Se alargó el cable del motor, se utilizó la biblioteca previamente disponible, se compilaron los códigos de QTR, IR y motores, y se modificó el CAD. También se desarrolló código para dos tácticas de ataque. Archivos y diferencias pendientes de enlazar. |
| Reensayo equivalente | 125–160 | Se reportó compilación satisfactoria de los códigos de QTR, IR y motores. No se proporcionaron resultados emparejados V1/K1 ni mediciones del comportamiento físico de las tácticas. |
| Documentar, debatir, reflejar | 160–180 | Se identificó la necesidad de registrar la biblioteca utilizada, consolidar las versiones del código y CAD, y verificar físicamente las tácticas antes de concluir que mejoraron el desempeño. Evidencias personales E3 pendientes de confirmar. |

## 2 · Problema, hipótesis y trazabilidad

Para evitar confundir cambios distintos, la hipótesis principal de esta sección se enfoca en el bloqueo de compilación. El desempeño de las tácticas requiere un experimento posterior.

| Campo | Completar |
|---|---|
| Fallo / oportunidad de mejora observada (con evidencia) | Dificultad para incorporar la biblioteca XMotion en Arduino mediante ZIP, lo que bloqueó el avance de compilación. Captura y mensaje exacto pendientes de enlazar. |
| Dónde se presenta y cuántas veces | En el entorno Arduino utilizado durante el Día 3. Se reportó el incidente, pero no se registró el número de intentos o repeticiones. |
| Diagnóstico: causas alternativas que se consideraron | No se documentó una comparación formal de causas. Queda por revisar si el problema correspondía a la estructura del ZIP, la ubicación de la biblioteca, su versión o el nombre usado en la inclusión. Estas posibilidades no se consideran causas confirmadas. |
| Hipótesis contrastable: **si cambio X, espero que Y ocurra porque Z** | Si utilizamos la copia de la biblioteca XMotion previamente instalada y extraída, esperamos que los programas compilen sin errores relacionados con esa dependencia, porque el entorno podrá localizar sus archivos. |
| Variable independiente que se modifica | Copia y forma de incorporación de la biblioteca XMotion al entorno Arduino. |
| Métrica de resultado con unidad y criterio de mejora | Resultado de compilación por programa: satisfactorio o fallido; número de errores relacionados con la biblioteca. Criterio propuesto: compilar sin errores los programas de QTR, IR y motores. No se registraron tiempos de compilación. |
| Variables que se mantendrán iguales | Para una comparación controlada: mismo código de cada programa, computadora, versión del IDE, placa seleccionada y demás dependencias. No se confirmó documentalmente que todas estas condiciones permanecieran iguales durante la sesión. |
| Ensayos requeridos y forma de muestreo | Se reportó la compilación de tres programas: QTR, IR y motores. No se documentaron cinco repeticiones ni el número de compilaciones por programa. Para reproducir el resultado, compilar cada archivo identificado y conservar su salida completa. |
| Riesgo de sesgo/confusión y cómo se mitigará | Podrían haberse modificado simultáneamente el código y la biblioteca. Para mitigarlo, registrar versiones y comparar el mismo archivo antes y después del cambio. No atribuir a la biblioteca una mejora de comportamiento físico sin pruebas. |
| Parada de seguridad / condición de aborto | La compilación puede realizarse sin alimentar los motores. Para pruebas físicas posteriores: revisar aislamiento y polaridad, comenzar con ruedas elevadas y desconectar ante calentamiento anormal, olor, humo o movimiento inesperado. La detección del borde deberá tener prioridad sobre cualquier espera programada. |

## 3 · Colaboración y cambio técnico Kaizen 1

| Alias y alcance | Kata asociado (código o propio) | Qué cambió exactamente | Por qué | Código/CAD/commit y responsable de revisión | Validación de interfaz |
|---|---|---|---|---|---|
| A00574867 · Actuadores y cableado | Propio: extensión de cable de motor | Realizó una soldadura para alargar un cable de un motor. | Facilitar el recorrido y alcance del conductor dentro del montaje. | Fotografía y registro del cambio pendientes de enlazar. Revisor por confirmar. | Verificación de continuidad, aislamiento y ausencia de tensión mecánica pendiente de documentar. |
| Erik · Integración eléctrica | Propio: revisión de conexiones | Verificó el estado de las conexiones del minisumo. | Revisar el montaje antes de continuar con la integración y programación. | Evidencia y detalle de conexiones revisadas pendientes de incorporar. | No se proporcionó una lista de puntos verificados ni resultados de medición. |
| A00574867 · Entorno de programación | Propio: recuperación de dependencia XMotion | Utilizó una copia previamente instalada y extraída de la biblioteca tras la dificultad con el ZIP. | Desbloquear la compilación de los programas. | Versión y procedencia de la biblioteca pendientes de registrar. | Se reportó compilación satisfactoria de los códigos de QTR, IR y motores. |
| A00574867 · Pruebas de código por subsistema | Propio: compilación de sensores y motores | Compiló los programas de QTR, IR y motores. | Comprobar que los programas pudieran construirse en el entorno disponible. | Archivos y salidas de compilación pendientes de enlazar. | Compilación reportada como satisfactoria. Carga en placa, lecturas y accionamiento físico no documentados en este registro. |
| A00574867 · Diseño mecánico | Propio: ajuste de carcasa superior | Modificó el diseño CAD para preparar su impresión 3D. Se optó por una representación en cartón ante la ocupación de las impresoras. | Revisar dimensiones y continuar con el desarrollo físico sin esperar la impresión. | CAD, revisión y fotografías del cartón pendientes de incorporar. | Ajuste dimensional pendiente de registrar con medidas; resistencia y fijación de la pieza impresa sin validar. |
| A00574867 y Erik · Control y estrategia | Propio: tácticas de ataque | Desarrollaron código para una maniobra de retroceso, giro y búsqueda rápida, y una respuesta ante detección del rival por detrás con espera programada de 5 s condicionada a superficie negra. | Incorporar estrategias de búsqueda y respuesta al oponente. | Código, distribución exacta de autoría y revisor pendientes de incorporar. | Ejecución física y desempeño de las tácticas pendientes de validar. |

### Tácticas desarrolladas

1. **Retroceso, giro y búsqueda:** el robot retrocede, realiza un giro y busca detectar al rival para aproximarse con velocidad. Las duraciones y velocidades exactas deben recuperarse del código.

2. **Respuesta ante ataque trasero:** ante la detección del rival por detrás, se planteó una espera de 5 segundos mientras los sensores de borde indiquen superficie negra, seguida de una acción motriz opuesta al empuje esperado del rival y un cambio de orientación.

**Límite de interpretación:** los IR detectan presencia del rival; no se reportó un sensor que mida la fuerza de empuje. La segunda táctica es una respuesta programada, no un control de fuerza medido. Falta verificar en el código que la detección de línea blanca interrumpa inmediatamente la espera.

**Identificador de versión K1:** pendiente de asignar mediante commit o etiqueta y revisión del CAD.

**Otras modificaciones involuntarias o perturbaciones:** no se reportaron cambios involuntarios. Como cambios adicionales se registran la extensión del cable, las modificaciones CAD y el uso de cartón en lugar de la pieza impresa. La disponibilidad de impresoras afectó la fabricación.

## 4 · Ensayos comparables

**Enlace a datos crudos CSV:** [`../../datos/ensayos.csv`](../../datos/ensayos.csv).

**Protocolo:** [`../../pruebas/protocolo.md`](../../pruebas/protocolo.md).

No se proporcionaron ensayos emparejados bajo condiciones equivalentes. La siguiente tabla distingue lo reportado de lo que permanece pendiente; no representa cinco corridas ejecutadas.

| Prueba emparejada o bloque | Condición/escenario idéntico | V1, valor + unidad | K1, valor + unidad | Cambio / resultado | Incidencia o desviación |
|---:|---|---|---|---|---|
| 1 | Compilación del programa de QTR | Resultado individual no registrado. | Compilación satisfactoria reportada; número de intentos no registrado. | El programa pudo compilarse con el entorno disponible. | No se conservaron en este registro las salidas antes/después ni la identidad del archivo. |
| 2 | Compilación del programa de IR | Resultado individual no registrado. | Compilación satisfactoria reportada; número de intentos no registrado. | El programa pudo compilarse con el entorno disponible. | No se confirmó que el código fuera idéntico entre configuraciones. |
| 3 | Compilación del programa de motores | Resultado individual no registrado. | Compilación satisfactoria reportada; número de intentos no registrado. | El programa pudo compilarse con el entorno disponible. | La compilación no demuestra giro, velocidad o sentido de los motores. |
| 4 | Táctica de retroceso, giro y búsqueda | Sin medición registrada. | Sin medición registrada. | Código desarrollado; desempeño físico pendiente de comprobar. | Sin tiempos observados, trayectoria, velocidad ni número de corridas. |
| 5 | Respuesta a detección trasera y borde | Sin medición registrada. | Sin medición registrada. | Se planteó una espera programada de 5 s; duración real y respuesta física no medidas. | Pendiente comprobar interrupción por línea blanca y respuesta al rival. |

**N válido V1 / K1:** 0 / 0 para comparación emparejada. Se reportaron resultados de compilación de tres programas, pero no constituyen pares experimentales V1/K1 documentados.

**Resumen, variabilidad y tasa de éxito:** no calculables con los datos disponibles. No se registraron repeticiones, tiempos ni resultados individuales suficientes para estimar variabilidad o tasa de éxito.

**Incertidumbres/limitaciones:** faltan versiones de código y biblioteca, salidas de compilación, mapa de conexiones verificado y datos de ejecución física. Los 5 segundos corresponden a una consigna programada, no a una medición. El modelo de cartón no permite concluir cómo resistirá la carcasa impresa.

## 5 · Interpretación y decisión

- **¿La evidencia respalda, contradice o no permite decidir la hipótesis?** El resultado reportado es compatible con la hipótesis: al utilizar la biblioteca previamente instalada y extraída, se logró compilar los programas. Sin archivos, registros y condiciones equivalentes no puede confirmarse de manera aislada la causa del problema.

- **Si no hubo mejora, qué aprendimos:** se reportó una mejora operativa al desbloquear la compilación. Aprendimos que es necesario identificar y conservar las dependencias del proyecto. Todavía no hay datos para afirmar una mejora en el desempeño de combate.

- **¿Qué riesgo o compromiso generó el cambio?** Utilizar una biblioteca anterior sin registrar su versión dificulta reproducir el entorno. La extensión del cable requiere comprobar aislamiento y continuidad. La espera de 5 s podría retrasar una maniobra de escape si se implementa de forma bloqueante. El cartón permite revisar forma y espacio, pero no sustituye la validación de la pieza impresa.

- **Decisión:** conservar provisionalmente los cambios y recolectar más datos. La biblioteca permitió continuar, y el código y CAD representan avances de integración; las tácticas y el montaje deben validarse antes de considerarlos definitivos.

- **Siguiente pregunta para Kaizen 2:** ¿el robot puede ejecutar las tácticas de búsqueda y respuesta trasera manteniendo la detección del borde activa y prioritaria, sin salir del dohyō?

## 6 · Puerta de salida E3

- [ ] V1 y K1 tienen identificadores o referencias inequívocas.
- [ ] La hipótesis está conectada con una medida y un problema diagnosticado.
- [x] Se documentó una modificación técnica y su responsable.
- [ ] Ensayos y resultados mantienen condiciones comparables o exponen diferencias explícitamente.
- [x] La conclusión es honesta, incluso si el resultado es negativo.
- [ ] Cada estudiante registró su [E3 personal](../../participantes/_plantilla/dias/E3.md).

La hipótesis y la métrica están planteadas, pero el diagnóstico causal y la comparación controlada siguen pendientes. No se marca la condición de ensayos comparables porque no se proporcionaron pares V1/K1 ejecutados.

**Gate E3:** CONDICIONADO — propuesta de estado, pendiente de validación docente.

**Condiciones pendientes:** incorporar versiones y evidencias, registrar la biblioteca utilizada y realizar ensayos físicos reproducibles de sensores, motores y tácticas, incluyendo la prioridad de escape ante línea blanca.

**Revisor:** pendiente de asignar.

**Enlace a PR/commit:** pendiente de incorporar.