---
tipo: manual
tags:
  - inicio
---

# Manual de uso

Cómo se trabaja en este vault, paso a paso. La teoría del método está en [[00 Inicio/Sistema de estudio|Sistema de estudio]] y el uso de la IA en [[00 Inicio/IA como tutor matemático|IA como tutor matemático]]; esto es el manual de operaciones.

> [!abstract] La idea en una frase
> Capturas en clase, conviertes lo importante en notas atómicas con propiedades bien rellenadas, y los paneles te dicen cada día qué repasar, qué vaciar y qué repetir. Tú solo escribes notas y actualizas propiedades: las tablas se mantienen solas.

## Los cinco flujos

### 1. En clase

1. Crea la nota en `06 Clases` y ponle nombre; después `Cmd+P` → **Templater: Open insert template modal** → `Plantilla - Clase`. (Así se insertan todas las plantillas, salvo la sesión de estudio, que crea sola el botón de nota diaria.)
2. Nómbrala `AAAA-MM-DD - ASIG - tema` y rellena la propiedad `asignatura` con el código (`ALG1`, `ANA1`, `NUM`, `GEO1`, `ANA2`).
3. Captura sin obsesionarte con el orden: definiciones, ejemplos, dudas, indicaciones del profesor.
4. Al cerrar, escribe de memoria las tres ideas principales (la plantilla lo pide al final).

### 2. Después de clase, antes de 24 h: vaciar

1. Abre la clase pendiente desde la vista **Por vaciar** de [[06 Clases/Clases.base|Clases]].
2. Cada idea reusable se convierte en nota atómica con su plantilla: conceptos en `03 Conceptos`, teoremas en `04 Teoremas y demostraciones`, problemas en `05 Problemas`. No extraigas cada frase.
3. Rellena `asignatura` con uno o varios códigos. Usa una lista cuando la idea sea compartida, por ejemplo `[ALG1, ANA1]`.
4. Decide si merece repaso espaciado: conceptos y teoremas nucleares, definiciones precisas, resultados reutilizables y errores conceptuales llevan `repasar: true`; notas de referencia, índices y material meramente consultivo no.
5. Si `repasar: true`, conserva el nivel 0 y la revisión de mañana. Escribe las preguntas de recuperación que usarás sin mirar.
6. Cambia el `estado` de la nota de clase a `vaciada`.

### 3. Repaso diario, 10-20 minutos

1. Abre [[00 Inicio/Inicio|Inicio]]: la tabla **Repasos de hoy** lista lo que vence.
2. Nota por nota, recupera **sin mirar**: responde las preguntas de recuperación, reconstruye la demostración o repite el problema.
3. Después de mirar, registra tú el resultado y actualiza las propiedades de la escalera:

| Resultado | Acción manual |
|---|---|
| Preciso y sin apoyo | Pon `ultima_revision` en hoy, decide `confianza`, avanza un nivel y calcula `proxima_revision` con el nuevo intervalo. |
| Idea bien, precisión mal | Pon `ultima_revision` en hoy, usa `ámbar` y conserva o reduce el nivel según el fallo. |
| No puedo reconstruirlo | Pon `ultima_revision` en hoy, usa `rojo`, vuelve a nivel 0 y programa mañana. |

4. Los niveles 0–6 equivalen a 1, 3, 7, 21, 45, 90 y 180 días. `estado: dominado` nunca es automático: úsalo solo cuando cumpla el criterio de dominio del sistema.

### 4. Problemas

1. Crea el problema con `Plantilla - Problema`, nombre `ASIG - TNN - PNN - descripción breve`.
2. Intenta antes de pedir pistas; registra el bloqueo concreto en la nota.
3. Mueve `estado` según avanza: `pendiente` → `en_curso` → `resuelto`, o `repetir` si la idea no salió sola.
4. Un problema nace con `repasar: false`. Si debe repetirse, cambia a `estado: repetir`, `repasar: true` y pon `proxima_revision`; solo entonces entra en Repasos.
5. Cuando deje de necesitar repetición, decide si vuelve a `resuelto` con `repasar: false`.
6. Si el fallo revela un patrón, añade una fila al [[05 Problemas/Registro de errores|Registro de errores]] con su regla correctiva.

### 5. Revisión semanal, 30-45 minutos

1. El mismo día cada semana, abre [[07 Revisiones/Revisiones|Revisiones]] y pasa el checklist.
2. Crea la nota de la semana con `Plantilla - Revisión semanal`: semáforos por asignatura, errores recurrentes y un máximo de tres prioridades.

## Mapa del vault

| Carpeta | Qué vive ahí |
|---|---|
| `00 Inicio` | Este manual, el método, las convenciones y el panel de inicio |
| `01 Grado` | Plan del grado y del curso actual |
| `02 Asignaturas` | Una página por asignatura, con su material autogenerado |
| `03 Conceptos` | Una nota por concepto |
| `04 Teoremas y demostraciones` | Una nota por resultado importante |
| `05 Problemas` | Banco de problemas y registro de errores |
| `06 Clases` | Notas de clase, a la espera de ser vaciadas |
| `07 Revisiones` | Cola de repasos diarios e historial semanal |
| `08 Recursos` | Bibliografía y fuentes oficiales |
| `09 Diario` | Sesiones de estudio (nota diaria) |
| `90 Plantillas` | Las plantillas de todo lo anterior |
| `99 Adjuntos` | Imágenes y archivos |

## Propiedades que mueven el sistema

Los paneles filtran por estas propiedades. Si una propiedad está mal escrita, la nota no aparece donde debe.

| Propiedad | Valores | Qué controla |
|---|---|---|
| `tipo` | `concepto`, `teorema`, `problema`, `clase`, `sesion`, `experimento_numerico` | En qué paneles aparece la nota |
| `asignatura` | un código o lista de `ALG1`, `ANA1`, `NUM`, `GEO1`, `ANA2` | Las páginas de asignatura que la recogen |
| `estado` | notas: `borrador`, `en_progreso`, `revisar`, `dominado` · problemas: `pendiente`, `en_curso`, `repetir`, `resuelto` · clases: `capturada`, `vaciada` | La cola en la que está |
| `confianza` | `rojo`, `ámbar`, `verde` | El semáforo de dominio |
| `repasar` | `true`, `false` | Si la nota puede entrar en la escalera |
| `nivel_revision` | entero de `0` a `6` | El intervalo 1, 3, 7, 21, 45, 90 o 180 días |
| `ultima_revision` | fecha `AAAA-MM-DD` o vacía | Cuándo se hizo la última recuperación |
| `proxima_revision` | fecha `AAAA-MM-DD` | El día que reaparece en los repasos |

> [!warning] Los valores se escriben exactos
> Minúsculas, sin espacios extra y tal cual aparecen en la tabla (`ámbar` con tilde). Los paneles comparan por igualdad literal: `Rojo` o `en curso` no cuentan.

## Entornos matemáticos (callouts)

Los enunciados se escriben en callouts, como los entornos de LaTeX. Sintaxis: `> [!nombre] Título` y el contenido en líneas que empiezan por `>`. Pon siempre título.

> [!definicion] Grupo
> Un conjunto $G$ con una operación $\cdot : G \times G \to G$ asociativa, con elemento neutro y donde todo elemento tiene inverso.

> [!teorema] Lagrange
> Si $H$ es subgrupo de un grupo finito $G$, entonces $|H|$ divide a $|G|$.

> [!demostracion]
> Las clases laterales de $H$ particionan $G$ y todas tienen cardinal $|H|$.

> [!ejemplo] El círculo unidad
> $(S^1, \cdot)$ con la multiplicación compleja es un grupo.

> [!contraejemplo] Sin asociatividad no hay grupo
> $(\mathbb{Z}, -)$ no es un grupo: $(1-1)-1 \neq 1-(1-1)$.

> [!intuicion] Idea
> Un grupo es la abstracción de "las simetrías de algo".

Tipos disponibles: `definicion`, `teorema`, `lema`, `proposicion`, `corolario`, `demostracion` (cierra con ∎ automático), `ejemplo`, `contraejemplo`, `intuicion`, `estrategia`, `pista`, `problema`, `error`. Se escriben sin tilde.

> [!tip] Truco de autoexamen
> Un callout con `-` tras el corchete nace plegado: `> [!demostracion]- ...`. Pliega la demostración, intenta reconstruirla de memoria y despliega para comparar. Vale también para enunciados y definiciones.

## Escribir rápido

- **LaTeX**: `mk` abre `$...$`, `dm` abre `$$...$$`; dentro, `sr` → `^2`, `x1` → `x_1`, `//` → fracción, `@a` → `\alpha`, `Tab` salta fuera de las llaves. Atajos completos en [[00 Inicio/Plugins|Plugins]].
- **Tarjetas**: añade `#flashcards/ALG1` a una nota y escribe `pregunta::respuesta`. Repaso con `Cmd+P` → **Review flashcards**. Para micro-recuerdo; la reconstrucción completa va por la escalera.
- **Dibujos**: `Cmd+P` → **Excalidraw: Create new drawing**; se guardan en `99 Adjuntos/Excalidraw` y se incrustan con `![[nombre]]`.

## Trabajar con el agente

El agente conoce el vault por su `AGENTS.md` y sigue el contrato de [[00 Inicio/IA como tutor matemático|IA como tutor matemático]]: ejecuta primero el auditor determinista, no te hace el trabajo, no te sube semáforos y te obliga a recuperar antes de mirar. Las automatizaciones diarias y semanales solo informan; nunca escriben notas ni propiedades. Peticiones que sabe atender:

- **«¿Qué me toca hoy?»** — el parte del día: repasos vencidos, clases sin vaciar, notas sin fecha de repaso, rojos acumulados y fechas de examen próximas, con recomendación de por dónde empezar.
- **«Explícame [concepto], con un dibujo»** — explicación completa (definición, intuición, ejemplo, contraejemplo) con gráfica, esquema Mermaid o interactivo, y preguntas de recuperación al final.
- **«Ponme cinco problemas de [tema]»** — ejercicios graduados con las soluciones plegadas.
- **«Simulacro de [asignatura], 90 minutos»** — examen realista en tu carpeta de asignatura; lo corriges con él y los errores van al registro.
- **«Corrige mi demostración»** — señala el primer salto no justificado y te deja corregirlo a ti.
- **«Audita el vault»** — propiedades mal escritas, notas sin `proxima_revision`, enlaces rotos.

## Los paneles

| Panel | Dónde | Qué muestra |
|---|---|---|
| [[07 Revisiones/Repasos.base\|Repasos]] | Inicio y Revisiones | **Para hoy** (vencidos), **Próximos 7 días**, **En rojo**, **Sin programar** |
| [[03 Conceptos/Conceptos.base\|Conceptos]] | Índice de conceptos | Por asignatura, bandeja de entrada, semáforo |
| [[04 Teoremas y demostraciones/Teoremas.base\|Teoremas]] | Índice de teoremas | Por asignatura, pendientes de dominar, semáforo |
| [[05 Problemas/Problemas.base\|Problemas]] | Banco de problemas | Las colas por `estado` |
| [[06 Clases/Clases.base\|Clases]] | Carpeta de clases | Por vaciar y todas |
| [[02 Asignaturas/Material.base\|Material]] | Cada asignatura | Solo el material de esa asignatura, por tipo |

## Si una nota no aparece en un panel

1. Revisa `tipo`: es el filtro principal y va en minúsculas.
2. Revisa el valor exacto de `estado`, `confianza` o `asignatura` contra la tabla de arriba.
3. Si no sale en los repasos, comprueba `repasar`. En problemas, además debe tener `estado: repetir`.
4. Si es elegible pero no tiene fecha, aparecerá en **Sin programar**.
