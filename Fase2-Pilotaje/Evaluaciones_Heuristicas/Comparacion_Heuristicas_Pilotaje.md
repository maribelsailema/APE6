# 🔎 APE 6 – Fase 2: Comparación entre Evaluación Heurística y Pilotaje

## 📋 1. Información general

| Campo | Información |
|---|---|
| Proyecto | CaféU |
| Asignatura | Interacción Humano-Computador |
| Responsable | Sebastián Santana |
| Método 1 | Evaluación heurística de Nielsen |
| Método 2 | Prueba con usuarios mediante pensamiento en voz alta |
| Participantes | P1, P2 y P3 |
| Sesiones registradas | 16 de noviembre de 2026 |
| Fuente | Registros individuales publicados en GitHub |

## 🎯 2. Objetivo

Comparar los problemas identificados mediante inspección heurística con las dificultades registradas durante las pruebas de usabilidad de CaféU.

La comparación busca identificar coincidencias, diferencias y oportunidades de mejora sustentadas en evidencias.

## 📚 3. Documentación utilizada

### Evaluaciones

- [Evaluación visual de Sebastián](Sebastian.md).
- [Evaluación heurística de Wilson](Wilson.md).
- [Consolidado de heurísticas](Consolidado_Heuristicas.md).

### Pilotaje

- [Registro P1](../Participantes/P1.md).
- [Registro P2](../Participantes/P2.md).
- [Registro P3](../Participantes/P3.md).

## 🧪 4. Tareas ejecutadas

Los registros individuales contienen las siguientes seis tareas:

| ID | Situación |
|---|---|
| T1 | Consultar el catálogo y precio de una bebida |
| T2 | Filtrar productos por categoría |
| T3 | Personalizar un producto con instrucciones especiales |
| T4 | Agregar un alimento y comprobar el total |
| T5 | Eliminar un producto y comprobar el nuevo total |
| T6 | Confirmar el pedido y verificar su información |

## 📊 5. Resultados cuantitativos

### 5.1 Tiempos por tarea

| Tarea | P1 | P2 | P3 | Mediana |
|---|---:|---:|---:|---:|
| T1 | 34 s | 21 s | 24 s | 24 s |
| T2 | 28 s | 19 s | 18 s | 19 s |
| T3 | 52 s | 38 s | 41 s | 41 s |
| T4 | 48 s | 36 s | 39 s | 39 s |
| T5 | 31 s | 24 s | 22 s | 24 s |
| T6 | 42 s | 31 s | 29 s | 31 s |
| **Total** | **235 s** | **169 s** | **173 s** | **173 s*** |

*La mediana de la última fila se calcula sobre los tres tiempos totales por participante.*

### 5.2 Eficacia

| Tarea | Participantes que completaron | Tasa de éxito |
|---|---:|---:|
| T1 | 3/3 | 100 % |
| T2 | 3/3 | 100 % |
| T3 | 3/3 | 100 % |
| T4 | 3/3 | 100 % |
| T5 | 3/3 | 100 % |
| T6 | 3/3 | 100 % |

**Eficacia global:**

18 tareas completadas / 18 intentos × 100 = **100 %**.

### 5.3 Errores registrados

| Tarea | P1 | P2 | P3 | Total de errores no críticos |
|---|---:|---:|---:|---:|
| T1 | 1 | 0 | 0 | 1 |
| T2 | 0 | 0 | 0 | 0 |
| T3 | 1 | 0 | 0 | 1 |
| T4 | 1 | 0 | 1 | 2 |
| T5 | 0 | 0 | 0 | 0 |
| T6 | 0 | 0 | 0 | 0 |
| **Total** | **3** | **0** | **1** | **4** |

**Errores críticos:** 0.

**Observación metodológica:** El registro P3 clasifica como error no crítico de T4 una observación sobre la ausencia de animación o indicador destacado en la barra del pedido, aunque señala que encontró la barra sin dificultad. Conviene que Wilson y Alex revisen si corresponde mantener esa clasificación. Hasta entonces, este informe conserva el dato original.

### 5.4 Satisfacción

| Participante | SUS |
|---|---:|
| P1 | 82,5 |
| P2 | 85,0 |
| P3 | 80,0 |
| **Promedio** | **82,5** |

Los tres puntajes son superiores a 68 puntos, valor habitualmente utilizado como referencia descriptiva para SUS.

Estos resultados corresponden a los tres participantes registrados y no representan por sí solos una estimación generalizable de todos los estudiantes universitarios.

## 🔍 6. Comparación de hallazgos

### Hallazgo CP-01. Acceso al carrito

**Tarea:** T4.

**Heurísticas:** H1, H4 y H7.

**Observación heurística:**

La interfaz utiliza una barra inferior para acceder al pedido, sin un acceso equivalente en la cabecera.

**Evidencia del pilotaje:**

El registro P1 señala que el participante buscó inicialmente un ícono de carrito en la parte superior.

Después localizó la barra inferior y completó la tarea.

**Participantes con dificultad observada:** 1 de 3.

**Resultado:** Coincidencia entre la inspección y el pilotaje.

**Recomendación:** Mejorar la identificación del acceso al carrito.

---

### Hallazgo CP-02. Personalización del producto

**Tarea:** T3.

**Heurísticas:** H5 y H6.

**Observación heurística:**

El menú ofrece una acción directa para añadir productos y la personalización se encuentra en el detalle.

**Evidencia del pilotaje:**

P1 intentó utilizar inicialmente la opción directa antes de acceder al detalle para escribir "Sin azúcar".

Después completó la tarea correctamente.

**Participantes con dificultad observada:** 1 de 3.

**Resultado:** Coincidencia entre el riesgo identificado y la dificultad observada.

**Recomendación:** Presentar una opción de personalización más reconocible.

---

### Hallazgo CP-03. Eliminación de productos

**Tarea:** T5.

**Heurísticas:** H3 y H5.

**Observación heurística:**

La eliminación de un producto requiere revisar las posibilidades de recuperación.

**Evidencia del pilotaje:**

P1, P2 y P3 completaron T5 sin errores registrados.

En la entrevista final, P2 señaló que la eliminación inmediata debería permitir deshacer.

P3 recomendó aumentar el área táctil de la opción "Eliminar" y considerar una confirmación.

**Participantes que expresaron la preocupación:** 2 de 3.

**Participantes con error de eliminación registrado:** 0 de 3.

**Resultado:** Coincidencia con comentarios de mejora, pero no con errores observados durante T5.

**Recomendación:** Incorporar la opción "Deshacer" y revisar el tamaño del control táctil.

---

### Hallazgo CP-04. Acceso inicial al menú

**Tarea:** T1.

**Heurísticas:** H6 y H8.

**Evidencia del pilotaje:**

El registro P1 indica que el participante utilizó inicialmente la barra de búsqueda antes de reconocer el acceso principal "Ver Menú".

La tarea se completó de manera autónoma.

**Participantes con dificultad observada:** 1 de 3.

**Resultado:** Hallazgo específico registrado durante el pilotaje.

**Recomendación:** Revisar la jerarquía visual entre la búsqueda y la acción principal.

---

### Hallazgo CP-05. Retroalimentación al agregar productos

**Tarea:** T4.

**Heurística:** H1.

**Evidencia del pilotaje:**

El registro P3 incluye una observación sobre la ausencia de mayor realce visual o animación de la barra inferior al añadir productos.

El mismo registro indica que P3 localizó el acceso sin dificultad.

**Participantes que señalaron el aspecto:** 1 de 3.

**Resultado:** Oportunidad de mejora visual; no se ha demostrado un bloqueo de tarea.

**Recomendación:** Evaluar un indicador breve de actualización del carrito.

---

### Hallazgo CP-06. Comprensión del estado final

**Tarea:** T6.

**Heurísticas:** H1 y H2.

**Observación previa:**

La revisión visual planteó comprobar la claridad de los estados del pedido.

**Evidencia del pilotaje:**

P1, P2 y P3 completaron T6 y reconocieron la confirmación, el número de pedido y las indicaciones de pago y retiro.

No se registraron errores críticos ni no críticos en esta tarea.

**Resultado:** La posible confusión planteada en la inspección visual no se observó durante este pilotaje.

**Recomendación:** Conservar la claridad de la confirmación.

## 📋 7. Matriz comparativa final del pilotaje

| Código | Heurística | Tarea | Participantes relacionados | Evidencia | Comparación |
|---|---|---|---|---|---|
| CP-01 | H1, H4, H7 | T4 | P1 | Búsqueda inicial del carrito en cabecera | Coincidencia |
| CP-02 | H5, H6 | T3 | P1 | Duda entre añadir y personalizar | Coincidencia |
| CP-03 | H3, H5 | T5 | P2 y P3 | Sugerencias sobre eliminación y recuperación | Coincidencia parcial |
| CP-04 | H6, H8 | T1 | P1 | Uso inicial de búsqueda | Hallazgo del pilotaje |
| CP-05 | H1 | T4 | P3 | Observación sobre realce visual | Oportunidad de mejora |
| CP-06 | H1, H2 | T6 | P1, P2, P3 | Confirmación reconocida correctamente | Riesgo previo no observado |

## 💡 8. Recomendaciones priorizadas

| Prioridad propuesta | Mejora | Fundamentación |
|---|---|---|
| Alta | Mejorar el acceso al carrito | Dificultad observada en P1 |
| Alta | Permitir deshacer una eliminación | Riesgo señalado por P2 y P3 |
| Media | Diferenciar añadir y personalizar | Dificultad observada en P1 |
| Media | Mejorar claridad del acceso al menú | Dificultad inicial observada en P1 |
| Baja | Incorporar realce visual al añadir | Observación de P3, sin bloqueo |
| Mantener | Mensaje final de confirmación | T6 completada por los tres usuarios |

Las prioridades son recomendaciones de análisis, no evidencias de mejoras ya implementadas.

## ✅ 9. Conclusiones

La comparación entre las inspecciones disponibles y el pilotaje permite identificar coincidencias relevantes en la localización del carrito, la personalización de productos y la recuperación después de eliminar elementos.

Los tres participantes completaron las seis tareas. La eficacia global registrada fue del 100 %, con cuatro errores no críticos consignados y ningún error crítico.

La dificultad más clara relacionada con la navegación fue la búsqueda del carrito en la cabecera durante T4.

También se observaron dificultades recuperables al interpretar el acceso inicial al menú y la diferencia entre añadir un producto directamente o abrir su personalización.

Por otra parte, los participantes interpretaron correctamente la confirmación del pedido, por lo que la hipótesis inicial de confusión en ese estado no quedó respaldada por las sesiones registradas.

Los resultados sustentan recomendaciones concretas para mejorar la interacción sin afirmar que las correcciones ya fueron implementadas o verificadas.

---

**Responsable:** Sebastián Santana.

**Fuentes:** P1.md, P2.md, P3.md y evaluaciones heurísticas disponibles.

**Estado:** Comparación con el pilotaje documentado completada.