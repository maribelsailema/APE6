
# 📋 Plan de evaluación de usabilidad — Aula Abierta

## 1. Datos generales

| Campo | Información |
|---|---|
| Institución | Universidad Técnica de Ambato |
| Carrera | Ingeniería de Software |
| Semestre | Quinto |
| Asignatura | Interacción Humano-Computador |
| Práctica | APE 6 — Fase 1 |
| Prototipo | Aula Abierta |
| Modalidad | Grupal |
| Duración académica estimada | 2 horas |
| Docente | Ing. José Rubén Caiza Caizabuano, Mg. |
| Responsable del plan | Viviana |
| Estado | Planificación |

## 2. Descripción del prototipo

Aula Abierta es una interfaz web responsive para consultar información de talleres académicos y gestionar reservas.

El prototipo presenta la información de un taller, incluyendo nombre, horario y laboratorio, además de un panel denominado «Mi reserva».

La interacción contempla tres estados:

- Disponible: el estudiante puede reservar.
- Confirmada: la reserva se encuentra activa.
- Cancelada: la reserva fue anulada.

La interfaz fue planteada con HTML5 semántico, CSS Mobile-First y JavaScript.

En pantallas móviles se utiliza una columna y, desde un punto de corte de 48rem, una distribución de dos columnas.

El prototipo se evalúa como una interfaz de demostración, sin asumir que cuenta con autenticación, base de datos o persistencia de reservas.

## 3. Usuarios objetivo

Los usuarios objetivo son estudiantes universitarios que desean consultar talleres y gestionar una reserva.

Se consideran estudiantes con diferentes niveles de experiencia utilizando sitios web, tanto desde teléfonos móviles como desde computadoras.

### Necesidades

- Identificar el taller disponible.
- Consultar cuándo se realiza.
- Identificar dónde se desarrolla.
- Confirmar una reserva.
- Comprobar su estado.
- Cancelar cuando sea necesario.

## 4. Contexto de utilización

### Entorno físico

La evaluación se realizará en un espacio tranquilo, con iluminación adecuada, sin interrupciones y con conexión local o acceso estable al prototipo.

### Entorno tecnológico

Se utilizará un navegador web moderno en un equipo de escritorio o móvil.

El prototipo deberá estar disponible antes de iniciar cada sesión.

### Entorno social

Las tareas representan situaciones académicas habituales en las que un estudiante consulta información y decide participar en un taller.

### Condiciones de evaluación

- El participante no recibirá instrucciones sobre qué controles presionar.
- Se presentarán las tareas una por una.
- El moderador mantendrá una actitud neutral.
- Se permitirá que el participante piense en voz alta.
- Se registrarán dificultades sin interrumpir innecesariamente.

## 5. Pregunta de evaluación

**¿En qué medida los estudiantes universitarios pueden consultar la información de un taller, confirmar y cancelar una reserva en Aula Abierta de manera eficaz, eficiente y satisfactoria, utilizando la interfaz sin instrucciones sobre los controles?**

### Dimensiones

**Eficacia:** determinar si las tareas se completan correctamente.

**Eficiencia:** medir el tiempo empleado para completar cada tarea.

**Satisfacción:** conocer la percepción del usuario mediante el cuestionario SUS.

## 6. Objetivo general

Planificar una evaluación de usabilidad del prototipo Aula Abierta mediante inspección heurística y pruebas con usuarios, para comprobar la eficacia, eficiencia y satisfacción durante la consulta y gestión de reservas.

## 7. Objetivos específicos

1. Definir el contexto de uso del prototipo.
2. Preparar una inspección basada en las diez heurísticas de Nielsen.
3. Diseñar una prueba con pensamiento en voz alta.
4. Seleccionar tres participantes externos al equipo.
5. Establecer seis tareas con tiempos y criterios de éxito.
6. Definir métricas e instrumentos de recolección.
7. Preparar el cuestionario SUS.
8. Garantizar el tratamiento ético de los participantes.
9. Establecer criterios de preparación para la Fase 2.

## 8. Fundamento de ISO 9241-11

La norma ISO 9241-11:2018 define la usabilidad en relación con usuarios, objetivos y contextos de uso específicos.

Para este proyecto se consideran tres dimensiones principales.

| Dimensión | Aplicación en Aula Abierta |
|---|---|
| Eficacia | Completar correctamente las seis tareas |
| Eficiencia | Tiempo y recursos utilizados |
| Satisfacción | Percepción de facilidad y comodidad |

La evaluación se desarrollará en un contexto definido para que los resultados puedan interpretarse de manera coherente.

## 9. Método 1: Evaluación heurística

Se utilizarán las diez heurísticas de Nielsen como criterios de inspección.

| N.º | Heurística | Aspecto que se revisará |
|---|---|---|
| 1 | Visibilidad del estado | Mensajes de confirmación y cancelación |
| 2 | Relación con el mundo real | Lenguaje comprensible para estudiantes |
| 3 | Control y libertad | Posibilidad de cancelar |
| 4 | Consistencia y estándares | Etiquetas, controles y estilos |
| 5 | Prevención de errores | Bloqueo de reservas duplicadas |
| 6 | Reconocimiento antes que recuerdo | Información visible del taller |
| 7 | Flexibilidad y eficiencia | Facilidad de completar las acciones |
| 8 | Diseño minimalista | Jerarquía y claridad del contenido |
| 9 | Recuperación de errores | Información y alternativas ante fallos |
| 10 | Ayuda y documentación | Orientaciones cuando sean necesarias |

### Procedimiento planificado

El evaluador recorrerá la interfaz y examinará cada heurística.

Los problemas se registrarán indicando:

- Código del hallazgo.
- Heurística afectada.
- Descripción.
- Ubicación.
- Evidencia.
- Severidad.
- Recomendación.

### Escala de severidad

| Valor | Significado |
|---|---|
| 0 | No representa un problema |
| 1 | Problema cosmético |
| 2 | Problema menor |
| 3 | Problema importante |
| 4 | Problema crítico |

## 10. Método 2: Prueba con pensamiento en voz alta

Se utilizará la técnica de pensamiento en voz alta para conocer qué interpreta el estudiante mientras realiza las tareas.

El participante deberá expresar lo que busca, lo que espera que ocurra y las dudas que experimente.

### Instrucción inicial del moderador

"Durante esta actividad te presentaré seis situaciones relacionadas con Aula Abierta. Intenta resolverlas como lo harías normalmente. Mientras interactúas, expresa en voz alta lo que estás pensando. No estamos evaluando tus conocimientos, sino la facilidad de uso de la interfaz. Puedes detenerte cuando lo desees."

### Intervenciones permitidas

- ¿Qué estás pensando ahora?
- ¿Qué esperabas que ocurriera?
- ¿Qué información estás buscando?
- ¿Puedes seguir contándome lo que piensas?

### Intervenciones que deben evitarse

- Indicar dónde se encuentra una opción.
- Decir qué botón debe utilizarse.
- Corregir inmediatamente los errores.
- Sugerir la respuesta correcta.
- Presionar al participante para completar la tarea.

## 11. Participantes

Se seleccionarán tres estudiantes universitarios que no formen parte del grupo desarrollador.

Los participantes se identificarán mediante códigos:

- P01
- P02
- P03

No se publicarán nombres, números de identificación, correos personales ni otros datos que permitan reconocerlos.

### Criterios de selección

- Ser estudiante universitario.
- No pertenecer al grupo desarrollador.
- No haber participado en la implementación del prototipo.
- Aceptar voluntariamente el consentimiento informado.
- Poder interactuar con un navegador web.

No se exigirá experiencia avanzada en tecnología.

## 12. Tareas de evaluación

Se utilizarán seis tareas relacionadas con las funciones disponibles.

| ID | Objetivo |
|---|---|
| T01 | Identificar el nombre del taller |
| T02 | Consultar el horario |
| T03 | Identificar el laboratorio |
| T04 | Confirmar una reserva |
| T05 | Comprobar el estado de la reserva |
| T06 | Cancelar la reserva |

Las instrucciones completas, tiempos objetivo, tiempos máximos, respuestas correctas y criterios de éxito se registrarán en `evaluacion/matriz-tareas.md`.

## 13. Métricas

### Eficacia

La tasa de éxito se calculará como:

Tasa de éxito (%) = (tareas completadas correctamente / tareas intentadas) × 100

Se registrará el resultado de cada tarea como:

- Éxito.
- Fallo.
- No completada dentro del tiempo máximo.

### Eficiencia

Se registrará la duración de cada tarea en segundos.

Tiempo = instante de finalización − instante de inicio.

También se anotarán solicitudes de ayuda y dificultades que afecten el desarrollo de la tarea.

### Errores

**Error crítico:** impide completar una tarea o produce un resultado incorrecto importante.

**Error no crítico:** provoca una dificultad recuperable sin impedir la finalización.

### Satisfacción

Se utilizará el cuestionario SUS, compuesto por diez afirmaciones con una escala de respuesta de 1 a 5.

La puntuación se calculará individualmente después de finalizar las tareas.

## 14. Instrumentos

| Instrumento | Finalidad |
|---|---|
| Consentimiento informado | Garantizar participación voluntaria |
| Matriz de tareas | Estandarizar situaciones y criterios |
| Matriz heurística | Registrar problemas de diseño |
| Hoja de observación | Registrar tiempos, errores y ayudas |
| Cuestionario SUS | Medir satisfacción percibida |
| Criterios de validación | Comprobar preparación del protocolo |

## 15. Aspectos éticos

La evaluación respetará los siguientes principios:

**Participación voluntaria:** ninguna persona estará obligada a participar.

**Consentimiento informado:** se explicará el propósito, duración, actividades y tratamiento de la información.

**Anonimato en los resultados:** los registros publicados utilizarán códigos.

**Confidencialidad:** los documentos que permitan identificar a los participantes no se publicarán en GitHub.

**Derecho a retirarse:** los participantes podrán finalizar su participación sin consecuencias.

**Minimización de datos:** se recogerá únicamente información necesaria para evaluar la interfaz.

**Sin grabación por defecto:** no se realizarán grabaciones de voz, vídeo o pantalla identificables sin autorización específica.

## 16. Asignación de roles

| Integrante | Rol | Función |
|---|---|---|
| Viviana | Moderadora | Presentar tareas y mantener neutralidad |
| Wilson | Observador | Registrar comportamientos y dificultades |
| Sebastián | Soporte técnico | Preparar navegador y prototipo |
| Alex | Responsable de métricas | Registrar tiempos, éxito y errores |

## 17. Secuencia de una sesión de pilotaje

| Etapa | Duración estimada |
|---|---:|
| Bienvenida y explicación | 3 min |
| Consentimiento informado | 3 min |
| Introducción al pensamiento en voz alta | 2 min |
| Ejecución de seis tareas | 12 min |
| Cuestionario SUS | 4 min |
| Cierre y agradecimiento | 1 min |
| **Total estimado** | **25 min** |

Las duraciones son objetivos de planificación, no tiempos observados.

## 18. Criterios de preparación del protocolo

El protocolo estará preparado para pasar a la Fase 2 cuando:

1. El prototipo pueda abrirse sin errores que impidan las tareas.
2. Las seis tareas correspondan a funciones existentes.
3. Cada tarea tenga instrucciones neutrales.
4. Se hayan definido tiempos y criterios de éxito.
5. Exista una matriz para las diez heurísticas.
6. La hoja de observación permita registrar resultados.
7. El SUS contenga sus diez afirmaciones.
8. El consentimiento esté disponible.
9. Los cuatro roles estén definidos.
10. Los tres participantes sean externos al equipo y acepten participar antes de la sesión.
11. Se disponga de un procedimiento para detener o reprogramar una prueba ante fallos técnicos.
12. La documentación esté organizada en GitHub.

## 19. Resultados esperados

Se espera que la aplicación posterior del protocolo permita identificar:

- Tareas que presentan mayores dificultades.
- Errores frecuentes.
- Diferencias en los tiempos de realización.
- Problemas de comprensión.
- Aspectos visuales o funcionales que requieren mejora.
- Percepción general de usabilidad mediante SUS.

En esta fase no se presentan resultados de usuarios, ya que la evaluación todavía no ha sido ejecutada.

## 20. Conclusión

El plan de evaluación de Aula Abierta integra una inspección heurística y una prueba con usuarios para examinar la interfaz desde dos perspectivas complementarias.

Las heurísticas permitirán identificar posibles problemas de diseño, mientras que el pensamiento en voz alta permitirá conocer las dificultades experimentadas durante las tareas.

La definición de métricas, instrumentos y medidas éticas proporciona una base organizada para ejecutar la evaluación durante la Fase 2.

## 21. Referencias

[1] ISO, ISO 9241-11:2018, Ergonomics of human-system interaction — Part 11: Usability: Definitions and concepts, 2018.

[2] J. Nielsen, "10 Usability Heuristics for User Interface Design," Nielsen Norman Group, 1994.

[3] J. Brooke, "SUS: A Quick and Dirty Usability Scale," en Usability Evaluation in Industry, 1996.
