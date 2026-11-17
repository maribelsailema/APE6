# 🔍 Evaluación Heurística de CaféU – Viviana Sarco

**Universidad:** Universidad Técnica de Ambato  
**Carrera:** Ingeniería de Software – Quinto semestre  
**Asignatura:** Interacción Humano-Computador  
**Actividad:** APE 6 – Fase 2  
**Responsable de la evaluación:** Sarco Sailema Viviana Maribel  
**Usuario GitHub:** [@maribelsailema](https://github.com/maribelsailema)  
**Issue:** [APE6-F2-01 #9](https://github.com/maribelsailema/APE6/issues/9)

**Estado:** Borrador de análisis basado en las pantallas
compartidas y los registros del pilotaje.

**Pendiente:** Inspección individual del prototipo
por parte de Viviana, confirmación de hallazgos
y revisión de las severidades propuestas.

---

## 1. 🎯 Objetivo

Examinar el diseño de interacción de CaféU mediante
las diez heurísticas de usabilidad de Jakob Nielsen.

El análisis busca identificar problemas en la
navegación, comprensión de controles, prevención
de errores, recuperación y comunicación del
estado del sistema.

El documento servirá de base para la inspección
individual de la responsable.

---

## 2. 🧪 Objeto y alcance de la revisión

**Sistema:** CaféU  
**Tipo:** Prototipo interactivo de pedidos de cafetería  
**Usuarios objetivo:** Estudiantes universitarios

### Pantallas consideradas

1. Inicio.
2. Menú.
3. Detalle de producto.
4. Mi pedido.
5. Estado del pedido.
6. Modal de cancelación.
7. Confirmación.

### Enlace al prototipo

[☕ Abrir CaféU en Figma](https://www.figma.com/proto/mmnzX5MbN4kv4IhYOqlQR8/cafeU_prototipo?node-id=3-1700&p=f&scaling=min-zoom&content-scaling=fixed&page-id=0%3A1&starting-point-node-id=3%3A1700)

### Fuentes del borrador

- Capturas de las pantallas compartidas del prototipo.
- Matriz de seis tareas de Fase 1.
- Registros de los participantes P1, P2 y P3.

Los registros del pilotaje se utilizan como evidencia
complementaria; no sustituyen la inspección heurística
individual.

---

## 3. 📏 Escala de severidad

Se adopta la escala definida en el plan de evaluación:

| Nivel | Interpretación |
|---|---|
| 0 | No se identifica un problema |
| 1 | Problema cosmético |
| 2 | Problema menor |
| 3 | Problema importante |
| 4 | Problema crítico |
| P/V | Pendiente de verificar; no existe evidencia suficiente para puntuar |

Los valores presentados a continuación son
**propuestas de valoración**, sujetas a la revisión
personal de Viviana.

---

## 4. 🧩 Análisis de las diez heurísticas

### H1. Visibilidad del estado del sistema

**Severidad preliminar:** 2 – Problema menor.

**Pantallas relacionadas:** Menú y Mi pedido.

**Aspectos favorables:**

- El carrito muestra cantidad de productos y total.
- La pantalla de confirmación comunica que el pedido
  fue recibido.
- Se presenta un código de pedido identificable.

**Posible problema:**

Los cambios del carrito se muestran en una barra
inferior que puede pasar inadvertida para algunos
usuarios.

**Evidencia complementaria:**

En la tarea T4, P1 buscó el carrito en la parte
superior durante aproximadamente seis segundos
antes de localizar la barra inferior.

**Recomendación:**

Reforzar la visibilidad del carrito mediante una
señal textual y un acceso reconocible desde la cabecera.

**Verificación personal requerida:**

Confirmar si cada incorporación y eliminación
de productos produce una actualización visible
y comprensible.

---

### H2. Correspondencia entre el sistema y el mundo real

**Severidad preliminar:** 0 – Sin problema identificado
en los elementos revisados.

**Pantallas relacionadas:** Menú, Detalle, Mi pedido
y Confirmación.

**Aspectos favorables:**

- Los productos utilizan nombres cotidianos.
- Los importes se presentan en dólares.
- El sistema utiliza expresiones comprensibles
  como "Mi pedido" y "Pago en caja".
- La confirmación indica cómo retirar el pedido.

**Evidencia complementaria:**

Los registros P1, P2 y P3 señalan que los
participantes identificaron los productos,
los precios y el proceso de retiro.

**Recomendación:**

Mantener el lenguaje cotidiano y evitar
abreviaturas innecesarias.

**Verificación personal requerida:**

Revisar todos los textos visibles para
identificar términos técnicos o ambiguos.

---

### H3. Control y libertad del usuario

**Severidad preliminar:** 2 – Problema menor.

**Pantalla relacionada:** Mi pedido.

**Aspectos favorables:**

- La interfaz permite modificar cantidades.
- Se puede eliminar un producto antes de confirmar.
- Existe navegación de retorno entre pantallas.
- Se contempla una ruta de cancelación del pedido.

**Posible problema:**

La eliminación de un producto se realiza de
manera inmediata y no se aprecia una opción
para deshacer esa acción.

**Evidencia complementaria:**

P2 y P3 propusieron incorporar una confirmación
o una opción para deshacer después de eliminar.

No se registraron eliminaciones accidentales.

**Recomendación:**

Añadir una acción "Deshacer" que permita recuperar
el producto eliminado y el total correspondiente.

**Verificación personal requerida:**

Comprobar personalmente si la eliminación
es reversible y si la cancelación del pedido
requiere confirmación.

---

### H4. Consistencia y estándares

**Severidad preliminar:** 2 – Problema menor.

**Pantallas relacionadas:** Inicio, Menú y Mi pedido.

**Aspectos favorables:**

- Las acciones principales utilizan un estilo
  visual semejante.
- La distribución de las pantallas mantiene
  una organización consistente.

**Posible problema:**

El carrito utiliza principalmente una barra
inferior, mientras que algunos usuarios
esperan encontrarlo en la cabecera.

**Evidencia complementaria:**

P1 buscó un icono de carrito en la zona superior.

**Recomendación:**

Conservar el acceso inferior y evaluar un
acceso adicional en la cabecera.

**Verificación personal requerida:**

Comprobar que los botones con funciones
equivalentes mantengan nombres y comportamientos
consistentes en todas las pantallas.

---

### H5. Prevención de errores

**Severidad preliminar:** 2 – Problema menor.

**Pantallas relacionadas:** Menú, Detalle y Mi pedido.

**Aspectos favorables:**

- El pedido presenta un desglose de productos.
- Se muestra el importe antes de confirmar.
- Se utilizan controles para modificar cantidades.

**Posibles problemas:**

- El botón de incorporación directa puede generar
  confusión cuando se desea personalizar un producto.
- La eliminación inmediata puede producir errores
  accidentales.

**Evidencia complementaria:**

P1 experimentó una duda inicial en T3.
P2 y P3 señalaron el riesgo de eliminación accidental.

**Recomendación:**

Diferenciar "Añadir" de "Personalizar" y ofrecer
recuperación después de eliminar productos.

**Verificación personal requerida:**

Comprobar restricciones de cantidad, actualización
del total y prevención de pedidos inválidos.

---

### H6. Reconocimiento antes que recuerdo

**Severidad preliminar:** 1 – Problema cosmético.

**Pantallas relacionadas:** Inicio, Menú y Detalle.

**Aspectos favorables:**

- Los productos muestran nombre y precio.
- Las categorías permiten reconocer opciones.
- El resumen del carrito muestra los productos
  seleccionados y el total.

**Posible problema:**

No siempre resulta evidente que la personalización
de un café se encuentra en su vista de detalle.

**Evidencia complementaria:**

P1 consideró utilizar el botón directo "Añadir"
antes de entrar a la vista de personalización.

**Recomendación:**

Incluir una etiqueta "Personalizar" en productos
que admitan instrucciones especiales.

**Verificación personal requerida:**

Comprobar si la interfaz obliga a recordar
información de una pantalla anterior.

---

### H7. Flexibilidad y eficiencia de uso

**Severidad preliminar:** 0 – Sin problema identificado
en los recorridos registrados.

**Pantallas relacionadas:** Menú y Mi pedido.

**Aspectos favorables:**

- El menú incluye filtros por categoría.
- Algunos productos pueden añadirse directamente.
- Los productos con opciones especiales cuentan
  con una pantalla de detalle.
- El carrito permite actualizar su contenido.

**Evidencia complementaria:**

P2 y P3 completaron las tareas utilizando
sus respectivas interfaces de escritorio y móvil.

**Recomendación:**

Conservar las rutas rápidas y las opciones
de personalización.

**Verificación personal requerida:**

Revisar la navegación con teclado y la
posibilidad de operar los controles sin ratón.
Estas capacidades no quedaron demostradas
por las seis tareas del pilotaje.

---

### H8. Diseño estético y minimalista

**Severidad preliminar:** 1 – Problema cosmético.

**Pantallas relacionadas:** Inicio y Menú.

**Aspectos favorables:**

- La interfaz utiliza tarjetas para agrupar productos.
- La información principal tiene una organización
  visual relativamente sencilla.
- Los importes aparecen asociados con los productos.

**Posible problema:**

En Inicio, el campo de búsqueda y los mensajes
informativos pueden competir visualmente con el
acceso principal al menú.

**Evidencia complementaria:**

P1 intentó interactuar primero con el buscador
antes de seleccionar "Ver Menú".

**Recomendación:**

Revisar la jerarquía visual de Inicio y
destacar mejor la acción principal.

**Verificación personal requerida:**

Inspeccionar alineación, legibilidad,
contraste y organización visual.

No se asigna una calificación de conformidad
WCAG sin realizar mediciones específicas.

---

### H9. Ayuda para reconocer, diagnosticar y recuperarse de errores

**Severidad preliminar:** P/V – Pendiente de verificar.

**Pantallas relacionadas:** Mi pedido, Estado del pedido
y Modal de cancelación.

**Aspectos favorables:**

- Existe una pantalla de estado del pedido.
- El diseño contempla una confirmación
  antes de cancelar.

**Aspectos que requieren comprobación:**

- Qué ocurre si el carrito queda vacío.
- Qué mensaje aparece ante un pedido inválido.
- Cómo se recupera el usuario de una eliminación
  equivocada.
- Qué sucede si falla la confirmación.

**Evidencia complementaria:**

Las seis tareas del pilotaje no incluyeron
una falla de conexión ni una prueba de
recuperación después de vaciar completamente
el carrito.

**Recomendación:**

Evaluar escenarios de error y ofrecer mensajes
que expliquen el problema y la acción de recuperación.

**Verificación personal requerida:**

Provocar o recorrer los estados de error
disponibles en el prototipo.

No corresponde asignar severidad 0 solamente
porque no se observaron errores críticos
durante el pilotaje.

---

### H10. Ayuda y documentación

**Severidad preliminar:** 0 – Sin problema identificado
en la información contextual revisada.

**Pantallas relacionadas:** Inicio, Mi pedido
y Confirmación.

**Aspectos favorables:**

- Inicio presenta una explicación breve del proceso.
- Mi pedido informa sobre el pago en caja.
- Confirmación muestra los datos necesarios
  para retirar el pedido.

**Evidencia complementaria:**

Los participantes identificaron el número de
pedido, el tiempo estimado y el lugar de pago
en la tarea T6.

**Recomendación:**

Mantener instrucciones breves y situadas junto
a las acciones a las que corresponden.

**Verificación personal requerida:**

Comprobar si existen situaciones donde se
necesite ayuda adicional, especialmente
en cancelación y recuperación de errores.

---

## 5. 📊 Matriz resumen preliminar

| Heurística | Pantalla | Valor preliminar | Observación principal |
|---|---|---:|---|
| H1. Visibilidad del estado | Menú | 2 | El carrito puede pasar inadvertido |
| H2. Mundo real | Varias | 0 | Lenguaje cotidiano |
| H3. Control y libertad | Mi pedido | 2 | Eliminación sin deshacer |
| H4. Consistencia | Menú | 2 | Ubicación poco esperada del carrito |
| H5. Prevención de errores | Menú / Mi pedido | 2 | Riesgo en personalización y eliminación |
| H6. Reconocimiento | Detalle | 1 | Personalización poco evidente |
| H7. Eficiencia | Menú | 0 | Filtros y rutas rápidas |
| H8. Minimalismo | Inicio | 1 | Competencia visual de controles |
| H9. Recuperación de errores | Mi pedido / Estado | P/V | Escenarios de error no comprobados |
| H10. Ayuda | Inicio / Confirmación | 0 | Instrucciones contextuales |

Los valores no constituyen todavía el dictamen final
de la evaluadora.

---

## 6. 🔗 Relación preliminar con el pilotaje

| Tarea | Evidencia del pilotaje | Heurísticas relacionadas |
|---|---|---|
| T1 | P1 intentó utilizar primero el buscador | H6, H8 |
| T3 | P1 dudó entre añadir y personalizar | H5, H6 |
| T4 | P1 buscó el carrito en la cabecera | H1, H4 |
| T4 | P3 sugirió reforzar la señal del carrito | H1 |
| T5 | P2 y P3 recomendaron una opción para deshacer | H3, H5 |
| T6 | Los tres participantes reconocieron la confirmación | H1, H2, H10 |

**Diferencia metodológica:**

Las observaciones de P1, P2 y P3 son resultados de
pruebas con usuarios.

Las severidades heurísticas son interpretaciones
analíticas que requieren la inspección individual
de Viviana.

---

## 7. 🛠️ Recomendaciones preliminares

1. Mejorar la localización del acceso al carrito.
2. Diferenciar la incorporación directa de la personalización.
3. Añadir una opción para deshacer eliminaciones.
4. Revisar la jerarquía del acceso principal al menú.
5. Comprobar los mensajes ante errores.
6. Evaluar navegación por teclado y estados de foco.
7. Probar el comportamiento del carrito vacío.

Estas recomendaciones son propuestas y no cambios
implementados en el prototipo.

---

## 8. ✅ Lista de revisión personal de Viviana

Antes de presentar este archivo como evaluación
heurística individual definitiva, realizar:

- [ ] Abrir el prototipo de Figma.
- [ ] Recorrer Inicio y Menú.
- [ ] Revisar Detalle de producto.
- [ ] Comprobar cambios en cantidades y total.
- [ ] Inspeccionar el proceso de eliminación.
- [ ] Revisar Estado del pedido.
- [ ] Inspeccionar el modal de cancelación.
- [ ] Verificar la confirmación del pedido.
- [ ] Revisar las diez heurísticas por cuenta propia.
- [ ] Confirmar o corregir cada severidad.
- [ ] Distinguir problemas observados de riesgos potenciales.
- [ ] Registrar la fecha de inspección individual.
- [ ] Actualizar este documento con el dictamen final.

**Fecha de inspección individual:** Pendiente  
**Resultado final:** Pendiente de validación personal

---

## 9. 🎓 Conclusión preliminar

La información disponible sugiere que CaféU dispone
de una estructura comprensible para consultar,
modificar y confirmar pedidos.

Los registros de las pruebas muestran que los
participantes lograron completar las tareas,
aunque se presentaron dudas relacionadas con
el acceso al menú, la personalización del café
y la localización del carrito.

También se identificó una oportunidad de mejora
en la reversibilidad de la eliminación de productos.

La inspección personal deberá determinar si existen
problemas adicionales en los estados de error,
la accesibilidad y la navegación.

**Estado final de este documento:
borrador fundamentado, pendiente de evaluación
heurística individual por Viviana.**