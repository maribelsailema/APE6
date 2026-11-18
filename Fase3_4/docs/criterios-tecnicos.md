# Criterios técnicos de mejora – CaféU

**Proyecto:** CaféU  
**Actividad:** APE6-F3F4-04  
**Responsable:** Guachi Aucapiña Alex Fabricio  
**Propósito:** definir condiciones verificables para orientar las mejoras de usabilidad.

## 1. Objetivo

Establecer criterios técnicos que permitan convertir los hallazgos de usabilidad en tareas de mejora concretas. Cada criterio se relaciona con uno o más hallazgos H-XX y especifica qué debe comprobarse para considerar que la mejora está implementada.

Los criterios se plantean como condiciones de aceptación para futuras tareas de desarrollo o ajustes del prototipo. No significan que las mejoras ya estén implementadas.

## 2. Relación entre hallazgos y criterios

| Criterio | Hallazgo relacionado | Mejora propuesta | Prioridad orientativa |
|---|---|---|---|
| C-01 | H-01 | Incorporar acceso al pedido en la cabecera sin retirar la barra inferior | Alta |
| C-02 | H-02 | Hacer visible la actualización del carrito | Alta |
| C-03 | H-03 | Permitir recuperar un producto eliminado y ampliar el control | Alta |
| C-04 | H-04 | Diferenciar «Añadir» de «Personalizar» | Media |
| C-05 | H-05 | Reforzar «Ver Menú» frente al buscador en Inicio | Media |
| C-06 | H-06 | Definir el estado del carrito vacío | Verificación previa |
| C-07 | H-07 | Corregir el orden y significado de los estados del pedido | Verificar versión |
| C-08 | H-08 | Unificar el texto relacionado con el pago | Verificar versión |
| C-09 | H-09 | Definir mensajes y recuperación para situaciones de error | Verificación previa |
| C-10 | H-10 | Unificar detalles visuales y corregir textos | Baja |
| C-11 | H-11 | Comprobar el texto y las acciones del modal de cancelación | Verificación previa |
| C-12 | H-12 | Mostrar el tiempo estimado en la confirmación, si falta en la versión vigente | Condicional |

## 3. Criterios técnicos verificables

### C-01. Acceso visible al pedido

**Hallazgo relacionado:** H-01 – Acceso al pedido fuera de la ubicación esperada.

**Condición de aceptación:**
- La cabecera debe mostrar un acceso identificable al pedido.
- El acceso debe permanecer disponible durante la navegación por Inicio y Menú.
- Al seleccionarlo, debe abrir la pantalla «Mi Pedido».
- El contador debe coincidir con la cantidad actual de productos.
- La barra inferior existente debe conservar su funcionamiento.

**Comprobación:** agregar un producto, navegar entre Inicio y Menú y comprobar que el acceso superior abre el pedido y presenta la cantidad correcta.

### C-02. Retroalimentación al actualizar el carrito

**Hallazgo relacionado:** H-02 – Retroalimentación poco perceptible al añadir productos.

**Condición de aceptación:**
- Al agregar un producto, la cantidad y el total deben actualizarse.
- El cambio debe percibirse mediante una señal visual breve.
- La señal debe aparecer sin necesidad de recargar la pantalla.
- La señal no debe cubrir botones ni impedir continuar navegando.
- La actualización debe ocurrir en menos de un segundo desde la acción de añadir.

**Comprobación:** agregar dos productos consecutivamente y verificar que el contador, el total y la señal visual se actualicen en cada ocasión.

### C-03. Recuperación después de eliminar un producto

**Hallazgo relacionado:** H-03 – Eliminación inmediata sin recuperación y control pequeño.

**Condición de aceptación:**
- El control «Eliminar» debe disponer de un área interactiva de al menos 44 × 44 píxeles CSS.
- Después de eliminar un producto debe aparecer una notificación con la opción «Deshacer».
- La opción debe permanecer disponible durante un intervalo definido, por ejemplo, 5 segundos.
- Si el usuario selecciona «Deshacer» dentro del intervalo, el producto debe volver al pedido.
- La cantidad, el precio y las instrucciones especiales del producto recuperado deben conservarse.
- Si no se selecciona «Deshacer», el producto debe permanecer eliminado.

**Comprobación:** eliminar un producto y recuperarlo; repetir la prueba sin seleccionar «Deshacer» y verificar que el artículo no reaparezca.

### C-04. Diferenciación entre añadir y personalizar

**Hallazgo relacionado:** H-04 – «Añadir» directo no se diferencia de la personalización.

**Condición de aceptación:**
- Los productos que admitan instrucciones especiales deben mostrar una indicación visible de que pueden personalizarse.
- La acción para abrir las opciones debe distinguirse de la acción de añadir directamente.
- La pantalla de detalle debe permitir escribir y revisar las instrucciones.
- Las instrucciones deben conservarse al agregar el producto al pedido.

**Comprobación:** seleccionar un producto personalizable, identificar la opción sin ayuda, escribir «Sin azúcar» y verificar que la nota aparezca en el pedido.

### C-05. Jerarquía visual de Inicio

**Hallazgo relacionado:** H-05 – Buscador en competencia con «Ver Menú».

**Condición de aceptación:**
- «Ver Menú» debe identificarse como la acción principal de Inicio.
- El buscador no debe aparentar ser obligatorio para acceder al catálogo.
- Si el buscador está visible, debe permitir realizar una búsqueda funcional; si no está implementado, su presentación debe evitar generar expectativas de interacción.
- El acceso al menú debe funcionar desde la pantalla inicial.

**Comprobación:** presentar Inicio a una persona que no haya utilizado el prototipo y solicitarle que consulte el menú. Registrar si identifica el acceso principal sin indicaciones.

### C-06. Estado del carrito vacío

**Hallazgo relacionado:** H-06 – Estado del carrito vacío no definido.

**Condición de aceptación:**
- Al abrir «Mi Pedido» sin productos, debe mostrarse un mensaje que indique que el pedido está vacío.
- Debe existir una acción visible para regresar al menú o explorar productos.
- El botón de confirmar pedido debe estar deshabilitado o no disponible mientras no existan productos.
- El estado vacío no debe mostrar un total distinto de cero ni productos inexistentes.

**Comprobación:** iniciar con el carrito vacío, abrir «Mi Pedido» y verificar el mensaje, el acceso al menú y la imposibilidad de confirmar un pedido vacío.

**Condición previa:** comprobar primero si la versión vigente ya dispone de esta pantalla o variante.

### C-07. Secuencia de estados del pedido

**Hallazgo relacionado:** H-07 – Secuencia potencialmente confusa entre preparación y recepción.

**Condición de aceptación:**
- Después de confirmar, el sistema debe comunicar primero que el pedido fue recibido.
- El estado de preparación debe mostrarse después de la recepción.
- Los nombres de los estados deben describir situaciones comprensibles.
- El porcentaje de avance no debe mostrarse como un progreso real si no existe información que lo respalde.
- La navegación entre estados debe conservar el código del pedido.

**Comprobación:** recorrer el flujo de confirmación y verificar que el orden sea «Pedido recibido» y posteriormente «En preparación», sin mostrar estados contradictorios.

**Condición previa:** verificar que la secuencia identificada corresponda a la versión vigente del prototipo.

### C-08. Claridad de la información de pago

**Hallazgo relacionado:** H-08 – «Total pagado» antes de realizar el pago.

**Condición de aceptación:**
- Mientras el pago se realice presencialmente, la interfaz debe utilizar «Total a pagar» y no «Total pagado».
- El mensaje de pago en caja debe coincidir con el resumen del pedido.
- El mismo significado debe mantenerse en las pantallas de pedido, estado y comprobante.
- No debe indicarse que el usuario ya pagó si todavía debe cancelar en caja.

**Comprobación:** completar una compra y comparar los textos de las pantallas de resumen, estado y confirmación.

**Condición previa:** confirmar que el texto observado pertenece a la versión vigente.

### C-09. Mensajes y recuperación ante errores

**Hallazgo relacionado:** H-09 – Escenarios de error no cubiertos.

**Condición de aceptación:**
- Si falla la confirmación, debe mostrarse un mensaje que explique que el pedido no pudo confirmarse.
- El mensaje debe indicar una acción que permita reintentar o regresar al pedido.
- El contenido del carrito no debe perderse por un fallo de confirmación.
- Si se pierde la conexión, debe mostrarse un aviso comprensible y evitar presentar una confirmación que no haya ocurrido.
- Los mensajes deben evitar términos técnicos dirigidos al usuario.

**Comprobación:** simular los escenarios disponibles de fallo de conexión y confirmación; verificar el mensaje, la acción de recuperación y la conservación de los productos.

**Condición previa:** identificar cuáles de estos escenarios pueden probarse en el prototipo y cuáles requieren implementación.

### C-10. Consistencia de presentación y textos

**Hallazgo relacionado:** H-10 – Inconsistencias menores de presentación.

**Condición de aceptación:**
- La marca CaféU debe conservar la misma ubicación en las pantallas equivalentes.
- La categoría debe escribirse de forma consistente como «Sánduches».
- Los nombres de botones y categorías deben mantener la misma escritura en todo el recorrido.
- Los cambios visuales no deben alterar el funcionamiento de las tareas.

**Comprobación:** recorrer las pantallas del flujo y comparar la ubicación de la marca y la escritura de los textos.

### C-11. Verificación del modal de cancelación

**Hallazgo relacionado:** H-11 – Texto y conexiones del modal pendientes de verificación.

**Condición de aceptación:**
- El texto del modal debe poder leerse completo y explicar qué ocurre al cancelar.
- «Volver al pedido» debe cerrar el modal y conservar el pedido sin cambios.
- «Sí, cancelar» debe ejecutar la acción prevista y mostrar una confirmación comprensible.
- El usuario debe conocer las consecuencias antes de confirmar la cancelación.
- El modal debe poder cerrarse sin cancelar accidentalmente el pedido.

**Comprobación:** abrir el modal, probar «Volver al pedido» y comprobar que los productos se conservan; volver a abrirlo y probar «Sí, cancelar» en un entorno de prueba, verificando el resultado.

**Condición previa:** obtener una captura limpia y comprobar que los botones estén conectados. La existencia del modal en una pantalla no demuestra que la cancelación esté operativa de extremo a extremo.

### C-12. Tiempo estimado de preparación

**Hallazgo relacionado:** H-12 – Tiempo estimado ausente en una pantalla de confirmación.

**Condición de aceptación:**
- La pantalla de confirmación debe mostrar el tiempo estimado de preparación cuando ese dato esté disponible.
- El tiempo debe presentarse con un texto claro, por ejemplo, «Listo en aproximadamente 5–10 minutos».
- La información debe estar cerca del código del pedido o de las instrucciones de retiro.
- El tiempo mostrado debe ser coherente con el dato definido para la versión evaluada.

**Comprobación:** completar un pedido y verificar que el tiempo estimado aparezca en la pantalla final y coincida con la información establecida.

**Condición previa:** confirmar si la versión vigente ya presenta el tiempo estimado. Los registros de las sesiones de usuarios indican que sí lo mostraba en la versión utilizada durante las pruebas.

## 4. Criterios de priorización

| Prioridad | Criterios | Justificación |
|---|---|---|
| Alta | C-01, C-02, C-03 | Mejoran el acceso al pedido, la comprensión de cambios y la recuperación de acciones. |
| Media | C-04, C-05 | Reducen dudas durante la selección y el inicio de la compra. |
| Verificación previa | C-06, C-07, C-08, C-09, C-11, C-12 | Requieren comprobar la versión o el comportamiento antes de definir una corrección definitiva. |
| Baja | C-10 | Ajustes de presentación que no impiden completar las tareas. |

La prioridad es orientativa y debe revisarse con el equipo antes de crear o cerrar las tareas de implementación.

## 5. Trazabilidad y relación con las tareas

| Hallazgo | Tarea o pantalla relacionada | Criterio |
|---|---|---|
| H-01 | T4 – acceso a Mi Pedido | C-01 |
| H-02 | T4 – actualización del carrito | C-02 |
| H-03 | T5 – eliminación de producto | C-03 |
| H-04 | T3 – personalización | C-04 |
| H-05 | T1 – acceso inicial al menú | C-05 |
| H-06 | Mi Pedido – estado sin productos | C-06 |
| H-07 | T6 – estados posteriores a confirmar | C-07 |
| H-08 | T6 – resumen y pago | C-08 |
| H-09 | Flujo general – situaciones de error | C-09 |
| H-10 | Inicio, Menú y pantallas de pedido | C-10 |
| H-11 | Modal de cancelación | C-11 |
| H-12 | Comprobante de confirmación | C-12 |

## 6. Recomendaciones para convertir los criterios en tareas de mejora

Cada tarea de mejora debe incluir:

1. Identificador del hallazgo H-XX.
2. Identificador del criterio C-XX.
3. Descripción del problema y pantalla donde ocurre.
4. Evidencia que justifica la modificación.
5. Prioridad acordada por el equipo.
6. Condiciones de aceptación que puedan comprobarse.
7. Evidencia de la prueba realizada después del cambio.

No se debe marcar una mejora como completada únicamente porque se haya modificado el diseño. Es necesario comprobar que cumple las condiciones de aceptación.

## 7. Consideraciones para la validación

- Los criterios C-01 a C-05 responden a problemas respaldados por inspección y observaciones de usuarios.
- C-06 y C-09 requieren comprobar estados que no se ejecutaron durante las sesiones.
- C-07, C-08 y C-12 dependen de confirmar qué versión de las pantallas se utilizará como referencia.
- C-11 requiere verificar las conexiones y el contenido completo del modal.
- C-10 puede comprobarse mediante una revisión visual de todas las pantallas.

## 8. Conclusión

Los criterios definidos convierten los principales hallazgos de usabilidad de CaféU en condiciones concretas que pueden revisarse antes de considerar terminada una mejora. Se priorizan los problemas relacionados con el acceso al pedido, la retroalimentación, la eliminación y la personalización, sin dejar de registrar los aspectos que necesitan una comprobación adicional.

La aplicación de estos criterios permitirá que las próximas modificaciones respondan a problemas identificados y que su cumplimiento pueda demostrarse mediante pruebas y evidencias.

---
