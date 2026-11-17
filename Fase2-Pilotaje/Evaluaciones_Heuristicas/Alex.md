# Evaluación heurística individual — Alex

**Proyecto:** CaféU  
**Evaluador:** Alex  
**Actividad:** APE6-F2-04  
**Fecha de referencia:** 16 de noviembre de 2026  
**Método:** revisión individual basada en registros del pilotaje P1, P2 y P3, matriz de tareas, hoja de observación y matriz de heurísticas del repositorio.

## Nota sobre el alcance

Este documento es una evaluación heurística individual preliminar construida con la evidencia disponible en el ZIP. No se encontró un registro independiente de inspección directa de Alex con capturas y recorrido completo por cada pantalla/estado. En consecuencia, los juicios se limitan a lo observado o reportado durante el pilotaje. «Sin problema observado» no equivale a una certificación exhaustiva de cumplimiento.

**Escala de severidad:** 0 = no representa problema; 1 = cosmético; 2 = menor; 3 = mayor; 4 = crítico/catastrófico.

## Revisión de las diez heurísticas de Nielsen

### H1. Visibilidad del estado del sistema
**Resultado:** oportunidad de mejora. **Severidad preliminar: 2.**

La barra flotante inferior informa la cantidad de artículos y el total. Sin embargo, P1 buscó un acceso al carrito en la cabecera durante aproximadamente seis segundos, y P3 señaló que la barra no presenta animación o distintivo destacado al actualizarse. La información existe, pero su ubicación y realce pueden no ser suficientemente perceptibles.

**Evidencia:** T04, P1 y P3.  
**Recomendación:** reforzar el feedback al añadir productos y evaluar un acceso visible al carrito en la cabecera.

### H2. Correspondencia entre el sistema y el mundo real
**Resultado:** oportunidad de mejora localizada. **Severidad preliminar: 2.**

La terminología del flujo («Menú», «Añadir», «Mi pedido», «Paga al momento de retirar») es familiar. No obstante, P1 no identificó de inmediato que debía abrir el detalle para introducir instrucciones especiales y probó primero «Añadir» desde la tarjeta.

**Evidencia:** T03, P1.  
**Recomendación:** explicar con etiquetas claras la diferencia entre añadir directamente y personalizar.

### H3. Control y libertad del usuario
**Resultado:** riesgo de recuperación ante acciones accidentales. **Severidad preliminar: 2.**

P2 y P3 comentaron que la eliminación del producto es inmediata y que sería conveniente poder deshacerla o confirmarla. No se registraron eliminaciones accidentales durante T05.

**Evidencia:** comentarios de cierre de P2 y P3; T05 completada por los tres participantes.  
**Recomendación:** incorporar una opción temporal «Deshacer» o confirmación breve.

### H4. Consistencia y estándares
**Resultado:** oportunidad de mejora. **Severidad preliminar: 2.**

P1 esperaba encontrar el carrito en la esquina superior derecha, patrón habitual en interfaces de compra. CaféU utiliza una barra flotante inferior. La diferencia no impidió completar T04, pero produjo búsqueda adicional.

**Evidencia:** T04, P1.  
**Recomendación:** evaluar un acceso dual (cabecera y barra inferior), manteniendo consistencia visual y funcional.

### H5. Prevención de errores
**Resultado:** oportunidad de mejora preventiva. **Severidad preliminar: 2.**

Los comentarios de P2 y P3 identifican un riesgo de eliminación involuntaria por la acción inmediata y el tamaño reducido del enlace «Eliminar». No se registraron errores durante la ejecución, por lo que el riesgo es potencial.

**Evidencia:** entrevistas de cierre de P2 y P3.  
**Recomendación:** ampliar el área táctil y permitir deshacer la eliminación.

### H6. Reconocimiento antes que recuerdo
**Resultado:** oportunidad de mejora. **Severidad preliminar: 2.**

P1 necesitó descubrir que la personalización se encontraba en el detalle del producto y que el carrito se abría desde la barra inferior. Esto sugiere que algunas acciones no se reconocen con suficiente facilidad desde el contexto donde se necesitan.

**Evidencia:** T03 y T04, P1.  
**Recomendación:** mostrar etiquetas o indicaciones contextuales para «Personalizar» y «Ver mi pedido».

### H7. Flexibilidad y eficiencia de uso
**Resultado:** sin problema relevante observado en los registros. **Severidad: 0 provisional.**

P2 y P3 utilizaron directamente «Añadir» desde la tarjeta para el sánduche; P1 logró personalizar el café accediendo al detalle. Los registros muestran rutas de interacción distintas según la necesidad. La evidencia disponible no señala una barrera de eficiencia general en esta heurística.

**Evidencia:** T03 y T04, registros de P1, P2 y P3.  
**Recomendación:** conservar ambas rutas y hacer explícito cuándo corresponde cada una.

### H8. Diseño estético y minimalista
**Resultado:** sin problema confirmado; revisar jerarquía de inicio. **Severidad: 1 provisional.**

En T01, P1 confundió inicialmente el campo de búsqueda con el acceso para consultar el catálogo. La evidencia apunta a una posible competencia visual entre elementos de la pantalla de inicio, pero no permite afirmar que toda la interfaz presente exceso de información.

**Evidencia:** T01, P1.  
**Recomendación:** revisar la jerarquía visual entre el campo de búsqueda y el CTA «Ver Menú».

### H9. Ayudar a reconocer, diagnosticar y recuperarse de errores
**Resultado:** evidencia insuficiente para una conclusión completa. **Severidad: 0 provisional.**

Los participantes completaron T06 e identificaron el código de pedido, el tiempo estimado y el lugar de pago/retiro. No se registraron errores de sistema ni situaciones de recuperación durante las tareas. Los registros no prueban cómo respondería la interfaz ante fallos técnicos o estados inesperados.

**Evidencia:** T06, P1, P2 y P3.  
**Recomendación:** probar escenarios de error, carrito vacío y fallo de confirmación en una inspección específica.

### H10. Ayuda y documentación
**Resultado:** sin necesidad de ayuda observada durante el pilotaje. **Severidad: 0 provisional.**

Los tres participantes completaron las seis tareas sin solicitar ayuda ni recibir pistas. Esto indica que, para el flujo probado, no fue necesario recurrir a asistencia externa. No constituye una revisión exhaustiva de la sección informativa o de la documentación de la aplicación.

**Evidencia:** registros de ayuda = 0 para P1, P2 y P3.  
**Recomendación:** conservar la autonomía observada y validar el contenido informativo con usuarios de menor experiencia.

## Matriz resumen

| Heurística | Resultado | Severidad provisional | Evidencia principal |
|---|---|---:|---|
| H1 Visibilidad del estado | Oportunidad de mejora | 2 | T04, P1 y P3 |
| H2 Correspondencia con mundo real | Oportunidad de mejora localizada | 2 | T03, P1 |
| H3 Control y libertad | Riesgo de eliminación accidental | 2 | Cierre P2 y P3 |
| H4 Consistencia y estándares | Oportunidad de mejora | 2 | T04, P1 |
| H5 Prevención de errores | Riesgo potencial | 2 | Cierre P2 y P3 |
| H6 Reconocimiento antes que recuerdo | Oportunidad de mejora | 2 | T03 y T04, P1 |
| H7 Flexibilidad y eficiencia | Sin problema relevante observado | 0* | T03/T04 |
| H8 Diseño estético y minimalista | Revisar jerarquía de inicio | 1* | T01, P1 |
| H9 Recuperación de errores | Evidencia insuficiente; sin fallo observado | 0* | T06 |
| H10 Ayuda y documentación | Sin ayuda requerida en el flujo | 0* | Ayudas = 0 |

\* Severidad provisional basada únicamente en la evidencia del pilotaje; requiere inspección directa para confirmar.

## Conclusión individual

La evidencia del pilotaje muestra que CaféU permite completar el flujo de pedido con autonomía y sin errores críticos. Las principales oportunidades de mejora se relacionan con la visibilidad del carrito, la identificación de la ruta de personalización y la prevención de eliminaciones involuntarias. Para cerrar la evaluación heurística con mayor rigor, se recomienda una inspección directa de las diez heurísticas sobre la versión exacta del prototipo, documentando pantalla, estado, evidencia visual y severidad por cada hallazgo.

---
**Evaluador: Alex**
