# Evaluación Heurística Individual de Usabilidad — Prototipo CaféU


## 1. Introducción y Marco Metodológico

La **Evaluación Heurística** es un método de inspección de usabilidad analítico formalizado por Jakob Nielsen y Rolf Molich (1990), mediante el cual un evaluador experto examina la interfaz de un sistema interactivo confrontándola contra un conjunto consensuado de principios de diseño universalmente reconocidos (las 10 Heurísticas de Nielsen).

En el marco del APE 6, esta evaluación individual elaborada por **Wilson** cumple un rol estratégico de **triangulación metodológica**: combina la inspección analítica del diseño de CaféU con las evidencias cuantitativas y cualitativas observadas de primera mano durante la ejecución del pilotaje con tres estudiantes universitarios externos (`P1`, `P2`, `P3`).

---

## 2. Escala de Severidad de Problemas de Usabilidad

Para ponderar el impacto de los problemas identificados, se adopta la escala estándar de severidad de Jakob Nielsen (1995):

| Nivel | Clasificación | Criterio de Impacto en la Tarea |
| :---: | :--- | :--- |
| **0** | **No representa un problema** | Principio cumplido de forma satisfactoria. No se detectan fricciones ni dificultades para el usuario. |
| **1** | **Problema cosmético** | Inconsistencia superficial o estética menor. No afecta la ejecución de la tarea; corregir solo si sobra tiempo. |
| **2** | **Problema menor** | Produce duda, vacilación o demora leve en el usuario, pero este logra recuperarse por sí mismo. Prioridad media. |
| **3** | **Problema mayor / importante** | Causa confusión significativa, desorientación o induce a errores recurrentes. Debe corregirse prioritariamente. |
| **4** | **Problema crítico / catastrófico** | Impide por completo completar una tarea principal, genera pérdida de datos o bloquea al usuario. Corrección urgente obligatoria. |

---

## 3. Evaluación Detallada por Heurística (10 Heurísticas de Nielsen)

### Heurística H1: Visibilidad del estado del sistema
> *«El sistema debe mantener siempre informados a los usuarios de lo que está ocurriendo, mediante una retroalimentación adecuada y en un tiempo razonable.»*

- **Diagnóstico General:** **Satisfactorio con oportunidades de mejora en microinteracciones.**
- **Análisis por Vistas:**
  - **Pantalla de Inicio (`Inicio`):** El estado del usuario autenticado es visible en la cabecera mediante las iniciales (*"JD"* y *"Hola, Julia"*).
  - **Pantalla de Menú (`Menú`):** Al tocar el botón *"Añadir"*, el sistema actualiza la barra inferior flotante (*"2 items · $4.25 | Ver mi pedido"*). Sin embargo, durante el pilotaje se observó que la participante `P1` buscó el carrito en el *header* y no advirtió de inmediato la barra inferior fija por falta de una microinteracción dinámica de realce.
  - **Pantalla de Confirmación (`Confirmación`):** El cumplimiento es ejemplar. El checkmark verde de gran tamaño, el título *"¡Pedido recibido! Ya estamos preparando todo para ti"*, la tarjeta destacada con el código `#CU-104` y la indicación de tiempo (5 a 10 minutos) transmiten certeza absoluta.
- **Severidad Asignada:** **Nivel 2 (Problema menor).**
- **Recomendación Técnica:** Implementar una microinteracción de rebote vertical suave (*bounce* de 4 px) o cambio temporal de color en la barra flotante al momento de sumar un producto, complementado con un badge de notificación en la parte superior.

---

### Heurística H2: Correspondencia entre el sistema y el mundo real
> *«El sistema debe hablar el lenguaje de los usuarios, con palabras, frases y conceptos familiares para ellos, en lugar de términos orientados al sistema. Seguir convenciones del mundo real.»*

- **Diagnóstico General:** **Excelente cumplimiento.**
- **Análisis por Vistas:**
  - Los textos utilizan metáforas e indicaciones directas del contexto universitario ecuatoriano: *"Evita la fila: pide tu café aquí"*, *"Haz tu pedido y recógelo en la caja rápida"*, *"Paga al momento de retirar tu pedido"*.
  - Las categorías de productos (*Bebidas calientes*, *Sánduches*, *Snacks*) corresponden con la nomenclatura cotidiana de una cafetería de facultad.
  - La moneda está expresada en dólares de curso legal con formato claro (`$1.50`, `$2.75`, `$4.25`).
  - El campo de *Instrucciones especiales* contiene un placeholder ejemplificador intuitivo (*"Ej. Sin azúcar, leche aparte..."*).
- **Severidad Asignada:** **Nivel 0 (No representa un problema).**

---

### Heurística H3: Control y libertad del usuario
> *«Los usuarios suelen realizar acciones por error y necesitan una 'salida de emergencia' claramente marcada para abandonar el estado no deseado sin tener que pasar por un diálogo extendido.»*

- **Diagnóstico General:** **Bueno, con una vulnerabilidad en la eliminación de ítems.**
- **Análisis por Vistas:**
  - La navegación es abierta y reversible: todas las pantallas interiores cuentan con un botón de retroceso (`< Menú`, `< Detalle`, `< Mi pedido`). En la pantalla de revisión de pedido se incluye el enlace explícito `+ Seguir comprando`.
  - **Vulnerabilidad detectada:** En la pantalla `Revisar Pedido`, al presionar el texto *"Eliminar"*, el producto se borra de manera inmediata e irreversible sin solicitar confirmación ni permitir deshacer (*Undo*). Durante la sesión con `P2` y `P3`, ambos usuarios señalaron que en un teléfono con pantalla táctil esto puede provocar borrados accidentales al intentar presionar controles contiguos.
- **Severidad Asignada:** **Nivel 2 (Problema menor).**
- **Recomendación Técnica:** Al pulsar *"Eliminar"*, presentar un micro-diálogo de confirmación accesible o, preferentemente, mostrar un mensaje transitorio tipo *Toast / Snackbar* con la acción *"Deshacer"* durante 4 segundos.

---

### Heurística H4: Consistencia y estándares
> *«Los usuarios no deberían tener que preguntarse si diferentes palabras, situaciones o acciones significan lo mismo. Seguir las convenciones de la plataforma.»*

- **Diagnóstico General:** **Aceptable, con una desviación de convención e-commerce.**
- **Análisis por Vistas:**
  - **Consistencia Interna:** Óptima. Todos los botones de acción principal (*CTA*) comparten el estilo negro carbón (`#0f172a`), bordes redondeados y tipografía semibold de alto contraste.
  - **Consistencia Externa (Desviación observada):** En aplicaciones móviles comerciales de comercio electrónico y alimentación (UberEats, PedidosYa, Starbucks), el estándar de facto es colocar el ícono de acceso al carrito en la esquina superior derecha del encabezado. CaféU prescinde de dicho ícono y confía únicamente en la barra flotante inferior, lo cual provocó titubeos iniciales en `P1` (demora de 6 segundos buscando el carrito arriba).
- **Severidad Asignada:** **Nivel 2 (Problema menor).**
- **Recomendación Técnica:** Implementar un patrón de acceso dual: mantener la barra flotante inferior para flujo rápido y añadir un ícono de bolsa/carrito en la esquina superior derecha del *header* con un contador numérico dinámico de ítems.

---

### Heurística H5: Prevención de errores
> *«Mucho mejor que los buenos mensajes de error es un diseño cuidadoso que impida que ocurra un problema en primer lugar.»*

- **Diagnóstico General:** **Excelente cumplimiento.**
- **Análisis por Vistas:**
  - El selector de cantidad utiliza un componente *Stepper* con botones `[-] 1 [+]`, lo que elimina por completo la posibilidad de que el usuario introduzca valores negativos, letras, caracteres especiales o cantidades astronómicas por error de teclado.
  - El campo de notas especiales tiene un límite estricto de caracteres visible (`0/100`), evitando textos excesivamente largos que desborden los comprobantes de cocina.
  - El botón *"Confirmar pedido"* incluye el monto consolidado en su etiqueta (`Confirmar pedido · $4.25`), previniendo confirmaciones a ciegas.
- **Severidad Asignada:** **Nivel 1 (Problema cosmético).**

---

### Heurística H6: Reconocimiento antes que recuerdo
> *«Minimizar la carga de memoria del usuario haciendo visibles los elementos, las acciones y las opciones. El usuario no debería tener que recordar información de una parte a otra.»*

- **Diagnóstico General:** **Excelente cumplimiento.**
- **Análisis por Vistas:**
  - El usuario no necesita memorizar qué agregó: la pantalla `Mi pedido` desglosa con absoluta transparencia los nombres de los productos, sus cantidades unitarias, el subtotal, los impuestos incluidos y el total final.
  - En la vista de Detalle de producto, se visualiza la fotografía, descripción del sabor y categoría, asistiendo la toma de decisión sin recurrir a memoria previa.
- **Severidad Asignada:** **Nivel 0 (No representa un problema).**

---

### Heurística H7: Flexibilidad y eficiencia de uso
> *«Los aceleradores —invisibles para los usuarios novatos— pueden hacer que la interacción sea más rápida para los usuarios experimentados. Permitir a los usuarios personalizar acciones frecuentes.»*

- **Diagnóstico General:** **Muy buen desempeño.**
- **Análisis por Vistas:**
  - El sistema ofrece dos caminos para agregar productos: un camino directo para usuarios rápidos mediante el botón *"Añadir"* en la tarjeta del catálogo (utilizado eficazmente por `P2` y `P3` para el sánduche), y un camino profundo para personalización abriendo la vista de detalle.
  - Los chips de filtrado superior (*Todos, Bebidas calientes, Sánduches, Snacks*) actúan como eficientes aceleradores de navegación que evitan hacer scroll innecesario.
- **Severidad Asignada:** **Nivel 0 (No representa un problema).**

---

### Heurística H8: Diseño estético y minimalista
> *«Los diálogos no deben contener información que sea irrelevante o rara vez necesaria. Cada unidad extra de información compite con la información relevante y disminuye su visibilidad.»*

- **Diagnóstico General:** **Sobresaliente.**
- **Análisis por Vistas:**
  - La interfaz respeta la cuadrícula modular de 8 puntos (*8pt Grid System*), manteniendo márgenes limpios y generosos espacios en blanco que favorecen la respiración visual.
  - La jerarquía tipográfica es clara (H1 de bienvenida, H2 de categorías, H3 de nombres de producto y precios destacados en negrita).
  - La paleta cromática es sobria y funcional (carbón, blanco y toques verde esmeralda para el éxito), logrando un ratio de contraste accesible superior a 14:1 (cumpliendo con la norma WCAG 2.1 AAA).
- **Severidad Asignada:** **Nivel 0 (No representa un problema).**

---

### Heurística H9: Ayudar a los usuarios a reconocer, diagnosticar y recuperarse de errores
> *«Los mensajes de error deben expresarse en lenguaje claro (sin códigos crudos), indicar con precisión el problema y sugerir constructivamente una solución.»*

- **Diagnóstico General:** **Satisfactorio en flujos nominales.**
- **Análisis por Vistas:**
  - La pantalla de confirmación contiene mensajes tranquilizadores y explicativos: *"Muestra este número en caja"* y *"Recibirás un comprobante al realizar el pago"*, evitando la típica angustia del usuario de si su transacción se completó o si hubo un fallo de cobro.
  - **Oportunidad de mejora:** Si el usuario elimina todos los productos del carrito en la pantalla `Mi pedido`, no se visualiza claramente un estado vacío (*Empty State*) asistido que lo invite amablemente a volver al menú con un botón llamativo.
- **Severidad Asignada:** **Nivel 1 (Problema cosmético / menor).**
- **Recomendación Técnica:** Diseñar una vista de estado vacío para el carrito con ilustración amigable y el texto: *"Tu pedido está vacío. Explora nuestro menú para agregar algo rico"*.

---

### Heurística H10: Ayuda y documentación
> *«Aunque es mejor que el sistema se pueda usar sin documentación, puede ser necesario proporcionar ayuda y documentación. Dicha información debe ser fácil de buscar, centrada en la tarea del usuario y no ser demasiado extensa.»*

- **Diagnóstico General:** **Excelente micro-documentación contextual.**
- **Análisis por Vistas:**
  - La sección *"¿Cómo funciona?"* en la pantalla de inicio con los tres pasos secuenciales (*1 Elige -> 2 Confirma -> 3 Retira*) actúa como un micro-onboarding no invasivo que alinea de inmediato las expectativas del estudiante universitario sin necesidad de leer manuales.
  - En la pantalla de revisión de pedido, el cuadro con el icono informativo *"Pago en caja: Paga al momento de retirar tu pedido"* resuelve la duda más frecuente de los usuarios antes de confirmar la compra.
- **Severidad Asignada:** **Nivel 0 (No representa un problema).**

---

## 4. Matriz Consolidada de Hallazgos Heurísticos

| Nro. | Heurística de Nielsen | Pantalla / Ubicación | Descripción del Problema Observado | Evidencia en Pilotaje | Severidad (0-4) | Solución Técnica Recomendada |
| :---: | :--- | :--- | :--- | :--- | :---: | :--- |
| **01** | **H1:** Visibilidad del estado | Menú (Catálogo) | El incremento de ítems en el carrito solo se refleja en la barra inferior fija; no hay feedback animado al pulsar "Añadir". | `P1` no miró hacia abajo y dudó si el producto se había sumado al pedido. | **2 (Menor)** | Incorporar animación de rebote (*micro-bounce*) en la barra inferior o un badge de notificación en la cabecera. |
| **02** | **H3:** Control y libertad | Revisar Pedido (`Mi pedido`) | La opción de "Eliminar" suprime el ítem de forma instantánea sin solicitar confirmación ni permitir deshacer. | `P2` y `P3` señalaron el riesgo de toques accidentales en pantallas táctiles. | **2 (Menor)** | Añadir un diálogo modal de confirmación o un *Snackbar* con la opción transitoria de *"Deshacer"*. |
| **03** | **H4:** Consistencia y estándares | Menú / Cabecera | Ausencia de un ícono de carrito de compras en la esquina superior derecha del encabezado (estándar e-commerce). | `P1` buscó durante 6 segundos el carrito en la parte superior de la pantalla. | **2 (Menor)** | Implementar acceso dual: botón de carrito en el *header* superior y barra flotante contextual inferior. |
| **04** | **H5:** Prevención de errores | Detalle de Producto | El botón directo "Añadir" en el catálogo puede confundir al usuario que desea agregar notas especiales. | `P1` intentó añadir y luego tuvo que retroceder para abrir la personalización. | **1 (Cosmético)** | Agregar un pequeño indicador de texto *"Personalizar"* en los productos que admiten instrucciones especiales. |
| **05** | **H9:** Diagnóstico y errores | Revisar Pedido (`Mi pedido`) | No se cuenta con una pantalla de estado vacío (*Empty State*) si el usuario remueve todos los ítems. | Observación de diseño en escenarios de carrito en cero. | **1 (Cosmético)** | Mostrar mensaje e ilustración amigable con un botón directo *"Explorar menú"* cuando el carrito quede vacío. |

---

## 5. Conclusiones de la Evaluación Heurística de Wilson

1. **Robustez y Claridad General:**  
   El prototipo móvil **CaféU** presenta una excelente calidad de diseño y arquitectura de información. De las 10 heurísticas de Nielsen inspeccionadas, 6 obtuvieron una calificación de **Severidad 0** (cumplimiento pleno), demostrando un trabajo sólido previo en cuanto a estética minimalista, correspondencia con el mundo universitario y facilidad de aprendizaje.
2. **Triangulación con el Pilotaje Real:**  
   Los resultados de las pruebas con `P1`, `P2` y `P3` (con una tasa de éxito del 100% y un puntaje SUS promedio de **82.5 / 100**) corroboran que la interfaz es altamente usable. Las únicas tres fricciones menores detectadas (visibilidad de la barra inferior, eliminación sin confirmación y ausencia de ícono de carrito en cabecera) fueron clasificadas con **Severidad 2**, lo que significa que generan dudas temporales pero no impiden a ningún usuario culminar exitosamente su pedido.
3. **Recomendaciones para la Fase de Refinamiento Final:**  
   Se recomienda al equipo incorporar la acción dual de acceso al carrito (cabecera y barra inferior) y la confirmación de eliminación de productos, consolidando una solución móvil de estándar profesional lista para su pase a producción.
