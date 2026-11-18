# 🔍 Evaluación Heurística Individual – CaféU

**Evaluador:** Sarco Sailema Viviana Maribel  
**Proyecto:** CaféU (Prototipo Figma)  
**Marco de referencia:** 10 Heurísticas de Usabilidad de Jakob Nielsen  
**Fecha de inspección:** 18 de noviembre de 2026  

## 1. Metodología
Se realizó una inspección cognitiva del prototipo interactivo de CaféU, recorriendo las tareas T1 a T6. Cada problema detectado se clasificó según la heurística de Nielsen violada, se le asignó una severidad (1-4) y se propuso una mejora concreta.

## 2. Matriz de Hallazgos Heurísticos

| ID | Problema Detectado | Heurística(s) de Nielsen Violada(s) | Severidad (1-4) | Justificación de la Severidad | Mejora Propuesta |
|:--:|:---|:---|:--:|:---|:---|
| **EH-01** | El campo de búsqueda "Buscar café..." compite visualmente con el botón principal "Ver Menú", causando vacilación inicial. | **H6** (Reconocimiento antes que recuerdo), **H8** (Diseño estético y minimalista) | **2** (Menor) | Frecuencia: Alta en nuevos usuarios. Impacto: Bajo (se recupera rápido). Persistencia: Fácil de corregir con diseño. | Aumentar el contraste y tamaño del CTA "Ver Menú". Cambiar el placeholder del buscador a "¿Qué se te antoja hoy?" para hacerlo más invitante. |
| **EH-02** | La opción para personalizar un producto (ej. "Sin azúcar") no es evidente desde la tarjeta del catálogo; el usuario intenta usar "Añadir" directamente. | **H2** (Correspondencia con el mundo real), **H7** (Flexibilidad y eficiencia de uso) | **3** (Mayor) | Frecuencia: Media. Impacto: Medio (obliga a retroceder y perder tiempo). Persistencia: Afecta el flujo principal. | Agregar un badge o texto visible que diga "Personalizable" en las tarjetas del catálogo. Separar visualmente los botones "Añadir" y "Ver detalles". |
| **EH-03** | Al agregar un producto, la barra inferior del carrito no ofrece una retroalimentación visual clara (animación o badge destacado) de que el estado cambió. | **H1** (Visibilidad del estado del sistema) | **3** (Mayor) | Frecuencia: Alta (en cada agregado). Impacto: Medio (genera incertidumbre: "¿Se agregó?"). | Implementar una micro-animación (ej. rebote o cambio de color temporal) en el ícono del carrito y en el contador de total al agregar un ítem. |
| **EH-04** | La acción "Eliminar" en el carrito se ejecuta inmediatamente sin confirmación ni opción de "Deshacer", y el área táctil es pequeña. | **H3** (Control y libertad del usuario), **H5** (Prevención de errores) | **4** (Crítica) | Frecuencia: Baja. Impacto: Alto (pérdida de todo el pedido y frustración). Persistencia: Riesgo latente en uso real. | Reemplazar la eliminación inmediata por un "Snackbar" (notificación temporal) con un botón "Deshacer" durante 5 segundos. Aumentar el padding del botón eliminar. |

## 3. Conclusión de la Evaluación Individual
El prototipo de CaféU posee un flujo lógico y cumple con las tareas básicas. Sin embargo, los hallazgos **EH-03** y **EH-04** representan riesgos significativos para la experiencia del usuario en un entorno real de cafetería, donde la prisa puede llevar a errores costosos. Se recomienda priorizar estas dos mejoras en el backlog antes de una próxima iteración de desarrollo.

