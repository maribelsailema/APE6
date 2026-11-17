# ☕ Matriz de heurísticas de Nielsen y revisión responsive — CaféU

## 📋 Identificación

| Campo | Información |
|---|---|
| Proyecto | CaféU — aplicación de pedidos de cafetería |
| Repositorio de referencia | [maribelsailema/APE4_Fase2](https://github.com/maribelsailema/APE4_Fase2) |
| Usuario objetivo documentado | Estudiantes universitarios |
| Flujo de referencia | Inicio → menú → detalle del producto → revisión del pedido → estado y confirmación |
| Estados descritos en APE 4 | Inicial, procesamiento, error/recuperación y éxito |
| Responsable de la planificación | Sebastián |
| Revisor | Alex |
| Destinataria de la matriz | Viviana |
| Resoluciones consideradas | 320 px, 360 px, 768 px y 1366 px |
| Estado | Instrumento preparado para la evaluación de Fase 2 |

## 📝 Propósito y uso

Esta matriz sirve para organizar la inspección heurística de CaféU y registrar problemas, evidencias, severidad y recomendaciones.

La documentación de APE 4 contiene antecedentes de evaluación sobre tres heurísticas y algunos aspectos de accesibilidad. Estos antecedentes se incluyen como referencia para la nueva revisión; **no equivalen a resultados obtenidos en la evaluación de APE 6**. Deben comprobarse en la versión del prototipo que se evalúe.

La revisión responsive en 320 px, 360 px, 768 px y 1366 px forma parte del alcance de esta matriz. En las fuentes de APE 4 disponibles no consta un registro específico de resultados de CaféU medidos en esos cuatro anchos, por lo que no se atribuyen resultados responsive no comprobados.

### Procedimiento

1. Abrir la versión de CaféU que se evaluará y confirmar qué pantallas e interacciones están disponibles.
2. Inspeccionar el flujo de pedido en cada resolución objetivo.
3. Revisar las diez heurísticas y los criterios visuales y de accesibilidad.
4. Comparar las observaciones actuales con los antecedentes del APE 4.
5. Registrar problemas nuevos solo si se observan en la inspección.
6. Asociar capturas o enlaces a cada hallazgo.
7. Aplicar la escala de severidad incluida abajo.
8. Consolidar las recomendaciones para entregar la matriz a Viviana.

## 📊 Escala de severidad

| Valor | Interpretación | Criterio |
|---:|---|---|
| 0 | No representa un problema | No se observa una dificultad relevante para la comprensión, accesibilidad o interacción. |
| 1 | Problema cosmético | Defecto visual menor que no afecta significativamente la tarea. |
| 2 | Problema menor | Produce duda, fricción o demora leve, pero la persona puede continuar. |
| 3 | Problema importante | Dificulta una acción importante, provoca confusión considerable o puede llevar a un error. |
| 4 | Problema crítico | Bloquea una tarea principal o puede causar una consecuencia grave sin recuperación razonable. |

Al asignar severidad se consideran el impacto en la tarea, la frecuencia esperable, la persistencia del problema y la posibilidad de recuperarse. Las severidades de los antecedentes siguientes son las que reportó APE 4; pueden modificarse si la nueva inspección aporta evidencia distinta.

## 🔎 Cobertura de las diez heurísticas

La tabla identifica los antecedentes disponibles. Las heurísticas que no fueron evaluadas explícitamente en la documentación consultada quedan identificadas como aspectos incluidos en el instrumento, sin atribuirles resultados previos.

| ID | Heurística | Antecedente disponible en APE 4 | Aspecto que se revisará en Fase 2 |
|---|---|---|---|
| H1 | Visibilidad del estado del sistema | APE 4 describió la barra de progreso, el mensaje de procesamiento y la confirmación del pedido. También registró la ausencia de tiempo estimado como observación cosmética. | Claridad del estado, progreso y resultado del pedido en cada resolución. |
| H2 | Correspondencia entre el sistema y el mundo real | No consta una evaluación específica de esta heurística en el material revisado. | Claridad del lenguaje, productos, precios, pago, retiro y orden del flujo. |
| H3 | Control y libertad del usuario | APE 4 describió opciones de regreso y un diálogo para desistir de la cancelación. También señaló revisar qué ocurre al retroceder desde el detalle. | Posibilidad de corregir, regresar, cancelar y conservar la información necesaria. |
| H4 | Consistencia y estándares | No consta una evaluación específica de esta heurística en el material revisado. | Consistencia de botones, etiquetas, iconos, navegación y estados visuales. |
| H5 | Prevención de errores | APE 4 describió el diálogo de confirmación de cancelación y los límites del control de cantidad. | Prevención de cancelaciones accidentales, cantidades inválidas y confirmaciones duplicadas. |
| H6 | Reconocimiento antes que recuerdo | No consta una evaluación específica de esta heurística en el material revisado. | Visibilidad de productos, cantidades, precios y resumen al tomar decisiones. |
| H7 | Flexibilidad y eficiencia de uso | No consta una evaluación específica de esta heurística en el material revisado. | Facilidad para localizar acciones y completar el flujo sin pasos innecesarios. |
| H8 | Diseño estético y minimalista | No consta una evaluación específica de esta heurística en el material revisado. | Jerarquía visual, densidad de información y elementos que puedan distraer. |
| H9 | Ayuda para reconocer, diagnosticar y recuperarse de errores | APE 4 describió el diálogo de cancelación y mecanismos de recuperación; no consta una evaluación completa de mensajes de error. | Claridad de errores, solución sugerida y conservación del contexto. |
| H10 | Ayuda y documentación | No consta una evaluación específica de esta heurística en el material revisado. | Disponibilidad y claridad de ayuda contextual para las acciones del pedido. |

## 🧾 Antecedentes documentados en APE 4

Estos registros proceden de la [evaluación de heurísticas y accesibilidad de APE 4](https://github.com/maribelsailema/APE4_Fase2/blob/5a948cb20c1514a5a6f49e9cce3e34fc474d8b9a/APE4-integral/prototipo/evaluacion-accesibilidad.md). Son antecedentes para comparar y revalidar, no hallazgos nuevos de APE 6.

| ID de referencia | Pantalla / componente | Heurística o criterio | Observación reportada en APE 4 | Severidad reportada | Recomendación o verificación para Fase 2 |
|---|---|---|---|---:|---|
| REF-H01 | Estado del pedido | H1: Visibilidad del estado | APE 4 reportó que la barra de progreso no mostraba un tiempo estimado. | 1 — Cosmético | Comprobar si la versión actual incluye una estimación y si esta ayuda a entender la espera. |
| REF-H02 | Diálogo de cancelación | H5: Prevención de errores | APE 4 reportó una posible confusión entre la acción de cancelar y la acción principal. | 2 — Menor | Verificar que la opción destructiva se distinga claramente de la opción para volver al pedido. |
| REF-H03 | Detalle del producto | H3: Control y libertad | APE 4 señaló revisar la respuesta de la interfaz al retroceder desde el detalle cuando existe información introducida. | 1 — Cosmético | Comprobar si los datos se conservan o si se informa claramente que podrían perderse. |
| REF-A01 | Texto auxiliar / menú | Accesibilidad: contraste | APE 4 reportó un ratio de contraste de 2.6:1 para un texto auxiliar antes de un ajuste. | 2 — Menor | Medir nuevamente el componente actual; APE 4 indicó que el texto fue ajustado en Figma. |
| REF-A02 | Detalle / control de cantidad | Accesibilidad: área de interacción | APE 4 reportó un marco visual de 36 px para el botón de decremento. | 1 — Cosmético | Medir el área interactiva actual y comprobar su facilidad de uso. |

> 📌 Las severidades anteriores son transcritas como antecedentes del APE 4. No deben presentarse como severidades obtenidas en una inspección nueva.

## 🧾 Registro de hallazgos de la evaluación APE 6

No hay hallazgos nuevos registrados en este documento. La matriz se entrega preparada para la inspección de Fase 2; los antecedentes de APE 4 están separados en la sección anterior.

| ID | Heurística / criterio | Resolución | Pantalla / componente | Hallazgo nuevo observado | Evidencia nueva | Impacto | Severidad APE 6 | Recomendación | Estado |
|---|---|---|---|---|---|---|---|---|---|
| — | — | — | — | No se han registrado hallazgos nuevos de APE 6. | No se han agregado evidencias nuevas. | — | — | — | Instrumento preparado |

### Ficha para añadir hallazgos nuevos

Duplicar esta ficha solo si durante la inspección se observa un problema:

#### H-01 — [Descripción breve]

- **Heurística o criterio relacionado:**
- **Pantalla o componente:**
- **Resolución:**
- **Estado del flujo del pedido:**
- **Comportamiento observado:**
- **Evidencia nueva:** captura o enlace.
- **Impacto para la persona:**
- **Severidad (0–4):**
- **Justificación de severidad:**
- **Recomendación concreta:**
- **Estado de la recomendación:**

## 📱 Revisión responsive

Las resoluciones se incluyen como tamaños objetivo de la inspección. La documentación de APE 4 disponible no registra resultados específicos de CaféU medidos en esos cuatro anchos; por ello, esta tabla consigna el alcance previsto y no afirma que las pruebas responsive ya se hayan ejecutado.

| Viewport objetivo | Tipo de vista | Aspectos a comprobar | Resultado responsive documentado en APE 4 |
|---:|---|---|---|
| 320 px | Móvil estrecho | Desbordamiento horizontal, legibilidad, tamaño y separación de controles, visibilidad de la acción principal. | No consta medición específica para CaféU en este ancho. |
| 360 px | Móvil | Flujo de lectura, visibilidad de producto, cantidad, precio y acciones del pedido. | No consta medición específica para CaféU en este ancho. |
| 768 px | Tableta / transición | Distribución, equilibrio entre áreas, navegación y jerarquía visual. | No consta medición específica para CaféU en este ancho. |
| 1366 px | Escritorio | Uso del espacio, longitud de línea, jerarquía y visibilidad de acciones. | No consta medición específica para CaféU en este ancho. |

### Criterios de observación responsive

En cada ancho se comprobará:

- ausencia de desplazamiento horizontal involuntario;
- contenido sin cortes ni superposiciones;
- lectura clara de nombres, descripciones, cantidades y precios;
- acceso visible a las acciones principales y secundarias;
- presentación comprensible del diálogo de cancelación, si está disponible;
- orden visual y secuencia de lectura coherentes;
- controles con espacio suficiente para su interacción.

## ♿ Revisión visual y de accesibilidad

Los datos siguientes se identifican como referencias históricas del APE 4. No son mediciones nuevas de APE 6.

| Elemento | Antecedente documentado en APE 4 | Criterio para la nueva revisión | Estado del dato |
|---|---|---|---|
| Texto auxiliar | Se reportó un contraste de 2.6:1 antes de un ajuste. | Medir los colores del componente en la versión evaluada y registrar herramienta y resultado. | Antecedente APE 4; no revalidado en APE 6. |
| Texto normal | APE 4 utilizó como referencia WCAG un mínimo de 4.5:1 para texto normal. | Comprobar el contraste del texto normal con el fondo. | Criterio de revisión. |
| Texto grande | APE 4 utilizó como referencia WCAG un mínimo de 3:1 para texto grande. | Comprobar el contraste del texto grande con el fondo. | Criterio de revisión. |
| Botón de decremento | APE 4 reportó un marco visual de 36 px en el control de decremento. | Medir el área interactiva actual y comprobar que el control sea fácil de accionar. | Antecedente APE 4; no revalidado en APE 6. |
| Foco de teclado | APE 4 incluyó la revisión de accesibilidad de controles y navegación. | Comprobar que el foco sea visible y que el orden de tabulación sea comprensible. | Criterio de revisión. |
| Estados del pedido | APE 4 describió estados inicial, procesamiento, error/recuperación y éxito. | Confirmar que cada estado se entienda por texto y señales visuales, no solo por color. | Antecedente funcional; adaptación responsive no medida aquí. |

## 🖼️ Evidencias de referencia del APE 4

Estas capturas corresponden al repositorio de APE 4 y sirven como contexto visual. No son evidencias nuevas de la inspección APE 6.

- [Inicio](https://github.com/maribelsailema/APE4_Fase2/blob/5a948cb20c1514a5a6f49e9cce3e34fc474d8b9a/APE4-integral/evidencias/pantallas/01_inicio.png)
- [Menú](https://github.com/maribelsailema/APE4_Fase2/blob/5a948cb20c1514a5a6f49e9cce3e34fc474d8b9a/APE4-integral/evidencias/pantallas/02_menu.png)
- [Detalle del producto](https://github.com/maribelsailema/APE4_Fase2/blob/5a948cb20c1514a5a6f49e9cce3e34fc474d8b9a/APE4-integral/evidencias/pantallas/03_detalle.png)
- [Revisión del pedido](https://github.com/maribelsailema/APE4_Fase2/blob/5a948cb20c1514a5a6f49e9cce3e34fc474d8b9a/APE4-integral/evidencias/pantallas/04_pedido.png)
- [Estado del pedido](https://github.com/maribelsailema/APE4_Fase2/blob/5a948cb20c1514a5a6f49e9cce3e34fc474d8b9a/APE4-integral/evidencias/pantallas/05_estado.png)
- [Diálogo de cancelación](https://github.com/maribelsailema/APE4_Fase2/blob/5a948cb20c1514a5a6f49e9cce3e34fc474d8b9a/APE4-integral/evidencias/pantallas/06_modal.png)
- [Confirmación del pedido](https://github.com/maribelsailema/APE4_Fase2/blob/5a948cb20c1514a5a6f49e9cce3e34fc474d8b9a/APE4-integral/evidencias/pantallas/07_confimacion.png)

## 💡 Recomendaciones de referencia para revalidar

Estas recomendaciones provienen de los antecedentes de APE 4 y deben contrastarse con el prototipo actual antes de declararlas vigentes:

| ID | Referencia | Acción propuesta para la revisión |
|---|---|---|
| R-01 | REF-H01 | Verificar si se necesita comunicar un tiempo estimado junto al progreso del pedido. |
| R-02 | REF-H02 | Comprobar la jerarquía visual de las acciones de cancelar y volver al pedido. |
| R-03 | REF-H03 | Revisar si al retroceder se conserva la información introducida o se advierte su pérdida. |
| R-04 | REF-A01 | Medir el contraste del texto auxiliar después del ajuste reportado en APE 4. |
| R-05 | REF-A02 | Medir el área interactiva del control de decremento en la versión evaluada. |

## 📌 Resumen para la entrega

- Las diez heurísticas están incluidas en la matriz de cobertura.
- Los antecedentes de APE 4 están identificados y separados de los hallazgos nuevos.
- Se consideran las cuatro resoluciones solicitadas.
- Se incluyen criterios de jerarquía visual, contraste, legibilidad, controles y accesibilidad.
- Se incluyen enlaces a la documentación y capturas del prototipo de referencia.
- No se atribuyen resultados responsive ni hallazgos nuevos que no estén documentados.
- **Responsable:** Sebastián.
- **Revisor:** Alex.
- **Destinataria de la matriz:** Viviana.