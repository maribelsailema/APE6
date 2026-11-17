# ☕ CaféU – APE 6: Planificación de la Evaluación de Usabilidad

> 🎓 **Universidad Técnica de Ambato**
> 🏛️ Facultad de Ingeniería en Sistemas, Electrónica e Industrial
> 💻 **Carrera:** Ingeniería de Software
> 📚 **Semestre:** Quinto
> 🧠 **Asignatura:** Interacción Humano-Computador
> 👨‍🏫 **Docente:** Ing. José Rubén Caiza Caizabuano, Mg.
> 📝 **Actividad:** APE 6 – Fase 1
> 🚀 **Proyecto:** CaféU



## 1. 📖 Descripción del proyecto

**CaféU** es un prototipo de interfaz web diseñado para que los estudiantes universitarios puedan realizar pedidos de cafetería **sin necesidad de comunicarse verbalmente** con el personal. 🗣️❌

El sistema permite:

- 📋 Consultar un menú
- 🛒 Seleccionar productos
- 👀 Revisar el pedido
- ✏️ Modificarlo
- ✅ Confirmar la compra

> 💡 El prototipo fue trabajado durante los **APE 4 y APE 5**, donde se analizaron los problemas de interacción, se realizaron propuestas de rediseño y se desarrollaron mejoras relacionadas con la navegación, la claridad de los botones y la confirmación del pedido.
>
> En el **APE 6** se planifica una evaluación de usabilidad para comprobar si los estudiantes pueden completar sus pedidos de manera **eficaz, eficiente y satisfactoria**. 🎯

---

## 2. 🎯 Objetivo general

Diseñar un **plan de evaluación de usabilidad** del prototipo CaféU, utilizando:

- 📘 La norma **ISO 9241-11**
- 🔟 Las **diez heurísticas de Nielsen**
- 🗣️ Pruebas con usuarios mediante **pensamiento en voz alta**

---

## 3. 🎯 Objetivos específicos

- 🔍 Identificar los usuarios y el contexto de utilización de CaféU.
- ❓ Formular una pregunta de evaluación basada en **eficacia, eficiencia y satisfacción**.
- 📐 Planificar una evaluación mediante las **diez heurísticas de Nielsen**.
- 👥 Diseñar una prueba con **tres participantes** externos al grupo.
- 📝 Preparar **seis tareas** relacionadas con el proceso de compra.
- 📊 Definir las **métricas de evaluación** y los instrumentos necesarios.
- 📋 Incorporar el cuestionario **System Usability Scale (SUS)**.
- 🔒 Garantizar la participación **voluntaria y confidencial**.
- ✅ Establecer **responsabilidades y criterios de validación**.

---

## 4. 🧩 Funcionalidades del prototipo

El prototipo CaféU contempla las siguientes funcionalidades:

| # | Funcionalidad | Icono |
|---|---|---|
| 1 | Visualización del menú de productos | 📋 |
| 2 | Selección de productos disponibles | 🛒 |
| 3 | Revisión de productos agregados al pedido | 👁️ |
| 4 | Modificación de cantidades o productos | ✏️ |
| 5 | Actualización del total del pedido | 💰 |
| 6 | Confirmación de la compra | ✅ |
| 7 | Visualización del mensaje de confirmación | 🎉 |

### 🧪 Caso de referencia

| Producto | Cantidad | Precio unitario | Subtotal |
|---|---:|---:|---:|
| ☕ Café | 1 | $1,50 | $1,50 |
| 🥪 Sánduche | 1 | $2,75 | $2,75 |
| **Total** | **2** | | **$4,25** |

> 🔎 Este caso permitirá evaluar si el usuario identifica correctamente los productos y el total antes de confirmar.

---

## 5. 👥 Equipo de trabajo

| 👤 Integrante | 💼 Responsabilidad | 🎭 Rol durante las pruebas |
|---|---|---|
| **Viviana** | 📄 Documentación y planificación | 🎙️ Moderadora |
| **Wilson** | 💻 HTML5 y pruebas con usuarios | 👁️ Observador |
| **Sebastián** | 📱 Diseño responsive | 🔧 Soporte técnico |
| **Alex** | 🔄 Interacción y métricas | 📈 Responsable de métricas |

---

## 6. 🧪 Métodos de evaluación

### 🔟 Evaluación heurística

Se utilizarán las **diez heurísticas de Nielsen** para identificar posibles problemas relacionados con:

- 🧭 Navegación
- 🎛️ Claridad de los controles
- 🛡️ Prevención de errores
- 🔁 Consistencia
- 🔔 Retroalimentación

### 🗣️ Pensamiento en voz alta

Se planificará una prueba con **tres estudiantes** ajenos al equipo desarrollador.

Los participantes realizarán **seis tareas** relacionadas con el pedido mientras expresan en voz alta lo que piensan. 🧠💭

---

## 7. 📊 Métricas de usabilidad

| Dimensión | 📏 Métrica |
|---|---|
| ✅ **Eficacia** | Tasa de tareas completadas |
| ⏱️ **Eficiencia** | Tiempo por tarea |
| ⚠️ **Errores** | Críticos y no críticos |
| 😊 **Satisfacción** | Cuestionario SUS |
| 🧐 **Dificultades** | Observación de comportamiento |

---

## 8. 👤 Participantes

Se contempla la participación de **tres estudiantes universitarios** externos al equipo desarrollador.

Se identificarán mediante códigos:

| Código | Estado |
|---|---|
| 🧑‍🎓 **P01** | Por confirmar |
| 🧑‍🎓 **P02** | Por confirmar |
| 🧑‍🎓 **P03** | Por confirmar |

> 🔐 **Confidencialidad:** No se publicarán nombres ni información personal.

---

## 9. 📁 Estructura del repositorio

```text
📦 APE6/
├── 📘 README.md
├── 📂 docs/
│   ├── 📄 plan-evaluacion.md
│   ├── 👥 participantes-roles.md
│   └── 📝 consentimiento-informado.md
├── 📂 evaluacion/
│   ├── 📋 matriz-tareas.md
│   ├── 🗣️ protocolo-pensamiento-voz-alta.md
│   ├── 🔍 evaluacion-heuristica.md
│   ├── 📐 matriz-heuristicas.md
│   ├── 📊 metricas-usabilidad.md
│   ├── 👁️ hoja-observacion.md
│   ├── 📝 cuestionario-sus.md
│   └── ✅ criterios-validacion.md
└── 📂 informe/
    └── 📕 APE6-Fase1-Plan-Evaluacion-CafeU.pdf