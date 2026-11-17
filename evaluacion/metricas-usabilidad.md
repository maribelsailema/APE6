# Métricas de usabilidad – Aula Abierta

**Actividad:** APE6-F1-04 · Fase 1  
**Prototipo:** Aula Abierta  
**Responsable:** Alex  
**Versión:** 1.0  
**Estado:** Instrumento de planificación; todavía no contiene resultados de pruebas.

## 1. Propósito

Establecer una forma uniforme de medir la eficacia, eficiencia y satisfacción de las personas que prueben el prototipo Aula Abierta durante la Fase 2. Los datos se registrarán por participante anónimo y por tarea.

## 2. Unidad de evaluación

- **Participante:** persona identificada únicamente con un código (P01, P02, P03…).
- **Tarea:** una de las seis actividades descritas en la hoja de observación.
- **Intento:** cada ocasión en que la persona comienza una tarea. Si debe repetirla, se registra un nuevo intento y se conserva el resultado del primero.
- **Sesión:** realización de las seis tareas y respuesta al cuestionario SUS.

No se registrarán nombres, cédulas, correos, teléfonos, usuarios institucionales ni otros datos que permitan identificar a la persona.

## 3. Eficacia: tasa de éxito

La eficacia representa si la persona logra el objetivo solicitado.

**Fórmula:**

`Tasa de éxito (%) = (Tareas completadas correctamente / Tareas intentadas) × 100`

Se considerará una tarea **completada correctamente** cuando la persona alcance el resultado esperado sin que el evaluador tenga que realizar la acción por ella. Una tarea terminada con un resultado incorrecto no cuenta como éxito.

Para el cálculo general se sumarán las tareas completadas correctamente por todos los participantes y se dividirán para el total de tareas intentadas. También se recomienda presentar el porcentaje por tarea para identificar cuáles generan más dificultades.

**Registro por tarea:**
- Éxito: Sí / No.
- Resultado: correcto / incorrecto / incompleto.
- ¿Necesitó ayuda?: Sí / No.
- Número de intentos: entero.

Una tarea abandonada después de iniciarse se registra como intentada y no completada. Una tarea que no se presentó por un problema ajeno al participante se marca como no aplicada y se excluye del denominador.

## 4. Eficiencia: tiempo por tarea

El tiempo se registrará en segundos.

- **Inicio:** momento en que el evaluador indica la tarea y la persona comienza a interactuar.
- **Finalización:** momento en que se alcanza el resultado esperado o se declara que la tarea no puede continuar.
- **Duración:** hora de finalización menos hora de inicio.

`Duración (segundos) = hora de finalización − hora de inicio`

Se utilizará un cronómetro o reloj con segundos. Se anotará el tiempo incluso cuando la tarea no se complete, indicando el resultado. Si se interrumpe por una causa externa (por ejemplo, falla del equipo o interrupción de la sesión), se anotará la interrupción y el tiempo no se interpretará como tiempo normal de ejecución.

Para cada tarea se podrá calcular el promedio de duración únicamente entre los intentos válidos. Se recomienda informar también el mínimo, máximo y cantidad de casos, para que un promedio no oculte diferencias importantes.

## 5. Clasificación de errores

### Error crítico

Situación que impide completar la tarea o provoca un resultado importante distinto del solicitado. Ejemplos aplicables al flujo de reservas:

- La persona intenta confirmar, pero la reserva no queda confirmada.
- La persona cancela una reserva cuando su objetivo era conservarla.
- El prototipo muestra un estado que no corresponde con la acción realizada.
- La persona queda bloqueada y no puede continuar con la tarea.
- Una acción provoca la pérdida de la reserva o de información necesaria para completarla.

Un error crítico se registra aunque la persona consiga recuperarse posteriormente. Se anotará su efecto y si pudo corregirse.

### Error no crítico

Dificultad que puede corregirse y que no impide alcanzar el objetivo final. Ejemplos:

- Hace clic inicialmente en un control equivocado y luego encuentra el correcto.
- Necesita más de un intento para localizar una opción.
- Regresa a una pantalla anterior por confusión, pero puede continuar.
- No comprende de inmediato una etiqueta, aunque finalmente realiza la acción correcta.

### Registro del error

Para cada evento se anotará: tarea, momento aproximado, descripción observable, tipo (crítico/no crítico), consecuencia, si se recuperó y si solicitó ayuda. Se describirá lo que ocurrió sin atribuir intenciones ni juzgar a la persona.

## 6. Solicitudes de ayuda

Se contará una solicitud cada vez que el participante pida orientación o que el evaluador deba intervenir para que pueda continuar.

- **Ayuda solicitada:** la persona pregunta qué debe hacer, dónde debe hacer clic o qué significa una opción.
- **Ayuda ofrecida:** el evaluador interviene sin que la persona la haya solicitado.
- **Tipo de ayuda:** aclaración de la consigna / orientación sobre la interfaz / explicación de una función / intervención para resolver un bloqueo.

El evaluador debe evitar dar pistas durante la ejecución. Si la persona pregunta, se registra la solicitud antes de responder. La ayuda recibida se describe brevemente. La tarea puede completarse, pero se debe indicar que requirió ayuda.

## 7. Satisfacción: cuestionario SUS

Al terminar las seis tareas, cada participante responderá las diez afirmaciones del cuestionario SUS, utilizando una escala de 1 a 5:

1 = Totalmente en desacuerdo  
2 = En desacuerdo  
3 = Neutral  
4 = De acuerdo  
5 = Totalmente de acuerdo

El procedimiento de puntuación está documentado en `cuestionario-sus.md`. El resultado SUS se expresa entre 0 y 100; no representa un porcentaje de respuestas positivas.

## 8. Resumen de indicadores a reportar

| Dimensión | Indicador | Forma de presentación |
|---|---|---|
| Eficacia | Tasa de éxito | Por tarea y global, en porcentaje |
| Eficiencia | Duración | Segundos por tarea; promedio y rango |
| Errores | Críticos y no críticos | Cantidad por tarea y descripción |
| Apoyo | Solicitudes/intervenciones | Cantidad y tipo por tarea |
| Satisfacción | Puntuación SUS | Puntuación por participante y resumen del grupo |

## 9. Reglas para interpretar los datos

- No se deben inventar, completar ni estimar resultados que no se hayan observado.
- Los resultados se presentarán únicamente después de ejecutar las sesiones.
- Una tasa de éxito alta no elimina la importancia de los errores críticos.
- Los tiempos deben analizarse junto con el éxito y las ayudas recibidas.
- La puntuación SUS debe acompañarse del número de respuestas válidas.
- Cualquier cambio en las tareas o en el prototipo debe quedar documentado para poder interpretar los resultados.
