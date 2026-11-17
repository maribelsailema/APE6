# APE6-F2-04 — Hallazgos preliminares de usabilidad

**Proyecto:** CaféU  
**Responsable:** Alex  
**Participantes:** P1, P2 y P3  
**Fecha de pilotaje:** 16 de noviembre de 2026  
**Base de análisis:** registros individuales de P1, P2 y P3; comentarios de cierre; documentación de tareas y heurísticas incluida en el ZIP.

## 1. Síntesis

Las 18 ejecuciones de tareas terminaron con éxito autónomo. No se registraron errores críticos ni solicitudes de ayuda. Se registraron cuatro errores no críticos: tres de P1 (T01, T03 y T04) y uno de P3 (T04). Además, P2 y P3 expresaron en la entrevista de cierre una preocupación sobre la eliminación inmediata y el tamaño del control «Eliminar» en el carrito; estos comentarios se consideran evidencia cualitativa de riesgo, no errores contabilizados durante T05.

Los hallazgos son preliminares y se limitan a tres participantes. Las heurísticas indicadas son asociaciones plausibles para orientar el refinamiento, no una afirmación de incumplimiento definitivo.

## 2. Hallazgos observados

### H01. El acceso principal al menú compite con el campo de búsqueda

- **Tarea afectada:** T01.
- **Participantes afectados:** 1 de 3 (P1).
- **Evidencia:** P1 pulsó inicialmente el campo «Buscar café, snacks...» creyendo que debía escribir, antes de advertir «Ver Menú». El registro reporta un error no crítico y una vacilación inicial.
- **Impacto:** demora breve y ambigüedad sobre cuál es el siguiente paso para consultar el catálogo.
- **Heurísticas relacionadas:** H6, reconocimiento antes que recuerdo; H8, diseño estético y minimalista; potencialmente H2, correspondencia con el mundo real, si el campo sugiere una función que no corresponde al objetivo inmediato.
- **Recomendación:** diferenciar visualmente el campo de búsqueda del CTA «Ver Menú» y reforzar la jerarquía del acceso al catálogo. Revisar que el placeholder no sugiera una acción no disponible en ese estado.
- **Severidad preliminar:** 2 — menor.

### H02. La personalización no es evidente desde la tarjeta del catálogo

- **Tarea afectada:** T03.
- **Participantes afectados:** 1 de 3 (P1).
- **Evidencia:** P1 intentó usar «Añadir» directamente desde la tarjeta, no encontró dónde escribir «Sin azúcar» y retrocedió para abrir el detalle tocando la tarjeta. El registro contabiliza un error no crítico.
- **Impacto:** el usuario debe deshacer el camino inicial y descubrir que la personalización está en otra vista.
- **Heurísticas relacionadas:** H2, correspondencia con el mundo real; H6, reconocimiento antes que recuerdo; H7, flexibilidad y eficiencia de uso.
- **Recomendación:** incorporar una indicación visible como «Personalizar» o «Ver opciones» en productos que admitan instrucciones especiales, y diferenciar claramente «Añadir» de «Abrir detalle».
- **Severidad preliminar:** 2 — menor.

### H03. La barra flotante del carrito no coincide con la expectativa de ubicación ni destaca su actualización

- **Tarea afectada:** T04.
- **Participantes afectados:** 2 de 3 (P1 y P3).
- **Evidencia:** P1 buscó durante aproximadamente seis segundos un carrito en la esquina superior derecha antes de encontrar la barra inferior. P3 localizó la barra, pero observó que no tiene animación de realce o badge destacado al agregar artículos. Ambos completaron T04; los registros contabilizan un ENC para cada uno.
- **Impacto:** descubrimiento tardío del acceso al pedido y retroalimentación poco perceptible tras añadir un producto.
- **Heurísticas relacionadas:** H1, visibilidad del estado del sistema; H4, consistencia y estándares; H6, reconocimiento antes que recuerdo.
- **Recomendación:** conservar la barra inferior y evaluar un acceso complementario al carrito en la cabecera. Añadir una señal breve y perceptible al actualizar el número de ítems y el total, sin generar distracción.
- **Severidad preliminar:** 2 — menor.

### H04. La acción «Eliminar» puede ejecutarse accidentalmente y ofrece poca protección

- **Tarea afectada:** T05.
- **Participantes afectados:** 2 de 3 (P2 y P3) en comentarios de cierre.
- **Evidencia:** P2 indicó que eliminar borra el ítem inmediatamente sin confirmación y sugirió confirmación o deshacer. P3 señaló que el enlace es texto pequeño y puede tocarse por accidente con el pulgar; propuso un área táctil mayor o confirmación. En las ejecuciones de T05, los tres participantes completaron la tarea y no se registraron ENC ni EC.
- **Impacto:** riesgo potencial de eliminación involuntaria y coste de recuperación si el usuario debe volver al catálogo.
- **Heurísticas relacionadas:** H3, control y libertad del usuario; H5, prevención de errores; H4, consistencia y estándares de controles táctiles.
- **Recomendación:** ofrecer «Deshacer» mediante snackbar temporal o una confirmación breve; ampliar el área táctil del control y separar «Eliminar» de acciones contiguas.
- **Severidad preliminar:** 2 — menor. Se trata de un riesgo reportado, no de un fallo observado durante la ejecución.

## 3. Matriz de trazabilidad

| Hallazgo | Tarea | Participantes | Evidencia cuantitativa/cualitativa | Heurísticas |
|---|---|---|---|---|
| H01 — Búsqueda compite con CTA | T01 | P1 (1/3) | 1 ENC; confusión inicial con el campo de búsqueda | H6, H8, posible H2 |
| H02 — Personalización poco visible | T03 | P1 (1/3) | 1 ENC; retroceso desde «Añadir» a detalle | H2, H6, H7 |
| H03 — Descubrimiento/realce del carrito | T04 | P1 y P3 (2/3) | 2 ENC; búsqueda de icono y falta de realce | H1, H4, H6 |
| H04 — Eliminación accidental | T05 | P2 y P3 (2/3) | Comentarios post-sesión; 0 errores durante T05 | H3, H5, H4 |

## 4. Evaluación heurística individual de Alex

La inspección que se documenta en `Evaluaciones_Heuristicas/Alex.md` es una evaluación individual preliminar basada en la evidencia de las sesiones y los instrumentos del repositorio. No se dispone en el ZIP de un acta independiente de inspección pantalla por pantalla realizada por Alex ni de capturas que permitan certificar cada estado visual. Por ello, las heurísticas sin evidencia directa se identifican como «sin problema observado en los registros» y no como cumplimiento exhaustivamente verificado.

## 5. Priorización sugerida

1. **Prioridad alta de refinamiento:** H03 (acceso/feedback del carrito) y H04 (prevención de eliminación accidental), por afectar el control y la comprensión del pedido.
2. **Prioridad media:** H02 (descubrimiento de personalización), por provocar retroceso y tiempo adicional.
3. **Prioridad media-baja:** H01 (jerarquía entre búsqueda y acceso al menú), por ser una confusión breve y recuperable.

La prioridad es una recomendación de trabajo para la siguiente iteración, no una medición estadística.

## 6. Conclusión

CaféU permitió que P1, P2 y P3 completaran todas las tareas sin ayuda y sin errores críticos. Las oportunidades de mejora se concentran en la visibilidad de acciones y controles, la personalización del producto y la prevención de eliminaciones accidentales. La siguiente iteración debería validar las soluciones propuestas con nuevas sesiones, manteniendo los mismos criterios de registro y comparando tiempos, errores y satisfacción.

---
*APE6-F2-04 · Responsable: Alex.*
