# 🧾 APE 6 – Fases 3 y 4: Matriz de hallazgos de usabilidad de CaféU

## 📋 1. Información general

| Campo | Información |
|---|---|
| Actividad | APE6-F3F4-03 · Matriz de hallazgos |
| Proyecto | CaféU |
| Identificadores | H-01 … H-12 (únicos y estables en todos los documentos de la fase) |

**Fuentes de esta matriz:** las cuatro evaluaciones heurísticas independientes ([Viviana](../../Fase2-Pilotaje/Evaluaciones_Heuristicas/Viviana.md), [Wilson](../../Fase2-Pilotaje/Evaluaciones_Heuristicas/Wilson.md), [Sebastián F2](../../Fase2-Pilotaje/Evaluaciones_Heuristicas/Sebastian.md) y [F3](../resultados/heuristica-sebastian.md), [Alex](../../Fase2-Pilotaje/Evaluaciones_Heuristicas/Alex.md)), los registros del pilotaje ([P1](../../Fase2-Pilotaje/Participantes/P1.md), [P2](../../Fase2-Pilotaje/Participantes/P2.md), [P3](../../Fase2-Pilotaje/Participantes/P3.md)) y la evidencia de flujo E-IMG02 ([captura con conexiones](../evidencias/flujo-figma-con-conexiones.png)).

**Documentos hermanos:** el proceso de comparación y consenso está en [consolidacion-heuristicas.md](consolidacion-heuristicas.md); el cruce con los usuarios, en [triangulacion.md](triangulacion.md); las condiciones técnicas y limitaciones (L-xx), en [soporte-tecnico-f3.md](soporte-tecnico-f3.md).

## 📏 2. Convenciones

- **Severidad:** 0 sin problema · 1 cosmético · 2 menor · 3 mayor · 4 crítico · **P/V** pendiente de verificación (evidencia insuficiente para puntuar honestamente).
- **Severidad consensuada:** propuesta fundamentada en la comparación de los cuatro evaluadores; su ratificación se registra en el acta de la revisión grupal ([consolidacion §8](consolidacion-heuristicas.md)). Mientras el acta no exista, se cita como «propuesta».
- **Clasificación (triangulación):** `Ambos` = detectado por inspección heurística y observado en usuarios · `Solo heurística` = detectado por evaluadores, no observado en sesiones · `Solo usuarios` = aparecido en pruebas, no detectado en inspección.
- **Evidencia de usuarios:** se distingue *error no crítico observado (ENC)* de *comentario de cierre*; los comentarios no se convierten retroactivamente en errores de ejecución (criterio de [Resumen_Metricas.md](../../Fase2-Pilotaje/Resumen_Metricas.md)).

## 📊 3. Matriz consolidada

| ID | Hallazgo | Pantalla / componente | Heurísticas | Sev. V / W / A / S | Sev. consensuada (propuesta) | Evidencia heurística | Evidencia de usuarios | Clasificación | Mejora propuesta |
|---|---|---|---|---|:--:|---|---|---|---|
| H-01 | El acceso al pedido no coincide con la convención de ubicación (sin ícono de carrito en cabecera) | Menú · barra flotante / cabecera | H4, H6 | 2 / 2 / 2 / 2 | **2** (unánime, por ratificar) | Viviana H4; Wilson HW-03; Alex H4; Sebastián F3 | P1·T4: ENC, buscó el carrito ~6 s en la cabecera; comentario de cierre | **Ambos** | Acceso dual: ícono de carrito con contador en la cabecera + barra flotante actual |
| H-02 | Retroalimentación poco perceptible al añadir productos | Menú · barra flotante | H1 | 2/3 / 2 / 2 / 2 | **2** (propuesta; Viviana difiere: 2 F2 / 3 EH-03) | Viviana H1/EH-03; Wilson HW-01; Alex H1; Sebastián F3 | P3·T4: ENC, señaló falta de animación/badge (localizó la barra sin problema) | **Ambos** | Realce breve de la barra al actualizar (micro-animación o badge) sin distraer |
| H-03 | «Eliminar» suprime el ítem de inmediato, sin confirmación ni deshacer; control de texto pequeño | Mi Pedido · enlace «Eliminar» | H3, H5, H8 | 2/4 / 2 / 2 / 2 | **2** (propuesta; Viviana difiere: 2 F2 / 4 EH-04) | Viviana H3/H5/EH-04; Wilson HW-02; Alex H3/H5; Sebastián OBS-S01→F3 | P2 y P3: comentarios de cierre (riesgo de toque accidental); P1·T5: «letras chiquitas»; 0 errores en T5 | **Ambos** (evidencia de usuarios = comentarios, no error de ejecución) | Snackbar «Deshacer» temporal o confirmación breve; ampliar área táctil (ref. 44×44 px) |
| H-04 | «Añadir» directo no se diferencia de la personalización en el detalle | Menú · tarjetas / Detalle | H5, H6, H2 | 2/3 / 1 / 2 / 2 | **2** (discrepancia §7.1 consolidación) | Viviana H5/H6/EH-02; Wilson HW-04; Alex H2/H6; Sebastián F3 | P1·T3: ENC, intentó «Añadir», no encontró dónde escribir y retrocedió al detalle | **Ambos** | Etiqueta «Personalizar» / «Ver opciones» en productos con instrucciones especiales |
| H-05 | El campo de búsqueda de Inicio compite con el CTA «Ver Menú» | Inicio · buscador / banner | H6, H8, H5 | 1/2 / 0 / 1–2 / 2 | **2** (discrepancia §7.2 consolidación) | Viviana H8/EH-01; Alex H8 y Hallazgos H01; Sebastián F3 (Wilson no lo registró) | P1·T1: ENC, pulsó el buscador creyendo que debía escribir | **Ambos** | Reforzar jerarquía del CTA; diferenciar el buscador o activarlo solo donde funcione |
| H-06 | Estado de carrito vacío no definido en el flujo | Mi Pedido · estado vacío | H9, H5 | P/V / 1 / 0\* / 1 | **1** diseño (comportamiento P/V) | Wilson HW-05; Viviana H9 (pregunta); Alex H9 (recomienda probar); Sebastián F3 | Ninguna (las tareas no vaciaron el carrito) | **Solo heurística** | Diseñar estado vacío con mensaje y CTA «Explorar menú»; verificar comportamiento real |
| H-07 | Secuencia de estados potencialmente confusa: «Preparando… 50 %» antes de «¡Pedido recibido!» | Estado → Confirmación | H1, H2 | NF / NF / NF / 2 | 2 (propuesta individual, por contrastar) | Sebastián F2 OBS-S02 → F3 (cableado «Tras pausa», E-IMG02) | Ninguna (la versión piloteada no muestra esta pantalla según los registros; L-01) | **Solo heurística** | Reordenar/renombrar estados: confirmación de recepción primero y preparación después; verificar transición |
| H-08 | «Total pagado» en Estado contradice el pago en caja y el «Total a pagar» de Confirmación | Estado · resumen | H2, H4 | NF / NF / NF / 2 | 2 (propuesta individual, por contrastar) | Sebastián F3 (E-IMG02-P05 vs P07) | Ninguna (pantalla no mencionada en registros; L-01) | **Solo heurística** | Cambiar rótulo a «Total a pagar» y unificarlo en todas las pantallas |
| H-09 | Escenarios de error y recuperación no cubiertos (fallo de confirmación, conexión, pedido inválido) | Varias | H9 | P/V / — / 0\* / P/V | **P/V** (vacío de cobertura) | Viviana H9; Alex H9; Sebastián F2/F3 | Ninguna (0 errores críticos; los escenarios no se probaron) | **Solo heurística** | Inspección específica de estados de error; definir mensajes claros con acción de recuperación |
| H-10 | Inconsistencias menores de presentación: posición de la marca en cabecera; chip «Sanduches» sin tilde | Varias / Menú · chips | H4 | NF / NF / NF / 1 | 1 (propuesta individual, por contrastar) | Sebastián F3 (E-IMG02) | Ninguna | **Solo heurística** | Unificar cabecera y corregir «Sánduches» |
| H-11 | Modal de cancelación: texto de consecuencias parcialmente ilegible en la evidencia; destinos por verificar | Modal de cancelación | H3, H5, H9 | NF / NF / NF / P/V | **P/V** (limitación de evidencia) | Sebastián F2 OBS-S03 → F3 (anotación «Tras pausa» oculta el cuerpo; L-06) | Ninguna (la cancelación no formó parte de las tareas) | **Solo heurística** | Captura limpia del modal; verificar que «Volver al pedido» conserva el pedido y «Sí, cancelar» informa consecuencias |
| H-12 | La confirmación no muestra tiempo estimado de preparación en la versión capturada | Confirmación | H1, H10 | NF / NF / NF / 2 cond. | 2 (propuesta individual condicional a L-01) | Sebastián F3 (E-IMG02-P07); antecedente APE 4 (matriz-heuristicas H1) | Ninguna sobre el problema; P1/P2/P3 reportaron y valoraron el tiempo en la versión piloteada | **Solo heurística** | Confirmar versión vigente; si falta el dato, restaurarlo («Listo en ~5–10 min») |

**Leyenda:** V = Viviana · W = Wilson · A = Alex · S = Sebastián (F3). NF = no registrado por ese evaluador. 0\* = «sin evidencia suficiente», no «sin problema» (convención de Alex.md). «1–2» en A para H-05: 1 en su evaluación individual, 2 en Hallazgos_Preliminares.

### Resumen de clasificación

| Clasificación | Hallazgos | Total |
|---|---|:--:|
| Confirmado por ambos métodos | H-01, H-02, H-03, H-04, H-05 | **5** |
| Solo heurística | H-06, H-07, H-08, H-09, H-10, H-11, H-12 | **7** |
| Solo usuarios | — (verificación explícita en [triangulacion §6](triangulacion.md)) | **0** |

## 🗂️ 4. Fichas de hallazgo

Formato de ficha heredado de la [matriz de heurísticas de Fase 1](../../Fase1/evaluacion/matriz-heuristicas.md). Las citas de usuarios son textuales de los registros publicados.

### H-01 — Acceso al pedido fuera de la convención de ubicación

- **Heurísticas:** H4 (consistencia y estándares), H6 (reconocimiento).
- **Pantalla/estado:** Menú con productos agregados; cabecera sin ícono de carrito.
- **Comportamiento observado:** el acceso al pedido vive en la barra flotante inferior («2 ítems · $4.25 · Ver mi pedido →») y en la pestaña «Mi pedido» de la navegación inferior; no existe en la cabecera, donde los usuarios de apps de compra lo esperan.
- **Evidencia heurística:** Viviana (H4=2), Wilson (HW-03=2, cita el estándar de e-commerce), Alex (H4=2), Sebastián F3 (inspección de E-IMG02-P01/P02).
- **Evidencia de usuarios:** P1, T4 (ENC): «miro arriba... no hay carrito... ah, abajo apareció una franja flotante»; búsqueda de ~6 s. Cierre de P1: «pondría también un ícono arriba para encontrarlo más rápido». P2 y P3 localizaron la barra sin dificultad.
- **Severidad:** 2 propuesta (unánime 4/4). Frecuencia: cada revisión del pedido. Impacto: demora leve, sin bloqueo. Persistencia: costo en primeros usos.
- **Mejora:** acceso dual (ícono con contador en cabecera + barra flotante), manteniendo consistencia visual.
- **Estado:** listo para backlog; ratificación grupal pendiente.

### H-02 — Retroalimentación poco perceptible al añadir

- **Heurísticas:** H1 (visibilidad del estado).
- **Pantalla/estado:** Menú, al pulsar «Añadir».
- **Comportamiento observado:** la cantidad y el total se actualizan en la barra inferior sin un distintivo de cambio observable (badge, realce). La dinámica exacta no es verificable en la captura (L-02/L-04).
- **Evidencia heurística:** Viviana (H1=2), Wilson (HW-01=2), Alex (H1=2), Sebastián F3.
- **Evidencia de usuarios:** P3, T4 (ENC según registro): «notó que la barra flotante negra no tiene una animación de rebote o badge numérico destacado al sumar ítems, aunque la localizó sin problemas». *Nota metodológica:* la comparación de Fase 2 cuestionó si esta observación debe contar como ENC; el dato se conserva tal como fue registrado y se marca la duda.
- **Severidad:** 2 propuesta (unánime 4/4). Frecuencia: cada adición. Impacto: duda leve. Persistencia: cada compra.
- **Mejora:** micro-animación de realce o badge temporal al actualizar la barra.
- **Estado:** listo para backlog; verificar dinámica real en Figma.

### H-03 — Eliminación inmediata sin recuperación y control pequeño

- **Heurísticas:** H3 (control y libertad), H5 (prevención), H8 (jerarquía/tamaño).
- **Pantalla/estado:** Mi Pedido, enlace «Eliminar» junto a cada ítem.
- **Comportamiento observado:** el flujo no ofrece confirmación ni «Deshacer»; el control es un texto subrayado gris, de menor jerarquía que precios y steppers.
- **Evidencia heurística:** Viviana (H3=2, H5=2), Wilson (HW-02=2), Alex (H3=2, H5=2), Sebastián (OBS-S01 en F2 → 2 en F3).
- **Evidencia de usuarios:** cierre de P2: «borra el ítem de inmediato sin pedir confirmación... un usuario descuidado podría hacer clic por error». Cierre de P3: «es un texto plano pequeño; a veces con el pulgar es fácil presionar sin querer... mejor un ícono de basurero con un área táctil más amplia o un diálogo rápido». P1, T5: «al ladito dice en letras chiquitas "Eliminar"». **0 errores registrados en T5 por los tres participantes.**
- **Severidad:** 2 propuesta (unánime 4/4). Frecuencia: cada eliminación. Impacto: costo de recuperación (re-añadir y reconfigurar). Persistencia: no se mitiga con aprendizaje. Cláusula de escalado a 3 si se observan eliminaciones accidentales.
- **Mejora:** snackbar «Deshacer» (p. ej., 4 s) o confirmación breve; ampliar área táctil y separar de controles contiguos.
- **Estado:** listo para backlog (el riesgo está respaldado por 2/3 usuarios + 4/4 evaluadores).

### H-04 — Añadir directo vs. personalización

- **Heurísticas:** H5, H6, H2.
- **Pantalla/estado:** tarjetas del Menú y Detalle de producto.
- **Comportamiento observado:** «Añadir» agrega sin pasos; las instrucciones especiales solo existen en el Detalle, sin indicación en la tarjeta.
- **Evidencia heurística:** Viviana (H5=2, H6=1), Wilson (HW-04=1), Alex (H2=2, H6=2), Sebastián F3 (2).
- **Evidencia de usuarios:** P1, T3 (ENC): «si le doy a Añadir se añade de una... no, mejor toco la tarjeta... ¡ahí sí!, se abrió la pantalla de Detalle».
- **Severidad:** 2 propuesta; discrepancia documentada (Wilson 1). Frecuencia: cada personalización. Impacto: retroceso y riesgo de perder la instrucción. Persistencia: aprendible.
- **Mejora:** etiqueta «Personalizar» o «Ver opciones» en productos que admiten instrucciones; diferenciar visualmente ambas acciones.
- **Estado:** listo para backlog tras ratificar la severidad en la revisión grupal.

### H-05 — Buscador de Inicio compite con «Ver Menú»

- **Heurísticas:** H6, H8, H5.
- **Pantalla/estado:** Inicio, primer contacto.
- **Comportamiento observado:** el campo de búsqueda («¿Qué se te antoja hoy?» en la captura; «Buscar café, snacks...» en la versión piloteada) ocupa una posición prominente y sugiere escribir; la acción que avanza es «Ver Menú». En la captura el buscador no tiene conexión (L-04).
- **Evidencia heurística:** Viviana (H8=1), Alex (H8=1; Hallazgos H01=2), Sebastián F3 (2); Wilson no lo registró (H8=0).
- **Evidencia de usuarios:** P1, T1 (ENC): «intento buscar aquí en la barrita... ah no, aquí abajo hay un botón negro grande que dice "Ver Menú"».
- **Severidad:** 2 propuesta; discrepancia documentada (0/1/2). Frecuencia: primer uso. Impacto: paso equivocado breve. Persistencia: un solo uso.
- **Mejora:** reforzar la jerarquía del CTA; condicionar el buscador a que funcione o reducir su prominencia en Inicio.
- **Estado:** listo para backlog tras ratificar la severidad.

### H-06 — Carrito vacío sin estado definido

- **Heurísticas:** H9, H5.
- **Pantalla/estado:** Mi Pedido con 0 ítems (no representado en el flujo).
- **Comportamiento observado:** no existe pantalla/variante de estado vacío en E-IMG02; se desconoce si «Confirmar pedido» se inhabilitaría.
- **Evidencia heurística:** Wilson (HW-05=1), Viviana (H9, pregunta abierta), Alex (H9 0\* con recomendación de probar), Sebastián F3 (1 diseño / P/V comportamiento).
- **Evidencia de usuarios:** ninguna; T5 dejó un ítem y ninguna tarea vació el carrito.
- **Severidad:** 1 propuesta (vacío de diseño); comportamiento P/V.
- **Mejora:** estado vacío con mensaje amigable y CTA «Explorar menú»; bloquear confirmación sin ítems.
- **Estado:** verificación funcional previa; luego backlog.

### H-07 — Secuencia de estados del pedido

- **Heurísticas:** H1, H2.
- **Pantalla/estado:** Estado de pedido → Confirmación (transición automática «Tras pausa»).
- **Comportamiento observado:** tras confirmar, el usuario ve «Preparando tu pedido… 50 %» y luego «¡Pedido recibido!»; la recepción se comunica después de la preparación. La barra fija en 50 % es limitación del prototipo (L-03), no se puntúa como error de usuario.
- **Evidencia heurística:** Sebastián (OBS-S02 en F2 → hallazgo concreto en F3 con E-IMG02-P05/P07 y el cableado).
- **Evidencia de usuarios:** ninguna; los registros de T6 no mencionan la pantalla de estado (diferencia de versión, L-01).
- **Severidad:** 2 propuesta individual, pendiente de contraste grupal y verificación interactiva.
- **Mejora:** comunicar primero la recepción («Pedido recibido») y después la preparación; hacer que el progreso refleje estados reales o eliminar el porcentaje ficticio.
- **Estado:** verificación + contraste grupal antes de backlog.

### H-08 — «Total pagado» antes de pagar

- **Heurísticas:** H2, H4.
- **Pantalla/estado:** Estado de pedido, resumen.
- **Comportamiento observado:** P05 rotula «Total pagado $4.25» mientras P04 informa «Paga al retirar tu pedido. Sin cobro en la app.» y P07 usa «Total a pagar».
- **Evidencia heurística:** Sebastián F3 (E-IMG02-P05 vs P07).
- **Evidencia de usuarios:** ninguna (pantalla no mencionada en los registros; L-01).
- **Severidad:** 2 propuesta individual. Frecuencia: cada pedido. Impacto: malentendido sobre dinero. Persistencia: constante.
- **Mejora:** unificar el rótulo «Total a pagar» en estado y confirmación.
- **Estado:** verificación de versión + contraste grupal antes de backlog.

### H-09 — Escenarios de error no cubiertos

- **Heurísticas:** H9.
- **Pantalla/estado:** todo el flujo (estados de fallo no representados).
- **Comportamiento observado:** el flujo capturado no define mensajes ni recuperación ante fallo de confirmación, pérdida de conexión o pedido inválido.
- **Evidencia heurística:** Viviana (H9 P/V), Alex (H9 0\* + recomendación), Sebastián (H9 parcial en F2, P/V en F3).
- **Evidencia de usuarios:** ninguna; 0 errores críticos en 18 ejecuciones, pero los escenarios de error no formaron parte de las tareas.
- **Severidad:** P/V. No se asigna 0 (no probado ≠ inexistente) ni 3 (no demostrado).
- **Mejora:** recorrer/provocar los estados de error disponibles; definir mensajes en lenguaje claro con acción de recuperación que conserve el pedido.
- **Estado:** tarea de verificación asignable en la revisión grupal; no es todavía una corrección de backlog.

### H-10 — Inconsistencias menores de presentación

- **Heurísticas:** H4.
- **Pantalla/estado:** cabeceras de P01–P07; chips del Menú.
- **Comportamiento observado:** marca «CaféU» a la izquierda en P01/P02/P05/P07 y a la derecha en P03/P04; chip «Sanduches» sin tilde frente a «Sánduche»/«Sánduches».
- **Evidencia heurística:** Sebastián F3 (E-IMG02).
- **Evidencia de usuarios:** ninguna.
- **Severidad:** 1 propuesta individual (cosmético, sin impacto en tarea).
- **Mejora:** unificar posición de marca y corregir la tilde.
- **Estado:** backlog menor tras contraste grupal.

### H-11 — Modal de cancelación por verificar

- **Heurísticas:** H3, H5, H9.
- **Pantalla/estado:** Modal «¿Deseas cancelar tu pedido?».
- **Comportamiento observado:** el modal existe con salidas «Volver al pedido» y «Sí, cancelar» (mecanismo correcto de prevención); el cuerpo del texto está parcialmente oculto por la anotación «Tras pausa» en la evidencia (L-06) y los destinos de ambos botones no están confirmados.
- **Evidencia heurística:** Sebastián (OBS-S03 en F2 → H-11 en F3).
- **Evidencia de usuarios:** ninguna; la cancelación no se incluyó en las seis tareas.
- **Severidad:** P/V (limitación de evidencia, no defecto demostrado).
- **Mejora:** captura limpia; verificar que «Volver al pedido» conserva el pedido y que «Sí, cancelar» explica las consecuencias en lenguaje claro.
- **Estado:** tarea de verificación; no es corrección de backlog hasta comprobar el comportamiento.

### H-12 — Tiempo estimado ausente en la confirmación capturada

- **Heurísticas:** H1, H10.
- **Pantalla/estado:** Confirmación.
- **Comportamiento observado:** E-IMG02-P07 no muestra tiempo de preparación; la matriz de tareas T6 y los registros P1–P3 sí lo incluyen («5 a 10 minutos») para la versión piloteada. APE 4 ya había registrado esta ausencia como observación (matriz-heuristicas, fila H1).
- **Evidencia heurística:** Sebastián F3 + antecedente APE 4.
- **Evidencia de usuarios:** ninguna sobre el problema (probaron otra versión); P3 valoró el dato: «el tiempo de 5 a 10 minutos te permite calcular si alcanzas a retirar antes de que empiece tu clase».
- **Severidad:** 2 propuesta condicional (3 si el equipo pondera el objetivo «pedir sin comunicación verbal» como esencial).
- **Mejora:** confirmar la versión vigente; si el dato falta, restaurarlo junto a las instrucciones de retiro.
- **Estado:** verificación de versión (L-01) + contraste grupal antes de backlog.

## 🎯 5. Priorización para el backlog (criterio de evidencia suficiente)

| Grupo | Hallazgos | Criterio | Acción |
|---|---|---|---|
| **Listos para backlog (prioridad alta)** | H-01, H-02, H-03 | Severidad unánime 4/4 + evidencia de usuarios (ENC o comentarios de 2/3) | Diseñar e implementar en la siguiente iteración |
| **Listos para backlog (prioridad media)** | H-04, H-05 | Evidencia doble (heurística + usuarios); severidad con discrepancia documentada | Ratificar severidad en revisión grupal y pasar a backlog |
| **Backlog menor** | H-10 | Evidencia visual directa; cosmético | Corregir junto a otros cambios de UI |
| **Verificación previa requerida** | H-06, H-09, H-11 | Vacíos de diseño/cobertura sin comportamiento comprobado | Asignar verificación funcional; no son correcciones hasta comprobar |
| **Condicionados a versión + contraste grupal** | H-07, H-08, H-12 | Hallazgos nuevos de F3 sobre la captura; L-01 sin resolver | Confirmar versión vigente y contrastar con los otros evaluadores |

Esta priorización es coherente con la de Fase 2 ([Hallazgos_Preliminares §4](../../Fase2-Pilotaje/Hallazgos_Preliminares.md)): acceso/feedback del carrito y eliminación protegida primero; personalización y jerarquía de Inicio después. Ningún hallazgo P/V se propone como corrección implementable sin la verificación previa: **no se infla el backlog con problemas no demostrados**.

## ✅ 6. Control de consistencia

- Los identificadores H-01…H-12 se usan de forma idéntica en [heuristica-sebastian.md](../resultados/heuristica-sebastian.md), [consolidacion-heuristicas.md](consolidacion-heuristicas.md), [triangulacion.md](triangulacion.md) y este documento.
- Las severidades por evaluador coinciden con las publicadas en sus documentos (trazabilidad en [consolidacion §5–6](consolidacion-heuristicas.md)).
- Las citas de usuarios son textuales de P1.md, P2.md y P3.md; los conteos (18/18 tareas, 4 ENC, 0 EC, SUS 82,5) coinciden con [Resumen_Metricas.md](../../Fase2-Pilotaje/Resumen_Metricas.md).
- Ningún hallazgo carece de fuente: cada fila remite a un documento individual, a un registro de participante o a la evidencia E-IMG02.

---