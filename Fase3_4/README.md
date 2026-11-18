# 🚀 Fases 3 y 4 – Evaluación Heurística y Consolidación Final

**Proyecto:** CaféU – Sistema de pedidos para cafetería universitaria  
**Institución:** Universidad Técnica de Ambato – FISEI – Ingeniería de Software  
**Asignatura:** Interacción Humano-Computador (IHC)  
**Actividad:** APE 6 – Fases 3 y 4  
**Docente:** Ing. José Rubén Caiza Caizabuano, Mg.  
**Rama de trabajo:** `feature/ape6-f3f4-documentacion`  
**Fecha de entrega:** 19 de noviembre de 2026

---

## 👥 Equipo Responsable

| Integrante | Rol en Fases 3 y 4 |
|:---|:---|
| **Sarco Sailema Viviana Maribel** | Moderadora, documentación e integración del proyecto |
| **Pillapa Tubón Wilson Joseph** | Observador y aplicador de sesiones de Fase 3 |
| **Santana Durán Sebastián Israel** | Consolidación de matriz de hallazgos y triangulación |
| **Guachi Aucapiña Alex Fabricio** | Métricas ISO/SUS y análisis cuantitativo |

---

## 🎯 1. Objetivo de las Fases 3 y 4

Ajustar el protocolo de evaluación a partir de los hallazgos del pilotaje de la Fase 2, aplicar la evaluación heurística formal con las 10 heurísticas de Nielsen, y consolidar todos los resultados, métricas y el backlog de mejoras en el informe académico final de la UTA.

---

## 📋 2. Actividades Desarrolladas

### 🔧 Fase 3 – Ajustes y Evaluación Heurística
1. **Revisión del pilotaje:** Se analizó el documento `Fase2-Pilotaje/Ajustes_Protocolo_V1_V2.md` para incorporar las correcciones documentales detectadas (eliminación de referencias a "Aula Abierta", unificación del SUS, hoja de observación adaptada a CaféU).
2. **Protocolo V2:** Se preparó la versión definitiva del protocolo para las nuevas sesiones, incluyendo el procedimiento de reinicio con **F5** y la verificación del estado inicial.
3. **Tarea de refuerzo T7:** Se incorporó la tarea *"Cancelación de un pedido"*, documentando la limitación del prototipo en Figma para este flujo.
4. **Evaluación heurística individual:** Cada integrante inspeccionó el prototipo aplicando las 10 heurísticas de Nielsen, registrando problemas, severidades y propuestas de mejora.

### 📊 Fase 4 – Consolidación y Conclusiones
1. **Triangulación de resultados:** Se cruzaron las métricas de Alex, la matriz de Sebastián y las evaluaciones heurísticas de Viviana y Wilson.
2. **Backlog de mejoras:** Se crearon Issues en GitHub priorizadas (P1, P2, P3, P4) con trazabilidad a hallazgos (`H-XX`) y criterios (`C-XX`).
3. **Conclusiones académicas:** Se respondieron las preguntas teóricas sobre la diferencia entre interfaz funcional e interfaz usable, y la distinción entre verificación y validación según Boehm (1984).
4. **Informe final:** Se integró todo en el documento académico con formato UTA.

---

## 📊 3. Consolidación de Resultados

### ✅ Métricas ISO/SUS (Responsable: Alex)

| Indicador | Resultado |
|:---|:---|
| Tasa de éxito (eficacia) | **100%** (18/18 tareas completadas) |
| Tiempo mediano acumulado | **173 segundos** (dentro del máximo de 450 s) |
| Errores críticos | **0** |
| Errores no críticos | **4** |
| Puntaje SUS promedio | **82.5** (Nivel: *Excelente*) |

### 🔍 Matriz de Hallazgos Consolidada (Responsable: Sebastián)

| ID | Hallazgo | Tarea | Participantes | Heurística | Severidad |
|:--:|:---|:--:|:--:|:---|:--:|
| **H01** | El acceso al menú compite con el campo de búsqueda | T1 | P1 | H6, H8 | 2 |
| **H02** | La personalización no es evidente desde el catálogo | T3 | P1 | H2, H6, H7 | 3 |
| **H03** | La barra del carrito no destaca su actualización | T4 | P1, P3 | H1, H4, H6 | 3 |
| **H04** | La acción "Eliminar" no ofrece recuperación | T5 | P2, P3 | H3, H5, H4 | 4 |

### 🧠 Evaluación Heurística Individual (Responsable: Viviana)

| ID | Problema | Heurística | Severidad | Mejora Propuesta |
|:--:|:---|:---|:--:|:---|
| **EH-01** | Confusión entre buscador y CTA "Ver Menú" | H6, H8 | 2 | Aumentar contraste del CTA principal |
| **EH-02** | Personalización oculta en tarjetas del catálogo | H2, H7 | 3 | Agregar badge "Personalizable" |
| **EH-03** | Falta de feedback al agregar al carrito | H1 | 3 | Micro-animación en el ícono del carrito |
| **EH-04** | Eliminación inmediata sin "Deshacer" | H3, H5 | 4 | Implementar Snackbar con opción "Deshacer" |

---

## 🛠️ 4. Backlog de Mejoras (Issues de GitHub)

| Prioridad | Issue | Hallazgo | Criterio | Descripción |
|:--:|:---|:--:|:--:|:---|
| **P1** | #01 | H04, EH-04 | C-01 (H3, H5 Nielsen) | Implementar feedback visual y opción "Deshacer" al eliminar productos |
| **P2** | #02 | H02, EH-02 | C-02 (H2 Nielsen) | Diferenciar visualmente "Añadir" de "Personalizar" |
| **P3** | #03 | H01, EH-01 | C-03 (H8 Nielsen) | Mejorar jerarquía visual entre buscador y acceso al menú |
| **P4** | #04 | T7 | C-04 (Documental) | Documentar limitación del flujo de cancelación en Figma |

---

## 🎓 5. Conclusiones del Laboratorio

### ¿Una interfaz que funciona técnicamente puede ser una mala interfaz?

**Sí.** El funcionamiento técnico (código que compila, botones que navegan, bases de datos que guardan) es condición necesaria pero **no suficiente** para la calidad del software. En CaféU, el prototipo "funciona" técnicamente: permite agregar y eliminar productos. Sin embargo, si un usuario elimina un producto por error y no tiene forma de recuperarlo, la interfaz es deficiente desde la perspectiva de la Interacción Humano-Computador. Una mala interfaz ignora el modelo mental del usuario, genera frustración y aumenta la carga cognitiva, independientemente de que el código esté libre de errores de compilación.

### Verificación vs. Validación (Boehm, 1984)

Según Barry Boehm, estas dos actividades responden a preguntas distintas:

| Concepto | Pregunta clave | Aplicación en CaféU |
|:---|:---|:---|
| **Verificación** | *"¿Estamos construyendo el producto correctamente?"* | Revisar que el prototipo cumpla especificaciones, que los botones tengan interacciones configuradas, y que se respeten las heurísticas de Nielsen. Es una evaluación interna y estática. |
| **Validación** | *"¿Estamos construyendo el producto correcto?"* | Probar con los participantes P1, P2 y P3 que el sistema realmente resuelve la necesidad del estudiante (pedir rápido en el descanso) y que el flujo es comprensible. Es una evaluación externa y dinámica con el usuario final. |

---


## 📚 6. Referencias

- Boehm, B. W. (1984). *Software Engineering Economics*. Prentice Hall.
- ISO 9241-11. *Ergonomic requirements for office work with visual display terminals – Guidance on usability*.
- Nielsen, J. (1994). *10 Usability Heuristics for User Interface Design*. Nielsen Norman Group.
- Brooke, J. (1996). *SUS: A Quick and Dirty Usability Scale*.

---

### ☕ CaféU – FISEI – Universidad Técnica de Ambato
*Proyecto académico de Interacción Humano-Computador – Quinto Semestre*