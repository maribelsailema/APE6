# 🎓 Conclusiones del Laboratorio – Fases 3 y 4 (CaféU)

**Proyecto:** CaféU  
**Equipo:** Viviana Sarco, Wilson Pillapa, Sebastián Santana, Alex Guachi  
**Institución:** Universidad Técnica de Ambato – FISEI  

## 1. Síntesis de la Triangulación de Resultados
La consolidación de las Fases 3 y 4 permite cruzar tres fuentes de evidencia:
1. **Métricas Cuantitativas (Alex):** Tasa de éxito del 100% en tareas, pero con tiempos que superan el objetivo en tareas de personalización (T3) y eliminación (T5). Puntaje SUS promedio de 82.5 (Excelente).
2. **Matriz de Hallazgos (Sebastián):** Convergencia en la detección de problemas de visibilidad del carrito y riesgo en la eliminación de productos.
3. **Evaluación Heurística (Viviana/Wilson):** Confirmación de que las violaciones a las heurísticas H1 (Visibilidad) y H5 (Prevención de errores) son la causa raíz de las vacilaciones registradas en las métricas.

Esta triangulación valida que, aunque el sistema es *eficaz* (los usuarios logran la tarea), su *eficiencia* puede optimizarse significativamente con ajustes de interfaz de bajo costo.

## 2. Respuesta a la Pregunta Central del Laboratorio
**¿Una interfaz que funciona técnicamente puede ser una mala interfaz?**

**Sí, absolutamente.** El funcionamiento técnico (que el código compile, que un botón lleve a otra pantalla o que la base de datos guarde un registro) es una condición necesaria, pero no suficiente, para la calidad del software. 
En el caso de CaféU, el prototipo "funciona" técnicamente: permite agregar y eliminar productos. Sin embargo, si un usuario elimina un producto por error y no tiene forma de recuperarlo (falta de "Deshacer"), la interfaz es deficiente desde la perspectiva de la Interacción Humano-Computador. Una mala interfaz ignora el modelo mental del usuario, genera frustración y aumenta la carga cognitiva, independientemente de que el backend o el código frontend estén libres de errores de compilación. La usabilidad evalúa la experiencia humana, no solo la ejecución del código.

## 3. Verificación vs. Validación (Según Boehm, 1984)
Basado en el planteamiento clásico de Barry Boehm, distinguimos claramente ambas actividades en nuestro proyecto:

*   **Verificación:** Responde a la pregunta *"¿Estamos construyendo el producto correctamente?"*. En CaféU, esto se aplicó al revisar que el prototipo cumpliera con las especificaciones de diseño, que los botones tuvieran las interacciones de Figma configuradas, y que la evaluación heurística confirmara el cumplimiento de estándares (como las 10 heurísticas de Nielsen). Es una evaluación interna y estática.
*   **Validación:** Responde a la pregunta *"¿Estamos construyendo el producto correcto?"*. En CaféU, esto se logró mediante el pilotaje con los participantes P1, P2 y P3. Validamos que el sistema realmente resuelve la necesidad del estudiante universitario (pedir rápido en el descanso) y que el flujo es comprensible para ellos. Es una evaluación externa y dinámica con el usuario final.

## 4. Recomendaciones Finales
1. Implementar de inmediato el patrón de diseño "Undo" (Deshacer) para la eliminación de productos en el carrito.
2. Mejorar la jerarquía visual entre el buscador y el acceso al menú principal.
3. Mantener el cuestionario SUS unificado y contextualizado a CaféU para futuras iteraciones, garantizando la trazabilidad de las métricas de satisfacción.