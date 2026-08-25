# Plugins

Los índices, colas y repasos funcionan con Bases (nativo). Estos plugins comunitarios están instalados y configurados; cada uno resuelve una fricción concreta.

## Latex Suite (+ extensión)

Autocompletado de LaTeX mientras escribes. Lo esencial:

- `mk` abre matemática en línea `$...$`; `dm` abre bloque `$$...$$`.
- Dentro de matemáticas: `sr` → `^2`, `cb` → `^3`, un número tras una letra se hace subíndice (`x1` → `x_1`), `//` → fracción, `@a` → `\alpha`.
- `Tab` salta fuera de llaves y paréntesis.

La extensión añade además cierre automático de `$` y estilo display en línea. El cambio automático de teclado viene desactivado (está pensado para hebreo y árabe).

## Templater

Motor de las plantillas. Configurado con carpeta `90 Plantillas`.

- Insertar plantilla en la nota activa: `Cmd+P` → **Templater: Open insert template modal**.
- Las plantillas rellenan solas `fecha`, `proxima_revision` (mañana, el primer peldaño real) y los títulos de los callouts.
- Excepción: `Plantilla - Sesión de estudio` usa sintaxis `{{date}}` porque la procesa el plugin de notas diarias del núcleo. No la conviertas a sintaxis Templater.
- El plugin de plantillas del núcleo está desactivado para que solo haya una vía de inserción.

## Spaced Repetition

Tarjetas con LaTeX para micro-recuerdo (fórmulas, hipótesis, definiciones cortas). La escalera de `proxima_revision` sigue siendo el sistema principal para reconstrucción completa; las tarjetas la complementan, no la sustituyen.

- En cualquier nota, añade `#flashcards/ALG1` (el sufijo crea el mazo de la asignatura) y escribe tarjetas: `pregunta::respuesta`, o cierre `la identidad es ==única==`.
- Repasar: `Cmd+P` → **Spaced Repetition: Review flashcards**, botones Otra vez / Difícil / Bien / Fácil.
- Ignora `90 Plantillas` y `99 Adjuntos`. La revisión de notas por etiqueta `#review` no se usa: para eso está la escalera.

## Excalidraw

Dibujos para geometría, diagramas de dependencias y esquemas de demostraciones.

- Crear: `Cmd+P` → **Excalidraw: Create new drawing**.
- Los dibujos se guardan en `99 Adjuntos/Excalidraw` y se incrustan con `![[nombre del dibujo]]`.

## Regla

Antes de instalar otro plugin: que duela su ausencia. Cada plugin añade mantenimiento.
