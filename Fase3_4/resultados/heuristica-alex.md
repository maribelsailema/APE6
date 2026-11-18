# Evaluación heurística individual – CaféU

**Evaluador:** Guachi Aucapiña Alex Fabricio  
**Proyecto:** CaféU – Sistema de pedidos para cafetería universitaria  
**Actividad:** APE6-F3F4-04  
**Rol:** Cronometrista y responsable de métricas  
**Marco de referencia:** Diez heurísticas de usabilidad de Jakob Nielsen  
**Versión evaluada:** Prototipo CaféU utilizado en las sesiones de Fase 3  
**Estado del documento:** Evaluación individual documentada; requiere confirmación visual final del evaluador sobre la versión vigente del prototipo.

## 1. Objetivo y alcance

El propósito de esta evaluación es identificar problemas de usabilidad que puedan dificultar la consulta del menú, la personalización de productos, la revisión del pedido y la confirmación de una compra en CaféU.

La revisión considera las diez heurísticas de Nielsen y utiliza como evidencia las observaciones registradas durante las tareas T1–T7, los comentarios de los participantes y los hallazgos consolidados por el equipo. Se diferencia entre problemas observados durante las pruebas, riesgos señalados por los participantes y aspectos que todavía requieren comprobación en el prototipo.

**Alcance y limitación:** este documento organiza la evaluación individual para la entrega. Los elementos identificados como pendientes de verificación no se presentan como defectos confirmados. Antes de declarar concluida la inspección personal, se debe recorrer la versión vigente de Figma y comprobar las pantallas y conexiones señaladas en este documento.

## 2. Escala de severidad

| Valor | Nivel | Descripción |
|---:|---|---|
| 0 | Sin problema observado | No se identificó una dificultad con la evidencia disponible. No equivale a una certificación completa. |
| 1 | Cosmético | Detalle visual menor que no afecta de forma importante las tareas. |
| 2 | Menor | Puede generar dudas, pasos adicionales o pequeñas demoras, pero permite continuar. |
| 3 | Mayor | Produce confusión importante, errores repetidos o retrasos considerables. |
| 4 | Crítico | Impide una tarea importante o puede ocasionar consecuencias graves para el usuario. |
| P/V | Pendiente de verificación | No existe evidencia suficiente para asignar una severidad definitiva. |

La severidad se justifica considerando frecuencia, impacto y persistencia. No se asigna una severidad alta únicamente porque una situación sea posible: debe existir evidencia que respalde su efecto.

## 3. Revisión de las diez heurísticas

### H1. Visibilidad del estado del sistema

**Resultado:** oportunidad de mejora.  
**Severidad propuesta:** 2 – Menor.

La barra inferior permite consultar la cantidad de productos y el total del pedido. Sin embargo, después de agregar un producto, la actualización podría destacarse mejor para que el usuario perciba inmediatamente el cambio. En la evaluación se señaló que la barra no presenta un realce visual suficientemente evidente, como una animación breve o un distintivo temporal.

**Evidencia:** observación de P3 durante T4 y hallazgo consolidado H-02. La observación se refiere a la percepción del cambio, no a que el producto no se haya agregado.

**Recomendación:** destacar brevemente la barra inferior y actualizar de forma visible el contador cuando se agrega o modifica un producto. La retroalimentación debe ser rápida y no distraer.

### H2. Correspondencia entre el sistema y el mundo real

**Resultado:** oportunidad de mejora localizada.  
**Severidad propuesta:** 2 – Menor.

La aplicación utiliza términos cercanos a la actividad cotidiana de una cafetería, como «Menú», «Añadir», «Mi pedido» y «Paga al retirar». No obstante, la diferencia entre añadir un producto directamente y abrir su detalle para personalizarlo no queda suficientemente clara desde la tarjeta del catálogo.

**Evidencia:** P1, durante T3, intentó inicialmente utilizar «Añadir» y luego accedió al detalle para escribir «Sin azúcar». Este comportamiento está relacionado con H-04.

**Recomendación:** utilizar una etiqueta visible como «Personalizar» o «Ver opciones» en los productos que admiten instrucciones especiales.

### H3. Control y libertad del usuario

**Resultado:** riesgo de recuperación insuficiente después de eliminar un producto.  
**Severidad propuesta:** 2 – Menor.

En el carrito, la acción «Eliminar» retira el producto inmediatamente. No se identifica una opción visible para recuperar el artículo eliminado sin volver al catálogo. Esta situación puede resultar incómoda si el usuario toca el control por equivocación o cambia de opinión.

**Evidencia:** comentarios de cierre de P2 y P3; observación de P1 sobre el tamaño reducido del texto «Eliminar». No se registraron eliminaciones accidentales durante T5.

**Recomendación:** incorporar una notificación temporal con la opción «Deshacer» y permitir que el usuario recupere el producto sin repetir todo el proceso.

### H4. Consistencia y estándares

**Resultado:** oportunidad de mejora en la ubicación de los accesos.  
**Severidad propuesta:** 2 – Menor.

El acceso al pedido se encuentra principalmente en la barra inferior. Un usuario acostumbrado a aplicaciones de compra puede buscar también el carrito en la parte superior de la pantalla. La ausencia de ese acceso adicional puede ocasionar una búsqueda breve.

**Evidencia:** P1, durante T4, buscó inicialmente el carrito en la cabecera y luego localizó la barra inferior. Hallazgo consolidado H-01.

**Recomendación:** mantener la barra inferior y evaluar un acceso adicional al carrito en la cabecera, con un contador que refleje la cantidad de productos.

### H5. Prevención de errores

**Resultado:** oportunidad de mejora preventiva.  
**Severidad propuesta:** 2 – Menor.

La eliminación inmediata y el tamaño reducido del control pueden favorecer toques involuntarios, especialmente en pantallas táctiles. Aunque no se produjo una eliminación accidental durante las pruebas, los participantes identificaron el riesgo.

También se debe hacer más clara la diferencia entre añadir un producto directamente y acceder a sus opciones de personalización.

**Evidencia:** comentarios de P2 y P3 sobre «Eliminar»; P1 durante T3; hallazgos H-03 y H-04.

**Recomendación:** ampliar el área interactiva de eliminación, incorporar «Deshacer» y diferenciar las acciones «Añadir» y «Personalizar».

### H6. Reconocimiento antes que recuerdo

**Resultado:** oportunidad de mejora en la identificación de acciones.  
**Severidad propuesta:** 2 – Menor.

El usuario debería reconocer desde la tarjeta del producto si puede añadirlo directamente o si dispone de opciones de personalización. Asimismo, el acceso al pedido debería ser fácil de localizar durante la navegación.

**Evidencia:** P1 necesitó cambiar de ruta durante T3 y buscó inicialmente el acceso al carrito en T4. Hallazgos H-01 y H-04.

**Recomendación:** mostrar las opciones disponibles directamente en las tarjetas y mantener accesos al pedido fáciles de identificar.

### H7. Flexibilidad y eficiencia de uso

**Resultado:** sin problema importante confirmado en las tareas evaluadas.  
**Severidad propuesta:** 0 – Sin problema observado.

Los participantes pudieron utilizar diferentes rutas para añadir productos. El botón «Añadir» permite incorporar productos sin pasos adicionales, mientras que el detalle permite introducir instrucciones especiales. Esta variedad puede facilitar el uso, siempre que ambas opciones estén claramente identificadas.

**Evidencia:** registros de T3 y T4 de P1, P2 y P3.

**Recomendación:** conservar las dos posibilidades de interacción, pero explicar visualmente cuándo se añade directamente y cuándo se accede a la personalización.

### H8. Diseño estético y minimalista

**Resultado:** oportunidad de mejora en la jerarquía visual de Inicio.  
**Severidad propuesta:** 2 – Menor.

En la pantalla inicial, el campo de búsqueda puede competir con el botón «Ver Menú». Un usuario puede interpretar que debe escribir en el campo antes de consultar los productos, aunque el botón sea el acceso principal al catálogo.

**Evidencia:** P1, durante T1, intentó utilizar primero el campo de búsqueda y después identificó el botón «Ver Menú». Hallazgo H-05.

**Recomendación:** destacar «Ver Menú» como acción principal y reducir la prominencia del buscador si no es necesario para iniciar la compra.

### H9. Ayudar a reconocer, diagnosticar y recuperarse de errores

**Resultado:** cobertura insuficiente de escenarios de error.  
**Severidad propuesta:** P/V – Pendiente de verificación.

Las tareas realizadas no incluyeron pruebas de pérdida de conexión, fallos al confirmar un pedido o intentos de confirmar con el carrito vacío. Por tanto, no se puede asegurar que la aplicación ofrezca mensajes claros y alternativas para recuperarse de esas situaciones.

La tarea T7 permitió identificar una limitación en la cancelación del pedido, pero debe diferenciarse de los escenarios generales de error.

**Evidencia:** ausencia de escenarios de error en T1–T7 y hallazgo H-09.

**Recomendación:** comprobar los estados de error disponibles y definir mensajes sencillos que expliquen qué ocurrió y qué puede hacer el usuario para continuar.

### H10. Ayuda y documentación

**Resultado:** sin necesidad de ayuda observada durante las tareas.  
**Severidad propuesta:** 0 – Sin problema observado en el flujo evaluado.

Los participantes completaron las tareas principales sin solicitar ayuda. Esto muestra que el flujo probado pudo utilizarse sin asistencia externa. Sin embargo, no representa una revisión completa de posibles instrucciones o ayudas para situaciones no incluidas en las pruebas.

**Evidencia:** cero solicitudes de ayuda registradas para P1, P2 y P3.

**Recomendación:** conservar la claridad de las instrucciones actuales y revisar si se necesita información breve para situaciones especiales, como cancelar un pedido o resolver un problema de confirmación.

## 4. Hallazgos relacionados con la evaluación

| ID consolidado | Problema | Severidad propuesta | Evidencia principal |
|---|---|---:|---|
| H-01 | Acceso al pedido poco visible en la cabecera | 2 | P1, T4 |
| H-02 | Retroalimentación poco perceptible al añadir productos | 2 | P3, T4 |
| H-03 | Eliminación inmediata sin opción de deshacer | 2 | Comentarios P2 y P3; observación P1 |
| H-04 | Diferencia poco clara entre añadir y personalizar | 2 | P1, T3 |
| H-05 | Buscador compite con «Ver Menú» | 2 | P1, T1 |
| H-06 | Estado del carrito vacío no definido | 1 / P/V | Inspección pendiente |
| H-07 | Secuencia de estados del pedido por comprobar | 2 / P/V | Evidencia de una versión del prototipo |
| H-08 | Uso de «Total pagado» antes del pago | 2 / P/V | Evidencia de una versión del prototipo |
| H-09 | Escenarios de error no cubiertos | P/V | No se probaron |
| H-10 | Inconsistencias menores de presentación | 1 | Inspección visual documentada |
| H-11 | Texto y conexiones del modal de cancelación por verificar | P/V | Evidencia visual incompleta |
| H-12 | Tiempo estimado ausente en una pantalla de confirmación | 2 / P/V | Depende de la versión vigente |

Los identificadores H-01 a H-12 corresponden a la matriz consolidada del equipo. Las severidades marcadas como P/V o condicionadas no deben convertirse en defectos confirmados sin una comprobación adicional.

## 5. Observación especial sobre la cancelación (T7)

Los tres participantes intentaron localizar una opción para cancelar el pedido después de confirmar la compra. Los registros indican que no encontraron una acción funcional de cancelación en el recorrido utilizado.

- P1 buscó la opción y terminó identificando que debía acudir a caja.
- P2 señaló que no existía un botón para cancelar desde el comprobante.
- P3 identificó la misma limitación y sugirió una opción de cancelación durante un tiempo breve.

El protocolo consideró como éxito conceptual que el usuario comprendiera el estado del pedido. Sin embargo, la cancelación efectiva no se pudo realizar. Por ello, la limitación debe mantenerse como una oportunidad de mejora importante y no como una cancelación exitosa.

La matriz consolidada también contiene un hallazgo sobre un modal de cancelación cuya legibilidad y conexiones requieren verificación. Es necesario comprobar que se trate de la misma versión del prototipo antes de concluir que existe o no un flujo funcional.

## 6. Conclusión individual

CaféU permite realizar las principales tareas de consulta, selección, personalización, revisión y confirmación del pedido sin que los participantes necesiten ayuda. Las dificultades identificadas se concentran en la localización del carrito, la retroalimentación al agregar productos, la identificación de las opciones de personalización y la recuperación después de eliminar un artículo.

La limitación de cancelación posterior a la confirmación merece atención porque los tres participantes intentaron encontrar esa opción y no pudieron ejecutar la acción en el recorrido probado. Además, se requiere comprobar los estados de error, el carrito vacío y las diferencias entre las pantallas de estado y confirmación.

Las recomendaciones de esta evaluación son propuestas de mejora. Su efectividad deberá comprobarse mediante una nueva revisión del prototipo y, posteriormente, con pruebas de usabilidad.

---
