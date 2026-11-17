# Matriz de Diseño de Seis Tareas de Evaluación de Usabilidad


## 1. Contexto y Articulación con el Plan de Evaluación (`docs/`)

El presente documento forma parte integral del **Plan de Evaluación de Usabilidad de CaféU**, complementando directamente los instrumentos formalizados en la carpeta `docs/`:
- `docs/plan-evaluacion.md`: Define el marco general, pregunta de evaluación, objetivos y métricas.
- `docs/participantes-roles.md`: Establece la distribución del equipo (Viviana como Moderadora, Wilson como Observador, Alex en Métricas y Sebastián en Soporte) y los perfiles de los participantes (`P01`, `P02`, `P03`).
- `docs/consentimiento-informado.md`: Garantiza el tratamiento ético y la confidencialidad de la información.

### 1.1 Pregunta de Evaluación Oficial del Proyecto
> *«¿En qué medida los estudiantes universitarios pueden seleccionar productos, revisar, modificar y confirmar un pedido en CaféU de manera eficaz, eficiente y satisfactoria, sin recibir instrucciones directas sobre cómo utilizar la interfaz?»*  
*(Fuente: `docs/plan-evaluacion.md` y `README.md`).*

### 1.2 Arquitectura y Vistas de Interfaz del Prototipo CaféU
Las seis tareas fueron diseñadas y parametrizadas estrictamente sobre los flujos y elementos de interfaz de las cinco vistas del prototipo:

| Nro. | Pantalla / Vista | Elementos de Interfaz y Datos Visibles |
| :---: | :--- | :--- |
| **1** | **Inicio (Onboarding y Acceso Rápido)** | Cabecera con marca `CaféU` y perfil `JD`. Saludo contextual (*"Hola, Julia"*). Campo de búsqueda (*"Buscar café, snacks..."*). Banner de valor (*"Evita la fila: pide tu café aquí - Haz tu pedido y recógelo en la caja rápida"*). Botón de acción principal `Ver Menú ->`. Sección de 3 pasos (*1 Elige -> 2 Confirma -> 3 Retira*). |
| **2** | **Menú (Catálogo de Productos y Filtros)** | Encabezado navegable `< Menú` con buscador (*"Buscar en el menú"*). Filtros por chips (*Todos*, *Bebidas calientes*, *Sánduches*, *Snacks*). Contador de *"8 disponibles"*. Catálogo de productos: **Café americano ($1.50)**, **Sánduche ($2.75)**, **Capuchino ($2.00)**, **Galleta de avena ($1.25)** con botones individuales `Añadir`. Barra flotante persistente: *"2 items · $4.25 \| Ver mi pedido ->"*. |
| **3** | **Detalle de Producto (Personalización)** | Encabezado `< Detalle`. Título `Café americano` con precio `$1.50` y categoría `Bebida caliente`. Descripción sensorial (*"Espresso suave combinado con agua caliente..."*). Selector de unidades `[-] 1 [+]`. Campo de texto para *Instrucciones especiales* (*"Ej. Sin azúcar, leche aparte..."* con contador `0/100`). Botón de acción fija: `Añadir al pedido · $1.50`. |
| **4** | **Revisar Pedido (Carrito de Compras)** | Encabezado `< Mi pedido` con contador *"2 items en tu pedido"*. Lista con selector `[-] 1 [+]` y enlace de texto `Eliminar`: Café americano ($1.50) y Sánduche ($2.75). Enlace `+ Seguir comprando`. Resumen de compra: Subtotal $4.25, Total **$4.25**. Cuadro informativo: *"Pago en caja: Paga al momento de retirar tu pedido"*. Botón CTA: `Confirmar pedido · $4.25`. |
| **5** | **Confirmación (Ticket y Retiro)** | Retroalimentación de éxito con checkmark animado en verde. Título `¡Pedido recibido! - Ya estamos preparando todo para ti`. Tarjeta de comprobante: **NÚMERO DE PEDIDO: #CU-104** (*"Muestra este número en caja"*). Tarjeta informativa: *"Paga y retira en caja rápida · Tu pedido estará listo en aproximadamente 5-10 minutos"*. Resumen *"2 items · $4.25"*. Botón `Volver al inicio` y leyenda *"Recibirás un comprobante al realizar el pago"*. |

---

## 2. Matriz Sintética de las Seis Tareas de Usabilidad

| ID | Situación de Uso | Vista de Interfaz | Consigna Neutral (Leída por la Moderadora Viviana) | $T_{\text{obj}}$ | $T_{\max}$ | Respuesta Correcta | Criterio de Éxito Observable |
| :---: | :--- | :---: | :--- | :---: | :---: | :--- | :--- |
| **T1** | Consultar catálogo y precio individual de bebida | Inicio $\rightarrow$ Menú | *"Estás planificando tu desayuno antes de entrar a clases. Revisa la oferta de la cafetería, averigua cuál es el precio individual de un Café americano y dímelo en voz alta."* | 30 s | 60 s | "$1.50" (o "Un dólar con cincuenta centavos") | Accede al Menú desde Inicio, localiza la tarjeta de "Café americano" y verbaliza con exactitud "$1.50". |
| **T2** | Filtrar por categoría y seleccionar aperitivo ligero | Menú | *"No deseas un plato fuerte ni bebidas, solo un bocadillo rápido. Filtra las opciones para ver únicamente los snacks y dime qué producto aparece disponible y cuánto cuesta."* | 30 s | 60 s | "Galleta de avena" a "$1.25" | Utiliza el chip de filtro "Snacks" en el Menú y verbaliza "Galleta de avena" y su precio "$1.25". |
| **T3** | Configurar producto con instrucciones especiales | Menú $\rightarrow$ Detalle | *"Has elegido tomar un Café americano. Accede a sus opciones de preparación, añade la instrucción especial de 'Sin azúcar' e incorpóralo a tu pedido."* | 45 s | 90 s | Escribe "Sin azúcar" en el campo de texto y pulsa "Añadir al pedido · $1.50" | Ingresa al Detalle, completa el campo de instrucciones y confirma la acción con el botón CTA. |
| **T4** | Sumar alimento al pedido y comprobar desglose de cuenta | Menú $\rightarrow$ Revisar Pedido | *"Deseas acompañar tu bebida con un sánduche. Agrégalo a tu compra, accede a la pantalla de revisión de tu pedido y dime cuál es el valor total a cancelar."* | 45 s | 90 s | Agrega Sánduche ($2.75), abre "Mi pedido" (2 ítems) y dice "$4.25" | Añade el sánduche, abre el resumen de orden y constata verbalmente el total de "$4.25". |
| **T5** | Modificar pedido eliminando un ítem | Revisar Pedido | *"Te diste cuenta de que ya no vas a comer el sánduche porque trajiste refrigerio. Quítalo de tu lista de pedido para quedarte únicamente con el café y dime cuál es el nuevo total."* | 30 s | 60 s | Presiona "Eliminar" en el Sánduche y reporta el nuevo total de "$1.50" | Remueve el sánduche de la lista y verifica que el total se recalculó a "$1.50". |
| **T6** | Confirmar pedido y verificar retiro, pago y ticket | Revisar Pedido $\rightarrow$ Confirmación | *"Tu orden está lista para ser enviada. Confirma el pedido en la pantalla y averigua qué número de pedido te asignó el sistema, en cuánto tiempo estará listo y qué debes hacer para pagarlo y retirarlo."* | 45 s | 90 s | 1. Número: "#CU-104"<br>2. Tiempo: "5 a 10 minutos"<br>3. Pago/Retiro: "En caja rápida" | Presiona "Confirmar pedido", arriba a la pantalla de confirmación y verbaliza los tres datos solicitados. |

> **Armonización con el Cronograma de `docs/`:** La suma de tiempos máximos de las 6 tareas es de 7 minutos (420 segundos), acoplándose perfectamente al bloque de **12 minutos** asignado para la ejecución de tareas en `docs/plan-evaluacion.md` (Sección 17).

---

## 3. Fichas Técnicas Detalladas de las Tareas

### Tarea T1: Consulta de catálogo y precio individual de bebida
- **ID:** T1
- **Nombre:** Consulta de producto y precio en el catálogo
- **Vista de Interfaz:** Inicio hacia Menú de productos
- **Tipo de Tarea:** Consulta / Navegación inicial
- **Objetivo:** Evaluar la visibilidad del botón de acceso al menú (`Ver Menú ->`) y la claridad tipográfica del precio en la tarjeta de producto.
- **Situación Contextual:** Un estudiante abre la aplicación móvil antes de su primera clase para verificar si el café americano se ajusta a su presupuesto.
- **Consigna Neutral (Leída por Viviana):**  
  > *"Estás planificando tu desayuno antes de entrar a clases. Revisa la oferta de la cafetería, averigua cuál es el precio individual de un Café americano y dímelo en voz alta."*
- **Estado Inicial:** Pantalla de Inicio.
- **Tiempo Objetivo ($T_{\text{obj}}$):** 30 segundos | **Tiempo Máximo ($T_{\max}$):** 60 segundos
- **Respuesta Correcta:** *"$1.50"* (o *"Un dólar con cincuenta centavos"*).
- **Criterio de Éxito Observable:**
  - **Éxito (Sí):** Pulsa el botón "Ver Menú ->", ubica la tarjeta de "Café americano" y verbaliza "$1.50" en $\le 60\text{ s}$ de forma autónoma.
  - **Con ayuda:** Localiza el precio tras la pista única del moderador.
  - **Fallo (No):** Supera los 60 s, confunde el precio o abandona la búsqueda.
- **Errores Críticos:** Indicar el precio del Capuchino ($2.00) o de la Galleta ($1.25); no salir de la pantalla de inicio.
- **Errores No Críticos:** Intentar escribir en el buscador en lugar de pulsar el botón del menú; leer primero el banner promocional.
- **Heurística de Nielsen:** H1 (Visibilidad del estado del sistema) y H8 (Diseño estético y minimalista).

---

### Tarea T2: Filtrado por categoría y selección de aperitivo ligero
- **ID:** T2
- **Nombre:** Filtrado por categorías temáticas en el menú
- **Vista de Interfaz:** Menú de productos
- **Tipo de Tarea:** Búsqueda asistida por filtros / Reconocimiento
- **Objetivo:** Comprobar si los chips de filtrado horizontal (*Todos*, *Bebidas calientes*, *Sánduches*, *Snacks*) son intuitivos para aislar categorías específicas de alimentos.
- **Situación Contextual:** El estudiante solo tiene un receso de 10 minutos y busca un snack rápido para llevar al aula.
- **Consigna Neutral (Leída por Viviana):**  
  > *"No deseas un plato fuerte ni bebidas, solo un bocadillo rápido. Filtra las opciones para ver únicamente los snacks y dime qué producto aparece disponible y cuánto cuesta."*
- **Estado Inicial:** Menú con el filtro activo en "Todos".
- **Tiempo Objetivo ($T_{\text{obj}}$):** 30 segundos | **Tiempo Máximo ($T_{\max}$):** 60 segundos
- **Respuesta Correcta:** *"Galleta de avena a $1.25"*.
- **Criterio de Éxito Observable:**
  - **Éxito (Sí):** Presiona el chip "Snacks", reconoce la "Galleta de avena" y verbaliza su nombre y precio ($1.25) en $\le 60\text{ s}$.
  - **Con ayuda:** Activa el filtro tras recibir la pista única.
  - **Fallo (No):** No identifica los chips de categoría o supera el tiempo límite.
- **Errores Críticos:** Seleccionar una categoría errónea; manifestar que no hay snacks.
- **Errores No Críticos:** Intentar deslizar la lista verticalmente antes de aplicar el chip; pulsar el botón de añadir antes de leer el precio.
- **Heurística de Nielsen:** H4 (Consistencia y estándares) y H7 (Flexibilidad y eficiencia de uso).

---

### Tarea T3: Configuración y personalización con instrucciones especiales
- **ID:** T3
- **Nombre:** Personalización de pedido en detalle de producto
- **Vista de Interfaz:** Menú hacia Detalle de producto
- **Tipo de Tarea:** Configuración / Entrada de datos / Acción de compra
- **Objetivo:** Evaluar la facilidad para abrir la vista detallada de un producto y la comprensión del campo de instrucciones especiales de cocina.
- **Situación Contextual:** El usuario requiere comunicar a los baristas que su café debe ser preparado sin azúcar por razones de salud.
- **Consigna Neutral (Leída por Viviana):**  
  > *"Has elegido tomar un Café americano. Accede a sus opciones de preparación, añade la instrucción especial de 'Sin azúcar' e incorpóralo a tu pedido."*
- **Estado Inicial:** Menú de productos.
- **Tiempo Objetivo ($T_{\text{obj}}$):** 45 segundos | **Tiempo Máximo ($T_{\max}$):** 90 segundos
- **Respuesta Correcta:** Tocar el Café americano para abrir la vista de Detalle, escribir "Sin azúcar" en el cuadro de *Instrucciones especiales* y presionar *"Añadir al pedido · $1.50"*.
- **Criterio de Éxito Observable:**
  - **Éxito (Sí):** Completa la personalización y añade el café al pedido en $\le 90\text{ s}$ sin asistencia.
  - **Con ayuda:** Añade el producto con la instrucción tras la pista única.
  - **Fallo (No):** Añade el café rápido desde el menú sin abrir detalle, perdiendo la instrucción personalizada.
- **Errores Críticos:** Pulsar el botón directo `Añadir` en el menú general omitiendo las instrucciones; salir sin añadir el ítem.
- **Errores No Críticos:** Titubeo ante el contador de caracteres (0/100); tocar accidentalmente el selector de unidades `[-] 1 [+]`.
- **Heurística de Nielsen:** H2 (Correspondencia mundo real) y H6 (Reconocimiento antes que recuerdo).

---

### Tarea T4: Sumar alimento al pedido y comprobar desglose de cuenta
- **ID:** T4
- **Nombre:** Adición secundaria y verificación del total consolidado
- **Vista de Interfaz:** Menú hacia Revisar Pedido (Mi pedido)
- **Tipo de Tarea:** Transacción combinada / Supervisión de costos
- **Objetivo:** Evaluar la visibilidad y uso de la barra flotante inferior del carrito (*"2 items · $4.25 | Ver mi pedido"*) y la claridad del desglose monetario.
- **Situación Contextual:** El estudiante decide sumar un sánduche a su compra y necesita saber con certeza el total a pagar para preparar su dinero en efectivo.
- **Consigna Neutral (Leída por Viviana):**  
  > *"Deseas acompañar tu bebida con un sánduche. Agrégalo a tu compra, accede a la pantalla de revisión de tu pedido y dime cuál es el valor total a cancelar."*
- **Estado Inicial:** Carrito con 1 café americano previamente agregado.
- **Tiempo Objetivo ($T_{\text{obj}}$):** 45 segundos | **Tiempo Máximo ($T_{\max}$):** 90 segundos
- **Respuesta Correcta:** Añadir el producto *"Sánduche"* ($2.75), abrir la pantalla de revisión de pedido y verbalizar el total: *"$4.25"*.
- **Criterio de Éxito Observable:**
  - **Éxito (Sí):** Añade el sánduche, abre la pantalla "Mi pedido" y lee en voz alta "$4.25" en $\le 90\text{ s}$ de forma autónoma.
  - **Con ayuda:** Accede al desglose tras la pista única.
  - **Fallo (No):** No logra acceder al carrito o menciona un valor diferente al total consolidado.
- **Errores Críticos:** No encontrar el acceso al pedido; confundir el subtotal con el total.
- **Errores No Críticos:** Buscar un icono de carrito en la parte superior antes de notar la barra inferior flotante.
- **Heurística de Nielsen:** H1 (Visibilidad del estado del sistema) y H4 (Consistencia y estándares).

---

### Tarea T5: Modificación de orden / Eliminación de ítem en el carrito
- **ID:** T5
- **Nombre:** Control, rectificación y reversibilidad en el carrito
- **Vista de Interfaz:** Revisar Pedido (Mi pedido)
- **Tipo de Tarea:** Reversibilidad / Edición de pedido
- **Objetivo:** Comprobar si el usuario detecta la opción de eliminar productos y si el sistema recalcula el total de inmediato de manera comprensible.
- **Situación Contextual:** El estudiante recuerda que trajo un refrigerio de casa y decide que ya no gastará en el sánduche, conservando solo el café.
- **Consigna Neutral (Leída por Viviana):**  
  > *"Te diste cuenta de que ya no vas a comer el sánduche porque trajiste refrigerio. Quítalo de tu lista de pedido para quedarte únicamente con el café y dime cuál es el nuevo total."*
- **Estado Inicial:** Pantalla de Revisar Pedido con 2 ítems ($4.25).
- **Tiempo Objetivo ($T_{\text{obj}}$):** 30 segundos | **Tiempo Máximo ($T_{\max}$):** 60 segundos
- **Respuesta Correcta:** Presionar el enlace *"Eliminar"* en la fila del Sánduche ($2.75) y verbalizar el total recalculado: *"$1.50"*.
- **Criterio de Éxito Observable:**
  - **Éxito (Sí):** Elimina el sánduche y expresa el nuevo total de "$1.50" en $\le 60\text{ s}$ sin asistencia.
  - **Con ayuda:** Elimina el ítem tras recibir la pista única.
  - **Fallo (No):** Elimina el café por error, confirma la compra sin eliminar el sánduche o supera los 60 s.
- **Errores Críticos:** Eliminar el café dejando el sánduche; confirmar el pedido sin eliminar.
- **Errores No Críticos:** Intentar pulsar el botón `[-]` repetidamente en lugar de tocar directamente "Eliminar".
- **Heurística de Nielsen:** H3 (Control y libertad del usuario) y H5 (Prevención de errores).

---

### Tarea T6: Confirmación del pedido y verificación de entrega y pago
- **ID:** T6
- **Nombre:** Confirmación transaccional y lectura del comprobante de retiro
- **Vista de Interfaz:** Revisar Pedido hacia Confirmación
- **Tipo de Tarea:** Cierre transaccional / Comprensión de instrucciones post-compra
- **Objetivo:** Evaluar si la pantalla de confirmación comunica con claridad el número de orden, el tiempo de preparación y el método de pago en caja física.
- **Situación Contextual:** El estudiante confirma su pedido y necesita saber qué código mostrar en el mostrador, cuánto tardará y cómo debe pagar.
- **Consigna Neutral (Leída por Viviana):**  
  > *"Tu orden está lista para ser enviada. Confirma el pedido en la pantalla y averigua qué número de pedido te asignó el sistema, en cuánto tiempo estará listo y qué debes hacer para pagarlo y retirarlo."*
- **Estado Inicial:** Pantalla de Revisar Pedido.
- **Tiempo Objetivo ($T_{\text{obj}}$):** 45 segundos | **Tiempo Máximo ($T_{\max}$):** 90 segundos
- **Respuesta Correcta:**
  1. Número de pedido: *"#CU-104"*
  2. Tiempo estimado: *"5 a 10 minutos"*
  3. Instrucción de pago y retiro: *"Pagar y retirar en caja rápida"* mostrando el número en caja.
- **Criterio de Éxito Observable:**
  - **Éxito (Sí):** Pulsa el botón "Confirmar pedido", arriba a la pantalla de confirmación y verbaliza los tres datos solicitados en $\le 90\text{ s}$ sin auxilio.
  - **Con ayuda:** Verbaliza los datos tras la pista única de la moderadora.
  - **Fallo (No):** No identifica el número de orden o confunde la modalidad de pago.
- **Errores Críticos:** Asumir que ya se debitó el dinero en línea sin leer la instrucción física; confundir el número de orden con el valor monetario.
- **Errores No Críticos:** Pulsar apresuradamente el botón "Volver al inicio" sin leer primero los detalles de retiro.
- **Heurística de Nielsen:** H1 (Visibilidad del estado del sistema) y H9 (Reconocimiento y diagnóstico).

---

## 4. Métricas de Usabilidad según ISO 9241-11

| Dimensión | Métrica Específica | Responsable de Medición | Método de Cálculo |
| :--- | :--- | :--- | :--- |
| **Eficacia** | Tasa de Éxito ($TE$) | Alex (Métricas) | $\left( \frac{\text{Participantes con Éxito (Sí)}}{\text{Total de Participantes (3)}} \right) \times 100$ |
| **Eficiencia** | Tiempo en Tarea ($TT$) | Alex (Métricas) | Cronometraje individual en segundos ($s$) desde el fin de la lectura hasta la respuesta |
| **Eficiencia** | Tasa de Errores | Wilson (Observador) y Alex | Conteo y clasificación de Errores Críticos ($EC$) y Errores No Críticos ($ENC$) |
| **Satisfacción** | Cuestionario SUS | Alex y Wilson | 10 ítems (escala 1 a 5) normalizados a escala 0-100 con factor $\times 2.5$ |

---

## 5. Regla de Pista Única y Procedimiento de Restablecimiento

### 5.1 Regla de Pista Única Estandarizada
- **Condición de Disparo:** Si el participante se mantiene en silencio o bloqueo motor durante más de **15 segundos**, o solicita asistencia explícitamente.
- **Frase Oficial (Leída por Viviana):**  
  > *"Vuelve a leer la tarea y revisa las opciones que tienes en pantalla."*
- **Efecto de Registro:** Alex marcará **Pista = Sí** y el resultado se computará como **"Con ayuda"**.

### 5.2 Restablecimiento del Prototipo entre Participantes (`P01`, `P02`, `P03`)
Sebastián (Soporte técnico) aplicará el siguiente procedimiento de reinicio:
1. Volver el prototipo a la vista inicial (Inicio).
2. Limpiar el estado en memoria del carrito de compras (vaciar los ítems a cero).
3. Asegurar que los filtros por chips regresen al estado por defecto (*"Todos"*).
4. Comprobar que la resolución del dispositivo o emulador esté calibrada según el perfil del participante (Móvil para `P01` y `P03`; Escritorio para `P02`).
