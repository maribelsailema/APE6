# 📋 Protocolo de Evaluación de Usabilidad – Fase 3 (CaféU)

**Proyecto:** CaféU – Sistema de pedidos para cafetería universitaria  
**Institución:** Universidad Técnica de Ambato – FISEI – Ingeniería de Software  
**Asignatura:** Interacción Humano-Computador (IHC)  
**Responsable:** Sarco Sailema Viviana Maribel (Moderadora)  
**Fecha de aplicación:** [Insertar fecha de las sesiones de Fase 3]  
**Versión del protocolo:** V2 (Ajustado post-pilotaje)

---

## 1. 🎯 Objetivo
Evaluar la usabilidad del prototipo CaféU tras los ajustes realizados, midiendo la eficacia, eficiencia y satisfacción del usuario al interactuar con las tareas principales del flujo de pedido, incorporando una tarea de refuerzo y garantizando la consistencia del entorno de prueba.

## 2. 🔄 Procedimiento de Reinicio y Estado Inicial
Para garantizar la validez de los tiempos y la ausencia de sesgos entre participantes, se establece el siguiente protocolo de reinicio obligatorio antes de cada sesión:
1. El moderador recargará el prototipo de Figma presionando **F5** (o `Cmd + R` en macOS).
2. Se verificará visualmente que:
   - El contador del carrito de compras indique **0 artículos**.
   - No existan notas de personalización ("Sin azúcar", etc.) pre-cargadas en ningún producto.
   - La vista inicial sea la pantalla de "Inicio" o "Menú Principal".
3. Solo tras esta verificación se iniciará el cronómetro y la grabación de la sesión.

## 3. 📋 Matriz de Tareas (T1 – T7)
*Nota: Los tiempos máximos han sido corregidos para sumar un total de 450 segundos (7 min 30 s), resolviendo la inconsistencia aritmética de la Fase 1.*

| ID | Tarea | Instrucción Neutral al Usuario | Respuesta / Estado Esperado | Tiempo Objetivo | Tiempo Máximo | Criterio de Éxito |
|:--:|:---|:---|:---|:--:|:--:|:---|
| **T1** | Consultar precio | "Busca el precio de un café americano." | Visualiza el precio: USD 1,50. | 30 s | 60 s | Precio correcto visible sin ayuda. |
| **T2** | Filtrar categoría | "Muestra únicamente los productos de la categoría Snacks." | Se filtra y muestra "Galleta de avena, USD 1,25". | 30 s | 60 s | Filtro aplicado correctamente. |
| **T3** | Personalizar | "Agrega un café americano e indica que lo quieres 'Sin azúcar'." | El producto en el carrito muestra la nota "Sin azúcar". | 45 s | 90 s | Nota de personalización registrada. |
| **T4** | Agregar y revisar | "Agrega un sánduche y revisa el total de tu pedido." | El total mostrado es exactamente USD 4,25. | 45 s | 90 s | Total correcto en el resumen. |
| **T5** | Eliminar producto | "Elimina el sánduche de tu pedido." | El total vuelve a ser USD 1,50. | 30 s | 60 s | Ítem removido, total actualizado. |
| **T6** | Confirmar pedido | "Finaliza y confirma tu compra." | Muestra comprobante con código, tiempo de espera y modalidad de pago. | 45 s | 90 s | Comprobante generado exitosamente. |
| **T7** | Cancelar pedido *(Refuerzo)* | "Ya realizaste un pedido, pero cambiaste de opinión. Intenta cancelarlo y comprueba qué información te muestra la aplicación." | Visualización de mensaje o flujo de cancelación. | 30 s | 60 s | El usuario comprende el estado de la cancelación. |

> **⚠️ Limitación documentada de la Tarea T7:** 
> Tras la verificación en el prototipo de Figma, se detectó que el recorrido de "Cancelación de un pedido ya confirmado" no está cableado (no tiene interacciones configuradas más allá de la pantalla de comprobante). Por lo tanto, durante la sesión, si el usuario no encuentra la opción, el moderador registrará este hecho como un **hallazgo de usabilidad (falta de affordance o flujo incompleto)** en lugar de un error del usuario, y se procederá a evaluar la claridad de los mensajes en la pantalla de comprobante actual.

## 4. 📝 Instrumentos de Recolección de Datos


- **Consentimiento Informado:** Versión CaféU (garantiza anonimato, uso académico y derecho a retirarse).
- **Hoja de Observación V2:** Adaptada exclusivamente a las columnas de las tareas T1 a T7, diferenciando claramente entre *Error Crítico*, *Error No Crítico*, *Vacilación* y *Sugerencia del usuario*.
- **Cuestionario SUS:** Versión unificada y adaptada contextualmente (ej. "Creo que me gustaría usar CaféU con frecuencia").

---
