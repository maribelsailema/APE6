# 🔺 APE 6 – Fase 4: Triangulación metodológica de CaféU

## 📋 1. Información general

| Campo | Información |
|---|---|
| Actividad | APE6-F3F4-03 · Triangulación metodológica |
| Proyecto | CaféU |
| Método 1 | Evaluación heurística de Nielsen (cuatro evaluadores independientes) |
| Método 2 | Pruebas con usuarios mediante pensamiento en voz alta (P1, P2, P3 · 16-nov-2026 · registros de Wilson) |

## 🎯 2. Objetivo y reglas del cruce

Cruzar cada hallazgo de la [matriz consolidada](matriz-hallazgos.md) con los registros de usuarios y clasificarlo en una de tres categorías:

| Categoría | Definición operativa |
|---|---|
| **Confirmado por ambos métodos** | El problema fue detectado por la inspección heurística **y** se observó en las sesiones (error no crítico registrado, dificultad observada o comentario explícito del participante sobre ese mismo problema). |
| **Solo heurística** | Detectado por los evaluadores, pero no observado en las sesiones (porque no ocurrió, porque las tareas no lo cubrieron o porque la versión piloteada difiere). |
| **Solo usuarios** | La dificultad apareció en las pruebas y ningún evaluador la había detectado en la inspección. |

**Reglas de honestidad aplicadas:**

1. Un *comentario de cierre* se registra como evidencia cualitativa de riesgo, **no** como error de ejecución (criterio de [Resumen_Metricas.md](../../Fase2-Pilotaje/Resumen_Metricas.md) y [Hallazgos_Preliminares.md](../../Fase2-Pilotaje/Hallazgos_Preliminares.md)).
2. «No observado» no significa «inexistente»: las seis tareas no cubrieron errores de sistema, carrito vacío ni cancelación.
3. Las citas de usuarios son textuales de los registros publicados; no se parafrasean como si fueran observaciones nuevas.
4. La clasificación se hace **a nivel de componente e mecanismo de interacción**, porque la captura de Figma analizada en F3 y la versión descrita en los registros del pilotaje presentan diferencias de texto y alcance (limitación L-01, [soporte-tecnico-f3.md](soporte-tecnico-f3.md)). Los componentes nucleares (barra flotante, «Eliminar», «Añadir» vs. detalle, buscador de Inicio, CTA «Ver Menú») existen en ambas y hacen válido el cruce.

## 📚 3. Fuentes

**Heurísticas:** [Viviana.md](../../Fase2-Pilotaje/Evaluaciones_Heuristicas/Viviana.md) · [Wilson.md](../../Fase2-Pilotaje/Evaluaciones_Heuristicas/Wilson.md) · [Alex.md](../../Fase2-Pilotaje/Evaluaciones_Heuristicas/Alex.md) · [Sebastian.md (F2)](../../Fase2-Pilotaje/Evaluaciones_Heuristicas/Sebastian.md) · [heuristica-sebastian.md (F3)](../resultados/heuristica-sebastian.md).

**Usuarios:** [P1.md](../../Fase2-Pilotaje/Participantes/P1.md) · [P2.md](../../Fase2-Pilotaje/Participantes/P2.md) · [P3.md](../../Fase2-Pilotaje/Participantes/P3.md) · [Resumen_Metricas.md](../../Fase2-Pilotaje/Resumen_Metricas.md) · [Hallazgos_Preliminares.md](../../Fase2-Pilotaje/Hallazgos_Preliminares.md).

**Contexto cuantitativo del pilotaje (verificado en las fuentes):** 18/18 tareas completadas autónomamente (100 % de eficacia) · 0 errores críticos · 4 errores no críticos (P1: T1, T3, T4; P3: T4) · 0 solicitudes de ayuda · medianas por tarea 24/19/41/39/24/31 s · SUS 82,5 (P1) / 85,0 (P2) / 80,0 (P3), promedio 82,5.

## 🔺 4. Triangulación por hallazgo

### H-01 · Acceso al pedido fuera de la convención de ubicación

| Campo | Registro |
|---|---|
| **Evidencia heurística** | Viviana H4=2 («el carrito usa barra inferior; algunos usuarios esperan la cabecera»); Wilson HW-03=2 (desviación del estándar e-commerce); Alex H4=2; Sebastián F3 (sin ícono en cabecera en E-IMG02-P01/P02). |
| **Evidencia de usuarios** | P1·T4, ENC registrado: buscó ~6 s un carrito en la esquina superior derecha. Verbatim: «miro arriba... no hay carrito... ah, abajo apareció una franja flotante». Cierre de P1: «todas las apps lo tienen ahí... pondría también un ícono arriba». P2/P3 sin dificultad. Afectados: 1/3. |
| **Clasificación** | **Confirmado por ambos métodos.** |
| **Interpretación** | La inspección predijo el punto exacto de fricción que el pilotaje confirmó. La convención externa importa en primeros usos; la barra inferior funciona una vez descubierta. No bloquea la tarea (los 3 completaron T4 dentro del tiempo máximo). |
| **Mejora propuesta** | Acceso dual: ícono de carrito con contador en la cabecera + barra flotante actual. |

### H-02 · Retroalimentación poco perceptible al añadir

| Campo | Registro |
|---|---|
| **Evidencia heurística** | Viviana H1=2; Wilson HW-01=2 (sin feedback animado al pulsar «Añadir»); Alex H1=2; Sebastián F3 (sin distintivo de cambio observable). |
| **Evidencia de usuarios** | P3·T4, registrado como ENC: «notó que la barra flotante negra no tiene una animación de rebote o badge numérico destacado al sumar ítems, aunque la localizó sin problemas». Afectados: 1/3. *Nota:* la [comparación de Fase 2](../../Fase2-Pilotaje/Evaluaciones_Heuristicas/Comparacion_Heuristicas_Pilotaje.md) señaló que Wilson y Alex deben revisar si esta observación merece clasificarse como ENC; el dato original se conserva. |
| **Clasificación** | **Confirmado por ambos métodos** (con la nota metodológica anterior). |
| **Interpretación** | El estado se actualiza, pero el cambio no se anuncia. Fricción de percepción, no de función. Con H-01 forma el par «descubrir el carrito / notar que cambió». |
| **Mejora propuesta** | Realce breve (micro-animación o badge temporal) al actualizar cantidad y total. |

### H-03 · Eliminación inmediata sin recuperación y control pequeño

| Campo | Registro |
|---|---|
| **Evidencia heurística** | Viviana H3=2/H5=2; Wilson HW-02=2 (borrado instantáneo sin confirmación ni undo); Alex H3=2/H5=2; Sebastián OBS-S01→F3=2 (control pequeño, sin recuperación en el flujo). |
| **Evidencia de usuarios** | **Comentarios de cierre (2/3):** P2: «borra el ítem de inmediato sin pedir confirmación... un usuario descuidado podría hacer clic por error y tendría que volver a buscar el producto». P3: «es un texto plano pequeño; a veces con el pulgar es fácil presionar sin querer... mejor un ícono de basurero con un área táctil más amplia o un diálogo rápido». P1·T5 verbatim: «al ladito dice en letras chiquitas "Eliminar"». **Errores en T5: 0/3.** |
| **Clasificación** | **Confirmado por ambos métodos**, con precisión: la evidencia de usuarios es *cualitativa de riesgo percibido* (comentarios + descripción del control), no un error de ejecución observado. |
| **Interpretación** | Cuatro evaluadores y dos participantes convergen en el mismo riesgo con la misma solución (deshacer/confirmar + área táctil). Que no ocurrieran borrados accidentales en 3 ejecuciones no descarta el riesgo en uso real con pulgar y prisa; tampoco lo demuestra. Severidad 2 con cláusula de escalado a 3 si se observa el accidente. |
| **Mejora propuesta** | Snackbar «Deshacer» temporal o confirmación breve; ampliar área táctil (ref. 44×44 px) y separar de controles contiguos. |

### H-04 · Añadir directo vs. personalización

| Campo | Registro |
|---|---|
| **Evidencia heurística** | Viviana H5=2/H6=1; Wilson HW-04=1; Alex H2=2/H6=2; Sebastián F3=2. |
| **Evidencia de usuarios** | P1·T3, ENC registrado: intentó «Añadir» desde la tarjeta, no encontró dónde escribir y retrocedió al detalle. Verbatim: «si le doy a Añadir se añade de una... no, mejor toco la tarjeta... ¡ahí sí!». Duda de ~5 s según observación de Wilson. Afectados: 1/3 (P2/P3 abrieron el detalle directamente). |
| **Clasificación** | **Confirmado por ambos métodos.** |
| **Interpretación** | La doble ruta es una fortaleza de eficiencia (H7) pero su señalización es débil (H5/H6): el costo lo paga quien personaliza. La discrepancia de severidad (Wilson 1 vs. mayoría 2) se resuelve con el dato observado: hubo un error de ruta real, más que una molestia cosmética. |
| **Mejora propuesta** | Etiqueta «Personalizar»/«Ver opciones» en productos con instrucciones especiales; diferenciar «Añadir» de «Abrir detalle». |

### H-05 · Buscador de Inicio compite con «Ver Menú»

| Campo | Registro |
|---|---|
| **Evidencia heurística** | Viviana H8=1; Alex H8=1 y Hallazgos H01=2; Sebastián F3=2 (buscador prominente sin conexión en la captura). Wilson no lo registró (H8=0). |
| **Evidencia de usuarios** | P1·T1, ENC registrado: pulsó el campo de búsqueda creyendo que debía escribir. Verbatim: «intento buscar aquí en la barrita... ah no, aquí abajo hay un botón negro grande que dice "Ver Menú"». Vacilación inicial de ~4 s. Afectados: 1/3. |
| **Clasificación** | **Confirmado por ambos métodos.** |
| **Interpretación** | En Fase 2 este punto fue «hallazgo del pilotaje» (CP-04) porque la inspección visual disponible no lo había marcado; la inspección F3 sí lo detecta en el diseño, por lo que ahora queda confirmado por ambos. La affordance del buscador invita a una acción que no es el camino de la tarea (y que en la captura ni siquiera está cableada). |
| **Mejora propuesta** | Reforzar jerarquía del CTA «Ver Menú»; reducir prominencia del buscador en Inicio o condicionarlo a que funcione. |

### H-06 · Carrito vacío sin estado definido

| Campo | Registro |
|---|---|
| **Evidencia heurística** | Wilson HW-05=1; Viviana H9 (pregunta abierta «qué ocurre si el carrito queda vacío»); Alex H9 0\* con recomendación de probarlo; Sebastián F3 (sin estado vacío en el flujo). |
| **Evidencia de usuarios** | **Ninguna.** T5 eliminó un ítem dejando uno; ninguna tarea vació el carrito. |
| **Clasificación** | **Solo heurística.** |
| **Interpretación** | Vacío de diseño detectado por inspección que las tareas no pudieron exponer. Su existencia real en el prototipo debe verificarse antes de corregir (podría existir una variante no capturada). |
| **Mejora propuesta** | Verificar comportamiento; diseñar estado vacío con CTA «Explorar menú» e impedir confirmar sin ítems. |

### H-07 · Secuencia de estados del pedido

| Campo | Registro |
|---|---|
| **Evidencia heurística** | Sebastián F2 OBS-S02 (hipótesis) → F3: con el cableado «Tras pausa» se concreta que «Preparando… 50 %» precede a «¡Pedido recibido!» (E-IMG02-P05/P07). |
| **Evidencia de usuarios** | **Ninguna.** Los tres participantes describen pasar de «Confirmar pedido» a la confirmación final sin mencionar la pantalla de estado; la versión piloteada parece no incluirla (L-01). En T6, 0 errores: la hipótesis de confusión de Fase 2 **no se observó** en el pilotaje (coincide con CP-06). |
| **Clasificación** | **Solo heurística.** |
| **Interpretación** | Hallazgo dependiente de versión: describe un riesgo de la versión capturada, no un fallo observado. Debe confirmarse qué versión es la vigente antes de tratarse como problema real del producto. |
| **Mejora propuesta** | Confirmar recepción antes de mostrar preparación; eliminar el porcentaje ficticio o ligarlo a estados reales. |

### H-08 · «Total pagado» antes de pagar

| Campo | Registro |
|---|---|
| **Evidencia heurística** | Sebastián F3: «Total pagado $4.25» en Estado vs. «Sin cobro en la app» en Mi Pedido y «Total a pagar» en Confirmación (E-IMG02). |
| **Evidencia de usuarios** | **Ninguna** (pantalla de estado no mencionada en los registros; L-01). Ningún participante reportó creer que se le había cobrado. |
| **Clasificación** | **Solo heurística.** |
| **Interpretación** | Inconsistencia semántica con potencial de malentendido monetario; el pilotaje no la expuso porque (según los registros) esa pantalla no formó parte del flujo probado. |
| **Mejora propuesta** | Unificar «Total a pagar» en todas las pantallas posteriores a la confirmación. |

### H-09 · Escenarios de error no cubiertos

| Campo | Registro |
|---|---|
| **Evidencia heurística** | Viviana H9 P/V; Alex H9 0\* + recomendación explícita; Sebastián F2/F3 parcial. |
| **Evidencia de usuarios** | **Ninguna.** 0 errores críticos y 0 solicitudes de ayuda en 18 ejecuciones; los escenarios de fallo no se probaron. |
| **Clasificación** | **Solo heurística** (vacío de cobertura compartido por ambos métodos: ninguno lo ha evaluado). |
| **Interpretación** | La ausencia de errores en el pilotaje no certifica la recuperación ante errores. Es el hueco de evaluación más importante para la siguiente iteración. |
| **Mejora propuesta** | Inspección específica de estados de error (fallo de confirmación, conexión, pedido inválido) y diseño de mensajes con recuperación. |

### H-10 · Inconsistencias menores de presentación

| Campo | Registro |
|---|---|
| **Evidencia heurística** | Sebastián F3 (posición de marca; «Sanduches» sin tilde). |
| **Evidencia de usuarios** | **Ninguna.** |
| **Clasificación** | **Solo heurística.** |
| **Interpretación** | Cosmético; sin efecto observable en las tareas. |
| **Mejora propuesta** | Unificar cabecera y corregir tilde. |

### H-11 · Modal de cancelación por verificar

| Campo | Registro |
|---|---|
| **Evidencia heurística** | Sebastián OBS-S03 (F2) → H-11 (F3): cuerpo del modal oculto por la anotación; destinos de botones sin confirmar. |
| **Evidencia de usuarios** | **Ninguna.** La cancelación no formó parte de las seis tareas. |
| **Clasificación** | **Solo heurística** (verificación pendiente, no defecto demostrado). |
| **Interpretación** | El mecanismo de prevención existe y es correcto en su estructura; lo que falta es evidencia legible de su contenido y comportamiento. |
| **Mejora propuesta** | Captura limpia + recorrido interactivo de cancelación y desistimiento. |

### H-12 · Tiempo estimado ausente en la confirmación capturada

| Campo | Registro |
|---|---|
| **Evidencia heurística** | Sebastián F3 (E-IMG02-P07 sin tiempo); antecedente APE 4 (ausencia ya observada antes). |
| **Evidencia de usuarios** | **Ninguna sobre el problema** (la versión piloteada sí mostraba «5 a 10 minutos» y los tres lo reportaron correctamente en T6). Evidencia indirecta del valor del dato: P3, cierre: «el tiempo de 5 a 10 minutos te permite calcular si alcanzas a retirar antes de que empiece tu clase». |
| **Clasificación** | **Solo heurística** (condicionada a versión). |
| **Interpretación** | Si la captura es la versión vigente, se trata de una regresión de un dato que los usuarios demostraron usar y valorar; si la captura es anterior, el hallazgo se cierra como diferencia de versión. La triangulación aporta aquí el argumento de valor del usuario, no la confirmación del fallo. |
| **Mejora propuesta** | Confirmar versión; restaurar el tiempo estimado si falta. |

## 📊 5. Matriz resumen de la triangulación

| ID | Heurística(s) | Evidencia de usuarios | Participantes | Clasificación | Severidad consensuada (propuesta) |
|---|---|---|---|---|:--:|
| H-01 | H4, H6 | ENC T4 + cierre | P1 (1/3) | Ambos | 2 |
| H-02 | H1 | ENC T4 (con nota metodológica) | P3 (1/3) | Ambos | 2 |
| H-03 | H3, H5, H8 | Comentarios de cierre + verbatim T5; 0 errores T5 | P2, P3 (2/3) | Ambos (riesgo percibido) | 2 |
| H-04 | H5, H6, H2 | ENC T3 | P1 (1/3) | Ambos | 2 |
| H-05 | H6, H8, H5 | ENC T1 | P1 (1/3) | Ambos | 2 |
| H-06 | H9, H5 | Ninguna (no cubierto) | — | Solo heurística | 1 / P/V |
| H-07 | H1, H2 | Ninguna (versión distinta) | — | Solo heurística | 2 propuesta |
| H-08 | H2, H4 | Ninguna (versión distinta) | — | Solo heurística | 2 propuesta |
| H-09 | H9 | Ninguna (no cubierto) | — | Solo heurística | P/V |
| H-10 | H4 | Ninguna | — | Solo heurística | 1 propuesta |
| H-11 | H3, H5, H9 | Ninguna (no cubierto) | — | Solo heurística | P/V |
| H-12 | H1, H10 | Ninguna sobre el problema; valor del dato reportado | — | Solo heurística | 2 propuesta cond. |

**Totales: 5 confirmados por ambos métodos · 7 solo heurística · 0 solo usuarios.**

## 🔍 6. Verificación explícita de «solo usuarios»

Para afirmar que ningún hallazgo es «solo usuarios» se revisó cada dificultad registrada en las sesiones y se comprobó que la inspección heurística la cubre:

| Dificultad registrada en usuarios | Tarea | ¿Cubierta por inspección? | Hallazgo |
|---|---|---|---|
| P1 pulsó el buscador antes de «Ver Menú» | T1 | Sí (Viviana H8, Alex H8/H01, Sebastián F3) | H-05 |
| P1 dudó entre «Añadir» y abrir el detalle | T3 | Sí (Viviana H5/H6, Wilson HW-04, Alex H2/H6, Sebastián F3) | H-04 |
| P1 buscó el carrito en la cabecera | T4 | Sí (Viviana H4, Wilson HW-03, Alex H4, Sebastián F3) | H-01 |
| P3 señaló falta de realce al añadir | T4 | Sí (Viviana H1, Wilson HW-01, Alex H1, Sebastián F3) | H-02 |
| P2/P3 pidieron deshacer/confirmación y mayor área táctil | T5 (cierre) | Sí (los cuatro evaluadores) | H-03 |
| T2 y T6 sin dificultades registradas | T2, T6 | — | — |

**Conclusión:** no existe dificultad de usuarios sin contraparte heurística. Esto es coherente con un pilotaje de flujo nominal (sin errores críticos) y con una inspección que contó con la evidencia completa del flujo. No debe interpretarse como que los métodos son redundantes: la inspección aportó 7 hallazgos que las sesiones no podían exponer (estados no probados y diferencias de versión).

## ⚠️ 7. Validez y limitaciones de la triangulación

1. **Muestra pequeña:** 3 participantes; los resultados son descriptivos, no generalizables (criterio del README y Resumen_Metricas).
2. **Diferencia de versión/artefacto (L-01):** la captura F3 y los registros difieren en textos, chips, contador y alcance de pantallas; el registro de P2 menciona «recálculo dinámico en el DOM», lo que sugiere que el pilotaje pudo ejecutarse sobre una implementación HTML y no sobre el prototipo Figma. **Pendiente de confirmar con Wilson y Viviana.** El cruce se hizo por componentes comunes; los hallazgos dependientes de versión (H-07, H-08, H-12) quedan condicionados.
3. **Comentarios ≠ errores:** el riesgo de eliminación (H-03) está respaldado por percepción de usuarios, no por fallos observados; se mantiene la distinción en todo el documento.
4. **Clasificación ENC de P3·T4:** pendiente de revisión por Wilson y Alex (nota heredada de la comparación de Fase 2); no altera la clasificación de H-02 como confirmado por ambos.
5. **Cobertura de tareas:** seis tareas nominales; error de sistema, carrito vacío y cancelación quedaron fuera (H-06, H-09, H-11 no pudieron observarse).
6. **Independencia:** las evaluaciones de Viviana y Alex se declaran preliminares por sus autores y usan el pilotaje como insumo; la convergencia con los usuarios es por tanto parcialmente esperable y no se presenta como corroboración fully independiente. La inspección F3 de Sebastián y la de Wilson sí aportan juicio de diseño independiente.

## 🎓 8. Conclusiones (insumo para Viviana) y criterios técnicos (insumo para Alex)

**Para las conclusiones del informe (Viviana):**

1. Los dos métodos convergen en cinco problemas concretos (H-01…H-05), todos de severidad menor propuesta (2): el flujo es eficaz (18/18) y la fricción se concentra en descubribilidad y recuperación, no en capacidad de completar la tarea.
2. La convergencia más fuerte es H-03 (4/4 evaluadores + 2/3 usuarios pidiendo la misma solución): la recuperación tras eliminar es la mejora con mayor respaldo conjunto.
3. La inspección heurística amplió el alcance más allá del flujo nominal: 7 hallazgos «solo heurística» señalan estados no probados (vacío, error, cancelación) y diferencias de versión que la siguiente iteración debe cerrar.
4. Ningún problema observado justifica severidad 3–4 con la evidencia actual; los escalamientos quedan condicionados a verificación (cláusulas en H-03 y H-12).
5. La satisfacción alta (SUS 82,5) es compatible con estos hallazgos: los usuarios completan todo y valoran la claridad, pero tropiezan en puntos específicos y recuperables.

**Para los criterios técnicos del backlog (Alex):** usar la priorización por evidencia de [matriz-hallazgos §5](matriz-hallazgos.md): cinco hallazgos listos (tres unánimes + dos con severidad por ratificar), uno cosmético, tres verificaciones previas y tres condicionados a versión. Ningún P/V entra como corrección sin verificación.

---