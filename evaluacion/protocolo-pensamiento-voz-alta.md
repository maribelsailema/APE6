# Protocolo de Evaluación de Usabilidad: Pensamiento en Voz Alta (Think-Aloud Protocol)



## 1. Fundamentación y Articulación con `docs/`

El presente protocolo operacionaliza la técnica de **Pensamiento en Voz Alta** (*Think-Aloud Protocol*), formalizada por Clayton Lewis (1982) y Jakob Nielsen (1993) a partir de los estudios cognitivos de Ericsson & Simon (1984), articulándose directamente con la planificación del proyecto definida en la carpeta `docs/`:
- **`docs/plan-evaluacion.md`:** Fundamento normativo bajo ISO 9241-11:2018 y secuencia de la sesión de 25 minutos.
- **`docs/participantes-roles.md`:** Asignación formal de roles del equipo y selección de los 3 perfiles de participantes (`P01`, `P02`, `P03`).
- **`docs/consentimiento-informado.md`:** Protocolo de ética, confidencialidad y participación voluntaria.

### 1.1 Objetivo del Protocolo en CaféU
Obtener acceso directo al modelo mental del estudiante universitario durante la consulta, personalización, revisión y confirmación de pedidos rápidos, identificando barreras de usabilidad sin condicionar la interacción mediante instrucciones sobre botones.

---

## 2. Distribución de Roles del Equipo (Según `docs/participantes-roles.md`)

Para asegurar la validez metodológica y evitar interferencias, cada integrante del equipo asume una función específica:

```
       ┌────────────────────────────────────────────────────────┐
       │             PARTICIPANTE (P01 / P02 / P03)             │
       └───────────────────────────▲────────────────────────────┘
                                   │ Interacción Directa
       ┌───────────────────────────▼────────────────────────────┐
       │                 MODERADORA (Viviana)                   │
       │  - Conduce la sesión verbalmente                       │
       │  - Lee consentimiento y consignas neutrales            │
       │  - Aplica preguntas sonda no directivas                │
       │  - Administra la regla de pista única                  │
       └──────────────┬──────────────────────────┬──────────────┘
                      │                          │
        Datos Cuantitativos        Datos Cualitativos
                      │                          │
       ┌──────────────▼────────────┐ ┌───────────▼──────────────┐
       │  RESPONSABLE DE MÉTRICAS  │ │    OBSERVADOR (Wilson)   │
       │          (Alex)           │ │  - Registra dificultades │
       │  - Cronómetro digital (s) │ │  - Citas textuales       │
       │  - Tasa de éxito (Sí/No)  │ │  - Lenguaje no verbal    │
       │  - Conteo de errores      │ │  - Heurísticas violadas  │
       └───────────────────────────┘ └──────────────────────────┘
                      │                          │
                      └────────────┬─────────────┘
                                   │ Soporte Técnico
       ┌───────────────────────────▼────────────────────────────┐
       │                SOPORTE TÉCNICO (Sebastián)             │
       │  - Configura resolución (Móvil P01/P03; PC P02)        │
       │  - Gestiona software de grabación y navegador          │
       │  - Restablece el prototipo a la pantalla 01_Inicio     │
       └────────────────────────────────────────────────────────┘
```

| Integrante | Rol Asignado | Responsabilidades Operativas |
| :--- | :--- | :--- |
| **Viviana** | Moderadora | Presenta el propósito, gestiona el consentimiento informado, lee textualmente las consignas de las tareas y formula preguntas sonda ante silencios. No señala pantallas ni sugiere acciones. |
| **Wilson** | Observador | Registra comportamientos, vacilaciones, comentarios textuales (*verbatim*), expresiones de frustración/alivio y mapea las fricciones con las 10 heurísticas de Jakob Nielsen. |
| **Alex** | Responsable de Métricas | Cronometra con precisión de segundos cada tarea, evalúa el cumplimiento binario del criterio de éxito (Sí / Con ayuda / No), cuantifica errores y entrega el cuestionario SUS. |
| **Sebastián** | Soporte Técnico | Calibra el entorno tecnológico, comprueba el funcionamiento del prototipo antes de cada sesión, gestiona la grabación y realiza el reinicio entre participantes. |

---

## 3. Cronograma Operativo de la Sesión (25 Minutos)

Conforme a la Sección 17 de `docs/plan-evaluacion.md`, cada sesión individual se desarrollará en 25 minutos:

| Etapa | Responsable Principal | Duración Planificada |
| :--- | :--- | :---: |
| 1. Bienvenida y contextualización | Viviana (Moderadora) | 3 min |
| 2. Lectura y firma del consentimiento informado | Viviana y Participante | 3 min |
| 3. Inducción al pensamiento en voz alta y calentamiento | Viviana y Wilson | 2 min |
| 4. Ejecución de las seis tareas de usabilidad (T1 a T6) | Todo el equipo | 12 min |
| 5. Aplicación del Cuestionario SUS (10 ítems) | Alex (Métricas) | 4 min |
| 6. Entrevista de cierre (*Debriefing*) y agradecimiento | Viviana y Wilson | 1 min |
| **Total Estimado** | — | **25 min** |

---

## 4. Guion de Inducción para el Participante (Lectura por Viviana)

La moderadora Viviana leerá **palabra por palabra** el siguiente guion de bienvenida e inducción:

---

> ### 📢 Guion de Apertura de la Sesión
> 
> *"¡Hola! Muchas gracias por colaborar con nosotros. Mi nombre es Viviana y junto con mis compañeros de la carrera de Software de la Universidad Técnica de Ambato estamos desarrollando una práctica para la materia de Interacción Humano-Computador.*
> 
> *El día de hoy vamos a probar un prototipo de aplicación web móvil llamado **CaféU**, diseñado para que los estudiantes universitarios puedan consultar el menú de la cafetería, personalizar su pedido y enviarlo con anticipación para retirarlo en caja rápida.*
> 
> *Antes de empezar, quiero enfatizar tres aspectos esenciales:*
> 1. ***Estamos evaluando el diseño de la aplicación, NO tus habilidades.*** *Tú no puedes cometer ningún error el día de hoy. Cualquier duda, confusión o tropiezo se debe únicamente a que la interfaz aún tiene oportunidades de mejora.*
> 2. ***Tus datos son totalmente confidenciales.*** *Tu participación se registrará únicamente mediante un código anónimo (`P01`, `P02` o `P03`) y los datos se utilizarán exclusivamente para fines académicos, tal como indica el consentimiento informado que acabamos de revisar.*
> 3. ***La prueba es 100% voluntaria.*** *Si en algún momento deseas hacer una pausa o terminar la sesión, puedes decírmelo con total libertad.*
> 
> *Durante la prueba utilizaremos una técnica llamada **Pensamiento en Voz Alta**. Esto significa que te pediremos que vayas expresando en voz alta todo lo que pasa por tu mente mientras interactúas con la pantalla: dinos qué información estás viendo, qué estás buscando, qué esperas que ocurra antes de tocar un control y qué sensaciones o dudas te genera lo que aparece en pantalla.*
> 
> *Por favor, imagínate que estás solo frente a tu teléfono hablando contigo mismo en voz alta. Yo no podré darte instrucciones sobre cómo resolver las tareas porque deseamos observar si la interfaz es clara por sí misma. Sin embargo, si en algún momento te quedas en silencio, te recordaré amablemente que sigas contándonos lo que piensas.*
> 
> *¿Tienes alguna duda antes de comenzar?"*

---

## 5. Ejercicio de Calentamiento (*Warm-up*)

Para vencer la timidez inicial y practicar el monólogo exterior:

> ### ☕ Consigna de Calentamiento (60 segundos)
> *"Para practicar cómo pensar en voz alta, hagamos un ejercicio rápido. Imagina que vas a comprar un café en un mostrador físico tradicional. Cuéntame en voz alta paso a paso: ¿cómo le preguntarías a la persona que atiende qué opciones tienen, cómo decidirías qué tamaño pedir y qué harías si te dicen que se agotó el azúcar?"*

Viviana modela la técnica si el participante duda: *"Exacto, así como dices: 'Miraría la pizarra de precios, preguntaría qué tipo de leche usan...'"*. Una vez comprobada la soltura verbal, Sebastián proyecta la pantalla `01_Inicio.png` de CaféU.

---

## 6. Pauta de Intervenciones Neutrales del Moderador

Durante la resolución de las tareas, la moderadora mantendrá neutralidad estricta. Queda prohibido aprobar con la cabeza, sonreír para validar o gesticular ante fallas.

### 6.1 Banco de Preguntas Sonda Neutrales Permitidas
| Situación en Pantalla | Intervención Estándar de la Moderadora |
| :--- | :--- |
| **Silencio sostenido (> 5 segundos)** | *"¿Qué estás pensando en este momento?"* |
| **El usuario explora la pantalla con la vista** | *"¿Qué información estás buscando?"* |
| **El usuario toca un control y vacila** | *"¿Qué esperabas que ocurriera al tocar ahí?"* |
| **El usuario llega a la pantalla de confirmación** | *"¿Qué te llama la atención de lo que muestra la pantalla?"* |
| **El usuario pregunta: '¿Lo hice bien?'** | *"Cuéntame tú qué interpretas de lo que muestra la pantalla en este momento."* |
| **El usuario pregunta: '¿Dónde está el sánduche?'** | *"Explora la pantalla y cuéntame si logras encontrarlo."* |

### 6.2 Prohibiciones Expresas (Vicios de Moderación)
❌ **NUNCA** decir: *"Toca el botón Añadir"*, *"Presiona Ver Menú"*, *"Mira abajo en la barra flotante"*, *"Filtra por snacks"*, *"Toca eliminar"*.  
❌ **NUNCA** decir: *"¡Muy bien!"*, *"Exacto"*, *"Eso era"*.  
❌ **NUNCA** señalar la pantalla con las manos ni con el puntero del ratón.

---

## 7. Protocolo de Bloqueo y Regla de Pista Única

Si el participante experimenta un bloqueo cognitivo por más de **15 segundos continuos** o manifiesta estar perdido:
1. Viviana leerá con tono calmado y estrictamente literal:
   > *"Vuelve a leer la tarea y revisa las opciones que tienes en pantalla."*
2. Alex (Métricas) anotará de inmediato: **Pista = Sí** en la hoja de control, registrando la tarea como **"Con ayuda"**.
3. Si transcurre el tiempo restante hasta alcanzar el $T_{\max}$ sin resolución, Viviana cerrará amablemente:
   > *"No te preocupes, pasemos a la siguiente actividad."* *(Resultado: **No**).*

---

## 8. Aspectos Observables Clave (Guía para el Observador Wilson)

Wilson centrará su observación cualitativa en los siguientes puntos clave de la interfaz de CaféU:

1. **Pantalla 01_Inicio:** ¿El usuario identifica de inmediato el botón `Ver Menú ->` o intenta interactuar con los elementos estáticos de *"¿Cómo funciona?"* o el buscador?
2. **Pantalla 02_Menu:**
   - ¿Reconoce que los chips (*Bebidas calientes*, *Sánduches*, *Snacks*) son botones de filtrado?
   - ¿Detecta la barra flotante inferior del carrito (*"2 items · $4.25 | Ver mi pedido"*) o busca un icono en la cabecera superior?
3. **Pantalla 03_Detalle_Producto:**
   - ¿Comprende que para personalizar debe tocar la tarjeta y no el botón directo de añadir?
   - ¿El campo de texto libre para notas especiales genera dudas?
4. **Pantalla 04_Revisar_Pedido:**
   - ¿Ubica con facilidad el enlace de texto *"Eliminar"* para quitar productos?
   - ¿Lee y comprende la nota *"Pago en caja: Paga al momento de retirar tu pedido"* o busca opciones para pagar con tarjeta?
5. **Pantalla 05_Confirmacion:**
   - ¿Identifica claramente el código `#CU-104` como su identificador de retiro en barra?
   - ¿Nota la estimación de 5 a 10 minutos para gestionar su tiempo?

---

## 9. Hoja de Observación y Registro Individual de Sesión

```text
========================================================================================
HOJA DE OBSERVACIÓN Y REGISTRO DE USABILIDAD · APE 6
Universidad Técnica de Ambato · FISEI · Carrera de Software · HCI
Caso de Estudio: Aplicación Móvil CaféU
========================================================================================

DATOS GENERALES DE LA SESIÓN:
----------------------------------------------------------------------------------------
Código del Participante: [ P01 / P02 / P03 ]    Fecha y Hora: _________________________
Moderadora: Viviana                            Observador: Wilson
Responsable de Métricas: Alex                  Soporte Técnico: Sebastián
Dispositivo: [ ] Móvil Físico (P01 / P03)      [ ] Computadora / Laptop (P02)
Grabación: [ ] Autorizada en consentimiento    [ ] No autorizada
Estado Inicial Verificado (Pantalla 01 vacía): [ ] Sí [ ] No
----------------------------------------------------------------------------------------

REGISTRO DE LAS SEIS TAREAS:
----------------------------------------------------------------------------------------
T1: Consulta de catálogo y precio individual de bebida (01_Inicio -> 02_Menu)
- Tiempo medido: ______ s (Meta: 30 s | Máx: 60 s)
- Resultado: [ ] Sí (sin ayuda)   [ ] Con ayuda (pista)   [ ] No (falló/superó máx)
- ¿Pidió repetir la consigna?: [ ] Sí  [ ] No
- ¿Accedió por "Ver Menú" o por el buscador?: __________________________________________
- Errores Críticos (EC): ________________________________________________________________
- Errores No Críticos (ENC): ____________________________________________________________
- Citas Textuales (Verbatim): "________________________________________________________"
- Heurística de Nielsen asociada: [ ] H1  [ ] H4  [ ] H8  [ ] Ninguna

----------------------------------------------------------------------------------------
T2: Filtrado por categoría y selección de snack (02_Menu)
- Tiempo medido: ______ s (Meta: 30 s | Máx: 60 s)
- Resultado: [ ] Sí (sin ayuda)   [ ] Con ayuda (pista)   [ ] No (falló/superó máx)
- ¿Presionó el chip "Snacks" con facilidad?: [ ] Sí  [ ] No (hizo scroll vertical)
- Errores Críticos (EC): ________________________________________________________________
- Errores No Críticos (ENC): ____________________________________________________________
- Citas Textuales (Verbatim): "________________________________________________________"
- Heurística de Nielsen asociada: [ ] H4  [ ] H7  [ ] H8  [ ] Ninguna

----------------------------------------------------------------------------------------
T3: Configuración y personalización con instrucciones especiales (02_Menu -> 03_Detalle)
- Tiempo medido: ______ s (Meta: 45 s | Máx: 90 s)
- Resultado: [ ] Sí (sin ayuda)   [ ] Con ayuda (pista)   [ ] No (falló/superó máx)
- ¿Tocó la tarjeta para abrir detalle o intentó añadir rápido?: __________________________
- Errores Críticos (EC): ________________________________________________________________
- Errores No Críticos (ENC): ____________________________________________________________
- Citas Textuales (Verbatim): "________________________________________________________"
- Heurística de Nielsen asociada: [ ] H2  [ ] H6  [ ] H8  [ ] Ninguna

----------------------------------------------------------------------------------------
T4: Sumar alimento al pedido y comprobar desglose de cuenta (02_Menu -> 04_Pedido)
- Tiempo medido: ______ s (Meta: 45 s | Máx: 90 s)
- Resultado: [ ] Sí (sin ayuda)   [ ] Con ayuda (pista)   [ ] No (falló/superó máx)
- ¿Detectó de inmediato la barra flotante inferior del carrito?: [ ] Sí  [ ] No
- Errores Críticos (EC): ________________________________________________________________
- Errores No Críticos (ENC): ____________________________________________________________
- Citas Textuales (Verbatim): "________________________________________________________"
- Heurística de Nielsen asociada: [ ] H1  [ ] H4  [ ] H7  [ ] Ninguna

----------------------------------------------------------------------------------------
T5: Modificación de orden / Eliminación de ítem en el carrito (04_Pedido)
- Tiempo medido: ______ s (Meta: 30 s | Máx: 60 s)
- Resultado: [ ] Sí (sin ayuda)   [ ] Con ayuda (pista)   [ ] No (falló/superó máx)
- Método de eliminación usado: [ ] Enlace "Eliminar"   [ ] Stepper [-] hasta cero
- Errores Críticos (EC): ________________________________________________________________
- Errores No Críticos (ENC): ____________________________________________________________
- Citas Textuales (Verbatim): "________________________________________________________"
- Heurística de Nielsen asociada: [ ] H3  [ ] H5  [ ] H6  [ ] Ninguna

----------------------------------------------------------------------------------------
T6: Confirmación del pedido y verificación de entrega y pago (04_Pedido -> 05_Confirm)
- Tiempo medido: ______ s (Meta: 45 s | Máx: 90 s)
- Resultado: [ ] Sí (sin ayuda)   [ ] Con ayuda (pista)   [ ] No (falló/superó máx)
- ¿Identificó el número #CU-104?: [ ] Sí  [ ] No
- ¿Identificó el tiempo de 5-10 min?: [ ] Sí  [ ] No
- ¿Comprendió que el pago se realiza en caja rápida?: [ ] Sí  [ ] No
- Citas Textuales (Verbatim): "________________________________________________________"
- Heurística de Nielsen asociada: [ ] H1  [ ] H2  [ ] H9  [ ] Ninguna
========================================================================================
```

---

## 10. Cuestionario de Usabilidad SUS (System Usability Scale)

Al culminar la tarea T6, Alex entrega al participante el cuestionario SUS estandarizado (Brooke, 1996) con 10 afirmaciones en escala Likert del 1 (*Totalmente en desacuerdo*) al 5 (*Totalmente de acuerdo*):

1. Creo que me gustaría utilizar la aplicación móvil CaféU frecuentemente entre mis clases.
2. Encontré la aplicación innecesariamente compleja para ordenar en la cafetería.
3. Considero que la aplicación fue fácil e intuitiva de usar.
4. Creo que necesitaría asistencia técnica para poder pedir mi comida con esta app.
5. Las funciones de búsqueda, personalización y carrito estaban bien integradas.
6. Percibí inconsistencias notables en las pantallas o en la forma de ordenar.
7. Imagino que cualquier compañero estudiante aprendería a usar CaféU muy rápidamente.
8. Encontré la aplicación engorrosa o confusa al momento de revisar el pedido.
9. Me sentí seguro y confiado al confirmar mi pedido en la pantalla.
10. Necesité aprender muchas cosas antes de poder usar la aplicación.

### 10.1 Procedimiento de Puntuación
- **Ítems impares (1, 3, 5, 7, 9):** $\text{Puntos} = \text{Respuesta} - 1$
- **Ítems pares (2, 4, 6, 8, 10):** $\text{Puntos} = 5 - \text{Respuesta}$
- **Puntaje Global:** $\text{SUS} = \left( \sum_{i=1}^{10} \text{Puntos}_i \right) \times 2.5$ (Escala 0 a 100, umbral estándar $\ge 68$).

---

## 11. Cierre y Entrevista Post-Sesión (*Debriefing*)

Viviana formula las dos preguntas abiertas cualitativas de cierre:
1. *"¿Qué fue lo que más te gustó o qué parte del proceso sentiste más rápida y clara?"*
2. *"Si pudieras cambiar o mejorar un elemento de las pantallas de CaféU, ¿cuál sería y por qué?"*

Viviana y Wilson agradecen formalmente al estudiante y Sebastián procede al restablecimiento del entorno para el siguiente participante.
