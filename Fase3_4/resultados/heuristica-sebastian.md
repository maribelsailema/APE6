# ☕ APE 6 – Fases 3 y 4: Evaluación heurística individual de CaféU — Sebastián Santana

## 📋 1. Información general

| Campo | Información |
|---|---|
| Universidad | Universidad Técnica de Ambato – FISEI |
| Carrera | Ingeniería de Software · Quinto semestre |
| Asignatura | Interacción Humano-Computador |
| Actividad | APE6-F3F4-03 · Evaluación heurística individual |
| Proyecto | CaféU |
| Responsable | Santana Durán Sebastián Israel |
| Rol | Soporte técnico y consolidación heurística |
| Rama | `feature/ape6-f3f4-heuristicas` |
| Instrumento base | [Procedimiento de evaluación heurística (Fase 1)](../../Fase1/evaluacion/evaluacion-heuristica.md) y [matriz de heurísticas (Fase 1)](../../Fase1/evaluacion/matriz-heuristicas.md) |
| Antecedente individual | [Evaluación visual de Fase 2 (Sebastian.md)](../../Fase2-Pilotaje/Evaluaciones_Heuristicas/Sebastian.md) |

## 🎯 2. Objetivo

Inspeccionar personalmente el prototipo CaféU contra las diez heurísticas de Nielsen, identificar problemas de interacción, documentar la pantalla o componente afectado, asignar severidades justificadas mediante frecuencia, impacto y persistencia, y proponer mejoras con evidencia adjunta.

Esta evaluación es **independiente**: las severidades se asignan por criterio de inspección propio. Los datos de los participantes P1–P3 no se utilizan para puntuar; el cruce con las pruebas con usuarios se realiza por separado en [triangulacion.md](../docs/triangulacion.md).

## 🔗 3. Objeto de evaluación y evidencia

**Prototipo:** [CaféU en Figma](https://www.figma.com/proto/mmnzX5MbN4kv4IhYOqlQR8/cafeU_prototipo?node-id=3-1700&p=f&scaling=min-zoom&content-scaling=fixed&page-id=0%3A1&starting-point-node-id=3%3A1700) (enlace publicado en el README del repositorio; verificación de disponibilidad en [soporte-tecnico-f3.md](../docs/soporte-tecnico-f3.md)).

### Pantallas del flujo (códigos heredados de la Fase 2)

| Código | Pantalla | Función |
|---|---|---|
| P01 | Inicio | Presentar CaféU y dar acceso al menú. |
| P02 | Menú | Catálogo con filtros, precios y acción «Añadir». |
| P03 | Detalle de producto | Descripción, cantidad e instrucciones especiales. |
| P04 | Mi Pedido | Revisión, cantidades, eliminación y total. |
| P05 | Estado de pedido | Seguimiento del pedido confirmado. |
| P06 | Modal de cancelación | Confirmación previa a cancelar el pedido. |
| P07 | Confirmación | Comunicación de pedido recibido y datos de retiro. |

### Evidencias utilizadas

| Código | Evidencia | Ubicación |
|---|---|---|
| E-IMG01 | Captura general de las siete pantallas (Fase 2). | [evidencias/flujo_cafeu-7-pantallas.png](../../Fase2-Pilotaje/Evaluaciones_Heuristicas/evidencias/flujo_cafeu-7-pantallas.png) |
| E-IMG02 | Captura del flujo de Figma **con las conexiones de prototipado visibles** (aporte de esta fase). | [evidencias/flujo-figma-con-conexiones.png](../evidencias/flujo-figma-con-conexiones.png) |

E-IMG02 corresponde al mismo contenido visual que E-IMG01 (mismas pantallas y textos), pero muestra el cableado del prototipo: nodos de origen, flechas de destino y la transición automática etiquetada «Tras pausa». Esto permite evaluar, además del diseño estático, la **navegación prototipada** entre pantallas.

**Limitación de la evidencia:** una captura no permite verificar animaciones, recálculo de totales, comportamiento de componentes interactivos (steppers, campos de texto), navegación por teclado ni adaptación responsive. Todo juicio que dependa de ello queda marcado como pendiente. Las diferencias entre esta captura y los textos citados en los registros del pilotaje están documentadas como limitación técnica L-01 en [soporte-tecnico-f3.md](../docs/soporte-tecnico-f3.md).

## 🧭 4. Método y escala

Se siguió el procedimiento de la Fase 1: recorrido del flujo principal (Inicio → Menú → Detalle → Mi Pedido → Estado → Confirmación) y de las rutas de retorno y cancelación, revisando cada pantalla contra las diez heurísticas. La severidad se asigna con la escala 0–4 de la Fase 1, considerando **impacto, frecuencia esperable, persistencia, recuperación y alcance**:

| Valor | Interpretación |
|---:|---|
| 0 | No representa un problema. |
| 1 | Cosmético: defecto menor que no afecta significativamente la tarea. |
| 2 | Menor: duda, fricción o demora leve; la persona puede continuar. |
| 3 | Mayor / importante: confusión considerable o error probable; recuperación con esfuerzo. |
| 4 | Crítico: bloquea una tarea principal o causa una consecuencia grave sin recuperación razonable. |
| P/V | Pendiente de verificación: la evidencia disponible no permite puntuar honestamente. |

Los identificadores H-XX remiten a la [matriz de hallazgos consolidada](../docs/matriz-hallazgos.md).

## 🚶 5. Recorrido documentado del flujo

Observaciones verificables en E-IMG02 (detalle del cableado en [soporte-tecnico-f3.md](../docs/soporte-tecnico-f3.md)):

1. **P01 Inicio:** saludo «Hola, Julia», campo de búsqueda «¿Qué se te antoja hoy?», banner «Evita la fila» con CTA «Ver Menú» (conectado a P02), explicación en tres pasos, horario de la cafetería y navegación inferior (Inicio · Menú · Mi pedido) con conexiones.
2. **P02 Menú:** chips «Todos», «Bebidas calientes», «Sanduches»; cuatro productos (Café americano $1.50, Sánduche $2.75, Capuchino $2.00, Galleta $1.25) con botón «Añadir» cada uno; la tarjeta del café está conectada a P03; barra flotante «2 ítems · $4.25 · Ver mi pedido →» conectada a P04. **No se observan conexiones desde los botones «Añadir»** ni desde el buscador.
3. **P03 Detalle:** retroceso «‹» conectado a P02; categoría, nombre, precio y descripción; stepper de cantidad «− 1 +»; «Instrucciones especiales (Opcional)» con ejemplo «Ej. Sin azúcar, por favor.» y contador que aparenta **0/120**; CTA «Añadir al pedido · $1.50» conectado a P04.
4. **P04 Mi Pedido:** dos ítems con stepper y enlace de texto «Eliminar» (subrayado, gris, de menor jerarquía que precios y controles); «+ Seguir comprando»; resumen Subtotal/Total $4.25; aviso «Pago en caja — Paga al retirar tu pedido. Sin cobro en la app.»; CTA «Confirmar pedido · $4.25» conectado a P05. **No se observan conexiones desde «Eliminar» ni desde los steppers.** El retroceso «‹» parece apuntar a P03 (verificación pendiente).
5. **P05 Estado de pedido:** «Preparando tu pedido…», barra de progreso fija en 50 %, número #CU-104, resumen y **«Total pagado $4.25»**; «Cancelar pedido» conectado a P06; «Volver al inicio» conectado a P01; transición automática **«Tras pausa»** hacia P07.
6. **P06 Modal de cancelación:** «¿Deseas cancelar tu pedido?» con cuerpo de texto parcialmente oculto por la anotación «Tras pausa» de la captura; botones «Volver al pedido» y «Sí, cancelar», ambos con nodo de conexión (destinos aparentes: P04 y P01; verificación pendiente).
7. **P07 Confirmación:** distintivo de verificación (círculo negro con check blanco), «¡Pedido recibido! Tu próxima pausa ya está en marcha. Nos vemos en la cafetería.», tarjeta «TU NÚMERO DE PEDIDO #CU-104», resumen «2 ítems · **Total a pagar** $4.25», instrucción «Retira y paga en caja» y CTA «Volver al inicio» conectado a P01. **No se muestra tiempo estimado de preparación.**

## 🔟 6. Evaluación de las diez heurísticas

### H1. Visibilidad del estado del sistema

**Evidencia:** P02 (barra flotante con cantidad y total), P05 (mensaje de preparación, barra de progreso, número de pedido), P07 (distintivo de éxito, número y resumen). E-IMG02-P02, P05, P07.

**Aspectos favorables:** existen mecanismos de estado en las tres etapas clave del pedido; el número #CU-104 se repite en P05 y P07, lo que permite identificar el pedido sin memoria adicional.

**Problemas identificados:**

- **H-02 · Retroalimentación poco perceptible al añadir (P02).** La barra flotante es el único indicador contextual del carrito en el catálogo y no presenta distintivo de cambio (badge, realce) observable en la captura. *Severidad: 2 (menor).* **Frecuencia:** en cada adición de producto. **Impacto:** el usuario puede dudar de si el producto se agregó; demora leve, no bloqueo. **Persistencia:** se repite en cada compra; la animación no es verificable estáticamente (por eso el realce se evalúa como diseño visible, no como comportamiento). **Recuperación:** inmediata al mirar la barra. **Alcance:** acción esencial (revisar el pedido).
- **H-07 · Secuencia de estados potencialmente confusa (P05 → P07).** Tras «Confirmar pedido», el flujo muestra «Preparando tu pedido… 50 %» y, mediante una transición automática «Tras pausa», llega a «¡Pedido recibido!». Semánticamente, la recepción del pedido se comunica *después* de su preparación, lo que puede hacer dudar de si el pedido fue aceptado o de si el estado retrocedió. *Severidad propuesta: 2 (menor).* **Frecuencia:** en cada pedido confirmado. **Impacto:** confusión sobre el estado real; no impide completar la tarea. **Persistencia:** estructural del flujo, no se aprende a evitar. **Nota:** la barra fija en 50 % es una limitación del prototipo (L-03), no un error del usuario; el problema puntuado es la semántica de la secuencia. Verificación interactiva pendiente.
- **H-12 · La confirmación no muestra tiempo estimado (P07).** La versión capturada no informa cuándo estará listo el pedido; los registros del pilotaje y la matriz de tareas T6 sí lo incluyen («5 a 10 minutos»), y en APE 4 ya se registró esta ausencia como observación. *Severidad propuesta: 2 (menor), condicionada a confirmar la versión vigente (L-01).* **Frecuencia:** en cada pedido. **Impacto:** el estudiante no puede planificar su retiro «entre clases» sin preguntar al personal, lo que debilita el objetivo central de CaféU (pedir sin comunicación verbal). **Persistencia:** constante. Si el equipo pondera ese objetivo como esencial, podría justificarse 3; se deja como punto de discusión grupal.

**Resultado:** heurística parcialmente satisfecha; tres problemas registrados (2, 2 propuesto, 2 propuesto).

### H2. Correspondencia entre el sistema y el mundo real

**Evidencia:** vocabulario de cafetería en todas las pantallas («Menú», «Mi Pedido», «Pago en caja», «Retira y paga en caja»), precios en dólares junto a cada producto, ejemplo de instrucción «Ej. Sin azúcar, por favor.». E-IMG02-P02…P07.

**Aspectos favorables:** terminología cotidiana y coherente con el contexto universitario; el aviso «Sin cobro en la app» anticipa la duda más frecuente sobre el pago.

**Problemas identificados:**

- **H-08 · «Total pagado» contradice el modelo de pago (P05).** El estado del pedido rotula el resumen como «Total pagado $4.25» cuando el pago aún no ocurrió (P04: «Paga al retirar tu pedido. Sin cobro en la app.»; P07: «Total a pagar»). El usuario puede creer que ya se le cobró. *Severidad propuesta: 2 (menor).* **Frecuencia:** en cada pedido confirmado. **Impacto:** malentendido sobre una cuestión de dinero; se resuelve leyendo P07, pero genera desconfianza. **Persistencia:** constante en P05; además es inconsistente con P07 (ver H4). Verificación de versión pendiente (L-01).
- **H-07** (compartida con H1): la secuencia «Preparando…» → «¡Pedido recibido!» no sigue el orden temporal que el usuario espera de un pedido de cafetería.

**Resultado:** terminología general correcta; dos problemas localizados de semántica de estados y etiquetas.

### H3. Control y libertad del usuario

**Evidencia:** retrocesos «‹» en P03 y P04; «+ Seguir comprando» en P04; «Cancelar pedido» en P05 con modal de confirmación en P06 («Volver al pedido» / «Sí, cancelar»); «Volver al inicio» en P05 y P07; steppers y «Eliminar» en P04. E-IMG02-P03…P06.

**Aspectos favorables:** el flujo ofrece salidas en todas las etapas; la cancelación del pedido completo exige confirmación previa, y el modal ofrece una salida segura («Volver al pedido»).

**Problemas identificados:**

- **H-03 · Eliminación de ítems sin confirmación ni deshacer (P04).** El enlace «Eliminar» es la única vía para retirar un ítem y el flujo capturado no muestra ningún mecanismo de recuperación (ni confirmación, ni snackbar «Deshacer», ni estado intermedio). Evolución de mi observación OBS-S01 de Fase 2: el control se confirma visualmente pequeño y de baja jerarquía, y la ausencia de recuperación se confirma a nivel de diseño de flujo. *Severidad: 2 (menor).* **Frecuencia:** en cada eliminación. **Impacto:** un toque accidental obliga a volver al catálogo y reconfigurar el producto (incluida cualquier instrucción especial). **Persistencia:** se repite mientras exista el control; no se mitiga con el aprendizaje. **Recuperación:** posible pero con costo de pasos. **Alcance:** acción esencial de modificación del pedido. No se asigna 3 porque la recuperación es sencilla y la evidencia estática no demuestra eliminaciones accidentales reales; si la verificación interactiva o una nueva prueba las muestra, corresponde reevaluar a 3.
- **H-11 · Consecuencias de la cancelación no legibles en la evidencia (P06).** El cuerpo del modal está parcialmente oculto por la anotación «Tras pausa»; no puede verificarse qué informa al usuario sobre la pérdida de los productos seleccionados. *Severidad: P/V.* Es una limitación de la evidencia (L-06), no un defecto demostrado del diálogo. Acción: captura limpia y recorrido interactivo.

**Observación técnica (no puntuada):** el retroceso «‹» de P04 parece conectado a P03 (Detalle) y no al origen real del usuario (L-05). En un prototipo Figma el retroceso es estático; se registra como limitación a verificar, no como problema de interacción confirmado.

**Resultado:** buenas salidas globales; un problema de recuperación ante eliminación y una verificación pendiente.

### H4. Consistencia y estándares

**Evidencia:** estilo uniforme de CTA (fondo oscuro, esquina redondeada), tarjetas de producto homogéneas, precios junto al nombre, navegación inferior en P01/P02. E-IMG02 completa.

**Aspectos favorables:** identidad visual reconocible y acciones principales con apariencia consistente en todo el flujo.

**Problemas identificados:**

- **H-01 · El acceso al pedido no sigue la convención de ubicación (P01/P02).** No existe ícono de carrito en la cabecera; el acceso se concentra en la barra flotante inferior y en la pestaña «Mi pedido» de la navegación inferior. El patrón dominante en aplicaciones de compra sitúa el carrito en la esquina superior derecha. *Severidad: 2 (menor).* **Frecuencia:** cada vez que el usuario quiere revisar su pedido desde el catálogo. **Impacto:** búsqueda adicional del acceso; demora leve. **Persistencia:** se repite hasta que el usuario aprende la ubicación; el costo se concentra en primeros usos. **Alcance:** acción esencial (revisar/confirmar). Matiz respecto a Fase 2: la versión capturada sí ofrece la pestaña «Mi pedido» en la navegación inferior, por lo que el acceso no es único; el problema es la ausencia del punto que los usuarios esperan, no la inexistencia de acceso.
- **H-10 · Inconsistencias menores de presentación.** (a) La marca «CaféU» aparece a la izquierda en P01/P02/P05/P07 y a la derecha en P03/P04, con microcopy central distinto («DEL MENÚ A TU PAUSA», «TU PAUSA ESTÁ CERCA»). (b) El chip dice «Sanduches» (sin tilde) mientras el producto dice «Sánduche» y la documentación usa «Sánduches». *Severidad: 1 (cosmético).* **Frecuencia:** en cada navegación. **Impacto:** no afecta la tarea; solo uniformidad percibida. **Persistencia:** constante.
- **H-08** (compartida con H2): «Total pagado» (P05) frente a «Total a pagar» (P07) es también una inconsistencia de etiquetado entre pantallas equivalentes.

**Resultado:** consistencia interna buena; desviación de convención externa y detalles menores registrados.

### H5. Prevención de errores

**Evidencia:** stepper «− 1 +» en P03/P04 (impide cantidades inválidas por teclado), resumen completo antes de confirmar en P04, CTA con importe («Confirmar pedido · $4.25»), modal de cancelación en P06, contador de caracteres en instrucciones especiales. E-IMG02-P03, P04, P06.

**Aspectos favorables:** el diseño previene varios errores clásicos: cantidades inválidas, confirmación a ciegas (el total viaja en el botón) y cancelación accidental del pedido completo.

**Problemas identificados:**

- **H-03** (compartida con H3): la eliminación inmediata de ítems es el punto donde el diseño no previene el error ni ofrece recuperación.
- **H-04 · «Añadir» directo no se diferencia de la personalización (P02/P03).** La tarjeta ofrece «Añadir» sin ninguna indicación de que las instrucciones especiales viven en el detalle; quien quiere personalizar debe descubrirlo por ensayo y error. *Severidad: 2 (menor).* **Frecuencia:** cada vez que un producto requiera personalización. **Impacto:** ruta equivocada y retroceso; riesgo de añadir sin la instrucción deseada (p. ej., «Sin azúcar» por razones de salud). **Persistencia:** se aprende tras el primer uso, pero el diseño no lo enseña. **Recuperación:** sencilla. **Alcance:** acción importante de configuración.
- **H-06 · Estado de carrito vacío no definido (P04).** El flujo capturado no incluye ninguna pantalla o variante para el carrito sin ítems; no puede saberse qué ve el usuario si elimina todo, ni si «Confirmar pedido» quedaría inhabilitado. *Severidad propuesta: 1 (cosmético/menor como vacío de diseño), con comportamiento P/V.* **Frecuencia:** ocasional (usuarios que descartan todo el pedido). **Impacto:** potencial desorientación; no demostrado. **Persistencia:** estado no cubierto. Requiere verificación funcional antes de puntuar el comportamiento.
- **H-05** (compartida con H6/H8): el campo de búsqueda de P01 sugiere una acción que el flujo capturado no ofrece (sin conexión visible), lo que puede inducir un primer paso inútil.

**Resultado:** prevención sólida en cantidad, total y cancelación; tres huecos registrados.

### H6. Reconocimiento antes que recuerdo

**Evidencia:** nombre y precio visibles en cada tarjeta; resumen del pedido en P04, P05 y P07; número de pedido repetido; categorías como chips. E-IMG02-P02, P04, P05, P07.

**Aspectos favorables:** el usuario no necesita memorizar nada entre pantallas: qué pidió, cuánto cuesta y su número de pedido están siempre a la vista. Esta es una de las fortalezas del diseño.

**Problemas identificados:**

- **H-04** (compartida con H5): la personalización no es reconocible desde el punto donde se necesita (la tarjeta del catálogo).
- **H-01** (compartida con H4): el acceso al pedido obliga a recordar/descubrir una ubicación no convencional.
- **H-05 · El buscador de Inicio compite con el CTA principal (P01).** El campo «¿Qué se te antoja hoy?» ocupa una posición prominente sobre el banner y sugiere escribir, mientras la acción real para avanzar es «Ver Menú». *Severidad: 2 (menor).* **Frecuencia:** primer uso de la aplicación. **Impacto:** primer paso equivocado y vacilación breve; el CTA se encuentra enseguida. **Persistencia:** de un solo uso (se aprende), por lo que no corresponde 3. **Recuperación:** inmediata y autónoma. Se asigna 2 y no 1 porque el elemento induce una acción errónea real, no solo una molestia estética.

**Resultado:** información contextual excelente; dos problemas de descubribilidad y uno de jerarquía.

### H7. Flexibilidad y eficiencia de uso

**Evidencia:** doble ruta de adición (botón directo «Añadir» en tarjeta y ruta de detalle para personalizar), chips de filtro, stepper en el carrito, «+ Seguir comprando». E-IMG02-P02, P03, P04.

**Aspectos favorables:** el diseño contempla atajos para usuarios rápidos (añadir directo) y una ruta profunda para quienes personalizan; los filtros evitan desplazamientos innecesarios.

**Observaciones:**

- La eficiencia real no es medible desde una captura; los tiempos del pilotaje se contrastan en la triangulación, no aquí.
- **Limitación técnica L-04:** en la captura, los botones «Añadir» del catálogo no muestran conexión de prototipado. Si no estuvieran cableados en la versión vigente, la ruta rápida no existiría en el prototipo (aunque sí en el diseño). Se registra como verificación prioritaria en [soporte-tecnico-f3.md](../docs/soporte-tecnico-f3.md), no como problema de diseño.
- No existe adición de varias unidades desde el catálogo (hay que abrir detalle o usar el stepper del carrito). Se considera aceptable para el alcance de CaféU; **severidad 0** con nota.

**Resultado:** sin problema de diseño puntuado; una verificación técnica prioritaria.

### H8. Diseño estético y minimalista

**Evidencia:** fondos claros, tarjetas agrupadas, jerarquía tipográfica clara (títulos, precios en negrita), un solo CTA principal por pantalla. E-IMG02 completa.

**Aspectos favorables:** la información relevante (producto, precio, acción) domina sobre la decoración; no se observa exceso de información en ninguna pantalla.

**Problemas identificados:**

- **H-05** (compartida con H6): en P01, el buscador y los bloques informativos compiten con la acción principal.
- **H-03** (componente visual, compartida con H3/H5): «Eliminar» es un enlace de texto pequeño y gris, de menor jerarquía que los controles vecinos; su área táctil aparenta reducida para uso con pulgar. La medición en píxeles queda pendiente de verificación a tamaño original (referencia orientativa de 44 × 44 px de la guía de Fase 1, no certificación).

**Resultado:** diseño limpio; los problemas registrados son de jerarquía y de tamaño de control, ya puntuados en sus hallazgos.

### H9. Ayuda para reconocer, diagnosticar y recuperarse de errores

**Evidencia:** modal de cancelación (P06) como único mecanismo de recuperación explícito del flujo; ausencia de pantallas de error, de carrito vacío y de fallo de confirmación en E-IMG02.

**Aspectos favorables:** la cancelación del pedido está protegida por confirmación con salida segura.

**Problemas identificados:**

- **H-09 · Escenarios de error no cubiertos.** El flujo no define qué ocurre ante un fallo (conexión, confirmación fallida, pedido inválido) ni cómo se recupera el usuario conservando su pedido. *Severidad: P/V.* No es honesto asignar 0 porque el pilotaje no registrara errores, ni asignar 3 sin haber provocado un estado de error. Es un **vacío de cobertura** que requiere inspección interactiva específica. Coincide con lo señalado por Viviana (H9 P/V) y Alex (H9 0 provisional con recomendación de probar errores) en sus evaluaciones.
- **H-06** (compartida con H5): carrito vacío sin estado definido.
- **H-11** (compartida con H3): texto de consecuencias del modal no verificable en la evidencia actual.

**Resultado:** evaluación parcial; un vacío de cobertura y dos verificaciones registradas.

### H10. Ayuda y documentación

**Evidencia:** «Tu café, en tres pasos» (1. Elige · 2. Confirma · 3. Retira) y horario «Campus central · Lun–Vie, 7:00–18:00» en P01; «Pago en caja» en P04; «Retira y paga en caja» con instrucciones del número de pedido en P07. E-IMG02-P01, P04, P07.

**Aspectos favorables:** micro-onboarding no invasivo y ayuda contextual situada junto a cada acción; el usuario sabe qué hacer antes, durante y después del pedido sin manual.

**Problemas identificados:**

- **H-12** (compartida con H1): la ayuda de retiro en P07 no incluye el tiempo estimado de preparación en la versión capturada, dato que los usuarios necesitan para decidir si alcanzan a retirar antes de su siguiente clase.

**Resultado:** ayuda contextual bien resuelta; un dato ausente registrado.

## 📊 7. Resumen de mis hallazgos y severidades

| ID | Problema | Pantalla | Heurísticas | Mi severidad | Estado |
|---|---|---|---|---:|---|
| H-01 | Acceso al pedido sin ícono en cabecera (convención de ubicación) | P01/P02 | H4, H6 | 2 | Inspección visual + cableado |
| H-02 | Retroalimentación poco perceptible al añadir | P02 | H1 | 2 | Realce estático; dinámica P/V |
| H-03 | Eliminación inmediata sin deshacer; control pequeño | P04 | H3, H5, H8 | 2 | Flujo sin recuperación; medición P/V |
| H-04 | «Añadir» no se diferencia de personalizar | P02/P03 | H5, H6, H2 | 2 | Inspección visual + cableado |
| H-05 | Buscador de Inicio compite con «Ver Menú» | P01 | H6, H8, H5 | 2 | Inspección visual + cableado |
| H-06 | Carrito vacío no definido en el flujo | P04 | H9, H5 | 1 (diseño) / P/V (comportamiento) | Verificación funcional |
| H-07 | Secuencia «Preparando… 50 %» → «¡Pedido recibido!» | P05/P07 | H1, H2 | 2 (propuesta) | Verificación interactiva |
| H-08 | «Total pagado» contradice el pago en caja | P05 | H2, H4 | 2 (propuesta) | Verificación de versión |
| H-09 | Escenarios de error no cubiertos | Varias | H9 | P/V | Inspección de errores |
| H-10 | Inconsistencias menores (marca en cabecera; «Sanduches») | Varias/P02 | H4 | 1 | Inspección visual |
| H-11 | Modal de cancelación: consecuencias no legibles en evidencia | P06 | H3, H5, H9 | P/V | Captura limpia + recorrido |
| H-12 | Confirmación sin tiempo estimado (versión capturada) | P07 | H1, H10 | 2 (propuesta, condicional) | Verificación de versión |

Las severidades marcadas «propuesta» corresponden a hallazgos nuevos de esta fase que los demás evaluadores aún no han contrastado; su valor consensuado se decide en la revisión grupal ([consolidacion-heuristicas.md](../docs/consolidacion-heuristicas.md)).

## ✅ 8. Aspectos positivos que deben conservarse

1. Resumen del pedido repetido en revisión, estado y confirmación (H6).
2. Importe dentro del CTA de confirmación: previene confirmaciones a ciegas (H5).
3. Stepper de cantidad: previene entradas inválidas (H5).
4. Modal de cancelación con salida segura «Volver al pedido» (H3, H5).
5. Micro-onboarding en tres pasos y avisos contextuales de pago/retiro (H10).
6. Doble ruta de adición y filtros por categoría (H7).
7. Lenguaje de cafetería cercano y precios siempre visibles (H2).

## 🔄 9. Evolución respecto a mi evaluación de Fase 2

| Observación F2 | Estado en F3 |
|---|---|
| OBS-S01 (visibilidad de «Eliminar») | Confirmada visualmente y ampliada: se integra en H-03 con severidad 2 justificada; medición táctil pendiente. |
| OBS-S02 (comprensión de la secuencia de estados) | Ampliada con la evidencia del cableado «Tras pausa»: se concreta en H-07 (secuencia semántica) y H-08 («Total pagado»). |
| OBS-S03 (modal ilegible por anotación) | Se mantiene como H-11 con severidad P/V; sigue siendo limitación de evidencia, no defecto demostrado. |

## 📝 10. Verificaciones interactivas pendientes (a realizar en Figma)

Lista para ejecutar antes de la revisión grupal; registrar fecha y resultado en [soporte-tecnico-f3.md](../docs/soporte-tecnico-f3.md):

- [ ] Recorrer el prototipo completo con el enlace publicado y confirmar que carga.
- [ ] Confirmar destinos de: «‹» en Mi Pedido, «Volver al pedido» y «Sí, cancelar» en el modal.
- [ ] Comprobar si «Añadir» (catálogo), «Eliminar» y los steppers están prototipados.
- [ ] Verificar si existe variante de carrito con 1 ítem ($1.50) y estado vacío.
- [ ] Leer el texto completo del modal de cancelación y capturar sin anotaciones.
- [ ] Confirmar si la versión vigente muestra tiempo estimado en la confirmación.
- [ ] Confirmar el límite real del contador de instrucciones (0/120 en captura vs. 0/100 en documentos previos).
- [ ] Medir el área táctil de «Eliminar» a tamaño original.
- [ ] Provocar/recorrer estados de error disponibles.

## 🎓 11. Conclusión individual

CaféU presenta un flujo de pedido bien estructurado, con lenguaje cercano, información siempre visible y mecanismos sólidos de prevención en cantidad, total y cancelación. Los problemas que identifico se concentran en: (1) la descubribilidad del acceso al pedido y de la personalización, (2) la ausencia de recuperación tras eliminar un ítem, (3) la jerarquía del acceso inicial al menú y (4) la semántica de los estados posteriores a la confirmación («Preparando…» antes de «¡Pedido recibido!», «Total pagado» antes de pagar, y ausencia de tiempo estimado en la versión capturada).

Ningún problema observado bloquea una tarea principal, por lo que no asigno severidades 3 ni 4 en esta inspección; los valores 3 quedarían reservados para lo que demuestre la verificación interactiva o una nueva prueba con usuarios. Las severidades propuestas para hallazgos nuevos se someterán a la comparación del equipo antes de darse por consensuadas.

---