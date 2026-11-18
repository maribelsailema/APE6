# APE 6 – Fase 3: Registro de soporte técnico

## 1. Información general

| Campo | Información |
|---|---|
| Proyecto | CaféU |
| Responsable | Santana Durán Sebastián Israel |
| Actividad | APE6-F3F4-03 |
| Fecha de comprobación | Pendiente de recorrido interactivo documentado |
| Evidencia estática | [Flujo con conexiones](../evidencias/flujo-figma-con-conexiones.png) |
| Prototipo | [Abrir CaféU en Figma](https://www.figma.com/proto/mmnzX5MbN4kv4IhYOqlQR8/cafeU_prototipo?node-id=3-1700&p=f&scaling=min-zoom&content-scaling=fixed&page-id=0%3A1&starting-point-node-id=3%3A1700) |

## 2. Comprobaciones realizadas

| Comprobación | Resultado verificable | Estado |
|---|---|---|
| Disponibilidad del prototipo publicado | Existe enlace público registrado en el repositorio y en esta documentación. | Pendiente confirmar carga desde otro equipo/sesión |
| Conexiones entre pantallas | La captura E-IMG02 muestra conexiones principales hacia Inicio, Menú, Detalle, Mi Pedido, Estado y Confirmación. | Verificado visualmente |
| Navegación T1–T7 | T1–T6 aparecen representadas por el flujo capturado; T7 no se observa en el recorrido principal. | T7 pendiente de verificación interactiva |
| Reinicio entre sesiones | El procedimiento técnico se define en el protocolo de Fase 3. | Pendiente ejecutar y registrar en las sesiones |
| Limitaciones técnicas | Una captura no demuestra comportamiento dinámico ni estados vacíos de error. | Documentado |

## 3. Recorrido verificable de T1–T7

| Tarea | Recorrido observado | Evidencia / limitación |
|---|---|---|
| T1 Consultar precio | Inicio → CTA «Ver Menú» → Menú → Café americano con $1.50. | La captura muestra el nodo de origen y destino del CTA; el buscador no tiene conexión visible. |
| T2 Filtrar categoría | Menú → chips «Todos», «Bebidas calientes», «Sanduches», «Snacks». | Faltan interacciones observables en la captura para comprobar el filtrado dinámico. |
| T3 Personalizar | Menú → tarjeta/detalle → instrucciones especiales → «Añadir al pedido». | La tarjeta de café tiene conexión a Detalle; no se observan conexiones desde los botones directos «Añadir». |
| T4 Agregar y revisar | Menú → barra flotante → Mi Pedido → total. | El conteo dinámico y el realce al añadir no son verificables en una imagen. |
| T5 Eliminar | Mi Pedido → enlace «Eliminar» → recálculo esperado. | No se observan conexiones desde «Eliminar» ni desde los steppers. |
| T6 Confirmar | Mi Pedido → confirmar → Estado → Confirmación. | La transición «Tras pausa» hacia Confirmación aparece en la captura. |
| T7 Cancelar | Estado/Modal de cancelación aparece en el flujo; la evidencia no permite probar ambos destinos ni el texto completo. | Pendiente de captura limpia y recorrido interactivo. |

## 4. Limitaciones técnicas

- **L-01 Diferencia de versión:** la captura F3 presenta textos y alcance distintos de los registros P1–P3; no se afirma que ambos artefactos sean la misma versión sin verificarlos.
- **L-02 Retroalimentación dinámica:** animaciones, rebotes y badges no pueden demostrarse con una captura estática.
- **L-03 Barra de progreso:** «50 %» puede representar un estado fijo del artefacto y no el progreso real del sistema.
- **L-04 Conexiones incompletas:** el buscador, los botones «Añadir», «Eliminar» y los steppers no muestran conexiones visibles en E-IMG02.
- **L-05 Retroceso:** el destino de «‹» desde Mi Pedido aparece como P03, pero debe verificarse interactivamente.
- **L-06 Modal:** la anotación «Tras pausa» oculta parte del texto del modal de cancelación.

## 5. Diferenciación entre error del prototipo y problema de interacción

- El prototipo puede tener conexiones, variantes o textos ausentes; eso es un **problema del artefacto** hasta confirmarlo en el recorrido.
- La ubicación de un control, su jerarquía y la exigencia de una ruta adicional pueden ser **problemas de interacción** respaldados por observación o inspección.
- Ninguna relación o comportamiento dinámico se considera demostrado solo por una flecha o una captura estática.
- Los hallazgos dependientes de estas condiciones deben mantenerse como P/V o condicionales hasta completar la verificación.

## 6. Procedimiento de reinicio

Antes de cada sesión:

1. Recargar el enlace de Figma.
2. Confirmar que el pedido comienza vacío.
3. Volver a Inicio o al punto inicial definido para la sesión.
4. Comprobar que no haya cantidades, notas ni productos preseleccionados.
5. Registrar el dispositivo, navegador y versión visible.
6. Registrar fecha, hora y resultado de esta comprobación.

La ejecución y el registro de este procedimiento deben completarse antes de citar el soporte técnico como prueba funcional.
