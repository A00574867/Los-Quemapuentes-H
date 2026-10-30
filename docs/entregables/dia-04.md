---
kaizen_dojo: "2026"
formato: "Entregable diario G2"
evidencia: "E4"
dia: 4
responsable_registro: "equipo"
estado: "EN_PROCESO"
fecha: "POR_CONFIRMAR"
revision_docente: "PENDIENTE"
---

# E4 · Día 4 — ITERAR | Kaizen 2, robustez y preparación de demostración

> Registro del trabajo reportado por A00574867 y Erik. Las observaciones de montaje se distinguen de las mediciones y pruebas funcionales. Los enlaces, versiones y resultados no proporcionados quedan pendientes de incorporar.

## 0 · Contexto

**Fecha y dōjō:** pendientes de confirmar.

**Equipo/misión:** Los Quemapuentes-H / M01 · Mini-sumo autónomo con XMotion V3.

**Versiones trazables:** V1: conexiones iniciales de D2, identificador pendiente; K1: modificaciones de D3, identificador pendiente; K2: reorganización mecánica y eléctrica de D4 y código para 4 IR y 2 sensores de borde, identificador pendiente.

## 1 · Ruta de actividades del Día 4 (180 min)

Los intervalos corresponden a la planeación del formato. No se registraron tiempos reales por actividad.

| Actividad | Minutos | Registro requerido |
|---|---:|---|
| Revisión por pares y retroalimentación | 0–20 | A00574867 y Erik revisaron las conexiones y su distribución dentro del minisumo. No se reportó una revisión de otro equipo ni retroalimentación externa. |
| Diseño/ejecución Kaizen 2 | 20–70 | Se mejoraron las conexiones y se introdujeron dentro del robot. Se cambió la base inferior para obtener más espacio y se incorporó la pieza superior impresa en 3D, que facilitó el acceso. Se utilizaron segueta y taladro para habilitar espacios de paso o alojamiento de conexiones. |
| Comparación V1–K1–K2 | 70–115 | Se observó una mejora cualitativa en el alojamiento y accesibilidad del cableado. No se proporcionaron mediciones ni ensayos equivalentes para comparar las tres versiones. |
| Ensayo de robustez | 115–145 | Se identificaron una soldadura débil en un motor, atribuida a un cable mal pelado; un problema descrito como falta de corriente que motivó el cambio de motor; y poca precisión de las ruedas. No se documentó una perturbación controlada ni un ensayo formal de robustez. |
| Preparación de demo | 145–165 | Se creó código para 4 sensores IR y 2 sensores de borde, denominados QTR por el equipo, y se ajustó la distancia de detección de los IR. Valores, procedimiento y validación pendientes de documentar. |
| Gate de preparación | 165–180 | Preparación con restricciones: faltan la verificación de soldaduras y accionamiento, la revisión de las ruedas y la validación funcional del código y los sensores. Revisión docente pendiente. |

## 2 · Revisión por pares

Esta sección registra revisión interna. No se atribuyen observaciones a un equipo externo no identificado.

| Persona o equipo observador (alias) | Evidencia revisada | Observación útil / pregunta | Respuesta técnica y decisión | Cambio aceptado o descartado |
|---|---|---|---|---|
| A00574867 y Erik · revisión interna | Montaje físico y distribución del cableado; fotografías pendientes de enlazar | El cableado requería más espacio y mejor acceso dentro del robot. | Se reorganizaron las conexiones, se cambió la base inferior y se incorporó la pieza superior impresa en 3D. | Aceptado y realizado. |
| A00574867 y Erik · revisión interna | Unión de cable con uno de los motores | Se identificó una soldadura débil asociada con un cable mal pelado. | Queda pendiente documentar su reparación y verificar continuidad, aislamiento y sujeción. | Corrección necesaria; cierre pendiente de confirmar. |
| A00574867 y Erik · revisión interna | Accionamiento del robot; registro de prueba pendiente | Se reportó un problema descrito como falta de corriente. | Se cambió el motor. La causa eléctrica no se considera confirmada porque no se proporcionaron mediciones de corriente o voltaje. | Cambio de motor realizado; resultado posterior pendiente de registrar. |
| A00574867 y Erik · revisión interna | Ruedas y comportamiento mecánico; evidencia pendiente | Se observó poca precisión en las ruedas. | Se planteó sustituirlas por unas de metal y revisar ajuste al eje, alineación y dimensiones. | Sustitución propuesta, no confirmada como realizada. |

**Acuerdo de colaboración:** ambos integrantes trabajaron en la mejora de conexiones y montaje. La distribución exacta de las tareas de D4 y la forma de revisión cruzada quedan pendientes de registrar. Cada integrante deberá explicar y documentar sus propias modificaciones y revisar con su compañero las interfaces afectadas.

## 3 · Segundo ciclo Kaizen (K2)

| Campo experimental | Completar |
|---|---|
| Limitación o nueva oportunidad detectada en K1 | Dificultad para alojar y acceder al cableado dentro del minisumo. Durante D4 también se identificaron problemas de soldadura, accionamiento y precisión de ruedas. |
| Hipótesis K2 y fundamento | Si se reorganiza el cableado y se adapta la estructura para proporcionar más espacio y acceso, entonces será posible alojar las conexiones dentro del robot y facilitar su revisión, porque disminuirán las interferencias físicas entre cables y componentes. |
| Variable modificada y controles | Se modificaron la distribución del cableado, la base inferior y los espacios de montaje, incorporando además la pieza superior impresa. Se cambiaron también un motor y el código. Al existir varios cambios simultáneos, no puede aislarse la contribución de cada uno. Para comparaciones posteriores deberán mantenerse iguales batería, superficie, configuración y procedimiento. |
| Requisitos de seguridad antes del cambio | Desconectar la batería antes de soldar o mecanizar. Retirar o proteger la electrónica frente a virutas, sujetar las piezas al usar segueta y taladro, eliminar rebabas y revisar que los nuevos bordes no dañen cables. Verificar aislamiento y polaridad antes de energizar. El cumplimiento de estas acciones no se documentó en el reporte proporcionado. |
| Personas responsables y alcances implicados | A00574867 y Erik: integración eléctrica, montaje mecánico y control. Distribución individual de D4 pendiente de especificar. |
| Cambio exacto de código/CAD/configuración | Reorganización y alojamiento interno de conexiones; sustitución de base inferior; incorporación de pieza superior impresa en 3D; habilitación de espacios con segueta y taladro; sustitución de un motor; creación de código para 4 IR y 2 sensores de borde; ajuste reportado de la distancia de detección IR. Archivo, valores y método de ajuste pendientes de incorporar. |
| Enlace a commit, PR y versión K2 | Pendiente de incorporar. Conservar código y CAD anteriores antes de registrar K2. |
| Métrica, unidad y criterio para declarar éxito | Propuesta: conexiones alojadas respecto al total revisado; número de cables prensados o sometidos a tensión; tiempo de acceso al conector de alimentación en segundos. Criterio: cableado alojado sin interferencias, conexiones accesibles y ausencia de contacto con partes móviles. No se proporcionaron valores medidos. |

**Aclaración sobre sensores:** se conserva la denominación “QTR” usada en el reporte. El modelo exacto de los dos sensores de borde deberá confirmarse en el inventario y en el código.

**Aclaración sobre distancia IR:** se reportó un ajuste, pero no se indicó la distancia inicial, final ni si se realizó físicamente en el sensor o mediante cambios de lógica. La distancia real deberá verificarse con un blanco y una regla; no se infiere únicamente del programa.

## 4 · Comparación de evolución

Los siguientes registros organizan condiciones de comparación. No representan cinco ensayos ejecutados.

| Ensayo/condición equivalente | V1 (valor + unidad) | K1 (valor + unidad) | K2 (valor + unidad) | Incidencias o validez |
|---:|---|---|---|---|
| 1 · Alojamiento del cableado | Sin medición registrada; conexiones iniciales realizadas en D2. | Sin medición registrada; revisión y extensión de cable reportadas en D3. | Se reportó que las conexiones pudieron introducirse dentro del minisumo. Cantidad y porcentaje no registrados. | Comparación cualitativa; estructura y distribución cambiaron simultáneamente. |
| 2 · Acceso a conexiones | Tiempo no medido. | Tiempo no medido. | Mayor accesibilidad reportada con la pieza superior impresa. Tiempo no medido. | No existe procedimiento equivalente documentado para medir el acceso. |
| 3 · Integridad del cableado de motor | Sin medición registrada. | Se reportó una soldadura para extender un cable. | Se detectó una soldadura débil asociada con pelado deficiente. | No se confirmó si corresponde a la misma unión de D3. Reparación y medición pendientes. |
| 4 · Accionamiento y trayectoria | Sin medición registrada. | Compilación del programa de motores reportada; sin datos físicos comparables. | Cambio de motor y poca precisión de ruedas reportados. Corriente, velocidad y desviación no medidas. | Motor y montaje diferentes; no permite atribuir resultados a una sola modificación. |
| 5 · Sensores y programa | Sin datos funcionales registrados. | Compilación de programas de sensores reportada. | Código creado para 4 IR y 2 sensores de borde; ajuste de distancia IR reportado. Distancia en cm no registrada. | Configuración modificada; falta documentar lecturas, umbrales, distancias y pruebas de borde. |

**Registros fuente:** [`datos/ensayos.csv`](../../datos/ensayos.csv) y [`pruebas/protocolo.md`](../../pruebas/protocolo.md). Actualización pendiente de verificar.

**Síntesis (método, n, media/mediana, dispersión y éxito cuando proceda):** n válido de comparaciones cuantitativas V1–K1–K2 = 0. No se dispone de datos para calcular medias, medianas, dispersión o tasas de éxito. Se cuenta con observaciones cualitativas de montaje y problemas identificados.

**¿Qué mejora, qué empeora y qué no podemos concluir?** Mejoraron, según lo reportado, el alojamiento interno y el acceso al cableado. Se identificaron debilidades de soldadura y precisión de ruedas, pero no puede afirmarse que fueran causadas por K2. Tampoco puede concluirse que el cambio de motor resolvió el problema eléctrico o que el ajuste IR alcanzó una distancia concreta.

## 5 · Ensayo de robustez o variación de condiciones

No se reportó un ensayo controlado de robustez. Se proponen las siguientes comprobaciones para la próxima sesión:

| Cambio controlado de entorno (luz, suelo, batería, posición, rival, obstáculo o carga) | Riesgo y límite seguro | Predicción | Resultado / unidad / éxitos | ¿Se mantiene el objetivo? | Evidencia |
|---|---|---|---|---|---|
| Propuesto: cinco ciclos de acceso a conexiones y colocación de la carcasa, con batería desconectada | Evitar prensar cables, forzar conectores o dañar la LiPo. Detener ante interferencia física. | La distribución K2 permitirá acceder y volver a montar sin desplazar conexiones. | No ejecutado o no reportado; registrar ciclos correctos/5 e incidencias. | Pendiente de evaluar. | Fotografías y registro pendientes. |
| Propuesto: verificar cada IR con el mismo blanco a distancias definidas | Mantener motores deshabilitados y controlar posición e iluminación. | El ajuste permitirá detección repetible en el intervalo requerido. | No medido; registrar distancia en cm y detecciones por repetición. | Pendiente de evaluar. | CSV y video pendientes. |
| Propuesto: comprobar sensores de borde en negro y blanco, inicialmente con ruedas elevadas | No iniciar pruebas libres hasta verificar respuesta de escape y paro. | Ambos sensores distinguirán las superficies y activarán la respuesta correspondiente. | No medido; registrar lecturas y resultado por sensor. | Pendiente de evaluar. | CSV y video pendientes. |
| Propuesto: recorrido recto sobre la misma superficie tras verificar motor y ruedas | Área despejada y paro accesible. Detener ante desprendimiento, bloqueo o calentamiento anormal. | Un montaje alineado y firme reducirá desviaciones e irregularidades de desplazamiento. | No medido; registrar distancia recorrida y desviación lateral en cm. | Pendiente de evaluar. | Registro y video pendientes. |

**Límites de inferencia:** no existen resultados de robustez aportados. Los cambios de base, motor, cableado y programa impiden una atribución causal directa. Se deberá fijar una configuración K2, identificarla y repetir las pruebas bajo condiciones documentadas. Una rueda de metal no garantiza por sí sola mejor precisión: deben verificarse geometría, ajuste y superficie de contacto.

## 6 · Ensayo general de demostración

Guion propuesto para D5; no se registra como ensayo general ejecutado. Los responsables deben confirmar esta distribución.

| Segmento | Qué se demostrará en 20–60 s | Integrante responsable | Versión/código usado | Material requerido | Plan B ante fallo |
|---|---|---|---|---|---|
| Inicio / contexto | Explicar el objetivo del minisumo y los cambios de montaje entre D2 y D4. | A00574867, propuesto | Fotografías y CAD identificados; referencias pendientes. | Robot, imágenes y modelo de carcasa. | Explicar con imágenes y piezas sin energizar. |
| Prueba principal | Mostrar lectura de IR y sensores de borde; añadir movimiento solo después de validar accionamiento y paro. | Erik, propuesto | Programa K2 para 4 IR y 2 sensores de borde; commit pendiente. | Robot verificado, batería compatible, blanco y superficie negra/blanca. | Presentar lecturas con motores deshabilitados o un video real previamente validado, si se dispone de él. |
| Evidencia de mejora | Mostrar que el cableado está alojado y accesible, explicando el cambio de base y la pieza superior impresa. | A00574867, propuesto | Montaje K2 y fotografías de versiones anteriores. | Robot desconectado y evidencias de montaje. | Presentar fotografías comparativas, distinguiendo observaciones de mediciones. |
| Defensa de fronteras | Explicar los límites actuales: soldadura, diagnóstico eléctrico, ruedas y distancia IR pendiente de medir. | A00574867 y Erik, propuesto | Registro E4 y datos disponibles al momento. | Bitácora, código y protocolo. | Delimitar lo comprobado y presentar el plan de validación pendiente. |

**¿Robolympics es el evento externo posterior?** Por confirmar. D5 se documentará como demostración/calificación interna mientras no se confirme otro alcance. No se registra participación externa como realizada.

## 7 · Gate E4

- [ ] Existe un ciclo K2 explícito, con hipótesis, modificación y datos.
- [ ] Se conservan V1, K1, K2 y, en su caso, reversiones para reproducibilidad.
- [ ] Se efectuó una prueba de robustez documentada o se justificó por qué no era segura/factible.
- [ ] El equipo tiene guion, responsabilidades y plan de contingencia para D5.
- [ ] Cada participante actualizó [E4 personal](../../participantes/_plantilla/dias/E4.md).

Las modificaciones y la hipótesis están documentadas, pero faltan datos cuantitativos, versiones identificables y evidencia de robustez. El guion anterior es una propuesta pendiente