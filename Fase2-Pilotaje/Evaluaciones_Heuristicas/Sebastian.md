# ☕ APE 6 – Fase 2: Evaluación Heurística Individual de CaféU

## 📋 1. Información general

| Campo | Información |
|---|---|
| Universidad | Universidad Técnica de Ambato |
| Facultad | Facultad de Ingeniería en Sistemas, Electrónica e Industrial |
| Carrera | Ingeniería de Software |
| Asignatura | Interacción Humano-Computador |
| Semestre | Quinto |
| Proyecto | CaféU |
| Actividad | APE 6 – Fase 2 |
| Responsable | Santana Durán Sebastián Israel |
| Usuario GitHub | @SebasIsd |
| Rol | Diseño responsive y soporte técnico |
| Método | Evaluación heurística de Nielsen |
| Instrumento | Matriz de evaluación de la Fase 1 |
| Estado | Inspección visual preliminar documentada; validación individual e interactiva pendiente |

## 🎯 2. Objetivo

Analizar la interfaz del prototipo CaféU mediante las diez heurísticas de Nielsen, identificando aspectos positivos, posibles problemas de interacción y oportunidades de mejora relacionadas con la navegación, claridad visual, prevención de errores, control del usuario y adaptación de la interfaz.

La evaluación busca complementar las pruebas de usabilidad con usuarios desarrolladas durante la Fase 2 del APE 6.

## 📚 3. Documentación utilizada

Para mantener la continuidad con la Fase 1, se utilizaron los siguientes documentos del repositorio:

1. [Plan de evaluación de usabilidad](../../docs/plan-evaluacion.md).
2. [Procedimiento de evaluación heurística](../../evaluacion/evaluacion-heuristica.md).
3. [Matriz de heurísticas](../../evaluacion/matriz-heuristicas.md).
4. [Matriz de seis tareas](../../evaluacion/matriz-tareas.md).
5. [Hoja de observación](../../evaluacion/hoja-observacion.md).

Estos documentos establecen el procedimiento de evaluación, las diez heurísticas y la escala de severidad.

## 🔗 4. Prototipo evaluado

**Sistema:** CaféU.

**Herramienta:** Figma.

**Enlace:**

[☕ Abrir prototipo CaféU en Figma](https://www.figma.com/proto/mmnzX5MbN4kv4IhYOqlQR8/cafeU_prototipo?node-id=3-1700&p=f&scaling=min-zoom&content-scaling=fixed&page-id=0%3A1&starting-point-node-id=3%3A1700)

### Pantallas identificadas en la evidencia visual

| Código | Pantalla | Función |
|---|---|---|
| P01 | Inicio | Presentar CaféU y permitir acceder al menú. |
| P02 | Menú | Mostrar productos, precios y opciones para agregarlos al pedido. |
| P03 | Detalle del producto | Presentar información del producto y permitir seleccionar su cantidad. |
| P04 | Mi pedido | Revisar productos, cantidades, subtotales y total. |
| P05 | Estado de pedido | Mostrar información sobre el procesamiento del pedido. |
| P06 | Modal de cancelación | Solicitar confirmación antes de cancelar un pedido. |
| P07 | Confirmación | Comunicar que el pedido fue recibido y mostrar su resumen. |

### Evidencia utilizada

**E-IMG01:** Captura general de las siete pantallas del prototipo CaféU, proporcionada para esta revisión.

La imagen permite comprobar la organización visual de las pantallas, sus textos principales, la presentación de precios y los controles visibles.

**Limitación:** Esta evidencia no permite verificar automáticamente el funcionamiento de los enlaces, la navegación mediante teclado, los cambios de estado ni el comportamiento responsive en diferentes dispositivos.

## 🔍 5. Método de evaluación

La revisión documental y visual se desarrolló utilizando:

- Las diez heurísticas de Nielsen.
- El plan de evaluación de CaféU correspondiente a la Fase 1.
- La matriz heurística previamente elaborada.
- La captura del flujo general del prototipo.
- Los criterios de claridad visual, consistencia, reconocimiento y prevención de errores.

Se revisaron los elementos visibles de cada pantalla y se identificaron aspectos que necesitan una comprobación posterior.

No se atribuyen resultados de interacción que no puedan observarse en la captura.

## 📊 6. Escala de severidad

Se mantiene la escala establecida en la Fase 1.

| Nivel | Clasificación | Descripción |
|---|---|---|
| 0 | Sin problema | No se identifica un problema de usabilidad. |
| 1 | Cosmético | Defecto visual menor que no afecta significativamente la tarea. |
| 2 | Menor | Produce cierta dificultad, pero permite continuar. |
| 3 | Importante | Dificulta una acción relevante o puede provocar errores. |
| 4 | Crítico | Impide completar una tarea principal o recuperarse del error. |

Cuando la información visual es insuficiente, la severidad se registra como **pendiente de comprobación**.

## 🧩 7. Evaluación de las diez heurísticas de Nielsen

### H1. Visibilidad del estado del sistema

**Principio:** El sistema debe comunicar claramente lo que está ocurriendo.

**Evidencia visual:**

En la pantalla de estado del pedido aparece:

- El mensaje "Preparando tu pedido...".
- Una barra de progreso.
- Un indicador del 50 %.
- Un número de pedido.
- Un resumen de productos.
- El total del pedido.

La pantalla final presenta:

- Un ícono de confirmación.
- El mensaje "¡Pedido recibido!".
- El número de pedido.
- El resumen de la compra.

**Análisis:**

La interfaz presenta elementos visuales destinados a informar el estado de un pedido.

Sin embargo, debe comprobarse si la transición entre el estado de preparación y la confirmación final resulta comprensible para el usuario.

**Resultado:** Existen mecanismos visibles de retroalimentación.

**Pendiente:** Comprobar las transiciones y la interpretación del estado durante la navegación real.

### H2. Correspondencia entre el sistema y el mundo real

**Principio:** La interfaz debe utilizar palabras y conceptos familiares.

**Evidencia visual:**

Se identifican términos como:

- Menú.
- Café americano.
- Sánduche.
- Mi pedido.
- Confirmar pedido.
- Pago en caja.
- Pedido recibido.

Los productos incluyen representaciones gráficas y precios.

**Análisis:**

Los términos están relacionados con una compra habitual en una cafetería universitaria.

La asociación entre producto, precio y representación visual favorece la comprensión del contenido.

**Resultado:** La terminología principal resulta coherente con el contexto de una cafetería.

**Pendiente:** Confirmar mediante las pruebas si los participantes interpretan correctamente las instrucciones sobre el pago y retiro.

### H3. Control y libertad del usuario

**Principio:** El usuario debe poder corregir sus decisiones y regresar de acciones no deseadas.

**Evidencia visual:**

En las pantallas se identifican:

- Controles para modificar cantidades.
- Opciones para eliminar productos.
- Navegación de regreso.
- Botón para cancelar el pedido.
- Modal de confirmación de cancelación.
- Opción para volver al pedido.

**Análisis:**

El diseño contempla controles que permitirían modificar y cancelar acciones.

La presencia del modal también permite distinguir la intención de cancelar del efecto definitivo de esa decisión.

**Resultado:** Se observan controles relacionados con la libertad del usuario.

**Pendiente:** Verificar que las acciones funcionen y que los datos del pedido se conserven cuando corresponda.

### H4. Consistencia y estándares

**Principio:** Los elementos equivalentes deben conservar un comportamiento y una presentación coherentes.

**Evidencia visual:**

Se observa:

- Identidad CaféU en las pantallas.
- Uso de botones principales con fondo oscuro.
- Distribución de contenido mediante tarjetas y secciones.
- Presentación de precios junto a los productos.
- Navegación inferior en las pantallas donde corresponde.

**Análisis:**

La presentación general mantiene una identidad visual reconocible.

Las acciones principales se destacan mediante una apariencia relativamente uniforme.

**Resultado:** Se observa consistencia visual general.

**Pendiente:** Revisar el comportamiento de los controles equivalentes y los estados de foco, selección y deshabilitado.

### H5. Prevención de errores

**Principio:** El sistema debe ayudar a evitar decisiones equivocadas antes de que ocurran.

**Evidencia visual:**

La pantalla "Mi pedido" permite revisar:

- Productos.
- Cantidades.
- Precios.
- Subtotal.
- Total.
- Acción de confirmación.

El prototipo también presenta un modal antes de cancelar el pedido.

**Análisis:**

La revisión previa del pedido ofrece una oportunidad para detectar errores de selección o cantidades.

El modal de cancelación representa un mecanismo visual de prevención de acciones accidentales.

**Resultado:** Se identifican mecanismos visuales orientados a prevenir errores.

**Pendiente:** Comprobar el comportamiento ante cantidades inválidas, confirmaciones repetidas y cancelaciones.

### H6. Reconocimiento antes que recuerdo

**Principio:** La información necesaria debe estar disponible cuando el usuario la necesita.

**Evidencia visual:**

En la pantalla "Mi pedido" aparecen:

- Café americano.
- Sánduche.
- Cantidades.
- Precios.
- Resumen.
- Total de $4,25.

La pantalla de confirmación vuelve a presentar los productos y el importe.

**Análisis:**

La presentación del resumen reduce la necesidad de recordar lo seleccionado en pantallas anteriores.

El usuario dispone de información relevante para revisar el pedido antes de confirmarlo.

**Resultado:** Se observa información contextual que favorece el reconocimiento.

### H7. Flexibilidad y eficiencia de uso

**Principio:** La interfaz debe facilitar la ejecución de tareas sin pasos innecesarios.

**Evidencia visual:**

El diseño contempla el recorrido:

Inicio → Menú → Detalle → Mi pedido → Estado → Confirmación.

Se identifican acciones directas para agregar productos, revisar el pedido y confirmar.

**Análisis:**

El flujo visual organiza la compra en etapas reconocibles.

No obstante, la cantidad real de acciones, la facilidad de edición y los tiempos de ejecución deben comprobarse durante la interacción.

**Resultado:** El diseño presenta una secuencia de tareas estructurada.

**Pendiente:** Contrastar su eficiencia con los tiempos reales del pilotaje.

### H8. Diseño estético y minimalista

**Principio:** La interfaz debe destacar la información importante y evitar distracciones innecesarias.

**Evidencia visual:**

Se identifican:

- Fondos predominantemente claros.
- Ilustraciones de productos.
- Tarjetas con información agrupada.
- Títulos diferenciados.
- Botones principales destacados.
- Separación entre las secciones del pedido.

**Análisis:**

La organización busca priorizar los productos, precios, cantidades y acciones principales.

En la captura general, la información principal se distingue de los elementos decorativos.

**Resultado:** Se aprecia una estructura visual organizada.

**Pendiente:** Examinar cada pantalla a su tamaño original para valorar la legibilidad de textos secundarios y controles pequeños.

### H9. Ayuda para reconocer, diagnosticar y recuperarse de errores

**Principio:** Los mensajes deben explicar qué ocurrió y permitir la recuperación.

**Evidencia visual:**

La captura presenta un modal relacionado con la cancelación de pedidos.

No se incluye una pantalla específica de error de conexión, rechazo de pedido o cantidad inválida.

**Análisis:**

El modal permite observar una decisión de cancelación, pero no proporciona evidencia suficiente para evaluar la recuperación ante otros errores.

**Resultado:** Evaluación parcial.

**Pendiente:** Comprobar qué ocurre cuando una operación falla y si el sistema conserva el pedido.

### H10. Ayuda y documentación

**Principio:** Las instrucciones deben estar disponibles cuando sean necesarias.

**Evidencia visual:**

La pantalla de inicio presenta una explicación del proceso en tres pasos.

También se identifica información sobre el retiro y pago en caja en el estado final del pedido.

**Análisis:**

Estas indicaciones ayudan a comprender el funcionamiento general de CaféU.

No es posible determinar únicamente con la captura si existen otras ayudas contextuales durante situaciones de error.

**Resultado:** Se observan indicaciones orientadoras.

**Pendiente:** Revisar si las instrucciones son suficientes para usuarios que utilizan la aplicación por primera vez.

## 📋 8. Matriz general de evaluación

| ID | Heurística | Evidencia visual | Estado |
|---|---|---|---|
| H1 | Visibilidad del estado | Barra de progreso y confirmación final | Revisada visualmente; transición pendiente |
| H2 | Correspondencia con el mundo real | Productos, precios y lenguaje de cafetería | Revisada visualmente |
| H3 | Control y libertad | Cantidades, eliminar, regresar y cancelar | Revisada visualmente; funcionamiento pendiente |
| H4 | Consistencia y estándares | Botones, navegación y tarjetas | Revisada visualmente |
| H5 | Prevención de errores | Resumen previo y modal de cancelación | Revisada visualmente; validación pendiente |
| H6 | Reconocimiento antes que recuerdo | Resumen, cantidades, precios y total | Revisada visualmente |
| H7 | Flexibilidad y eficiencia | Secuencia de compra y acciones directas | Pendiente de tiempos reales |
| H8 | Diseño estético y minimalista | Jerarquía visual y agrupación | Revisada visualmente |
| H9 | Recuperación de errores | Modal de cancelación | Evaluación parcial |
| H10 | Ayuda y documentación | Instrucciones de inicio y pago | Revisada visualmente |

**Nota:** Esta matriz representa una inspección de las evidencias visuales. No equivale a una validación funcional de todas las heurísticas.

## ⚠️ 9. Aspectos que requieren comprobación

### OBS-S01. Visibilidad del control para eliminar productos

**Pantalla:** Mi pedido.

**Heurísticas relacionadas:** H3, H6 y H8.

**Evidencia:** E-IMG01.

**Descripción:**

En el resumen del pedido se identifica la opción "Eliminar" junto a cada producto.

En la captura general, esta etiqueta tiene menor presencia visual que los controles de cantidad y los precios.

**Riesgo identificado:**

La opción podría resultar menos fácil de localizar para usuarios que necesiten retirar un producto.

**Severidad:** Pendiente de comprobación a tamaño original.

**Recomendación:**

Revisar la legibilidad, el contraste, el área de interacción y la diferenciación del control "Eliminar".

**Estado:** Hipótesis visual; no constituye todavía un fallo confirmado.

### OBS-S02. Comprensión de la secuencia de estados

**Pantallas:** Estado de pedido y Confirmación.

**Heurísticas relacionadas:** H1 y H2.

**Evidencia:** E-IMG01.

**Descripción:**

La secuencia visual incluye un estado denominado "Preparando tu pedido..." y una pantalla final que comunica "¡Pedido recibido!".

**Riesgo identificado:**

Debe comprobarse si los usuarios entienden la relación temporal entre ambos mensajes y reconocen cuándo el pedido fue aceptado.

**Severidad:** Pendiente de comprobación mediante navegación y prueba de comprensión.

**Recomendación:**

Verificar que cada estado comunique inequívocamente si el pedido está enviado, recibido, en preparación o finalizado.

**Estado:** Hipótesis de comprensión; no constituye todavía un fallo confirmado.

### OBS-S03. Claridad del modal de cancelación

**Pantalla:** Modal de cancelación.

**Heurísticas relacionadas:** H3 y H5.

**Evidencia:** E-IMG01.

**Descripción:**

La captura presenta un diálogo para confirmar o desistir de la cancelación.

Se identifican las alternativas "Volver al pedido" y "Sí, cancelar".

**Observación:**

Una anotación superpuesta en la captura impide leer con total claridad parte del contenido del diálogo.

Esto constituye una limitación de la evidencia disponible y no demuestra que el diálogo real tenga un problema de legibilidad.

**Severidad:** No asignada.

**Recomendación:**

Revisar el diálogo directamente en el prototipo y conservar una captura sin anotaciones superpuestas.

**Estado:** Verificación pendiente.

## 📱 10. Revisión responsive

La Fase 1 establece los siguientes anchos de inspección:

| Ancho | Dispositivo de referencia | Aspectos que deben comprobarse | Estado |
|---|---|---|---|
| 320 px | Móvil estrecho | Contenido cortado y acciones visibles | Sin medición independiente |
| 360 px | Móvil | Orden de lectura y controles | Sin medición independiente |
| 768 px | Tableta | Distribución y navegación | Sin medición independiente |
| 1366 px | Escritorio | Uso del espacio y jerarquía | Sin medición independiente |

La evidencia recibida presenta pantallas de apariencia móvil, pero no permite confirmar el ancho CSS exacto ni demostrar una adaptación automática a las cuatro resoluciones.

Por tanto, no se declara conformidad responsive sin las mediciones correspondientes.

## 💡 11. Recomendaciones preliminares

| ID | Recomendación | Relación |
|---|---|---|
| REC-S01 | Verificar la visibilidad y el área interactiva de "Eliminar". | H3, H6, H8 |
| REC-S02 | Comprobar que la transición entre preparación y confirmación sea comprensible. | H1, H2 |
| REC-S03 | Validar que cancelar y volver al pedido produzcan resultados diferenciados. | H3, H5 |
| REC-S04 | Comprobar la actualización de cantidades y total. | H1, H5 |
| REC-S05 | Revisar comportamiento en 320, 360, 768 y 1366 px. | H4, H7, H8 |
| REC-S06 | Validar estados de error y opciones de recuperación. | H9 |
| REC-S07 | Revisar la navegación y el foco mediante teclado. | H3, H7 |

Estas recomendaciones deben validarse con observación directa del prototipo y los datos reales del pilotaje antes de clasificarlas como correcciones obligatorias.

## ✅ 12. Conclusión

La inspección visual preliminar de CaféU muestra una interfaz organizada alrededor de las etapas principales de compra: consulta del menú, selección de productos, revisión, modificación y confirmación.

La presentación de productos y precios, el resumen del pedido, los controles de edición y los mensajes de estado son elementos visibles que contribuyen a la comprensión de la tarea.

Se identificaron aspectos que necesitan comprobación adicional, especialmente la visibilidad de controles secundarios, la interpretación de los estados del pedido y el comportamiento de las opciones de cancelación.

La evidencia disponible permite documentar observaciones visuales, pero todavía no permite atribuir errores a participantes ni determinar el funcionamiento de todas las interacciones.

Los resultados de las pruebas con usuarios y la verificación independiente del prototipo permitirán confirmar o descartar estas hipótesis, asignar severidades justificadas y establecer recomendaciones definitivas.

---

**Responsable de la revisión individual:** Sebastián Santana.

**Validación funcional individual:** Pendiente de registro.

**Fuente visual:** E-IMG01 — Captura del flujo de siete pantallas de CaféU.

**Fuente metodológica:** Instrumentos de la Fase 1 del repositorio APE6.