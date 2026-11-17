# ✅ Verificación de la Fase 1 – Protocolo de Evaluación de CaféU

**Asignatura:** Interacción Humano-Computador  
**Institución:** Universidad Técnica de Ambato – FISEI  
**Carrera:** Ingeniería de Software – Quinto semestre  
**Actividad:** APE 6 – Fase 2  
**Responsable:** Sarco Sailema Viviana Maribel  
**Rol:** Moderadora y responsable de documentación  
**Issue:** [APE6-F2-01 #9](https://github.com/maribelsailema/APE6/issues/9)  
**Fecha de revisión documental:** 17 de noviembre de 2026

---

## 1. 🎯 Objetivo

Verificar la existencia, pertinencia y consistencia de los documentos
elaborados durante la Fase 1 del APE 6, antes de consolidar los
resultados del pilotaje con tres estudiantes externos al equipo.

El proyecto evaluado es CaféU, un prototipo de aplicación web que
permite consultar productos de cafetería, seleccionar alimentos,
personalizar pedidos, revisar importes y confirmar una compra.

La evaluación considera eficacia, eficiencia y satisfacción,
siguiendo el enfoque de ISO 9241-11.

---

## 2. 📁 Inventario de documentos de la Fase 1

| N.º | Documento | Ubicación | Verificación |
|---|---|---|---|
| 1 | Plan de evaluación | `docs/plan-evaluacion.md` | ✅ Disponible; corresponde a CaféU |
| 2 | Consentimiento informado | `docs/consentimiento-informado.md` | ✅ Disponible; corresponde a CaféU |
| 3 | Participantes y roles | `docs/participantes-roles.md` | ✅ Disponible; corresponde a CaféU |
| 4 | Matriz de seis tareas | `evaluacion/matriz-tareas.md` | ✅ Disponible; contiene seis tareas de CaféU |
| 5 | Protocolo de pensamiento en voz alta | `evaluacion/protocolo-pensamiento-voz-alta.md` | ✅ Disponible; corresponde a CaféU |
| 6 | Guía de evaluación heurística | `evaluacion/evaluacion-heuristica.md` | ✅ Archivo disponible |
| 7 | Matriz de heurísticas | `evaluacion/matriz-heuristicas.md` | ✅ Archivo disponible |
| 8 | Métricas de usabilidad | `evaluacion/metricas-usabilidad.md` | ⚠️ Disponible; menciona otro proyecto |
| 9 | Cuestionario SUS | `evaluacion/cuestionario-sus.md` | ⚠️ Disponible; menciona otro proyecto |
| 10 | Hoja de observación | `evaluacion/hoja-observacion.md` | ⚠️ Disponible; contiene tareas de reservas ajenas a CaféU |
| 11 | Criterios de validación | `evaluacion/criterios-validacion.md` | ⚠️ Disponible; menciona otro proyecto y escenarios de reservas |

**Resultado de la revisión:**

Los documentos fundamentales existen en el repositorio. Sin embargo,
la disponibilidad de un archivo no significa que todo su contenido
sea consistente con el prototipo CaféU.

Se identificaron diferencias entre algunos instrumentos de Fase 1,
que deberán corregirse para una próxima aplicación del protocolo.

---

## 3. 🧩 Correspondencia de las seis tareas con CaféU

La matriz principal `evaluacion/matriz-tareas.md` define:

| Tarea | Actividad | Respuesta o estado esperado |
|---|---|---|
| T1 | Consultar el precio del café americano | USD 1,50 |
| T2 | Filtrar productos de la categoría Snacks | Galleta de avena, USD 1,25 |
| T3 | Personalizar un café americano | Incorporar la nota "Sin azúcar" |
| T4 | Agregar un sánduche y revisar el pedido | Total de USD 4,25 |
| T5 | Eliminar el sánduche | Nuevo total de USD 1,50 |
| T6 | Confirmar y consultar el comprobante | Código #CU-104, espera de 5 a 10 minutos y pago en caja rápida |

Estas seis tareas corresponden al recorrido principal del
prototipo utilizado durante el pilotaje.

**Fuente:**
[`evaluacion/matriz-tareas.md`](../evaluacion/matriz-tareas.md)

---

## 4. ⚠️ Inconsistencias documentales identificadas

### I-01. Nombre incorrecto del proyecto

Los archivos de métricas, cuestionario SUS, hoja de observación y
criterios de validación contienen referencias a "Aula Abierta".

**Impacto:** Puede generar confusión respecto al sistema evaluado.

**Propuesta:** Preparar una versión corregida de los instrumentos
identificada expresamente como CaféU.

### I-02. Hoja de observación de otro flujo

La hoja de observación disponible en Fase 1 incluye actividades como:

- Identificar una reserva disponible.
- Confirmar una reserva.
- Cancelar una reserva.
- Iniciar una nueva reserva.

Estas tareas no corresponden al pedido de cafetería.

**Impacto:** Los campos generales de observación son reutilizables,
pero las consignas no son adecuadas para evaluar CaféU.

**Propuesta:** Crear una hoja V2 que utilice exactamente las tareas
T1 a T6 de `evaluacion/matriz-tareas.md`.

### I-03. Diferencias en la redacción del SUS

El documento `cuestionario-sus.md` contiene la formulación general
del cuestionario, mientras que el protocolo de pensamiento en voz
alta y los registros individuales incluyen redacciones
contextualizadas para CaféU.

**Impacto:** Es necesario identificar qué versión fue presentada
a los participantes para conservar la trazabilidad y facilitar
comparaciones futuras.

**Propuesta:** Definir una única versión para las siguientes
evaluaciones, conservar las respuestas originales y registrar
expresamente cualquier adaptación del instrumento.

### I-04. Criterios de validación sin cierre formal

El archivo `evaluacion/criterios-validacion.md` contiene una lista
de comprobación, pero no presenta todos los criterios marcados
como cumplidos para CaféU.

**Impacto:** No puede afirmarse que la lista de verificación original
quedó cerrada formalmente.

**Propuesta:** Revisar y documentar los criterios aplicables antes
de ejecutar un nuevo pilotaje.

### I-05. Diferencia en el tiempo máximo total

La matriz de tareas fija los siguientes tiempos máximos:

- T1: 60 segundos.
- T2: 60 segundos.
- T3: 90 segundos.
- T4: 90 segundos.
- T5: 60 segundos.
- T6: 90 segundos.

La suma correcta es:

**60 + 60 + 90 + 90 + 60 + 90 = 450 segundos (7 min 30 s).**

Una sección de la matriz indica 420 segundos.

**Propuesta:** Corregir el total documental a 450 segundos,
sin alterar los límites originales de las seis tareas.

---

## 5. 👥 Verificación del pilotaje

Según la confirmación de la moderadora y los registros disponibles,
el pilotaje se desarrolló el 16 de noviembre de 2026.

| Participante | Perfil | Consentimiento | Registro |
|---|---|---|---|
| P1 | Estudiante externo; dispositivo móvil | ✅ Aplicado | [P1.md](Participantes/P1.md) |
| P2 | Estudiante externo; computadora portátil | ✅ Aplicado | [P2.md](Participantes/P2.md) |
| P3 | Estudiante externo; dispositivo móvil | ✅ Aplicado | [P3.md](Participantes/P3.md) |

Las tres sesiones fueron moderadas por Viviana Sarco.

Los documentos publicados incluyen seis tareas por participante,
tiempos, resultados, errores, observaciones y respuestas SUS.

La evidencia personal del consentimiento no se incorpora al
repositorio público para proteger la identidad de los participantes.

---

## 6. 📊 Resumen de los resultados registrados

| Indicador | P1 | P2 | P3 |
|---|---:|---:|---:|
| Tareas completadas | 6/6 | 6/6 | 6/6 |
| Tiempo acumulado en tareas | 235 s | 169 s | 173 s |
| Errores críticos | 0 | 0 | 0 |
| Errores no críticos registrados | 3 | 0 | 1 |
| Solicitudes de ayuda | 0 | 0 | 0 |
| Puntaje SUS reportado | 82,5 | 85,0 | 80,0 |

**Resultados globales derivados de los registros:**

- Tareas completadas: 18 de 18.
- Tasa de éxito: 100 %.
- Errores críticos: 0.
- Errores no críticos registrados: 4.
- Tiempo mediano acumulado por participante: 173 segundos.
- Promedio de puntuaciones SUS reportadas: 82,5 puntos.

**Precisión metodológica:**

Los 173 segundos corresponden a la mediana de la suma de
duraciones de las seis tareas por participante. No incluyen
bienvenida, consentimiento, aplicación de SUS ni cierre de la sesión.

El registro P3 clasifica como error no crítico una observación
sobre la ausencia de animación o indicador destacado en el carrito,
aunque señala que el participante lo encontró sin dificultad.
Esta clasificación deberá revisarse antes de consolidar
definitivamente los errores.

---

## 7. 🔍 Comparación con los criterios originales

| Criterio | Referencia de Fase 1 | Resultado del pilotaje | Interpretación |
|---|---|---|---|
| Tres participantes externos | `docs/plan-evaluacion.md` | Tres registros P1–P3 | ✅ Cumplido según registros y confirmación de la moderadora |
| Seis tareas por participante | `evaluacion/matriz-tareas.md` | 18 ejecuciones | ✅ Cumplido |
| Éxito dentro del tiempo máximo | Máximos entre 60 y 90 s | Ninguna duración supera su límite | ✅ Cumplido |
| Pensamiento en voz alta | `evaluacion/protocolo-pensamiento-voz-alta.md` | Comentarios registrados en P1–P3 | ✅ Evidencia documental disponible |
| Consentimiento | `docs/consentimiento-informado.md` | Aplicado a los tres participantes | ✅ Confirmado por la moderadora |
| Cuestionario SUS | `evaluacion/cuestionario-sus.md` | Diez respuestas por participante | ✅ Resultados disponibles; versión textual por armonizar |
| Criterios de validación documental | `evaluacion/criterios-validacion.md` | Existen discrepancias de proyecto y tareas | ⚠️ Requiere corrección documental |

Los tiempos objetivo se cumplieron en 14 de las 18
ejecuciones. Las cuatro ejecuciones restantes superaron
el objetivo, pero ninguna excedió el tiempo máximo.

La Fase 1 no establece una meta global explícita de
tasa de éxito del 100 %. Por ello, el resultado observado
se reporta como dato, no como comparación con una meta
que no fue definida.

---

## 8. ✅ Conclusión de la verificación

La documentación de la Fase 1 proporciona una base
suficiente para identificar el método, las tareas, los
participantes, las métricas y las responsabilidades.

Los tres registros del pilotaje contienen resultados
que permiten analizar el desempeño de CaféU.

No obstante, se requiere una revisión documental debido
a las referencias a otro proyecto, diferencias en el SUS,
una hoja de observación incompatible y un error en la
suma de tiempos máximos.

Estas observaciones fundamentan las propuestas incluidas
en `Ajustes_Protocolo_V1_V2.md`.

**Estado:** Verificación documental realizada;
armonización del protocolo V2 propuesta, aún no implementada.