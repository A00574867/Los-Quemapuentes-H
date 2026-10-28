---
kaizen_dojo: "2026"
formato: "Entregable diario G2"
evidencia: "E2"
dia: 2
responsable_registro: "equipo"
estado: "EN_PROCESO"
fecha: "POR_CONFIRMAR"
revision_docente: "PENDIENTE"
---

# E2 · Día 2 — HACER | Primera integración funcional y línea base V1

> Registro del trabajo realizado por A00574867 y Erik. Las conexiones físicas no se consideran pruebas de funcionamiento. Los datos, archivos y evidencias no proporcionados quedan pendientes de incorporar.

## 0 · Identificación y continuidad

| Campo | Dato |
|---|---|
| Fecha, equipo, misión y plataforma | Fecha por confirmar. Equipo: Los Quemapuentes-H. Misión M01 · Mini-sumo autónomo. Plataforma: minisumo con placa XMotion V3. |
| Dōjō real y mesa/zona utilizada | Ubicación y puesto de trabajo pendientes de registrar. |
| Estado del gate E1 / cambios desde D1 | Aprobación del gate E1 pendiente de confirmar. Durante D2 se avanzó en las conexiones de sensores y motores; posteriormente se trabajó en el diseño CAD de la carcasa superior. |
| Kit por integrante / compromisos modificados | Erik realizó las conexiones de sensores infrarrojos y QTR a las borneras. A00574867 soldó los cables de los motores y posteriormente trabajó en el diseño CAD de la carcasa superior. Se sustituyeron algunas herramientas y consumibles ante la falta de material. |
| Materiales recibidos y pendientes | Se utilizaron sensores, QTR, borneras, motores y cables del equipo. Faltaron tijeras, silicón y filamento para impresión 3D. Se emplearon cinta aislante negra y pinzas para pelar cables. Cantidades, responsables de abastecimiento y correspondencia con IDs MAT pendientes de verificar en el inventario. |
| Objetivo técnico del Día 2 | Avanzar en la integración física del cableado de sensores y motores, y preparar el diseño de la carcasa superior. La validación eléctrica y funcional de la integración queda pendiente. |

## 1 · Ruta de las actividades de hoy (180 min)

Los intervalos siguientes corresponden a la estructura prevista del entregable. No se registraron tiempos reales por actividad.

| Bloque | Minutos | Registro requerido / evidencia |
|---|---:|---|
| Revisión de misión y compromisos | 0–15 | Se identificó la falta de tijeras, silicón y filamento. El trabajo se distribuyó entre conexión de sensores, soldadura de cables de motores y desarrollo posterior del CAD. Evidencia pendiente de enlazar. |
| Microlección aplicada | 15–35 | Se aplicaron técnicas de preparación de cables, conexión a borneras, soldadura y aislamiento. No se documentó una microlección formal ni una referencia específica. |
| Katas de integración | 35–105 | Erik conectó sensores infrarrojos y QTR a las borneras. A00574867 soldó los cables de los motores. Se utilizaron pinzas para pelar cables y cinta aislante negra. Fotografías de las contribuciones pendientes de incorporar. |
| Ensayos iniciales / línea base | 105–145 | No se reportaron ensayos funcionales ni mediciones eléctricas. Se completó el trabajo de conexiones reportado, pero no se verificó mediante datos el funcionamiento de sensores o motores. |
| Consolidación de evidencia | 145–170 | A00574867 trabajó posteriormente en el diseño CAD de la carcasa superior. Se identificó la necesidad de verificar las medidas reales y preparar su futura impresión 3D. Archivo CAD y evidencias pendientes de enlazar. |
| Gate E2 | 170–180 | Revisión docente pendiente. Se propone priorizar la verificación del cableado y la comprobación dimensional del CAD antes de continuar con pruebas e impresión. |

## 2 · Microlección e integración por alcances

**Tema que resolvió un problema real del equipo:** preparación, conexión y aislamiento de cables utilizando los recursos disponibles. Las pinzas permitieron pelar los cables y la cinta aislante negra se utilizó para aislar las conexiones ante la falta de otros materiales.

**Material / referencia utilizada:** componentes físicos del minisumo y herramientas disponibles. No se proporcionó una referencia técnica específica de la sesión.

| Alias | Alcance | Kata seleccionado / nuevo | Acción técnica ejecutada | Archivo, commit o plano | Estado (pendiente/probado/bloqueado) | Dependencia de otro integrante |
|---|---|---|---|---|---|---|
| A00574867 | Cableado de actuadores | Preparación y soldadura de conexiones de motores; identificación formal del kata pendiente | Soldó los cables de los motores del minisumo. | Evidencia fotográfica pendiente de incorporar. | pendiente: soldadura realizada, validación eléctrica y funcional no reportada | Requiere coordinación con Erik para revisar el conjunto de conexiones antes de energizar. |
| Erik — alias por confirmar | Sensores/percepción | Conexión de sensores a borneras; identificación formal del kata pendiente | Conectó los sensores infrarrojos y los QTR a las borneras. | Evidencia fotográfica y mapa de conexiones pendientes de incorporar. | pendiente: conexiones realizadas, lectura y calibración no reportadas | Requiere integración con la alimentación, el controlador y el cableado del resto del robot. |
| A00574867 | Estructura/mecánica | Diseño CAD de carcasa superior | Trabajó posteriormente en el modelo 3D de la carcasa superior, considerando los espacios para sensores y componentes. | Archivo CAD y revisión identificable pendientes de incorporar. | pendiente: comprobación dimensional; impresión bloqueada por falta de filamento | Requiere comprobar las posiciones reales de los sensores conectados por Erik y conseguir filamento. |

## 3 · Estado de integración V1

| Subsistema | Entrada | Salida esperada | Responsable | Prueba de integración y observación | Evidencia |
|---|---|---|---|---|---|
| Estructura/mecánica | Carcasa existente, ubicación de componentes y diseño CAD | Carcasa superior compatible con la base y con los huecos de sensores | A00574867 | Se avanzó en el diseño 3D. La correspondencia con las medidas físicas y la impresión siguen pendientes. | CAD y capturas pendientes de enlazar. |
| Energía y accionamiento | Motores y cables de conexión | Conductores soldados y posteriormente verificados para accionar los motores desde la XMotion V3 | A00574867 | Se soldaron los cables de los motores. No se reportaron pruebas de continuidad, consumo o giro. | Fotografías pendientes de enlazar. |
| Sensores/percepción | Sensores infrarrojos, QTR y borneras | Conexiones físicas y posterior lectura individual de cada sensor | Erik | Se realizaron las conexiones a las borneras. No se reportaron lecturas ni calibración. | Fotografías y mapa de conexiones pendientes de enlazar. |
| Control/software | XMotion V3 y señales de los sensores | Programa capaz de leer sensores y controlar motores | Responsable por definir | No se reportaron actividades de programación, carga de firmware o pruebas de control durante esta sesión. | Sin evidencia proporcionada. |
| Integración global | Cableado de sensores y motores | Conjunto conectado, verificado y preparado para pruebas funcionales | A00574867 y Erik | Se completó el trabajo de conexiones reportado utilizando herramientas y consumibles alternativos. La integración funcional no ha sido demostrada. | Fotografías del conjunto pendientes de incorporar. |

**Versión identificable:** pendiente de asignar mediante commit y nombre/revisión del archivo CAD. No se proporcionó una versión de firmware.

**Comportamiento que SÍ demuestra V1:** se reporta la ejecución del cableado de sensores a borneras y la soldadura de cables de motores. Esto demuestra avance de montaje, pero todavía no demuestra un comportamiento funcional del robot.

**Lo que aún falla o permanece sin validar:** no se ha reportado un fallo funcional reproducible. Permanecen pendientes la verificación eléctrica, la lectura de sensores, el accionamiento de motores, la comprobación dimensional de la carcasa y su impresión.

## 4 · Protocolo y línea base del robot (datos observados)

No se reportaron ensayos funcionales durante la sesión. Por ello, no existe una línea base cuantitativa del robot.

El protocolo y los datos deberán incorporarse en `pruebas/protocolo.md` y `datos/ensayos.csv` cuando se realicen las pruebas. Los procedimientos indicados a continuación son una propuesta para la siguiente sesión, no pruebas ya ejecutadas.

| Campo de validez experimental | Respuesta obligatoria |
|---|---|
| Pregunta y resultado que se quiere medir | Pendiente de ejecutar: comprobar si las conexiones permiten leer individualmente los 4 QTR y 5 infrarrojos, y accionar los dos motores desde la XMotion V3. |
| Métrica primaria + unidad | No medida. Propuesta: número de canales que responden correctamente respecto al total verificado y resultado de cada comprobación eléctrica. |
| Éxito/fallo (criterio cuantitativo u observable) | Propuesto: cada sensor cambia su lectura ante el estímulo correspondiente y cada motor responde a una orden individual, sin pérdida de conexión ni reinicio del controlador. |
| Lugar, configuración, pista/dohyō/estaciones/marcadores | No registrado. Para la próxima sesión se requiere banco de trabajo y superficie negra/blanca para los QTR. |
| Configuración del robot: batería, firmware y sensores | Plataforma XMotion V3, configuración prevista de 4 QTR y 5 IR. Batería utilizada, modelos exactos, firmware y mapa de pines no registrados para esta sesión. |
| Condiciones controladas: luz, rival, posición de inicio, etc. | No registradas; no se reportaron ensayos. En la siguiente sesión deberán documentarse iluminación, distancia al blanco y altura de los QTR. |
| Número de corridas planeadas / ejecutadas | Planeadas: no registradas. Ejecutadas: 0 reportadas. No se completó la serie de cinco ensayos porque el avance documentado se concentró en montaje y conexiones. |
| Procedimiento reproducible, responsable y seguridad/aborto | Propuesto: con la batería desconectada, revisar polaridad, continuidad y aislamiento; después verificar sensores individualmente y probar motores con ruedas elevadas. A00574867 y Erik deberán acordar responsables. Abortar y desconectar ante calentamiento anormal, humo, olor o movimiento inesperado. No se reportó la ejecución de este procedimiento. |
| Datos sin procesar y video/foto corta | No se proporcionaron mediciones ni registros de pruebas. Fotografías del montaje y enlaces pendientes de incorporar. |

| Ensayo | Condición inicial | Valor (+ unidad) | Éxito/fallo | Observación relevante / incidencia |
|---:|---|---|---|---|
| 1 | No ejecutado | No medido | No evaluado | No se reportó una corrida funcional. |
| 2 | No ejecutado | No medido | No evaluado | No se reportó una corrida funcional. |
| 3 | No ejecutado | No medido | No evaluado | No se reportó una corrida funcional. |
| 4 | No ejecutado | No medido | No evaluado | No se reportó una corrida funcional. |
| 5 | No ejecutado | No medido | No evaluado | No se reportó una corrida funcional. |

**Línea base resumida (no fabricada):** n válido = 0. No es posible calcular media, mediana, dispersión ni tasa de éxito. No hay ensayos descartados reportados; los cinco registros anteriores son espacios de seguimiento y no representan pruebas realizadas.

## 5 · Decisiones al cierre, bloqueos y Kaizen de mañana

| Fallo o cuello de botella observado | Hipótesis preliminar | Prioridad | Responsable | Material / apoyo necesario |
|---|---|---|---|---|
| Falta de tijeras y materiales de montaje, incluido silicón | La preparación del puesto de trabajo no cubrió todos los recursos necesarios. | Alta | A00574867 y Erik | Revisar inventario y preparar herramientas y consumibles antes de la próxima sesión. |
| Necesidad de utilizar recursos alternativos para pelado y aislamiento | La disponibilidad limitada obligó a adaptar el procedimiento de montaje. | Alta | A00574867 y Erik | Pinzas para pelar cables y material de aislamiento adecuado; revisar la cinta aplicada y la sujeción de los cables. |
| Cableado realizado sin validación funcional reportada | El avance se concentró en terminar las conexiones físicas. | Alta | A00574867 y Erik | Multímetro, mapa de conexiones, programa de prueba y alimentación compatible. |
| Medidas exactas y ajuste de la carcasa superior pendientes de comprobar | El modelo CAD debe contrastarse con la base y la posición real de los componentes. | Alta | A00574867 | Calibrador o regla, carcasa física y ubicación definitiva de sensores y conexiones. |
| Falta de filamento para imprimir la carcasa superior | No se contó con el consumible necesario para fabricar la pieza. | Alta para fabricación | Responsable de abastecimiento por definir | Conseguir filamento y confirmar acceso a impresora 3D. |
| Evidencias técnicas y versión identificable sin enlazar | El registro del trabajo aún debe consolidarse en el repositorio. | Media | A00574867 y Erik | Fotografías, archivo CAD, identificación de versión y commit del registro. |

- [ ] Hay prototipo V1, subsistema funcional verificable o fallo reproducible con condiciones registradas.
- [ ] Existen archivos fuente o evidencia técnica enlazada, además de videos de uso controlado cuando correspondan.
- [ ] Hay protocolo reproducible y valores basales con unidad o justificación de lo que no pudo medirse.
- [ ] Cada alumno actualizó su E2 personal con contribución propia y límite de capacidad actual.
- [ ] Se mantuvieron límites de seguridad y protección de datos.

Las casillas permanecen sin marcar hasta verificar sus condiciones. Se documentó el motivo de ausencia de mediciones, pero todavía faltan el protocolo formal, las evidencias y la revisión del equipo.

**Gate E2:** PENDIENTE DE REVISIÓN; no se registra aprobación sin validación docente.  
**Revisor:** pendiente.  
**Fecha:** por confirmar.

**Próxima prioridad de Kaizen 1:** revisar continuidad, polaridad y aislamiento del cableado; comprobar individualmente sensores y motores; verificar las medidas del CAD contra el robot físico y conseguir filamento para imprimir la carcasa superior.

**Enlace al commit/PR:** pendiente de crear y registrar.