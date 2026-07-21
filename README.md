# AI-Course-Flipped-Class

Cadena de **prompts** para rediseñar un sílabo universitario aplicando **Flipped
Classroom (aula invertida) y aprendizaje activo**, con ayuda de un asistente de IA que
actúa como diseñador instruccional. Caso de trabajo: la materia de **Álgebra Lineal**.

La IA no reemplaza la decisión académica del docente: no inventa información fuera de
los archivos, señala inconsistencias y marca todo lo que requiere verificación docente.

## Ramas

- **`main`** — solo los prompts y el material básico de entrada. Punto de partida
  limpio para aplicar el método a cualquier sílabo.
- **`ejemplos`** — lo mismo que `main` **más** los archivos ya corridos de ejemplo
  (`04_trabajo_generado/`): diagnóstico, resultados de aprendizaje, plan de unidad,
  materiales previos, actividad presencial, checklist y el sílabo rediseñado en `.docx`.

## Estructura

```
INSTRUCCIONES.md        # "Constitución" del proyecto: rol de la IA, criterios y formato de salida
01_contexto/            # Sílabo base a rediseñar (insumo principal)
02_referencias/         # Sílabo modelo con estructura antes/durante/después de clase
03_banco_preguntas/     # Ejemplo de formato de evaluación (no es contenido de la materia)
04_trabajo_generado/    # Salidas generadas por la IA (con contenido en la rama `ejemplos`)
  └── sesiones/         # Clases desarrolladas sesión por sesión (sesion_NN.md)
05_Prompts/             # La cadena de prompts (01 → 09)
```

## La cadena de prompts (`05_Prompts/`)

| # | Prompt | Salida |
|---|--------|--------|
| 01 | Inventario y reconocimiento de archivos | — |
| 02 | Diagnóstico del sílabo | `diagnostico.md` |
| 03 | Resultados de aprendizaje (3 versiones) | `resultados_aprendizaje.md` |
| 04 | Selección de unidad y mapa de secuenciación/evaluación | `mapa_unidad_evaluacion.md` |
| 05 | Plan de unidad con Flipped Classroom | `plan_unidad.md` |
| 06 | Guía de estudio previo (con recurso video/paper/práctica) | `materiales_previos.md` |
| 07 | Actividad presencial (aprendizaje activo) | `actividad_presencial.md` |
| 08 | Revisión crítica / control de calidad | — |
| 09 | **Generador de clase por sesión** (guion minuto a minuto) | `sesiones/sesion_NN.md` |

## Cómo usarlo

1. Coloca tu sílabo base en `01_contexto/` y ejecuta los prompts en orden (`01` → `09`).
2. Los prompts `06` y `09` buscan en internet el recurso previo (video, paper o
   práctica) y lo verifican, por lo que conviene ejecutarlos en un entorno con acceso
   web (p. ej. Claude Code o Claude con búsqueda web).
3. Todo enlace externo se marca con `⚠ requiere verificación docente`.
