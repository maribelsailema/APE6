# Métricas de usabilidad – ISO 9241-11 y cuestionario SUS

**Proyecto:** CaféU  
**Actividad:** APE6-F3F4-04  
**Responsable:** Guachi Aucapiña Alex Fabricio  
**Rol:** Cronometrista y responsable de métricas  
**Participantes:** P1, P2 y P3  
**Fecha de las sesiones:** 18 de noviembre de 2026

## 1. Objetivo

Presentar los resultados de eficacia, eficiencia y satisfacción obtenidos durante las pruebas de usabilidad de CaféU. Los cálculos se realizan a partir de los registros individuales de P1, P2 y P3, diferenciando las tareas principales de la tarea de refuerzo de cancelación.

Los tiempos se expresan en segundos y corresponden a la ejecución de cada tarea, no a la duración completa de las sesiones.

## 2. Alcance de las tareas y tiempos de referencia

El protocolo contempla siete tareas. T1–T6 corresponden al flujo principal de consulta y pedido. T7 es una tarea de refuerzo que busca comprobar si el participante comprende qué ocurre después de confirmar un pedido e intenta cancelarlo.

| Tarea | Descripción | Meta | Máximo |
|---|---|---:|---:|
| T1 | Consultar precio de café americano | 30 s | 60 s |
| T2 | Filtrar categoría Snacks | 30 s | 60 s |
| T3 | Personalizar café americano | 45 s | 90 s |
| T4 | Agregar sánduche y revisar el total | 45 s | 90 s |
| T5 | Eliminar el sánduche | 30 s | 60 s |
| T6 | Confirmar pedido y reconocer comprobante | 45 s | 90 s |
| T7 | Intentar cancelar el pedido (refuerzo) | 30 s | 60 s |
| **Total** | **T1–T7** | **255 s** | **450 s** |

## 3. Métricas de eficacia

### 3.1 Criterio de cálculo

La tasa de éxito autónomo se calcula de la siguiente manera:

`Tasa de éxito autónomo = (Tareas completadas correctamente sin ayuda / Total de tareas intentadas) × 100`

Se registran por separado:
- Tareas completadas correctamente sin ayuda.
- Tareas completadas con ayuda.
- Tareas incompletas o fallidas.
- Errores críticos y no críticos.
- Solicitudes de ayuda.

### 3.2 Resultados de las tareas principales (T1–T6)

Los tres participantes completaron las seis tareas principales sin solicitar ayuda.

| Indicador | Resultado |
|---|---:|
| Participantes | 3 |
| Tareas principales por participante | 6 |
| Tareas principales intentadas | 18 |
| Tareas principales completadas correctamente sin ayuda | 18 |
| Tareas principales completadas con ayuda | 0 |
| Tareas principales fallidas o incompletas | 0 |
| **Tasa de éxito autónomo T1–T6** | **100 %** |
| Solicitudes de ayuda | 0 |

Cálculo:

`(18 / 18) × 100 = 100 %`

### 3.3 Resultado específico de T7: intento de cancelación

T7 debe analizarse por separado porque el recorrido utilizado no permitió ejecutar la cancelación desde la interfaz.

| Indicador | Resultado |
|---|---:|
| Participantes que intentaron T7 | 3 |
| Cancelaciones ejecutadas desde la interfaz | 0 |
| Participantes que comprendieron la limitación | 3 |
| Solicitudes de ayuda | 0 |

La comprensión del estado se logró en 3 de 3 participantes (100 %). Sin embargo, la tasa de ejecución funcional de la cancelación fue 0 de 3 (0 %).

Por tanto, no se debe sumar T7 como una cancelación ejecutada correctamente. El protocolo consideró éxito conceptual la comprensión del estado del pedido; este resultado es diferente del éxito funcional de cancelar.

### 3.4 Resumen global de eficacia

| Forma de contabilización | Numerador / denominador | Resultado |
|---|---:|---:|
| Éxito autónomo en tareas principales T1–T6 | 18 / 18 | 100 % |
| Comprensión conceptual de T7 | 3 / 3 | 100 % |
| Cancelación efectiva en T7 | 0 / 3 | 0 % |
| Éxito funcional estricto considerando T1–T7 | 18 / 21 | 85,71 % |

El valor de 85,71 % considera que T7 solicitaba cancelar el pedido y que la acción no pudo ejecutarse. Se presenta como una lectura estricta de cumplimiento funcional. El 100 % de comprensión conceptual de T7 se conserva como indicador independiente, de acuerdo con la limitación descrita en el protocolo.

### 3.5 Errores y solicitudes de ayuda

| Participante | Errores críticos | Errores no críticos | Solicitudes de ayuda |
|---|---:|---:|---:|
| P1 | 0 | 2 | 0 |
| P2 | 0 | 1 | 0 |
| P3 | 0 | 1 | 0 |
| **Total** | **0** | **4** | **0** |

Los errores no críticos se relacionan con dudas o búsquedas de ruta durante T1, T3 y T7, según los registros individuales. No se registraron errores críticos ni solicitudes de ayuda.

**Nota:** los comentarios de cierre sobre riesgos potenciales, como eliminar accidentalmente un producto, no se contabilizan como errores de ejecución si no ocurrieron durante la tarea.

## 4. Métricas de eficiencia

### 4.1 Matriz de tiempos por tarea

Para cada tarea se ordenan los tres tiempos individuales y se obtiene la mediana. La mediana se compara con el tiempo objetivo y con el tiempo máximo definido en el protocolo.

| Tarea | Meta | P1 | P2 | P3 | Mediana | Cumplimiento de meta |
|---|---:|---:|---:|---:|---:|---|
| T1 | 30 s | 26 s | 18 s | 20 s | **20 s** | Cumple |
| T2 | 30 s | 22 s | 16 s | 15 s | **16 s** | Cumple |
| T3 | 45 s | 44 s | 32 s | 36 s | **36 s** | Cumple |
| T4 | 45 s | 41 s | 31 s | 33 s | **33 s** | Cumple |
| T5 | 30 s | 25 s | 20 s | 19 s | **20 s** | Cumple |
| T6 | 45 s | 35 s | 27 s | 25 s | **27 s** | Cumple |
| T7 | 30 s | 48 s | 39 s | 34 s | **39 s** | Supera la meta |

**Método:** la mediana corresponde al valor central de los tres tiempos ordenados de menor a mayor.

Ejemplo T1: 18, 20, 26 → mediana = 20 segundos.

### 4.2 Comparación con los tiempos máximos

| Tarea | Máximo | Mayor tiempo individual | Resultado |
|---|---:|---:|---|
| T1 | 60 s | 26 s | Dentro del máximo |
| T2 | 60 s | 22 s | Dentro del máximo |
| T3 | 90 s | 44 s | Dentro del máximo |
| T4 | 90 s | 41 s | Dentro del máximo |
| T5 | 60 s | 25 s | Dentro del máximo |
| T6 | 90 s | 35 s | Dentro del máximo |
| T7 | 60 s | 48 s | Dentro del máximo |

Todas las ejecuciones se mantuvieron dentro de los tiempos máximos. Sin embargo, T7 superó el tiempo objetivo de 30 segundos en los tres participantes (48, 39 y 34 segundos). Esto muestra que el intento de localizar la cancelación demandó más tiempo que el previsto, aunque no superó el máximo permitido.

### 4.3 Tiempo acumulado por participante

| Participante | Tiempo acumulado T1–T7 | Equivalencia aproximada |
|---|---:|---|
| P1 | **241 s** | 4 min 01 s |
| P2 | **183 s** | 3 min 03 s |
| P3 | **182 s** | 3 min 02 s |
| **Promedio** | **202 s** | **3 min 22 s** |
| **Mediana de los totales** | **183 s** | **3 min 03 s** |

Cálculo del promedio:

`(241 + 183 + 182) / 3 = 202 segundos`

La suma de los tiempos objetivo es 255 segundos y la suma de los tiempos máximos es 450 segundos. Los tres participantes finalizaron el conjunto de tareas dentro del máximo acumulado.

### 4.4 Interpretación de eficiencia

- T1–T6 presentan medianas inferiores a sus tiempos objetivo.
- T7 presenta una mediana de 39 segundos, superior a su meta de 30 segundos.
- Ninguna tarea superó su tiempo máximo individual.
- P2 y P3 registraron tiempos acumulados similares: 183 y 182 segundos.
- P1 registró 241 segundos, principalmente por mayores tiempos en T1, T3, T4 y T7.

La duración de T7 no debe interpretarse como tiempo necesario para completar una cancelación, porque la interfaz no permitió ejecutar esa acción. El tiempo corresponde al intento de localizar y comprender la ausencia de la opción.

## 5. Métricas de satisfacción: cuestionario SUS

### 5.1 Método de cálculo

El cuestionario SUS contiene diez afirmaciones con respuestas de 1 a 5.

- En los ítems impares (1, 3, 5, 7 y 9), se resta 1 a la respuesta.
- En los ítems pares (2, 4, 6, 8 y 10), se resta la respuesta a 5.
- Se suman los diez valores ajustados.
- El resultado se multiplica por 2,5.

`SUS = (suma de puntuaciones ajustadas) × 2,5`

La puntuación final se expresa en una escala de 0 a 100. No representa un porcentaje de éxito.

### 5.2 Puntajes individuales

| Participante | Suma ajustada | Puntaje SUS |
|---|---:|---:|
| P1 | 34 | **85,0** |
| P2 | 37 | **92,5** |
| P3 | 36 | **90,0** |

### 5.3 Cálculo del promedio

`Promedio SUS = (85,0 + 92,5 + 90,0) / 3`

`Promedio SUS = 267,5 / 3 = 89,17`

**Resultado promedio SUS: 89,17 puntos.**

### 5.4 Comparación con la referencia de 68 puntos

| Indicador | Puntaje |
|---|---:|
| Promedio SUS de CaféU | **89,17** |
| Referencia de comparación | **68,00** |
| Diferencia | **+21,17 puntos** |

El promedio obtenido supera en 21,17 puntos la referencia de 68. Esto indica una percepción favorable de usabilidad entre los tres participantes evaluados.

La puntuación debe interpretarse considerando que la muestra fue de tres participantes y que el cuestionario aplicado estaba contextualizado para CaféU. No permite afirmar que toda la población universitaria tendrá la misma percepción.

## 6. Resumen general de resultados

| Dimensión | Indicador | Resultado |
|---|---|---:|
| Eficacia | Éxito autónomo T1–T6 | 100 % |
| Eficacia | Comprensión conceptual T7 | 100 % |
| Eficacia | Cancelación funcional T7 | 0 % |
| Eficacia | Éxito funcional estricto T1–T7 | 85,71 % |
| Errores | Errores críticos | 0 |
| Errores | Errores no críticos | 4 |
| Asistencia | Solicitudes de ayuda | 0 |
| Eficiencia | Mediana T1 | 20 s |
| Eficiencia | Mediana T2 | 16 s |
| Eficiencia | Mediana T3 | 36 s |
| Eficiencia | Mediana T4 | 33 s |
| Eficiencia | Mediana T5 | 20 s |
| Eficiencia | Mediana T6 | 27 s |
| Eficiencia | Mediana T7 | 39 s |
| Satisfacción | Promedio SUS | 89,17 |
| Satisfacción | Diferencia frente a 68 | +21,17 |

## 7. Observaciones sobre consistencia de los registros

Al comparar los registros individuales con la tabla consolidada de sesiones, se identificaron diferencias en algunos tiempos de P1 y P2. Para que los cálculos sean reproducibles, esta entrega utiliza los tiempos escritos en las tablas individuales de cada participante.

| Tarea | P1 individual | P1 consolidado | P2 individual | P2 consolidado | P3 individual |
|---|---:|---:|---:|---:|---:|
| T1 | 26 s | 28 s | 18 s | 22 s | 20 s |
| T2 | 22 s | 24 s | 16 s | 18 s | 15 s |
| T3 | 44 s | 51 s | 32 s | 39 s | 36 s |
| T4 | 41 s | 42 s | 31 s | 35 s | 33 s |
| T5 | 25 s | 26 s | 20 s | 21 s | 19 s |
| T6 | 35 s | 32 s | 27 s | 26 s | 25 s |
| T7 | 48 s | 38 s | 39 s | 22 s | 34 s |
| **Total** | **241 s** | **241 s** | **183 s** | **183 s** | **182 s** |

Los totales coinciden, pero la distribución por tarea no coincide para P1 y P2. Se recomienda que el cronometrista y el observador revisen las hojas originales o las grabaciones para ratificar cuál registro debe considerarse definitivo. Hasta entonces, no se deben reemplazar silenciosamente los valores individuales.

También existe una diferencia de clasificación para T7: los registros individuales la describen como éxito conceptual con limitación de interfaz, mientras que el cumplimiento funcional de la acción de cancelar fue imposible. Este informe conserva ambas lecturas de forma separada.

## 8. Conclusiones

1. **Eficacia:** las seis tareas principales se completaron correctamente y sin ayuda, con una tasa de éxito autónomo del 100 %.
2. **Cancelación:** los tres participantes comprendieron la limitación de la interfaz, pero ninguno pudo cancelar el pedido desde el recorrido probado.
3. **Errores:** no se registraron errores críticos; se contabilizaron cuatro errores no críticos y ninguna solicitud de ayuda.
4. **Eficiencia:** las medianas de T1–T6 se mantuvieron por debajo de sus metas. T7 superó su meta, pero todas las tareas permanecieron dentro de sus máximos.
5. **Satisfacción:** el promedio SUS fue 89,17, superior en 21,17 puntos a la referencia de 68.
6. **Calidad de los registros:** antes de cerrar la entrega grupal se debe revisar la diferencia entre los tiempos individuales y los tiempos de la tabla consolidada.

## 9. Fuentes de verificación

- Registros individuales de ejecución y SUS de P1, P2 y P3.
- Protocolo de evaluación de Fase 3.
- Registro consolidado de sesiones de Fase 3.
- Matriz consolidada de hallazgos.
- Cuestionario SUS y su procedimiento de puntuación.

---
