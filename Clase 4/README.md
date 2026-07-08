# Ejercicios grupales con IA · Sesiones 3 y 4

Programa Liderazgo y Gestión Estratégica con IA · Mallplaza

> **Aviso.** Todos los documentos de este repositorio son **ficticios y de uso exclusivamente formativo**. Los nombres de empresas, personas, cifras, fechas y hechos no corresponden a procesos reales.

---

## Estructura del repositorio

```
/sesion-3-licitacion-con-trampas/
    Doc_A_Bases_Licitacion_LP-2026-041.docx
    Doc_B_Propuesta_Limpex.docx
    Doc_C_Reporte_NPS_Q1_2026.docx
/sesion-4-instalar-ia-en-el-equipo/
    Doc_F_Cuaderno_Trabajo_Equipo_S4.docx
    Doc_G1_Formato_Estandar_Minuta.docx
    Doc_G2_Politica_Reuniones_Minutas.docx
    Doc_G3_Ejemplo_Minuta_Publicable.docx
    Doc_H_Transcripcion_Prueba.docx
/facilitadores/          <- repositorio o carpeta PRIVADA, solo equipo docente
    Doc_D_Pauta_Facilitador_CONFIDENCIAL.docx
    Doc_E_Guia_Facilitador_S4_CONFIDENCIAL.docx
```

> ⚠️ **Los Docs D y E son confidenciales.** Contienen las trampas plantadas, los desafíos de la transcripción y las rúbricas. Si los participantes tendrán acceso a este repositorio, los documentos de facilitación deben vivir en un repositorio privado separado. Publicarlos invalida ambos ejercicios.

---

# Sesión 3 · La licitación con trampas

**Competencia:** un líder no produce el output con IA, lo valida.
**Duración:** 50–60 minutos · **Herramientas:** NotebookLM + Gemini.

Los participantes generan una recomendación de adjudicación con IA a partir de un set de documentos que contiene **9 defectos plantados** (cifras contradictorias, normativa obsoleta, supuestos sin respaldo, datos inventados, métricas mal interpretadas, omisiones críticas), y luego auditan el output de otro grupo con el Checklist de Validación de 7 puntos.

## Mecánica

### Fase 1 · Carga de fuentes en NotebookLM (8 min)
1. Cada grupo crea un notebook nuevo y carga las 3 fuentes: `Doc_A`, `Doc_B` y `Doc_C`.
2. Verifica que las 3 fuentes aparezcan indexadas y activas.

### Fase 2 · Generación de la recomendación ejecutiva (10 min)
Prompt sugerido para Gemini/NotebookLM:

```
Actúa como analista de procurement de Mallplaza Egaña. A partir de las
tres fuentes cargadas (bases de licitación, propuesta del proveedor y
reporte NPS), redacta una recomendación ejecutiva de máximo una página
para el comité de adjudicación de la Licitación LP-2026-041.

Debe incluir: (1) resumen de la propuesta, (2) fortalezas, (3) riesgos,
(4) recomendación final fundada (adjudicar, rechazar o condicionar).
Usa un tono ejecutivo y cita las cifras relevantes.
```

El grupo copia el output generado. **No lo audita todavía.**

### Fase 3 · Intercambio y auditoría adversarial (22 min)
1. Los grupos intercambian outputs (nadie audita el propio).
2. El grupo auditor aplica el **Checklist de 7 puntos** (Fuentes, Omisiones, Supuestos, Cifras, Contexto Mallplaza, Tono vs. fondo, Firma) y clasifica cada afirmación en:
   - **Trazable** · respaldada por las fuentes, cita verificada.
   - **Inventada** · no existe en ninguna fuente.
   - **Trazable a fuente contaminada** · la cifra existe, pero está mal usada o contradicha.
3. Uso clave de NotebookLM: hacer clic en cada cita para verificar que la fuente **dice lo que el output afirma**, y preguntar directamente por los datos sospechosos.
4. Veredicto escrito: hallazgos, clasificación y evidencia (documento y sección).

### Fase 4 · Puesta en común (12 min) y Fase 5 · Cierre (5 min)
El facilitador revela las 9 trampas con la pauta (Doc D) y asigna puntajes. Pregunta de cierre: *¿qué habría pasado si esta recomendación se firmaba sin auditar?*

## Puntajes

| Resultado | Puntos |
|---|---|
| Trampa detectada y explicada con la contradicción exacta | **+10** |
| Trampa detectada sin explicar la contradicción | **+5** |
| Falso positivo (acusar algo que las fuentes sí respaldan) | **−5** |

Máximo 90 puntos. La penalización por falso positivo instala el hábito central: **verificar antes de acusar**.

---

# Sesión 4 · Instalar IA en el equipo

**Competencia:** instalar IA no es repartir accesos, es un trabajo de diseño.
**Duración:** 75 minutos · **Herramientas:** NotebookLM + Gemini con Gems.

Cada equipo rediseña un proceso semanal real y construye el sistema mínimo completo: **Definition of Done** en criterios verificables, **Gema operativa** que la lleva embebida, **repositorio del equipo** en NotebookLM y **Operating Rhythm** con dueños y métricas. El Cuaderno de Trabajo (`Doc_F`) guía las 6 fases con plantillas.

## Mecánica (6 fases)

| Fase | Contenido | Tiempo |
|---|---|---|
| 1 · Elegir y mapear | Proceso semanal real, en 4 a 7 pasos | 10 min |
| 2 · Clasificar | Cada paso: agente, asistente o aplicativo (regla del 80%) | 10 min |
| 3 · Definition of Done | 5 a 8 criterios binarios, verificables por un tercero | 15 min |
| 4 · Construir el sistema | Gema con la DoD embebida + repositorio NotebookLM (Docs G1–G3 o documentos propios) | 15 min |
| 5 · Prueba de fuego cruzada | El grupo vecino evalúa el output **solo contra la DoD escrita** | 15 min |
| 6 · Operating Rhythm y medición | Ritos con dueño, línea base y metas a 90 días | 10 min |

## La prueba de fuego (Fase 5)

1. Cada grupo corre su Gema con la **transcripción de prueba** (`Doc_H`, simula la salida de Granola) o con un input real de su proceso.
2. Entrega al grupo vecino solo dos cosas: el output y su Definition of Done. Sin explicaciones verbales.
3. El evaluador emite veredicto por criterio: **PASA**, **NO PASA** o **NO PUEDO DECIDIR**.
4. Regla de oro: todo "no puedo decidir" significa que el criterio está mal escrito. Se reescribe en la misma sesión y se vuelve a someter.

La transcripción contiene **3 desafíos plantados** (documentados en la guía del facilitador, Doc E) que ponen a prueba tanto a la Gema como a la Definition of Done del grupo.

## Puntajes

| Resultado | Puntos |
|---|---|
| Criterio de la DoD propia aplicable por el evaluador sin preguntar | **+5** |
| Desafío de la transcripción resuelto correctamente por la Gema | **+10** |
| Criterio con veredicto "no puedo decidir" | **−5** (recuperable si se reescribe bien) |
| Información confidencial incluida en la minuta | **−10** |

---

## Requisitos previos (ambas sesiones)

- Cuenta Google con acceso a [NotebookLM](https://notebooklm.google.com) y [Gemini](https://gemini.google.com), con permisos para crear Gems.
- Grupos de 4 a 6 personas, cada grupo con al menos un computador.
- Documentos de la sesión descargados localmente por cada grupo antes de iniciar.
- El facilitador debe haber leído la guía confidencial correspondiente (Doc D o Doc E) completa antes de la sesión.

## Hilo conductor entre sesiones

El checklist de validación de S3 es el **criterio individual**; la Definition of Done, la Gema y el Operating Rhythm de S4 son ese criterio convertido en **estándar del equipo**. Hacerlo explícito en el cierre de S4 es el mensaje central del programa: **la IA acelera, el criterio firma**.

## Licencia y uso

Material desarrollado para el Programa Liderazgo y Gestión Estratégica con IA (Mallplaza). Uso interno del equipo docente. No redistribuir fuera del programa sin autorización.
