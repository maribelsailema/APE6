
# Plan de Evaluación de Usabilidad del Prototipo CaféU

## 1. Información general

| Campo | Información |
|---|---|
| Universidad | Universidad Técnica de Ambato |
| Carrera | Ingeniería de Software |
| Semestre | Quinto |
| Asignatura | Interacción Humano-Computador |
| Actividad | APE 6 – Fase 1 |
| Prototipo | CaféU |
| Docente | Ing. José Rubén Caiza Caizabuano, Mg. |
| Responsable | Viviana |
| Modalidad | Trabajo grupal |
| Tiempo académico | 2 horas |

## 2. Introducción

La usabilidad es un aspecto importante en el desarrollo de interfaces, ya que permite conocer si los usuarios pueden cumplir sus objetivos sin dificultades innecesarias.

En el caso de CaféU, se busca que los estudiantes universitarios puedan realizar pedidos de cafetería de manera sencilla, sin necesidad de comunicarse verbalmente con el personal.

Durante los APE 4 y 5 se trabajó en el análisis y rediseño del prototipo, considerando problemas relacionados con la navegación, la claridad de los botones y la confirmación de pedidos.

En esta nueva práctica se planifica una evaluación de usabilidad que permitirá comprobar la eficacia, eficiencia y satisfacción de los usuarios al interactuar con CaféU.

## 3. Definición del prototipo

### 3.1 Descripción del sistema

CaféU es una interfaz web que permite consultar productos de cafetería y realizar un pedido.

El usuario puede seleccionar productos, revisar los elementos agregados, modificar el pedido y confirmar la compra.

El sistema presenta un resumen del pedido y un mensaje de confirmación al finalizar.

### 3.2 Usuarios objetivo

Los principales usuarios son estudiantes universitarios que desean comprar productos de cafetería de manera rápida y sencilla.

Se consideran usuarios con diferentes niveles de experiencia utilizando aplicaciones web.

### 3.3 Contexto de utilización

**Contexto físico:** cafetería universitaria, aulas o espacios donde el estudiante pueda acceder al prototipo.

**Contexto tecnológico:** navegador web desde una computadora o dispositivo móvil.

**Contexto social:** estudiantes que desean realizar pedidos sin comunicarse verbalmente con el personal de cafetería.

**Contexto de uso:** consulta de productos, selección, revisión, modificación y confirmación de pedidos.

### 3.4 Flujo principal

```text
Inicio
  ↓
Menú de productos
  ↓
Selección de productos
  ↓
Revisión del pedido
  ↓
¿El pedido es correcto?
  ├── No → Modificar pedido → Revisar nuevamente
  └── Sí → Confirmar pedido
                    ↓
           Mensaje de confirmación
```

## 4. Pregunta de evaluación

**¿En qué medida los estudiantes universitarios pueden seleccionar productos, revisar, modificar y confirmar un pedido en CaféU de manera eficaz, eficiente y satisfactoria, sin recibir instrucciones directas sobre cómo utilizar la interfaz?**

Esta pregunta contempla tres dimensiones:

### Eficacia

Determinar si el usuario puede completar correctamente las tareas relacionadas con el pedido.

### Eficiencia

Conocer cuánto tiempo necesita el usuario para realizar las tareas y qué dificultades encuentra durante el proceso.

### Satisfacción

Identificar la percepción del usuario respecto a la facilidad de uso mediante el cuestionario SUS.

## 5. Objetivo general

Planificar una evaluación de usabilidad del prototipo CaféU, aplicando los principios de ISO 9241-11, las heurísticas de Nielsen y pruebas con pensamiento en voz alta.

## 6. Objetivos específicos

1. Definir el contexto de utilización del prototipo.
2. Identificar el perfil de los usuarios.
3. Preparar una evaluación heurística.
4. Diseñar una prueba con pensamiento en voz alta.
5. Establecer seis tareas representativas.
6. Definir métricas de eficacia, eficiencia y satisfacción.
7. Preparar instrumentos de observación y cuestionario SUS.
8. Garantizar la participación voluntaria y confidencial.
9. Establecer criterios para la ejecución posterior.

## 7. Aplicación de ISO 9241-11

La norma ISO 9241-11:2018 establece un marco para comprender la usabilidad en relación con usuarios, objetivos y contextos de uso específicos.

Para CaféU se consideran:

| Dimensión | Aplicación |
|---|---|
| Eficacia | Completar correctamente un pedido |
| Eficiencia | Tiempo requerido y dificultades |
| Satisfacción | Opinión del usuario mediante SUS |

### Ejemplo

Se plantea que un estudiante realice el siguiente pedido:

- Un café de $1,50.
- Un sánduche de $2,75.

El total correcto es de $4,25.

Se evaluará si el estudiante logra seleccionar los productos, verificar el total y confirmar el pedido sin recibir ayuda directa.

## 8. Método 1: Evaluación heurística

La evaluación heurística permitirá identificar posibles problemas de usabilidad mediante las diez heurísticas de Nielsen.

| N.º | Heurística | Aplicación en CaféU |
|---|---|---|
| 1 | Visibilidad del estado del sistema | Mostrar productos agregados y confirmación |
| 2 | Relación con el mundo real | Utilizar nombres y precios comprensibles |
| 3 | Control y libertad del usuario | Permitir editar el pedido |
| 4 | Consistencia y estándares | Mantener estilos y controles coherentes |
| 5 | Prevención de errores | Evitar confirmaciones incorrectas |
| 6 | Reconocimiento antes que recuerdo | Mantener visible el resumen |
| 7 | Flexibilidad y eficiencia | Facilitar la selección y modificación |
| 8 | Diseño estético y minimalista | Mostrar información relevante |
| 9 | Reconocer y recuperar errores | Informar errores y permitir corrección |
| 10 | Ayuda y documentación | Mostrar indicaciones cuando sean necesarias |

### Procedimiento

El evaluador revisará las pantallas principales del prototipo y registrará los problemas encontrados.

Cada hallazgo incluirá:

- Código del problema.
- Pantalla donde ocurre.
- Heurística afectada.
- Descripción.
- Severidad.
- Evidencia.
- Recomendación.

### Escala de severidad

| Nivel | Descripción |
|---|---|
| 0 | No representa un problema |
| 1 | Problema cosmético |
| 2 | Problema menor |
| 3 | Problema importante |
| 4 | Problema crítico |

## 9. Método 2: Pensamiento en voz alta

La prueba con usuarios utilizará la técnica de pensamiento en voz alta.

Se solicitará al participante que exprese lo que piensa mientras realiza las tareas.

El propósito es conocer cómo interpreta la interfaz y qué dificultades encuentra.

### Instrucciones del moderador

"Vas a utilizar el prototipo CaféU para realizar algunas actividades relacionadas con un pedido de cafetería. Mientras avanzas, comenta lo que estás pensando, qué esperas encontrar y qué dudas tienes. No estamos evaluando tus capacidades, sino la facilidad de uso del sistema."

### Preguntas neutrales permitidas

- ¿Qué estás pensando en este momento?
- ¿Qué esperabas que ocurriera?
- ¿Qué estás buscando?
- ¿Puedes contarme qué estás intentando hacer?

### Indicaciones que deben evitarse

- Decir qué botón presionar.
- Mostrar dónde se encuentra una función.
- Corregir inmediatamente al participante.
- Indicar cuál es la respuesta correcta.

## 10. Participantes

Se seleccionarán tres estudiantes universitarios ajenos al equipo desarrollador.

| Código | Perfil previsto | Dispositivo |
|---|---|---|
| P01 | Estudiante con experiencia digital básica | Móvil |
| P02 | Estudiante con experiencia intermedia | Computadora |
| P03 | Estudiante que utiliza aplicaciones web habitualmente | Móvil |

Los perfiles son criterios de reclutamiento, no personas ya seleccionadas.

### Criterios de inclusión

- Ser estudiante universitario.
- No pertenecer al grupo desarrollador.
- Aceptar voluntariamente participar.
- Poder interactuar con un navegador web.

### Criterios de exclusión

- Haber desarrollado el prototipo.
- No aceptar participar.
- Haber recibido previamente las respuestas de las tareas.

## 11. Diseño general de las seis tareas

Las tareas se formularán mediante situaciones reales.

| ID | Situación de evaluación | Resultado esperado |
|---|---|---|
| T01 | Conocer qué productos se ofrecen | Identificar el menú |
| T02 | Elegir una bebida para el pedido | Seleccionar un café |
| T03 | Completar el pedido con un alimento | Agregar un sánduche |
| T04 | Comprobar el costo del pedido | Identificar $4,25 |
| T05 | Corregir un pedido antes de comprar | Modificar el contenido |
| T06 | Finalizar la compra | Confirmar y reconocer el resultado |

La matriz completa incluirá instrucciones, tiempos objetivo, tiempos máximos y criterios de éxito.

## 12. Métricas de usabilidad

### 12.1 Tasa de éxito

Se calculará mediante:

```text
Tasa de éxito (%) =
(Tareas completadas correctamente / Tareas intentadas) × 100
```

### 12.2 Tiempo por tarea

Se registrará el tiempo desde que el participante inicia una tarea hasta que la completa o alcanza el límite establecido.

### 12.3 Errores críticos

Se considerarán errores críticos aquellos que impidan completar la tarea o generen un pedido incorrecto que no sea corregido.

### 12.4 Errores no críticos

Serán dificultades recuperables, como seleccionar una opción equivocada y corregirla posteriormente.

### 12.5 Satisfacción

Se aplicará el cuestionario SUS de diez afirmaciones, con respuestas de 1 a 5.

El puntaje se calculará después de completar la sesión.

## 13. Instrumentos

| Instrumento | Finalidad |
|---|---|
| Consentimiento informado | Garantizar participación voluntaria |
| Matriz de seis tareas | Establecer instrucciones y criterios |
| Matriz heurística | Registrar problemas de usabilidad |
| Hoja de observación | Registrar tiempos, errores y dificultades |
| Cuestionario SUS | Evaluar satisfacción |
| Criterios de validación | Comprobar preparación del protocolo |

## 14. Aspectos éticos

La evaluación se desarrollará respetando:

**Participación voluntaria:** cada estudiante decidirá si desea participar.

**Confidencialidad:** la información recopilada se utilizará exclusivamente para fines académicos.

**Anonimato:** los resultados se identificarán mediante códigos.

**Derecho a retirarse:** los participantes podrán abandonar la evaluación sin consecuencias.

**Protección de información:** no se publicarán nombres, firmas ni datos personales en GitHub.

No se realizarán grabaciones identificables sin autorización adicional.

## 15. Asignación de roles

| Integrante | Rol | Responsabilidad |
|---|---|---|
| Viviana | Moderadora | Explicar las tareas y dirigir la sesión |
| Wilson | Observador | Registrar dificultades y comportamientos |
| Sebastián | Soporte técnico | Preparar el prototipo y dispositivos |
| Alex | Responsable de métricas | Registrar tiempos, errores y SUS |

## 16. Cronograma de evaluación

Se propone una duración aproximada de 25 minutos por participante.

| Actividad | Tiempo |
|---|---:|
| Bienvenida | 3 min |
| Consentimiento | 3 min |
| Explicación de pensamiento en voz alta | 2 min |
| Ejecución de seis tareas | 12 min |
| Cuestionario SUS | 4 min |
| Cierre | 1 min |
| **Total** | **25 min** |

Para tres participantes se estima un total de 75 minutos de sesiones individuales, sin incluir preparación y organización.

## 17. Criterios de validación

El protocolo estará preparado para la Fase 2 cuando:

1. El prototipo pueda abrirse correctamente.
2. Las seis tareas correspondan a funciones disponibles.
3. Cada tarea tenga instrucciones neutrales.
4. Se definan tiempos y criterios de éxito.
5. Se disponga de la matriz de Nielsen.
6. Exista una hoja de observación.
7. El cuestionario SUS incluya diez afirmaciones.
8. Se disponga del consentimiento informado.
9. Los cuatro roles estén asignados.
10. Se hayan previsto tres participantes externos al grupo.
11. Se establezca cómo actuar ante problemas técnicos.
12. La documentación esté organizada en GitHub.

## 18. Resultados esperados

Se espera que la aplicación posterior de las pruebas permita identificar:

- Dificultades al seleccionar productos.
- Problemas para revisar y modificar pedidos.
- Errores al interpretar precios.
- Dudas al confirmar la compra.
- Tiempo necesario para completar las tareas.
- Nivel de satisfacción percibida.

Estos resultados se obtendrán en la Fase 2.

## 19. Conclusión

El plan de evaluación de CaféU establece una metodología para analizar la facilidad de uso del prototipo mediante inspección heurística y pruebas con usuarios.

La combinación de ISO 9241-11, las heurísticas de Nielsen y el pensamiento en voz alta permitirá evaluar tanto los aspectos técnicos como la experiencia de los estudiantes.

La planificación de participantes, roles, métricas e instrumentos proporciona una base organizada para desarrollar la evaluación durante la siguiente fase.

## 20. Referencias

[1] ISO, *ISO 9241-11:2018. Ergonomics of human-system interaction — Part 11: Usability: Definitions and concepts*, 2018.

[2] J. Nielsen, “10 Usability Heuristics for User Interface Design,” Nielsen Norman Group, 1994.

[3] J. Brooke, “SUS: A Quick and Dirty Usability Scale,” en *Usability Evaluation in Industry*, 1996.
