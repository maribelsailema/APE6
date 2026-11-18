# Backlog de mejoras – CaféU | APE 6 Fases 3 y 4

**Responsable de consolidación:** Sarco Sailema Viviana Maribel  
**Base:** Hallazgos de pilotaje (H01–H04) + evaluación heurística individual (HV-01–HV-08)  
**Estado:** Propuestas priorizadas. Las Issues de GitHub se crearán una vez consolidados los resultados de Fase 3.

---

## Prioridades

| Prioridad | Significado |
|-----------|-------------|
| P1 | Alta – afecta control, feedback o descubrimiento frecuente |
| P2 | Media – mejora claridad y reduce errores no críticos |
| P3 | Media-baja – refinamiento de jerarquía visual |
| P4 | Baja / exploración – mejoras de robustez y escenarios de error |

---

## Lista priorizada

### P1 – Alta

| ID Mejora | Descripción | Hallazgo / Heurística | Criterio técnico | Issue prevista |
|-----------|-------------|------------------------|------------------|----------------|
| M-01 | Añadir feedback visible al actualizar el carrito (animación o badge) | H03 / HV-01 (H1) | C-01: El cambio de cantidad/total debe percibirse en < 1 s | Issue # (por crear) |
| M-02 | Incorporar «Deshacer» tras eliminar un ítem (snackbar 5–8 s) | H04 / HV-02 (H3, H5) | C-02: El usuario puede recuperar el ítem eliminado sin volver al menú | Issue # (por crear) |
| M-03 | Añadir acceso al carrito también en la cabecera | H03 / HV-03 (H4) | C-03: Existe al menos un acceso visible en la zona superior | Issue # (por crear) |

### P2 – Media

| ID Mejora | Descripción | Hallazgo / Heurística | Criterio técnico | Issue prevista |
|-----------|-------------|------------------------|------------------|----------------|
| M-04 | Diferenciar claramente «Añadir» de «Personalizar / Ver opciones» | H02 / HV-04, HV-05 (H5, H6) | C-04: Productos personalizables muestran etiqueta visible de personalización | Issue # (por crear) |
| M-05 | Ampliar área táctil del control «Eliminar» | H04 / HV-07 | C-05: Área mínima táctil acorde a buenas prácticas móviles | Issue # (por crear) |

### P3 – Media-baja

| ID Mejora | Descripción | Hallazgo / Heurística | Criterio técnico | Issue prevista |
|-----------|-------------|------------------------|------------------|----------------|
| M-06 | Reforzar jerarquía visual del CTA «Ver Menú» frente al buscador | H01 / HV-06 (H8) | C-06: El CTA principal es el elemento más destacado de la pantalla de inicio | Issue # (por crear) |

### P4 – Baja / exploración

| ID Mejora | Descripción | Hallazgo / Heurística | Criterio técnico | Issue prevista |
|-----------|-------------|------------------------|------------------|----------------|
| M-07 | Definir y mostrar mensajes de error y recuperación (carrito vacío, cancelación, fallo de confirmación) | HV-08 (H9) | C-07: Todo estado de error muestra mensaje + acción de recuperación | Issue # (por crear) |
| M-08 | Verificar y, si es necesario, completar el recorrido de cancelación (T7) en el prototipo | T7 / H3, H5, H9 | C-08: El flujo de cancelación es ejecutable y observable de extremo a extremo | Issue # (por crear) |

---

## Trazabilidad

Cada Issue de GitHub deberá incluir en su descripción:

- Referencia al hallazgo (H-XX o HV-XX).
- Referencia al criterio técnico (C-XX).
- Prioridad (P1–P4).
- Evidencia (participante, tarea o pantalla).
- Estado: propuesta (no implementada todavía).

---

## Nota metodológica

Las mejoras listadas son **propuestas** derivadas de evidencia de Fase 2 y de la inspección heurística individual. No se ha realizado aún una nueva prueba de usabilidad que demuestre su efecto. La Fase 4 debe mantener esta distinción clara entre hallazgos observados y mejoras solo propuestas.