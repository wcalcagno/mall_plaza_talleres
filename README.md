# La licitación con trampas

Ejercicio grupal de criterio y validación con IA · Sesión 3 · Programa Liderazgo y Gestión Estratégica con IA · Mallplaza

> **Aviso.** Todos los documentos de este repositorio son **ficticios y de uso exclusivamente formativo**. Los nombres de empresas, cifras, fechas y hechos no corresponden a procesos reales de licitación ni a resultados reales de medición.

---

## Propósito

Entrenar la competencia central de la Sesión 3: **un líder no produce el output con IA, lo valida**. Los participantes generan una recomendación ejecutiva con IA a partir de un set de documentos que contiene defectos plantados deliberadamente, y luego auditan el output de otro grupo aplicando el Checklist de Validación de 7 puntos.

El set contiene **9 trampas**: cifras contradictorias entre documentos, inconsistencias internas, normativa obsoleta, supuestos sin respaldo, un dato prestigioso inventado, una métrica mal interpretada, una fecha errónea, una omisión crítica y un error aritmético en la fuente "oficial".

---

## Contenido del repositorio

| Archivo | Descripción | ¿Quién lo recibe? |
|---|---|---|
| `Doc_A_Bases_Licitacion_LP-2026-041.docx` | Bases administrativas y técnicas. Es la "verdad de terreno" del ejercicio. | Participantes |
| `Doc_B_Propuesta_Limpex.docx` | Propuesta técnica y económica del proveedor ficticio. Contiene 8 de las 9 trampas. | Participantes |
| `Doc_C_Reporte_NPS_Q1_2026.docx` | Reporte de experiencia del visitante. Contiene 1 trampa interna. | Participantes |
| `Doc_D_Pauta_Facilitador_CONFIDENCIAL.docx` | Ubicación exacta de las 9 trampas, puntajes, falsos positivos esperables y guion de tiempos. | **Solo facilitadores** |

> ⚠️ **Doc D es confidencial.** Si los participantes tendrán acceso a este repositorio, muévanlo a un repositorio privado separado o a una carpeta con acceso restringido. Publicar la pauta invalida el ejercicio.

---

## Requisitos previos

- Cuenta Google con acceso a [NotebookLM](https://notebooklm.google.com) y [Gemini](https://gemini.google.com).
- Grupos de 4 a 6 personas, cada grupo con al menos un computador con proyección o pantalla compartida.
- Los 3 documentos (A, B y C) descargados localmente por cada grupo antes de iniciar.
- El facilitador debe haber leído la pauta (Doc D) completa antes de la sesión.

---

## Mecánica del ejercicio (50–60 minutos)

### Fase 1 · Carga de fuentes en NotebookLM (8 min)

1. Cada grupo crea un notebook nuevo en NotebookLM.
2. Carga los 3 documentos como fuentes: `Doc_A`, `Doc_B` y `Doc_C`.
3. Verifica que las 3 fuentes aparezcan indexadas y activas.

### Fase 2 · Generación de la recomendación ejecutiva (10 min)

Cada grupo pide a la IA una **recomendación de adjudicación** (aceptar, rechazar o condicionar la propuesta de Limpex). Prompt sugerido:

```
Actúa como analista de procurement de Mallplaza Egaña. A partir de las
tres fuentes cargadas (bases de licitación, propuesta del proveedor y
reporte NPS), redacta una recomendación ejecutiva de máximo una página
para el comité de adjudicación de la Licitación LP-2026-041.

Debe incluir: (1) resumen de la propuesta, (2) fortalezas, (3) riesgos,
(4) recomendación final fundada (adjudicar, rechazar o condicionar).
Usa un tono ejecutivo y cita las cifras relevantes.
```

4. El grupo exporta o copia el output generado. **No lo audita todavía.**

### Fase 3 · Intercambio y auditoría adversarial (22 min)

1. Los grupos intercambian outputs según el esquema que indique el facilitador (nadie audita el propio).
2. El grupo auditor aplica el **Checklist de Validación de 7 puntos** (Fuentes, Omisiones, Supuestos, Cifras, Contexto Mallplaza, Tono vs. fondo, Firma).
3. Cada afirmación relevante del output se clasifica en una de tres categorías:
   - **Trazable**: respaldada por las fuentes, cita verificada.
   - **Inventada**: no existe en ninguna fuente.
   - **Trazable a fuente contaminada**: la cifra existe, pero está mal usada, contradicha por otra fuente o es internamente inconsistente.
4. Uso recomendado de NotebookLM en la auditoría: hacer clic en cada cita para verificar que la fuente **dice lo que el output afirma**, y hacer preguntas directas del tipo "¿en qué fuente aparece el Ranking de Proveedores?" para detectar lo inventado.
5. El grupo auditor entrega un veredicto escrito: lista de hallazgos con su clasificación y la evidencia (documento y sección).

### Fase 4 · Puesta en común y puntajes (12 min)

El facilitador revela las 9 trampas usando la pauta (Doc D) y asigna puntajes por grupo.

### Fase 5 · Cierre (5 min)

Pregunta de cierre para cada grupo: *¿qué habría pasado si esta recomendación se firmaba sin auditar?* Vincular cada trampa encontrada (y las no encontradas) con el punto del checklist correspondiente.

---

## Sistema de puntajes

| Resultado | Puntos |
|---|---|
| Trampa detectada y explicada con la contradicción exacta | **+10** |
| Trampa detectada sin explicar la contradicción | **+5** |
| Falso positivo (acusar algo que las fuentes sí respaldan) | **−5** |

- Puntaje máximo: **90 puntos**.
- Desempeño sobresaliente: 6 o más trampas sin falsos positivos.
- La penalización por falso positivo es deliberada: instala el hábito de **verificar antes de acusar**, que es exactamente el criterio que la sesión busca desarrollar.

---

## Variante con Gems (opcional, +20 min)

Si el grupo avanza rápido o se dispone de tiempo adicional:

1. Cada grupo crea una **Gema "Auditor Mallplaza"** en Gemini, cuyas instrucciones incluyen el Checklist de 7 puntos y el contexto del negocio.
2. Se le entrega el output del otro grupo y se compara la auditoría de la Gema contra la auditoría humana.
3. Discusión: ¿qué objeciones de la Gema son válidas, cuáles genéricas y cuáles alucinadas? La conclusión esperada: **un Gem con buenas instrucciones sigue necesitando firma humana** (validación de segundo orden, puente directo a la Sesión 4).

---

## Notas para el facilitador

- Las trampas 6 (métrica cruzada) y 8 (omisión de garantías) son las más difíciles y las que mejor conversación generan. Reservar tiempo para ellas en la puesta en común.
- La lista de **falsos positivos esperables** de la pauta es tan importante como las trampas: ahí se juega la diferencia entre criterio y sospecha genérica.
- Si un grupo termina la Fase 2 muy rápido, pedirle un segundo formato con el mismo set (FAQ o resumen para gerencia) para reforzar el patrón "una fuente, varios productos verificables".
- Mensaje de cierre de la sesión: **la IA acelera, el criterio firma**.

---

## Licencia y uso

Material desarrollado para el Programa Liderazgo y Gestión Estratégica con IA (Mallplaza). Uso interno del equipo docente. No redistribuir fuera del programa sin autorización.
