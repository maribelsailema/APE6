# 📊 APE 6 – Fases 3 y 4: Consolidación de las cuatro evaluaciones heurísticas de CaféU

## 📋 1. Información general

| Campo | Información |
|---|---|
| Actividad | APE6-F3F4-03 · Consolidación heurística |
| Proyecto | CaféU |
| Método | Comparación de las evaluaciones independientes de los cuatro integrantes con las diez heurísticas de Nielsen |
| Antecedente | [Consolidado parcial de Fase 2](../../Fase2-Pilotaje/Evaluaciones_Heuristicas/Consolidado_Heuristicas.md) |


## 🎯 2. Objetivo

Recopilar las evaluaciones heurísticas independientes de Viviana, Wilson, Sebastián y Alex; comprobar la cobertura de las diez heurísticas; agrupar los problemas equivalentes sin perder la evidencia individual; asignar identificadores estables H-XX; registrar la severidad de cada evaluador; fundamentar la severidad consensuada con frecuencia, impacto y persistencia; y documentar las discrepancias que no puedan resolverse.

## 📥 3. Insumos y disponibilidad verificada

| Evaluador | Documento | Disponibilidad | Estado declarado por su autor |
|---|---|---|---|
| Viviana Sarco ([@maribelsailema](https://github.com/maribelsailema)) | [Viviana.md](../../Fase2-Pilotaje/Evaluaciones_Heuristicas/Viviana.md) | ✅ Publicado en `main` | Borrador fundamentado; inspección personal pendiente de validación. |
| Wilson Pillapa ([@W1LSONN](https://github.com/W1LSONN)) | [Wilson.md](../../Fase2-Pilotaje/Evaluaciones_Heuristicas/Wilson.md) | ✅ Publicado en `main` | Evaluación completa con matriz de cinco hallazgos (HW-01…HW-05). |
| Sebastián Santana ([@SebasIsd](https://github.com/SebasIsd)) | [Sebastian.md (F2)](../../Fase2-Pilotaje/Evaluaciones_Heuristicas/Sebastian.md) + [heuristica-sebastian.md (F3)](../resultados/heuristica-sebastian.md) | ✅ F2 en `main`; F3 en esta rama | F2: inspección visual preliminar. F3: inspección con evidencia de cableado; verificaciones interactivas marcadas. |
| Alex Guachi ([@A1EXF6A](https://github.com/A1EXF6A)) | [Alex.md](../../Fase2-Pilotaje/Evaluaciones_Heuristicas/Alex.md) | ✅ Publicado en `main` | Evaluación preliminar basada en registros del pilotaje; severidades provisionales marcadas con \*. |

**Nota de honestidad documental:** las cuatro evaluaciones existen y están publicadas, pero dos de ellas (Viviana y Alex) se declaran preliminares por sus propios autores. Esta consolidación las utiliza tal como están publicadas, registra esa condición y no la oculta: las severidades de esos documentos se tratan como *propuestas de sus autores*, no como dictámenes definitivos. La ratificación grupal (sección 8) debe considerar esta condición.

**Insumos complementarios:** [Hallazgos_Preliminares.md](../../Fase2-Pilotaje/Hallazgos_Preliminares.md) (Alex, H01–H04), [Comparacion_Heuristicas_Pilotaje.md](../../Fase2-Pilotaje/Evaluaciones_Heuristicas/Comparacion_Heuristicas_Pilotaje.md) (CP-01…CP-06) y registros [P1](../../Fase2-Pilotaje/Participantes/P1.md), [P2](../../Fase2-Pilotaje/Participantes/P2.md), [P3](../../Fase2-Pilotaje/Participantes/P3.md) (solo para trazabilidad; el cruce metodológico completo vive en [triangulacion.md](triangulacion.md)).

## ✅ 4. Comprobación de cobertura de las diez heurísticas

Cada integrante evaluó las diez heurísticas. ✔ = heurística abordada explícitamente en su documento.

| Heurística | Viviana | Wilson | Sebastián (F2→F3) | Alex |
|---|:--:|:--:|:--:|:--:|
| H1 Visibilidad del estado | ✔ | ✔ | ✔ | ✔ |
| H2 Correspondencia con el mundo real | ✔ | ✔ | ✔ | ✔ |
| H3 Control y libertad | ✔ | ✔ | ✔ | ✔ |
| H4 Consistencia y estándares | ✔ | ✔ | ✔ | ✔ |
| H5 Prevención de errores | ✔ | ✔ | ✔ | ✔ |
| H6 Reconocimiento antes que recuerdo | ✔ | ✔ | ✔ | ✔ |
| H7 Flexibilidad y eficiencia | ✔ | ✔ | ✔ | ✔ |
| H8 Diseño estético y minimalista | ✔ | ✔ | ✔ | ✔ |
| H9 Recuperación de errores | ✔ (P/V) | ✔ | ✔ (parcial→P/V) | ✔ (0\*) |
| H10 Ayuda y documentación | ✔ | ✔ | ✔ | ✔ |

\* Alex marca con \* severidades provisionales basadas solo en la evidencia del pilotaje. P/V = pendiente de verificación, convención ya usada en Fase 1 y en la evaluación de Viviana.

**Resultado: 4/4 evaluadores × 10/10 heurísticas.** Se cumple el criterio de cobertura.

## 🧩 5. Agrupación de problemas equivalentes (trazabilidad individual → H-XX)

Los problemas se agruparon por equivalencia de componente y mecanismo, conservando la referencia exacta a cada documento individual. Ningún hallazgo individual se descartó.

| ID | Problema agrupado | Viviana | Wilson | Alex | Sebastián |
|---|---|---|---|---|---|
| H-01 | Acceso al pedido: ubicación no convencional (sin ícono en cabecera) | H4 (2) | HW-03 (2) | H4 (2); Hallazgos H03 (parte) | F3 H4/H6 (2) |
| H-02 | Retroalimentación poco perceptible al añadir (barra flotante) | H1 (2); EH-03 F3 (3) | HW-01 (2) | H1 (2); Hallazgos H03 (parte) | F3 H1 (2) |
| H-03 | Eliminación inmediata sin confirmación ni deshacer; control pequeño | H3/H5 (2); EH-04 F3 (4) | HW-02 (2) | H3 (2), H5 (2); Hallazgos H04 | F2 OBS-S01 → F3 H3/H5/H8 (2) |
| H-04 | «Añadir» directo no se diferencia de la personalización | H5 (2), H6 (1); EH-02 F3 (3) | HW-04 (1) | H2 (2), H6 (2); Hallazgos H02 | F3 H5/H6/H2 (2) |
| H-05 | Buscador de Inicio compite con el CTA «Ver Menú» | H8 (1); EH-01 F3 (2) | — (H8: 0) | H8 (1); Hallazgos H01 (2) | F3 H6/H8/H5 (2) |
| H-06 | Estado de carrito vacío no definido | H9 (P/V, lo lista como pregunta) | HW-05 (1) | H9 (0\*, recomienda probarlo) | F3 H9/H5 (1 diseño / P/V comportamiento) |
| H-07 | Secuencia de estados «Preparando… 50 %» → «¡Pedido recibido!» | — | — | — | F2 OBS-S02 → F3 H1/H2 (2 propuesta) |
| H-08 | «Total pagado» en Estado contradice el pago en caja | — | — | — | F3 H2/H4 (2 propuesta) |
| H-09 | Escenarios de error y recuperación no cubiertos | H9 (P/V) | H9 nominal satisfecha (su vacío concreto → H-06) | H9 (0\*, recomienda inspección) | F2 H9 parcial → F3 H9 (P/V) |
| H-10 | Inconsistencias menores (posición de marca; «Sanduches» sin tilde) | — | — | — | F3 H4 (1) |
| H-11 | Modal de cancelación: consecuencias no verificables en la evidencia | — | — | — | F2 OBS-S03 → F3 H3/H5/H9 (P/V) |
| H-12 | Confirmación sin tiempo estimado en la versión capturada | — | — | — | F3 H1/H10 (2 propuesta condicional) |

**Criterio de agrupación:** H-01 y H-02 se separaron porque, aunque ambos afectan la barra del carrito, son mecanismos distintos (ubicación/convención vs. retroalimentación de cambio) y requieren soluciones distintas; Wilson ya los había separado (HW-03 / HW-01) y Alex los agrupó en H03: la separación conserva toda la evidencia y permite priorizar por separado. H-06 se separó de H-09 porque el carrito vacío es un estado concreto no definido, mientras H-09 es el vacío general de cobertura de errores.

**Trazabilidad con Fase 2:** C01→H-01/H-02 · C02→H-03 · C03→H-04 · C04→H-05 · C05→H-06. CP-01→H-01 · CP-02→H-04 · CP-03→H-03 · CP-04→H-05 · CP-05→H-02 · CP-06→verificación de H-07 (ver triangulación).

## 📏 6. Severidades por evaluador y propuesta de consenso

Escala: 0 sin problema · 1 cosmético · 2 menor · 3 mayor · 4 crítico · P/V pendiente de verificación · NF = el evaluador no registró ese problema específico (no equivale a 0).

| ID | Viviana | Wilson | Alex | Sebastián (F3) | Propuesta de consenso | Estado del consenso |
|---|:--:|:--:|:--:|:--:|:--:|---|
| H-01 | 2 | 2 | 2 | 2 | **2** | Convergencia unánime 4/4 · pendiente ratificación grupal |
| H-02 | 2 en F2 / 3 en EH-03 | 2 | 2 | 2 | **2** | Discrepancia Viviana documentada; pendiente ratificación grupal |
| H-03 | 2 en F2 / 4 en EH-04 | 2 | 2 | 2 | **2** | Discrepancia Viviana documentada; pendiente ratificación grupal |
| H-04 | 2 (H5) / 1 (H6) / 3 (EH-02) | 1 | 2 | 2 | **2** | Discrepancias documentadas (§7.1) · pendiente ratificación |
| H-05 | 1 (H8) / 2 (EH-01) | 0 (NF) | 1 individual / 2 en Hallazgos | 2 | **2** | Discrepancia documentada (§7.2) · pendiente ratificación |
| H-06 | P/V | 1 | 0\* | 1 / P/V | **1** (diseño) | Convergencia parcial (§7.3) · comportamiento P/V |
| H-07 | NF | NF | NF | 2 | 2 (propuesta individual) | Hallazgo nuevo F3 · requiere contraste grupal |
| H-08 | NF | NF | NF | 2 | 2 (propuesta individual) | Hallazgo nuevo F3 · requiere contraste grupal |
| H-09 | P/V | — | 0\* | P/V | **P/V** | Vacío de cobertura · inspección de errores requerida |
| H-10 | NF | NF | NF | 1 | 1 (propuesta individual) | Hallazgo nuevo F3 · requiere contraste grupal |
| H-11 | NF | NF | NF | P/V | **P/V** | Limitación de evidencia · captura limpia requerida |
| H-12 | NF | NF | NF | 2 condicional | 2 (propuesta individual condicional) | Hallazgo nuevo F3 · depende de confirmar versión (L-01) |

### Justificación de las severidades propuestas (frecuencia · impacto · persistencia)

- **H-01 = 2.** Frecuencia: cada revisión del pedido desde el catálogo. Impacto: búsqueda adicional y demora leve, sin bloqueo (los cuatro evaluadores coinciden; el pilotaje lo confirmó con recuperación autónoma). Persistencia:_costo concentrado en primeros usos; se aprende. Recuperación inmediata → menor, no mayor.
- **H-02 = 2.** Frecuencia: cada adición. Impacto: duda sobre si el producto se agregó; no impide continuar. Persistencia: se repite en cada compra. La dinámica exacta no es verificable estáticamente; el realce visible es insuficiente por diseño → menor.
- **H-03 = 2.** Frecuencia: cada eliminación. Impacto: costo de recuperación (volver al catálogo y reconfigurar, perdiendo instrucciones especiales). Persistencia: no se mitiga con el aprendizaje. No se asigna 3 porque no se demostraron eliminaciones accidentales reales y la recuperación es sencilla; **cláusula de escalado:** si la verificación interactiva o una nueva prueba registra eliminaciones accidentales, reevaluar a 3.
- **H-04 = 2.** Frecuencia: cada personalización. Impacto: ruta equivocada + retroceso; riesgo de añadir sin la instrucción deseada. Persistencia: se aprende tras el primer uso. La mayoría (3/4) propone 2; ver discrepancia §7.1.
- **H-05 = 2.** Frecuencia: primer uso. Impacto: primer paso equivocado observable (no solo estético). Persistencia: de un solo uso. 2 y no 1 porque induce una acción errónea real; 2 y no 3 porque la recuperación es inmediata. Ver discrepancia §7.2.
- **H-06 = 1 (diseño), comportamiento P/V.** Frecuencia: ocasional. Impacto: desorientación potencial, no demostrada. Persistencia: estado no cubierto. Solo Wilson puntuó (1); Viviana y Alex lo dejaron como pregunta/insuficiencia de evidencia. No se convierte un 0\* («sin evidencia») en «sin problema».
- **H-07 = 2 (propuesta).** Frecuencia: cada pedido. Impacto: confusión sobre el estado real, sin bloqueo. Persistencia: estructural del flujo. Requiere que los demás evaluadores lo contrasten en el prototipo antes de ratificar.
- **H-08 = 2 (propuesta).** Frecuencia: cada pedido. Impacto: malentendido sobre dinero («ya me cobraron»), resoluble leyendo la confirmación. Persistencia: constante en P05 e inconsistente con P07. Sujeto a confirmación de versión.
- **H-09 = P/V.** No hay evidencia de comportamiento ante errores; asignar cualquier valor numérico sería inventar. Acción: inspección específica de estados de error.
- **H-10 = 1 (propuesta).** Frecuencia: cada navegación. Impacto: nulo sobre la tarea. Persistencia: constante. Cosmético por definición.
- **H-11 = P/V.** La evidencia está parcialmente oculta; no es evaluable hasta obtener captura limpia y recorrido interactivo.
- **H-12 = 2 (propuesta condicional).** Frecuencia: cada pedido. Impacto: el usuario no puede planificar el retiro sin preguntar (debilita el objetivo «sin comunicación verbal»); si el equipo pondera ese objetivo como esencial, podría justificarse 3 — punto explícito de discusión. Persistencia: constante. Depende de confirmar qué versión es la vigente (L-01).

## ⚖️ 7. Discrepancias documentadas

### 7.1 H-04 — Personalización: Wilson 1 vs. mayoría 2

- **Posición de Wilson (HW-04 = 1):** lo trata como detalle cosmético de etiquetado; la tarea se completa y la doble ruta es una fortaleza de eficiencia.
- **Posición de Viviana (H5 = 2), Alex (H2/H6 = 2) y Sebastián (2):** el problema indujo una ruta equivocada con retroceso (no solo estética) y puede hacer que un producto llegue sin la instrucción deseada.
- **Fundamento de la propuesta 2:** frecuencia media, impacto moderado (pasos extra + riesgo de perder la instrucción), persistencia aprendible. La evidencia de usuarios (P1, T3) apoya que es más que cosmético.
- **Resolución propuesta:** 2, registrando el voto minoritario de Wilson. Si la revisión grupal no logra acuerdo, se mantiene la discrepancia en la matriz con ambas posiciones (no se fuerza consenso).

### 7.2 H-05 — Buscador vs. CTA: 0/1 vs. 2

- **Posición de Wilson (H8 = 0, no lo registra):** su inspección consideró la pantalla de inicio limpia y jerarquizada.
- **Posición de Viviana y Alex en sus evaluaciones individuales (H8 = 1):** competencia visual menor.
- **Posición de Alex en Hallazgos_Preliminares (H01 = 2) y de Sebastián (2):** el elemento indujo un error de interacción real y recuperable en el pilotaje; un error observado supera lo cosmético.
- **Resolución propuesta:** 2, dejando constancia de las tres posiciones (0, 1, 2). Es la discrepancia mayor del conjunto y debe votarse en la revisión grupal.

### 7.3 H-06 — Carrito vacío: 1 vs. P/V vs. 0\*

- Wilson puntuó 1 (vacío de diseño). Viviana lo dejó como pregunta abierta (P/V). Alex marcó 0\* aclarando que significa *evidencia insuficiente*, no ausencia de problema.
- **Resolución propuesta:** 1 como vacío de diseño (no hay estado vacío en el flujo), con el comportamiento real P/V hasta verificarlo. Se explicita que el 0\* de Alex no se computa como «sin problema».

### 7.4 Hallazgos nuevos de F3 (H-07, H-08, H-10, H-12)

Solo Sebastián los ha evaluado, porque surgen del análisis de la captura con conexiones aportada en esta fase. **No se les asigna severidad consensuada**: quedan como propuestas individuales a la espera del contraste de los otros tres evaluadores en la revisión grupal. H-07, H-08 y H-12 dependen además de aclarar la versión del prototipo (L-01 en [soporte-tecnico-f3.md](soporte-tecnico-f3.md)).

### 7.5 Diferencia de alcance entre evaluaciones

Wilson evaluó con detalle el flujo nominal y parte del pilotaje; Viviana y Alex construyeron sus evaluaciones principalmente sobre los registros del pilotaje (ellos lo declaran); Sebastián F3 inspeccionó el diseño y el cableado de la captura. Esto explica por qué unos detectaron problemas de interacción observada y otros de diseño estático, y por qué H-09 quedó P/V para todos: nadie ha provocado aún un estado de error. La consolidación no homogeneiza artificialmente estos alcances: los registra.

## 🗓️ 8. Revisión grupal de severidades (proceso y acta)

**Regla aplicada:** no se asigna severidad consensuada sin comparación del equipo. La comparación documental (secciones 5–7) está completada por el responsable de consolidación; la ratificación requiere la sesión grupal.

### Agenda propuesta (30–40 min)

1. Verificar que los cuatro autores reconocen su documento como base válida (5 min).
2. Recorrer H-01…H-03: ratificar H-01; debatir las discrepancias de Viviana en H-02 y H-03 (5 min).
3. Debatir y votar H-04 (§7.1) y H-05 (§7.2) (10 min).
4. Contrastar en el prototipo los hallazgos nuevos H-07, H-08, H-10, H-12 y fijar severidad o dejarlos P/V (10 min).
5. Acordar responsable y fecha para las verificaciones de H-06, H-09, H-11 (5 min).
6. Registrar acuerdos y desacuerdos persistentes en el acta (5 min).

### Acta de ratificación (completar en la sesión)

| Campo | Registro |
|---|---|
| Fecha y hora | _Pendiente_ |
| Modalidad | _Pendiente_ |
| Asistentes (usuarios GitHub) | _Pendiente_ |
| H-01 / H-02 / H-03 ratificadas | _Pendiente_ |
| H-04 decisión y votos | _Pendiente_ |
| H-05 decisión y votos | _Pendiente_ |
| H-06 decisión | _Pendiente_ |
| H-07 / H-08 / H-10 / H-12 decisión | _Pendiente_ |
| Verificaciones asignadas (H-06, H-09, H-11) | _Pendiente_ |
| Discrepancias que persisten | _Pendiente_ |
| Responsable de actualizar la matriz | Sebastián Santana |

Una vez completada el acta, actualizar la columna «Estado del consenso» de la sección 6 y de [matriz-hallazgos.md](matriz-hallazgos.md), cambiando «pendiente ratificación» por «ratificado (acta del [fecha])». Mientras tanto, **ningún documento debe citar estas severidades como consensuadas en firme**.

## 📤 9. Entrega y consistencia de identificadores

- **A Alex (revisor):** esta consolidación + [matriz-hallazgos.md](matriz-hallazgos.md) para fundamentar los criterios técnicos del backlog.
- **A Viviana (conclusiones):** [triangulacion.md](triangulacion.md) con la clasificación de cada hallazgo.
- **Identificadores:** H-01…H-12 son los identificadores únicos y estables en los cuatro documentos de esta fase. Las referencias de Fase 2 (HW-xx, C0x, CP-0x, H0x de Hallazgos_Preliminares) se conservan únicamente como trazabilidad en la sección 5; ningún documento nuevo las usa como identificador principal.
- **Criterio de backlog:** solo se proponen para el backlog los hallazgos con evidencia suficiente (ver sección de prioridades en [matriz-hallazgos.md](matriz-hallazgos.md)); los P/V se proponen como tareas de verificación, no como correcciones.

## ✅ 10. Conclusión

Las cuatro evaluaciones independientes están disponibles y cubren las diez heurísticas, con alcance documental distinto. H-01 converge con severidad 2; H-02 y H-03 tienen propuestas 2 y discrepancias registradas de Viviana (3 y 4). Existen además discrepancias para H-04 y H-05, una convergencia parcial para H-06, dos vacíos P/V (H-09, H-11) y cuatro hallazgos nuevos de la inspección F3 que requieren contraste grupal (H-07, H-08, H-10, H-12). Ninguna propuesta se presenta como consenso hasta completar el acta de la sección 8.

---