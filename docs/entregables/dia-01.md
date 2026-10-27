---
kaizen_dojo: "2026"
formato: "Entregable diario G2"
evidencia: "E1"
dia: 1
responsable_registro: "equipo"
estado: "PENDIENTE"
fecha: "2026-10-26"
revision_docente: "PENDIENTE"
---

# E1 · Día 1 — ATREVERSE | Contrato de misión, inventario y dōjō

> **Regla:** sustituir los corchetes, registrar lo realmente observado y enlazar a evidencias del repositorio. **No inventar datos ni marcar pruebas no realizadas.** Los archivos del equipo resumen el trabajo compartido; las reflexiones y evidencias personales van en `participantes/<alias>/dias/E1.md`.

## 0 · Identificación, equipo y logística del dōjō

| Campo obligatorio | Dato |
|---|---|
| Fecha y horario de esta sesión | [2026-10-26; 9:00–12:00, 180 min] |
| Nombre / alias del equipo | Los Quemapuentes H |
| Misión / plataforma | [M01 mini-sumo autónomo] |
| Objetivo verificable del robot (una frase) | [Acción + condiciones + éxito] |
| **Dōjō asignado — campus, edificio y sala/taller exactos** | **[León/ CTA / Sala de electrónica/ Nº de laboratorio 1]** |
| Puesto o zona dentro del dōjō | [Mesa, banco, espacio de vuelo, pista, dohyō o estación] |
| Horario / reserva confirmada | [Fechas y bloque horario; quien la autorizó] |
| Responsable del espacio y contacto institucional | [Nombre/cargo y canal institucional, sin publicar teléfonos privados] |
| Acceso, aforo y ajustes de accesibilidad | [Restricciones de ingreso, capacidad, adecuaciones necesarias] |
| Salidas, botiquín, extintor y punto de reunión | [Ubicación real validada al llegar] |
| Zonas segregadas por riesgo | [Vuelo / herramientas / tránsito AMR / ensayo de pista] |
| Ubicación de materiales y resguardo nocturno | [Gabinete/estante/inventario; responsable] |
| Plan de sustitución si falla el espacio | [Dōjō alternativo con autorización; no improvisar espacio de vuelo] |
| Instructor o supervisor presente en la sesión | [@alias / nombre institucional] |

> ⛔ **No se permite avanzar a pruebas físicas sin dōjō concreto y autorización del responsable.** No inventar salón, número de laboratorio ni recursos que no hayan sido confirmados.

## 1 · Integrantes, responsabilidades, accesibilidad y decisiones (0–15 min)

| Alias GitHub | Rol inicial | Carta y frontera (D/S/E; F1–F4) | Alcances ID (1–3) | Kit personal (archivo) | Necesidad de apoyo o accesibilidad acordada |
|---|---|---|---|---|---|
  | [@A00574867] | [Integración / documentación / seguridad / pruebas ...] | [D · F1 · D1] | [MS01, MS02] | [`../../participantes/alias/compromiso.md`](../../participantes/_plantilla/compromiso.md) | [Acordar con la persona sin registrar datos sensibles] |
| [@alias-2] | [...] | [...] | [...] | [enlace] | [...] |

**Acuerdo de colaboración:** [Cómo se toman decisiones, cómo se resuelven conflictos, apoyos senpai–kōhai, pausas y distribución equitativa de participación.]

## 2 · Demostración de la plataforma y seguridad (15–35 min)

| Elemento | Observación directa | Evidencia / vínculo |
|---|---|---|
| Plataforma base inspeccionada (estado, modelo, ID inventario) | [ ] | [enlace / foto no sensible] |
| Funciones existentes y límites comprobados | [ ] | [enlace] |
| Paro de emergencia / desconexión segura ensayados | [ ] | [enlace / tutor responsable] |
| Restricciones de competición o exhibición verificadas | [ ] | [fuente / por verificar] |
| Riesgos vistos y medidas activas | [ ] | [docs/seguridad.md] |

**Normas específicas según misión:**
- **M01:** protecciones de alimentación; desarmar motores antes de tocar ruedas; dohyō delimitado, rival de referencia y bordes seguros.
- **M03:** pista despejada, altura/posición de sensores controlada, baterías y ruedas comprobadas.
- **M04:** espacio interior autorizado, observador humano, altura y desplazamientos limitados, baterías y aterrizaje inmediato; *verificar modelo real de Tello*.
- **M05:** ROS 2 y TF/navegación listos; límites de velocidad, sensor de obstáculos, paro seguro y zona de tránsito marcada.

## 3 · Diagnóstico práctico colectivo (35–65 min)

**Condición inicial V0 de la plataforma:** [Robot completo / kit / subensambles / simulador; qué funciona y qué falta]

| Prueba diagnóstica | Condición y procedimiento | Resultado observado / unidad | Problema / causa probable | Evidencia |
|---|---|---|---|---|
| [1: movimiento o comunicación] | [...] | [...] | [...] | [enlace] |
| [2: lectura de sensor] | [...] | [...] | [...] | [enlace] |
| [3: comportamiento de la misión] | [...] | [...] | [...] | [enlace] |

**Capacidades ya disponibles y dependencias:** [qué módulos se pueden reutilizar, y qué necesita cada alcance de otro integrante.]

## 4 · Integración de Mission Forge C2 y pacto de alcances (65–100 min)

Cada participante debe colocar el archivo **Markdown original generado por la web** en:

`participantes/<alias>/compromiso.md`

Se conserva íntegro (incluido el frontmatter y la lista de katas). Los nuevos alcances/katas diseñados por el participante quedan claramente marcados como *propuesta propia* y requieren aprobación técnica.

**Catálogo de referencia:** [Google Sheets C2](https://docs.google.com/spreadsheets/d/1FKxFzoyu9KJb3RlOwB609vliS5hAtmwWFu2G2zG3Ky4/edit) · **Configurador Mission Forge:** [`herramientas/mission-forge-c2.html`](../../herramientas/mission-forge-c2.html) (descárgalo y ábrelo en el navegador; funciona sin Internet).

| Alias | Kit enlazado | Alcance principal | Complementos | Katas elegidos o nuevos | Horas mín.–máx. | Evidencia final esperada | Negociación aprobada |
|---|---|---|---|---|---|---|---|
| [A00574867] | [https://github.com/A00574867/Los-Quemapuentes-H/blob/main/participantes/_plantilla/Compromiso_A00574867] | [MS01] | [MS02 / ninguno] | [K1, K3 / propio] | [6–8 h] | [CAD ensamblado + prueba] | [Sí / Pendiente; revisor] |
| A00574506 | enlace | [MS01] | [MS02 / ninguno] | [K1, K3 / propio] | [6–8 h] | [CAD ensamblado + prueba] | [Sí / Pendiente; revisor] |

**Resultado de negociación grupal:** [Puntos de integración; interfaces entre códigos/firmware/sensores/estructura; prioridad si no hay tiempo.]

## 5 · Inventario exhaustivo y especificación de materiales

### 5.1 Inventario maestro del equipo

Inventario correspondiente a la misión **M01 · Mini-sumo autónomo**.

Los materiales disponibles fueron confirmados por el integrante que los posee. Su disponibilidad no implica que se haya validado su funcionamiento o compatibilidad.

**Convenciones:**
- **P/C:** por confirmar.
- **D1:** revisión de componentes, diseño y compatibilidad.
- **D2:** montaje, conexiones y primeras pruebas.
- **D3:** calibración y pruebas de combate.
- Los días son etapas de trabajo; las fechas de calendario están pendientes.
- En los recursos sin disponibilidad confirmada se usa **falta**, hasta verificar su compra o préstamo.
- No hay recursos reservados confirmados.

| ID | Categoría | Material o recurso (especificación exacta: modelo, medida, versión o característica) | Cantidad requerida + unidad | Cantidad confirmada | Fuente/proveedor o dueño | Ubicación física o ruta digital | Responsable | Estado (disponible/reservado/falta) | Alternativa compatible | Día requerido |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| MAT-001 | Estructura | Parte del chasis impresa en 3D; material, dimensiones y archivo CAD P/C | 1 pieza | 1 pieza | Integrante del equipo; dueño P/C | P/C | Encargado de mecánica P/C | disponible | Reimpresión a partir del CAD validado | D1 |
| MAT-002 | Estructura | Parte restante del chasis; geometría y material compatibles con MAT-001 | 1 pieza | 0 piezas | Servicio de impresión o laboratorio P/C | P/C | Encargado de mecánica P/C | falta | Rediseño de la pieza conservando las fijaciones y dimensiones permitidas | D2 |
| MAT-003 | Mecánica | Placa de latón; espesor, dimensiones, masa y función como cuña o lastre P/C | 1 pieza | 1 pieza | Integrante del equipo; dueño P/C | P/C | Encargado de mecánica P/C | disponible | Pieza equivalente según función, masa y reglamento | D1 |
| MAT-004 | Mecánica | Ruedas; diámetro, ancho, material y acoplamiento al eje P/C | 4 piezas, según diseño actual | 4 piezas | Integrante del equipo; dueño P/C | P/C | Encargado de mecánica P/C | disponible | Ruedas con acoplamiento y dimensiones compatibles | D1 |
| MAT-005 | Actuadores | Motores; modelo, cantidad, reductora, voltaje, RPM y corriente de bloqueo P/C | P/C según transmisión | Disponibles; cantidad P/C | Integrante del equipo; dueño P/C | P/C | Encargado de electrónica P/C | disponible | Motorreductores compatibles con ruedas, driver y batería | D1 |
| MAT-006 | Mecánica | Soportes de motores, acopladores y elementos de transmisión; diseño P/C | 1 juego según montaje | P/C | Laboratorio o proveedor P/C | P/C | Encargado de mecánica P/C | falta | Soportes impresos o comerciales compatibles | D2 |
| MAT-007 | Mecánica / consumibles | Tornillos, tuercas, arandelas, separadores y fijaciones; medidas según CAD | 1 juego según montaje | P/C | Ferretería o laboratorio P/C | P/C | Encargado de mecánica P/C | falta | Fijaciones equivalentes verificadas en el montaje | D2 |
| MAT-008 | Controlador | Placa XMotion ya soldada y con borneras; modelo, revisión, alimentación y capacidad de salidas P/C | 1 placa | 1 placa | Integrante del equipo; dueño P/C | P/C | Encargado de electrónica P/C | disponible | Controlador con suficientes entradas y salidas, compatible con sensores y motores | D1 |
| MAT-009 | Electrónica de potencia | Driver para motores; verificar primero si está integrado en la XMotion y si soporta la corriente requerida | P/C; externo solo si es necesario | Ningún driver externo confirmado | Proveedor P/C | P/C | Encargado de electrónica P/C | falta | Driver integrado de XMotion, si se valida su capacidad | D1 |
| MAT-010 | Sensores de borde | Sensores reflectivos QTR; modelo, alimentación, tipo de salida y montaje P/C | 4 piezas | 4 piezas | Integrante del equipo; dueño P/C | P/C | Encargado de electrónica P/C | disponible | Sensores reflectivos compatibles con la placa y la superficie del dohyō | D2 |
| MAT-011 | Sensores de rival | Sensores infrarrojos para detectar al oponente; modelo, alcance, alimentación y salida P/C | 5 piezas | 0 piezas | Proveedor P/C | P/C | Encargado de electrónica P/C | falta | Sensores de distancia compatibles con las entradas disponibles | D2 |
| MAT-012 | Mecánica | Soportes para sensores QTR y sensores de rival; altura y orientación según diseño | 1 juego para 9 sensores | P/C | Impresión 3D o laboratorio P/C | P/C | Encargado de mecánica P/C | falta | Soportes ajustables compatibles | D2 |
| MAT-013 | Alimentación | Batería LiPo; número de celdas, voltaje, capacidad, descarga, dimensiones y conector por definir según motores y placa | 1 batería | 0 baterías | Proveedor P/C | P/C | Encargado de electrónica P/C | falta | Otra LiPo que cumpla los requisitos eléctricos y de espacio | D2 |
| MAT-014 | Alimentación | Cargador balanceador compatible con la LiPo seleccionada y fuente de alimentación si la requiere | 1 conjunto | P/C | Proveedor o laboratorio P/C | P/C | Encargado de electrónica P/C | falta | Préstamo de cargador compatible verificado | D2 |
| MAT-015 | Protección eléctrica | Fusible y portafusible; corriente nominal según consumo y cableado | 1 conjunto | P/C | Proveedor P/C | P/C | Encargado de electrónica P/C | falta | Protección equivalente dimensionada para el sistema | D2 |
| MAT-016 | Paro / alimentación | Interruptor general o desconexión accesible; capacidad acorde con la corriente del robot | 1 conjunto | P/C | Proveedor P/C | P/C | Encargado de electrónica P/C | falta | Conector de desconexión accesible y adecuado para la corriente | D2 |
| MAT-017 | Cableado | Cables de potencia y señal; calibre, longitud y aislamiento según corriente y distribución | 1 juego según montaje | P/C | Proveedor o laboratorio P/C | P/C | Encargado de electrónica P/C | falta | Cable equivalente con capacidad eléctrica suficiente | D2 |
| MAT-018 | Conectores | Conectores para batería, motores y sensores; tipos y polaridad P/C | 1 juego según montaje | Borneras instaladas en XMotion; resto P/C | Proveedor o laboratorio P/C | P/C | Encargado de electrónica P/C | falta | Conectores compatibles, polarizados y asegurados | D2 |
| MAT-019 | Consumibles | Estaño, flux, termorretráctil, cinchos y cinta aislante | 1 juego | P/C | Laboratorio o proveedor P/C | P/C | Encargado de montaje P/C | falta | Consumibles equivalentes aptos para electrónica | D2 |
| MAT-020 | Herramientas | Cautín con soporte, pinzas, cortador y pelacables | 1 juego | P/C | Laboratorio o integrantes P/C | P/C | Encargado de montaje P/C | falta | Estación de soldadura y herramientas equivalentes | D2 |
| MAT-021 | Herramientas | Destornilladores, llaves y herramientas para ajustar o fabricar la placa de latón | 1 juego según fijaciones y proceso | P/C | Laboratorio o integrantes P/C | P/C | Encargado de mecánica P/C | falta | Servicio de fabricación del laboratorio | D1–D2 |
| MAT-022 | Instrumentos | Multímetro para continuidad, polaridad y voltaje; medición de corriente solo dentro de su capacidad | 1 instrumento | P/C | Laboratorio o integrantes P/C | P/C | Encargado de electrónica P/C | falta | Instrumento equivalente adecuado para las mediciones | D1–D3 |
| MAT-023 | Instrumentos | Báscula y calibrador o regla para verificar masa, dimensiones y montaje | 1 juego | P/C | Laboratorio o integrantes P/C | P/C | Encargado de mecánica P/C | falta | Instrumentos con resolución suficiente para el reglamento | D1–D3 |
| MAT-024 | Fabricación | Impresora 3D y filamento compatible con el diseño; tecnología y material P/C | Acceso a 1 impresora y material suficiente | P/C | Laboratorio o servicio externo P/C | P/C | Encargado de mecánica P/C | falta | Servicio externo de impresión | D1–D2 |
| MAT-025 | Cómputo / software | Computadora con puerto de comunicación, software CAD e IDE compatible con el modelo de XMotion; SO y versiones P/C | 1 equipo con software instalado | P/C | Integrante o laboratorio P/C | P/C | Encargado de programación P/C | falta | Equipo equivalente con herramientas y controladores compatibles | D1 |
| MAT-026 | Programación / conectividad | Cable de datos y controladores para programar la XMotion; interfaz y conector P/C | 1 conjunto | P/C | Integrante o proveedor P/C | P/C | Encargado de programación P/C | falta | Interfaz de programación admitida por el fabricante | D1–D2 |
| MAT-027 | Firmware / datos | Código fuente, mapa de pines, bibliotecas, parámetros de sensores y versión de firmware | 1 conjunto versionado | P/C | Desarrollo del equipo | Repositorio; rutas P/C | Encargado de programación P/C | falta | Firmware mínimo de pruebas compatible con la placa | D2 |
| MAT-028 | Documentación | Fichas técnicas, diagrama eléctrico, CAD, reglamento y registros de pruebas | 1 conjunto | P/C | Fabricantes, organización y equipo | Repositorio; rutas P/C | Responsable de documentación P/C | falta | Copias locales verificadas de la documentación | D1–D3 |
| MAT-029 | Red / colaboración | Acceso a internet para consultar documentación y sincronizar el repositorio; operación autónoma sin red prevista | 1 acceso durante preparación | P/C | Institución o integrante P/C | P/C | Encargado de programación P/C | falta | Documentación, instaladores y repositorio disponibles sin conexión | D1 |
| MAT-030 | Zona de pruebas | Dohyō o superficie de ensayo; diámetro, altura, acabado y borde según reglamento | 1 área de ensayo | P/C | Laboratorio o equipo P/C | P/C | Responsable de pruebas P/C | falta | Superficie provisional para calibración; validación final en dohyō reglamentario | D2–D3 |
| MAT-031 | Referencia de ensayo | Robot rival o blanco de referencia con dimensiones y superficie documentadas | 1 unidad | P/C | Equipo o laboratorio P/C | P/C | Responsable de pruebas P/C | falta | Blanco móvil para detección y objeto de prueba para empuje | D3 |
| MAT-032 | Medición / datos | Cronómetro o video y bitácora para registrar detección, escape del borde y resultados | 1 conjunto | P/C | Integrante del equipo P/C | Repositorio; ruta P/C | Responsable de pruebas P/C | falta | Teléfono con video y registro manual | D3 |
| MAT-033 | Seguridad | Gafas para fabricación, ventilación de soldadura, protección de carga LiPo y área despejada | 1 conjunto; gafas por operador | P/C | Laboratorio o equipo P/C | P/C | Responsable de seguridad P/C | falta | Área equipada del laboratorio | D1–D3 |
| MAT-034 | Seguridad / ensayo | Soporte estable para probar ruedas elevadas y procedimiento de paro documentado | 1 soporte y 1 procedimiento | P/C | Equipo o laboratorio P/C | Zona de pruebas; ruta del procedimiento P/C | Responsable de pruebas P/C | falta | Banco de pruebas que impida desplazamientos accidentales | D2 |

**Nota sobre el driver:** MAT-009 no implica una compra obligatoria. Primero se identificará la XMotion y se comprobará si su etapa de potencia puede manejar los motores seleccionados. Si cumple, se registrará como disponible e integrado en MAT-008.

**Nota sobre cantidades:** no se ha confirmado la cantidad de motores. Las cuatro ruedas disponibles no determinan por sí solas cuántos motores requiere el diseño.

El archivo [`datos/inventario_materiales.csv`](https://github.com/A00574867/Los-Quemapuentes-H/blob/main/datos/inventario_materiales.csv) deberá mantenerse sincronizado con este inventario.

### 5.2 Lista de cotejo específica por plataforma

**Misión seleccionada: M01 · Mini-sumo autónomo.**

| Elemento | Situación actual | Verificación pendiente |
| --- | --- | --- |
| Chasis y cuña | Parte del chasis impresa y placa de latón disponibles | Confirmar dimensiones, masa, material de impresión, función del latón y fabricar la parte restante |
| Ruedas, motores y soportes | 4 ruedas y motores disponibles | Contar motores; registrar modelo, voltaje, reductora, RPM, corriente de bloqueo y compatibilidad mecánica |
| Driver | Necesidad de driver externo por confirmar | Identificar la etapa de potencia de la XMotion y compararla con los requisitos de los motores |
| Controlador | XMotion soldada y con borneras disponible | Registrar modelo, revisión, alimentación, mapa de pines y entradas disponibles |
| Firmware | Disponibilidad y versión P/C | Preparar pruebas individuales, detección del borde, búsqueda del rival, ataque y paro |
| Batería, cargador y protección | LiPo pendiente; cargador y protecciones sin confirmar | Seleccionar componentes compatibles con motores, placa, espacio y consumo |
| Sensores de borde | 4 QTR disponibles | Confirmar modelo, salida, altura de montaje y calibración sobre negro y blanco |
| Sensores de rival | 5 infrarrojos pendientes | Definir modelo, alcance, orientación, alimentación y compatibilidad de señales |
| Cableado y conectores | Borneras de XMotion confirmadas; resto P/C | Definir calibres, conectores, polaridad, aislamiento y sujeción |
| Dohyō y rival de referencia | Sin disponibilidad confirmada | Conseguir área de ensayo y referencia para detección y empuje |
| CAD, impresión y herramientas | Acceso P/C | Revisar CAD y reservar fabricación y herramientas antes del montaje |
| Instrumentos | Disponibilidad P/C | Conseguir multímetro, báscula y herramienta de medición dimensional |
| Seguridad y paro | Implementación pendiente | Definir desconexión accesible, pruebas con ruedas elevadas y procedimiento de manejo de LiPo |
| Reglamento | Documento aplicable P/C | Verificar dimensiones, masa, arranque y restricciones antes de cerrar el diseño |

**Enlaces a fichas técnicas e instrucciones:**

Se incorporarán después de identificar los modelos reales. No se considerará validada una conexión únicamente por el aspecto o nombre comercial del componente.

| Documento requerido | URL o ruta |
| --- | --- |
| Manual y ficha técnica de la XMotion | Pendiente de identificar modelo |
| Ficha técnica de los motores | Pendiente de identificar modelo |
| Ficha técnica de los QTR | Pendiente de identificar modelo |
| Ficha técnica de sensores infrarrojos | Pendiente de seleccionar modelo |
| Manual de batería y cargador | Pendiente de seleccionar modelos |
| Diagrama eléctrico y mapa de pines | Pendiente de elaborar |
| Archivos CAD y de impresión | Pendiente de confirmar rutas |
| Reglamento de competencia | Pendiente de obtener |
| Procedimiento de pruebas y paro | Pendiente de elaborar |

### 5.3 Riesgos de recursos y abastecimiento

| Bloqueante | A qué alcance afecta | Solución prevista / fecha y responsable | Impacto si no se resuelve |
| --- | --- | --- | --- |
| Modelo y capacidad de XMotion sin identificar | Alimentación, programación y control de motores | Registrar modelo y consultar documentación en D1; encargado de electrónica P/C | No se puede cerrar el diagrama ni decidir si se requiere driver externo |
| Cantidad y especificaciones de motores sin registrar | Transmisión, batería y driver | Contar e identificar motores; verificar datos eléctricos y mecánicos en D1; responsables de mecánica y electrónica P/C | Selección de componentes y montaje pendientes |
| Batería LiPo pendiente | Funcionamiento autónomo | Seleccionar y conseguir batería después de validar motores y placa, antes de D2; encargado de electrónica P/C | No se pueden realizar pruebas autónomas |
| Cargador y protecciones sin confirmar | Carga y alimentación del robot | Conseguir cargador compatible, protección y desconexión antes de D2; encargado de electrónica P/C | No se autoriza la prueba alimentada con LiPo |
| Cinco sensores de rival pendientes | Búsqueda y ataque autónomos | Seleccionar modelos compatibles y conseguirlos antes de D2; encargado de electrónica P/C | Solo podrán probarse funciones que no requieran detección del rival |
| Parte de la carcasa sin imprimir | Integración y fijación de componentes | Validar CAD e imprimir antes del montaje de D2; encargado de mecánica P/C | Montaje final incompleto |
| Modelos y calibración de QTR pendientes | Detección del borde | Identificar sensores y calibrarlos sobre la superficie de ensayo en D2; responsables de electrónica y programación P/C | Riesgo de salida del dohyō; no realizar combate hasta validar |
| Masa y dimensiones sin verificar | Cumplimiento del reglamento | Obtener reglamento y medir conjunto, incluyendo latón y batería, en D1 y al terminar montaje; encargado de mecánica P/C | Posible necesidad de rediseño |
| Herramientas e instrumentos sin confirmar | Fabricación y verificación | Confirmar préstamo o disponibilidad antes de D2; encargado de montaje P/C | Retraso del montaje y de las comprobaciones eléctricas |
| Dohyō y rival de referencia sin confirmar | Validación del comportamiento | Gestionar área y referencia antes de D3; responsable de pruebas P/C | Pruebas parciales; desempeño de combate sin validar |
| Firmware y mapa de pines sin confirmar | Integración de sensores y actuadores | Documentar conexiones e implementar pruebas por subsistema en D2; encargado de programación P/C | No se puede validar el funcionamiento autónomo |

**Materiales completos para ejecutar el Día 2:** Parcial.

Hay componentes principales disponibles, pero faltan la batería LiPo, los cinco sensores de rival y la parte restante de la carcasa. También deben confirmarse el cargador, las protecciones, el montaje y la necesidad de driver externo.

**Confirmado por:** pendiente de revisión del docente y del responsable del equipo.  
**Fecha y hora de confirmación:** pendientes.
**Enlaces a fichas técnicas / instrucciones de conexión, fabricación y seguridad:** [URLs o rutas dentro del repositorio.]

### 5.4 Riesgos de recursos y abastecimiento

| **Bloqueante** | **A qué alcance afecta** | **Solución prevista / fecha y responsable** | **Impacto si no se resuelve** |
| --- | --- | --- | --- |
| Batería LiPo pendiente | Alimentación y funcionamiento autónomo | Seleccionar una batería compatible con los motores y la XMotion; conseguirla antes del Día 2. Responsable: encargado de electrónica, por definir. | No se podrán realizar pruebas autónomas del robot. |
| Cinco sensores infrarrojos pendientes | Detección del oponente y estrategia de ataque | Verificar compatibilidad y adquirir los cinco sensores antes del Día 2. Responsable: encargado de electrónica, por definir. | No se podrá validar la búsqueda y el ataque al rival. |
| Parte restante de la carcasa sin imprimir | Ensamble y sujeción de componentes | Revisar el diseño e imprimir la pieza antes del Día 2. Responsable: encargado de mecánica, por definir. | El montaje quedará incompleto y se retrasarán las pruebas de desplazamiento. |
| Necesidad de driver externo sin confirmar | Control y alimentación de los motores | Identificar el modelo de XMotion y verificar si su driver integrado, si lo tiene, soporta los motores; adquirir uno externo solo si es necesario. Revisar en el Día 1. Responsable: encargado de electrónica, por definir. | No se podrá completar la conexión y validación de los motores. |
| Especificaciones de los motores sin registrar | Selección de batería, driver y transmisión | Confirmar cantidad, voltaje, corriente de bloqueo, reductora y dimensiones durante el Día 1. Responsable: encargado de electrónica y mecánica, por definir. | Se retrasará la selección de componentes compatibles. |
| Cargador LiPo y protecciones sin confirmar | Carga y pruebas eléctricas | Conseguir cargador balanceador compatible, protección eléctrica y desconexión accesible antes del Día 2. Responsable: encargado de electrónica, por definir. | No se podrán realizar las pruebas con LiPo de forma segura. |
| Compatibilidad y calibración de los cuatro QTR pendientes | Detección del borde del dohyō | Identificar el modelo, comprobar conexiones y calibrar sobre la superficie de ensayo durante el Día 2. Responsable: encargado de programación, por definir. | El robot podría salir del dohyō; las pruebas de combate quedarán pendientes. |
| Montaje de motores, ruedas y placa de latón sin validar | Tracción, estabilidad y cumplimiento del reglamento | Revisar fijaciones, alineación, masa y dimensiones antes de las pruebas de movimiento. Responsable: encargado de mecánica, por definir. | Podrían requerirse ajustes o reimpresión de piezas. |
| Dohyō y rival de prueba sin confirmar | Validación de detección, escape del borde y empuje | Gestionar un espacio de ensayo y un rival o blanco de referencia antes del Día 3. Responsable: encargado de pruebas, por definir. | Solo se podrán realizar pruebas parciales del funcionamiento. |

## 6 · Kata 0 — exploración técnica de arranque (100–160 min)

| Integrante/alcance | Pregunta técnica | Mini-prueba o prototipo de exploración | Resultado o error observado | Evidencia enlazada | Acción necesaria antes de D2 |
|---|---|---|---|---|---|
| [@alias / ID] | [qué quiero verificar] | [qué hice] | [qué ocurrió] | [commit/foto/log] | [acción] |
| [@A00574867 | [Horarios para realizar modificaciones y/o conexiones al diseño del minisumo] | [Organizar los tiempos de acuerdo al diagrama, así como los horarios máximos de finalización de la modificación del minisumo] | [Pude organizarme mejor] | [https://app.notion.com/library/recents?spaceId=03f40535ed71811dbf1f0003b6f41898&p=40540535ed718007a7c1f25ce417ba5f&pm=s&pvs=140] | [Definir horarios de trabajo y fechas límite para cada modificación del minisumo, y registrarlos en el cronograma del equipo antes del Día 2.] |

**Integración entre subequipos:** [Qué interfaz se dejó validada: alimentación, dimensiones, tópicos, salida sensorial, etc.]

## 7 · Cierre: contrato técnico y puerta de salida E1 (160–180 min)

- [ ] El objetivo colectivo tiene condición de éxito verificable.
- [ ] Cada estudiante depositó **su kit Markdown original** en `participantes/<alias>/compromiso.md`.
- [ ] Cada estudiante completó [E1 personal](../../participantes/_plantilla/dias/E1.md) y definió frontera, evidencia y alcance negociado.
- [ ] El inventario está **completo** y cada recurso indica cantidad, especificación, disponibilidad y responsable.
- [ ] Se asignó **dōjō específico** con edificio, salón/taller, horarios, supervisión y autorización.
- [ ] Se inspeccionaron riesgos, paro y condiciones de seguridad de la plataforma.
- [ ] Se identificaron dependencias y bloqueos del Día 2; están bajo control o se ajustó la misión.
- [ ] El profesor aprobó el alcance y la seguridad, o registró observaciones y una alternativa viable.

**Estado del gate:** [APROBADO / APROBADO CON CONDICIONES / REPLANIFICAR].

**Condiciones, responsables, fecha y próxima decisión:** [ ... ]

**Revisor docente:** [ ... ] · **Enlace a commit/PR:** [ ... ]

**Criterio mínimo E1:** existe un contrato de misión y frontera individual, hay evidencia del punto de partida, un inventario verificable y un espacio de trabajo autorizado. La ausencia de algún material crítico NO debe esconderse.
