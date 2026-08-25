# Convenciones

## Nombres

- Concepto: `Nombre del concepto`.
- Teorema: `Teorema de ...` o el nombre descriptivo usado en clase.
- Problema: `ASIG - TNN - PNN - descripción breve`.
- Clase: `AAAA-MM-DD - ASIG - tema`.
- Sesión: `AAAA-MM-DD - sesión de estudio`.
- Simulacro: `AAAA-MM-DD - ASIG - Simulacro`.

Códigos sugeridos: `ALG1`, `ANA1`, `NUM`, `GEO1`, `ANA2`.

`asignatura` admite un código o una lista. En conceptos y teoremas compartidos, usa por ejemplo:

```yaml
asignatura:
  - ALG1
  - ANA1
```

## Estados

Conceptos y teoremas:

- `borrador`: capturado, todavía sin depurar.
- `en_progreso`: trabajado, pero aún no recuperable con soltura.
- `revisar`: parece correcto y necesita contraste o repetición.
- `dominado`: se puede explicar y aplicar sin apoyo.

Problemas: `pendiente`, `en_curso`, `repetir`, `resuelto`.

Clases: `capturada` hasta vaciarla en notas atómicas; después `vaciada`.

## Propiedades de repaso

- `repasar`: `true` solo para conocimiento que quieras recuperar de forma espaciada. Los problemas nacen con `false`.
- `nivel_revision`: entero de 0 a 6. Corresponde a 1, 3, 7, 21, 45, 90 y 180 días.
- `ultima_revision`: fecha del último intento de recuperación, formato `AAAA-MM-DD`; vacía antes del primero.
- `proxima_revision`: fecha del siguiente repaso, formato `AAAA-MM-DD`. La escalera de intervalos está en [[00 Inicio/Sistema de estudio|Sistema de estudio]].
- `confianza`: `rojo`, `ámbar` o `verde`, siempre en minúsculas.

Conceptos y teoremas entran en Repasos con `repasar: true` mientras no estén dominados. Un problema solo entra con `estado: repetir` y `repasar: true`.

Escribe los valores exactamente así: los paneles de Bases filtran por igualdad literal.

## Enlaces

Enlaza conceptos dentro de frases con significado. Evita listas de enlaces sin explicar la relación. Dentro de una tabla, la barra del alias se escapa: `[[ruta\|alias]]`; sin escapar, la tabla parte el enlace en dos columnas. Al crear una nota nueva, intenta añadir:

- Una idea previa de la que depende.
- Una idea posterior que ayuda a construir.
- Un problema donde aparece.

## Matemáticas en Markdown

- Fórmula en línea: `$a^2+b^2=c^2$`.
- Fórmula centrada:

```latex
$$
\sum_{k=1}^{n} k = \frac{n(n+1)}{2}
$$
```

Define la notación antes de usarla y conserva los cuantificadores relevantes.

Los enunciados van en callouts de entorno: `> [!definicion]`, `> [!teorema]`, `> [!demostracion]`, etc. La lista completa, con ejemplos renderizados, está en [[00 Inicio/Manual de uso|Manual de uso]].
