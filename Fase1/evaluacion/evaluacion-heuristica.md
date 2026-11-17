# ☕ Evaluación heurística de Nielsen y revisión responsive — CaféU

## 📋 Identificación

- **Proyecto:** CaféU — aplicación de pedidos de cafetería.
- **Repositorio de referencia:** [APE4_Fase2](https://github.com/maribelsailema/APE4_Fase2).
- **Responsable:** Sebastián.
- **Revisor:** Alex.
- **Destinataria de la matriz para el plan final:** Viviana.
- **Fase:** Planificación de la evaluación de usabilidad.
- **Estado:** Instrumento preparado; inspección pendiente.
- **Resoluciones que se revisarán:** 320 px, 360 px, 768 px y 1366 px.

## 🎯 Propósito

Preparar el procedimiento y los criterios para inspeccionar el prototipo CaféU aplicando las diez heurísticas de Nielsen. La revisión se enfocará en la comprensión del flujo de pedido, la jerarquía visual, la consistencia de los controles, la accesibilidad y la adaptación de la interfaz a distintas anchuras.

Este documento es una **guía para una evaluación futura**, no un informe de resultados. Los hallazgos, evidencias, severidades y recomendaciones se registrarán en [`matriz-heuristicas.md`](matriz-heuristicas.md) cuando se realice la inspección.

## 🧭 Prototipo y alcance

CaféU es una propuesta de aplicación para que estudiantes consulten productos de cafetería y realicen pedidos. La documentación de APE 4 describe pantallas y recorridos relacionados con:

- inicio y menú de productos;
- detalle de producto;
- revisión del pedido y cantidades;
- estado o procesamiento del pedido;
- diálogo de confirmación para cancelar;
- confirmación del pedido.

La inspección deberá considerar las pantallas, estados y recorridos disponibles en la versión concreta del prototipo que se evalúe. No se debe asumir que una interacción funciona solo porque esté descrita en documentación previa.

### 🔗 Documentación y evidencias del APE 4

Estos materiales sirven como **referencia del prototipo y antecedentes del proyecto**:

- [Diagnóstico de usabilidad de CaféU](https://github.com/maribelsailema/APE4_Fase2/blob/5a948cb20c1514a5a6f49e9cce3e34fc474d8b9a/APE4-integral/diagnostico.md)
- [Evaluación de heurísticas y accesibilidad](https://github.com/maribelsailema/APE4_Fase2/blob/5a948cb20c1514a5a6f49e9cce3e34fc474d8b9a/APE4-integral/prototipo/evaluacion-accesibilidad.md)
- [Estados, retroalimentación y recorridos](https://github.com/maribelsailema/APE4_Fase2/blob/5a948cb20c1514a5a6f49e9cce3e34fc474d8b9a/APE4-integral/prototipo/estados-feedback.md)
- [Recorridos del prototipo](https://github.com/maribelsailema/APE4_Fase2/blob/5a948cb20c1514a5a6f49e9cce3e34fc474d8b9a/APE4-integral/prototipo/recorridos.md)

**Capturas de pantallas de referencia:**

- [Inicio](https://github.com/maribelsailema/APE4_Fase2/blob/5a948cb20c1514a5a6f49e9cce3e34fc474d8b9a/APE4-integral/evidencias/pantallas/01_inicio.png)
- [Menú](https://github.com/maribelsailema/APE4_Fase2/blob/5a948cb20c1514a5a6f49e9cce3e34fc474d8b9a/APE4-integral/evidencias/pantallas/02_menu.png)
- [Detalle del producto](https://github.com/maribelsailema/APE4_Fase2/blob/5a948cb20c1514a5a6f49e9cce3e34fc474d8b9a/APE4-integral/evidencias/pantallas/03_detalle.png)
- [Revisión del pedido](https://github.com/maribelsailema/APE4_Fase2/blob/5a948cb20c1514a5a6f49e9cce3e34fc474d8b9a/APE4-integral/evidencias/pantallas/04_pedido.png)
- [Estado del pedido](https://github.com/maribelsailema/APE4_Fase2/blob/5a948cb20c1514a5a6f49e9cce3e34fc474d8b9a/APE4-integral/evidencias/pantallas/05_estado.png)
- [Diálogo de cancelación](https://github.com/maribelsailema/APE4_Fase2/blob/5a948cb20c1514a5a6f49e9cce3e34fc474d8b9a/APE4-integral/evidencias/pantallas/06_modal.png)
- [Confirmación del pedido](https://github.com/maribelsailema/APE4_Fase2/blob/5a948cb20c1514a5a6f49e9cce3e34fc474d8b9a/APE4-integral/evidencias/pantallas/07_confimacion.png)

> 📌 Las capturas y documentos anteriores son antecedentes del APE 4. No deben presentarse como evidencia de una nueva inspección ni como hallazgos de esta evaluación.

## ✅ Objetivo de la inspección

Identificar y documentar problemas potenciales que puedan dificultar que una persona:

1. encuentre y comprenda los productos del menú;
2. interprete la información y el precio de un producto;
3. modifique cantidades y entienda el total;
4. identifique el estado de su pedido;
5. confirme o cancele una acción con confianza;
6. se recupere de errores o acciones no deseadas;
7. use la interfaz de forma legible y accesible en distintos tamaños de pantalla.

## 📝 Procedimiento de inspección

### 1. Preparación

Antes de empezar la evaluación:

1. Identificar la versión y el enlace del prototipo que se inspeccionará.
2. Registrar la fecha, la persona evaluadora, el navegador y el dispositivo o modo de emulación.
3. Confirmar qué pantallas y transiciones están disponibles.
4. Revisar la interfaz en 320 px, 360 px, 768 px y 1366 px.
5. Tener abierta la [matriz de evaluación](matriz-heuristicas.md).
6. Guardar las nuevas capturas en una carpeta de evidencias, identificándolas por pantalla, estado y resolución.

### 2. Inspección

Para cada resolución:

1. Recorrer las pantallas disponibles del flujo de pedido.
2. Revisar las diez heurísticas con las preguntas de esta guía.
3. Comprobar la jerarquía visual, legibilidad, contraste, consistencia y navegación.
4. Observar qué información y acciones son visibles en cada estado.
5. Registrar cada problema observado en la matriz y adjuntar una evidencia.
6. Asignar la severidad de acuerdo con los criterios de este documento.
7. Si aún no hay evidencia suficiente para decidir, dejar la severidad pendiente.

### 3. Consolidación

Una vez realizada la inspección:

1. Revisar y consolidar hallazgos duplicados sin perder las resoluciones afectadas.
2. Diferenciar los problemas observados, las recomendaciones y los aspectos revisados sin problema.
3. Priorizar la revisión de los hallazgos que afecten el flujo principal de pedido.
4. Entregar la matriz y sus evidencias a Viviana para su integración en el plan final.
5. Identificar explícitamente como antecedentes las observaciones que provengan de documentación previa del APE 4.

## 🔍 Las diez heurísticas de Nielsen

Las siguientes preguntas orientan la inspección; **no afirman que exista un problema**.

### H1. Visibilidad del estado del sistema

El sistema debe mantener informada a la persona sobre lo que ocurre.

- ¿Se distingue si el pedido está en revisión, procesamiento, cancelado o confirmado?
- ¿La interfaz responde claramente al añadir un producto o modificar su cantidad?
- ¿El subtotal y el total se actualizan de forma comprensible?
- ¿La pantalla comunica claramente el resultado de confirmar el pedido?

### H2. Correspondencia entre el sistema y el mundo real

La interfaz debe usar lenguaje y conceptos familiares.

- ¿Los nombres de productos, cantidades, precios y acciones se entienden sin explicación técnica?
- ¿El flujo se parece a la forma en que la persona espera realizar un pedido?
- ¿Se entiende la información sobre pago y retiro, cuando aparece en el prototipo?
- ¿Los iconos y etiquetas tienen un significado reconocible en el contexto de una cafetería?

### H3. Control y libertad del usuario

La persona debe poder corregir acciones o salir de un estado no deseado.

- ¿Se puede volver a la pantalla anterior conservando el contexto necesario?
- ¿Se puede modificar o retirar un producto antes de confirmar, si esa opción existe?
- ¿La opción para cancelar está diferenciada de la opción para continuar?
- ¿El diálogo de cancelación permite desistir y regresar al pedido?
- ¿Se explica el efecto de una acción difícil de revertir?

### H4. Consistencia y estándares

Los patrones de interacción deben ser coherentes entre pantallas.

- ¿Los botones con funciones equivalentes mantienen estilos y etiquetas consistentes?
- ¿La navegación, las tarjetas y los controles de cantidad se presentan de manera uniforme?
- ¿Los estados de foco, selección y deshabilitado tienen una representación coherente?
- ¿El nombre y el comportamiento de cada acción son previsibles a lo largo del flujo?

### H5. Prevención de errores

El diseño debe reducir la probabilidad de cometer errores.

- ¿Se evita confirmar el pedido por accidente?
- ¿La interfaz impide cantidades inválidas o aclara sus límites?
- ¿Las acciones destructivas requieren confirmación adecuada?
- ¿Se pueden revisar productos, cantidades y total antes de confirmar?
- ¿Se evitan acciones duplicadas mientras se procesa una operación?

### H6. Reconocimiento antes que recuerdo

La interfaz debe hacer visibles las opciones y reducir la carga de memoria.

- ¿La información del producto está disponible donde se toma la decisión?
- ¿Se pueden reconocer productos, cantidades y precios sin recordar otra pantalla?
- ¿El resumen mantiene visible el contexto relevante del pedido?
- ¿Los controles indican sus acciones mediante texto, iconos reconocibles o ambos?

### H7. Flexibilidad y eficiencia de uso

La interfaz debe facilitar el uso eficiente sin dificultar el aprendizaje inicial.

- ¿Se encuentra con facilidad la acción principal de cada pantalla?
- ¿Se puede modificar una cantidad de forma directa?
- ¿El flujo evita pasos o desplazamientos innecesarios?
- ¿Se puede completar el flujo con los controles disponibles y, cuando aplique, con teclado?
- ¿La organización se adapta a móvil y escritorio sin ocultar acciones principales?

### H8. Diseño estético y minimalista

La interfaz debe priorizar la información relevante y evitar distracciones.

- ¿Producto, precio y acción principal tienen una jerarquía visual clara?
- ¿Los elementos decorativos compiten con la información importante?
- ¿El resumen del pedido y el total se distinguen del contenido secundario?
- ¿La interfaz evita la saturación visual y conserva espacio entre componentes?

### H9. Ayuda para reconocer, diagnosticar y recuperarse de errores

Los mensajes deben explicar el problema y ayudar a resolverlo.

- ¿Los mensajes explican qué ocurrió con palabras claras?
- ¿La interfaz indica qué acción puede realizarse para corregir el problema?
- ¿Se conserva la información necesaria después de un error?
- ¿Los errores se comunican con texto y no solamente mediante color o iconos?
- ¿Se entiende cómo cancelar y regresar al flujo anterior?

### H10. Ayuda y documentación

La orientación debe estar disponible cuando se necesite.

- ¿Se entiende cómo añadir, modificar o confirmar un pedido?
- ¿Las instrucciones sobre pago o retiro aparecen en el momento oportuno, si corresponden?
- ¿Las etiquetas aclaran las acciones menos evidentes?
- ¿La ayuda disponible es fácil de encontrar y comprender sin saturar la interfaz?

## 📊 Escala de severidad

| Valor | Interpretación | Criterio |
|---:|---|---|
| 0 | No representa un problema | No se observa una dificultad relevante para la comprensión, accesibilidad o interacción. |
| 1 | Problema cosmético | Defecto visual menor que no afecta significativamente la tarea. |
| 2 | Problema menor | Produce duda, fricción o demora leve, pero la persona puede continuar y completar la tarea. |
| 3 | Problema importante | Dificulta una acción importante, provoca confusión considerable o puede llevar a un error; la persona puede recuperarse con esfuerzo. |
| 4 | Problema crítico | Bloquea una tarea principal, impide acceder a información o acciones esenciales, o causa una consecuencia grave sin recuperación razonable. |

### Criterios para asignar severidad

Considerar conjuntamente:

- **Impacto:** cuánto afecta la comprensión, accesibilidad o finalización del pedido.
- **Frecuencia esperable:** con qué facilidad podría ocurrir en el flujo.
- **Persistencia:** si ocurre en una pantalla, estado o resolución, o en varios.
- **Recuperación:** si la persona puede corregirlo sin ayuda ni pérdida importante de información.
- **Alcance:** si afecta una acción secundaria o una acción esencial, como revisar o confirmar el pedido.

La severidad no debe asignarse por preferencia estética. Si hay desacuerdo, registrar el motivo y solicitar revisión.

## ♿ Criterios visuales y de accesibilidad

### Jerarquía visual

Revisar si:

- los títulos y nombres de producto se distinguen del texto secundario;
- los precios, cantidades y total son localizables;
- la acción principal destaca sin competir con opciones secundarias;
- el orden de lectura conduce de la información a la acción;
- el diálogo de cancelación distingue la opción segura de la destructiva.

### Contraste y legibilidad

Revisar si:

- el texto se distingue de su fondo en todos los estados y resoluciones;
- el tamaño, peso e interlineado permiten leer descripciones, precios y etiquetas;
- los mensajes de ayuda, error y estado son legibles;
- los estados no se comunican únicamente mediante color.

Como referencia de comprobación WCAG, revisar al menos **4.5:1 para texto normal** y **3:1 para texto grande**. Registrar colores, componente y herramienta de medición. No estimar ratios desde capturas comprimidas ni declarar conformidad sin medir la versión inspeccionada.

### Consistencia de controles y teclado

Revisar si:

- los botones equivalentes conservan estilo, etiqueta y ubicación previsibles;
- los controles de cantidad son comprensibles;
- los controles deshabilitados se distinguen de los disponibles;
- el foco de teclado es visible y su orden es lógico;
- la interfaz puede utilizarse con teclado en las acciones disponibles.

Registrar las dimensiones y separación de los controles táctiles que se midan. La referencia de 44 × 44 px puede utilizarse como orientación de diseño, pero no constituye por sí sola una certificación normativa.

## 📱 Revisión responsive

La anchura corresponde al viewport CSS del navegador. Registrar también la altura, navegador y si se usó un dispositivo real o emulación.

| Ancho | Vista de referencia | Aspectos prioritarios |
|---:|---|---|
| 320 px | Móvil estrecho | Texto y controles, contenido cortado, desbordamiento horizontal y visibilidad de la acción principal. |
| 360 px | Móvil | Flujo de lectura, separación de componentes, acceso a información del pedido y controles de cantidad. |
| 768 px | Tableta o punto de transición | Distribución del contenido, equilibrio entre áreas y continuidad del flujo. |
| 1366 px | Escritorio | Aprovechamiento del espacio, longitud de línea, jerarquía y visibilidad de acciones. |

En cada resolución revisar:

1. Que no haya desplazamiento horizontal involuntario.
2. Que el contenido y las acciones no se superpongan ni queden cortados.
3. Que nombres, descripciones, cantidades y precios sean legibles.
4. Que la acción principal y las alternativas sean localizables.
5. Que el diálogo de cancelación se visualice en el ancho disponible, si existe.
6. Que el orden visual y el orden de lectura sean comprensibles.
7. Que las nuevas capturas indiquen pantalla, estado y resolución.

> 📌 La documentación de APE 4 consultada describe pantallas y un prototipo en Figma. Esta guía propone revisar la adaptación observable del prototipo; no presupone que exista una implementación CSS ni que utilice una estrategia Mobile-First.

## ✅ Preparación para la Fase 2

El instrumento está preparado para la siguiente fase porque:

- incluye las diez heurísticas de Nielsen;
- define un procedimiento de inspección;
- define una escala de severidad de 0 a 4 y criterios para asignarla;
- contempla 320 px, 360 px, 768 px y 1366 px;
- incluye jerarquía visual, contraste, legibilidad, consistencia y accesibilidad;
- considera pantallas y estados del flujo de pedido de CaféU;
- permite registrar evidencias y recomendaciones;
- diferencia antecedentes del APE 4 de hallazgos de una inspección nueva;
- no presenta resultados como si la evaluación ya se hubiera ejecutado.