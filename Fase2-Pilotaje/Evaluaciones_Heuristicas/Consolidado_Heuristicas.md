# 📊 APE 6 – Fase 2: Consolidado de Evaluaciones Heurísticas de CaféU

## 📋 1. Información general

| Campo | Información |
|---|---|
| Proyecto | CaféU |
| Asignatura | Interacción Humano-Computador |
| Institución | Universidad Técnica de Ambato |
| Responsable | Sebastián Santana |
| Método | Evaluación heurística de Nielsen |
| Heurísticas | 10 |
| Evaluadores previstos | 4 |
| Estado | Consolidación parcial con las evaluaciones disponibles |

## 🎯 2. Objetivo

Consolidar las evaluaciones heurísticas individuales de CaféU, identificando problemas comunes, diferencias entre evaluadores, niveles de severidad y recomendaciones.

La consolidación también permitirá relacionar los problemas de diseño con las dificultades registradas durante el pilotaje.

## 👥 3. Evaluadores

| Evaluador | Documento | Disponibilidad verificada |
|---|---|---|
| Viviana Sarco | [Viviana.md](Viviana.md) | Publicado |
| Wilson Pillapa | [Wilson.md](Wilson.md) | Publicado |
| Sebastián Santana | [Sebastian.md](Sebastian.md) | Revisión visual preparada |
| Alex Guachi | [Alex.md](Alex.md) | Publicado |

La evaluación de Wilson fue publicada en GitHub.

El documento de Sebastián contiene la revisión visual preparada a partir de las pantallas disponibles.

Las evaluaciones de Viviana y Alex deben incorporarse una vez que sus responsables las completen independientemente.

## 🔍 4. Resultados de la evaluación de Wilson

La evaluación individual de Wilson documenta las diez heurísticas y presenta los siguientes problemas:

| Código | Heurística | Problema | Severidad reportada |
|---|---|---|---|
| HW-01 | H1 | Falta de realce de la barra inferior al agregar productos | 2 |
| HW-02 | H3 | Eliminación de productos sin una opción para deshacer | 2 |
| HW-03 | H4 | Ausencia de acceso al carrito en la cabecera | 2 |
| HW-04 | H5 | Posible confusión entre añadir directamente y personalizar | 1 |
| HW-05 | H9 | Estado de carrito vacío insuficientemente documentado | 1 |

**Fuente:** `Wilson.md`, matriz de hallazgos.

Estos niveles corresponden a la evaluación de Wilson. No se atribuyen automáticamente a los demás evaluadores.

## 🔄 5. Relación con las observaciones visuales de Sebastián

| Problema | Revisión visual de Sebastián | Evaluación de Wilson | Relación |
|---|---|---|---|
| Visibilidad del carrito | HS-01 | HW-01 y HW-03 | Coincidencia temática |
| Eliminación sin recuperación | HS-02 | HW-02 | Coincidencia temática |
| Añadir frente a personalizar | HS-03 | HW-04 | Coincidencia temática |
| Estado de carrito vacío | HS-04 | HW-05 | Aspecto pendiente de comprobación |

Las coincidencias temáticas permiten identificar aspectos comunes entre documentos.

No sustituyen la revisión individual y autónoma que debe realizar cada evaluador.

## 📊 6. Métricas verificadas del pilotaje

Se consultaron los registros P1, P2 y P3 publicados en GitHub.

| Métrica | Resultado |
|---|---:|
| Participantes registrados | 3 |
| Tareas por participante | 6 |
| Intentos totales de tarea | 18 |
| Tareas completadas correctamente | 18 |
| Tasa de éxito | 100 % |
| Errores críticos | 0 |
| Errores no críticos registrados | 4 |
| Mediana del tiempo acumulado por participante | 173 segundos |
| SUS promedio | 82,5/100 |

### Puntajes individuales

| Participante | Tiempo acumulado | Errores no críticos | SUS |
|---|---:|---:|---:|
| P1 | 235 s | 3 | 82,5 |
| P2 | 169 s | 0 | 85,0 |
| P3 | 173 s | 1 | 80,0 |

**Fuentes:** [P1](../Participantes/P1.md), [P2](../Participantes/P2.md) y [P3](../Participantes/P3.md).

## ⚠️ 7. Problemas relacionados con el pilotaje

| Problema | Participantes relacionados | Tipo de evidencia |
|---|---|---|
| Dificultad para localizar el carrito | P1 | Dificultad observada durante T4 |
| Confusión entre añadir y personalizar | P1 | Dificultad observada durante T3 |
| Uso inicial de la búsqueda en lugar del menú | P1 | Dificultad observada durante T1 |
| Eliminación sin posibilidad de deshacer | P2 y P3 | Comentarios de mejora posteriores |
| Falta de realce al añadir productos | P3 | Observación registrada durante T4 |

La identificación de un riesgo por parte de un participante no implica necesariamente que haya cometido un error al ejecutar la tarea.

## 🧩 8. Matriz consolidada provisional

| ID | Problema | Heurísticas | Evidencia | Severidad de referencia | Recomendación |
|---|---|---|---|---|---|
| C01 | Acceso al carrito poco evidente para algunos usuarios | H1, H4, H7 | P1-T4; HW-01; HW-03 | 2 | Mejorar la visibilidad del acceso |
| C02 | Eliminación inmediata sin deshacer | H3, H5 | Comentarios P2 y P3; HW-02 | 2 | Incorporar Deshacer |
| C03 | Diferencia poco evidente entre añadir y personalizar | H5, H6 | P1-T3; HW-04 | 1 | Añadir orientación contextual |
| C04 | Interacción inicial con búsqueda en lugar del menú | H6, H8 | P1-T1 | Por acordar | Mejorar claridad del acceso principal |
| C05 | Estado de carrito vacío por comprobar | H9 | HW-05 | 1 según Wilson | Verificar y diseñar recuperación |

Las severidades de referencia provienen de la evaluación publicada de Wilson, salvo donde se indica que deben acordarse.

La consolidación definitiva exige integrar las evaluaciones independientes restantes.

## 💡 9. Prioridades de mejora propuestas

### Prioridad 1: Recuperación de productos eliminados

Se recomienda incluir la acción "Deshacer" cuando el usuario elimina un producto.

La sugerencia está respaldada por la evaluación de Wilson y los comentarios finales de P2 y P3.

### Prioridad 2: Acceso al carrito

Se recomienda mejorar la identificación de la opción para revisar el pedido.

P1 buscó inicialmente el carrito en la parte superior antes de localizar la barra flotante inferior.

### Prioridad 3: Personalización de productos

Se recomienda diferenciar la acción directa "Añadir" de la apertura de las opciones de personalización.

P1 registró una dificultad recuperable durante la tarea T3.

### Prioridad 4: Estado del carrito vacío

Se recomienda comprobar el comportamiento del prototipo cuando se eliminan todos los productos.

Este escenario no queda demostrado por las seis tareas documentadas.

## ✅ 10. Conclusión

Las evaluaciones disponibles y el pilotaje permiten identificar aspectos comunes relacionados con el acceso al carrito, la eliminación de productos y la personalización del pedido.

Los tres participantes completaron las seis tareas, lo que evidencia un resultado favorable de eficacia dentro del pilotaje registrado.

No obstante, se documentaron dificultades recuperables y sugerencias que pueden orientar mejoras de interacción.

La consolidación actual utiliza los resultados publicados por Wilson y la revisión visual preparada para Sebastián.

Para cumplir íntegramente el requisito de cuatro evaluaciones independientes, todavía deben incorporarse y contrastarse las evaluaciones de Viviana y Alex.

---

**Responsable de consolidación:** Sebastián Santana.

**Revisor:** Alex Guachi.

**Estado:** Consolidación parcial basada en evidencia disponible.