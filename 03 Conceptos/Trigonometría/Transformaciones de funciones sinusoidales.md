---
tipo: concepto
asignatura:
  - ANA1
  - GEO1
tema: Trigonometría
estado: borrador
confianza: rojo
repasar: true
nivel_revision: 1
ultima_revision: 2026-09-02
fecha: 2026-09-01
proxima_revision: 2026-09-05
tags:
  - concepto
---

# Transformaciones de funciones sinusoidales

## Definición

> [!definicion] Forma general de una función sinusoidal
> Para $A\neq 0$ y $B\neq 0$, una función sinusoidal puede escribirse como
> $$
> y=A\sin(Bx-C)+D
> $$
> o, equivalentemente, como
> $$
> y=A\sin\bigl(B(x-h)\bigr)+D,
> \qquad h=\frac{C}{B}.
> $$
> Sus parámetros geométricos son
> $$
> \text{amplitud}=|A|,\qquad
> T=\frac{2\pi}{|B|},\qquad
> \text{línea media}: y=D,
> $$
> y su recorrido es $[D-|A|,D+|A|]$.

## Intuición

Se parte de la [[Gráficas de seno, coseno y tangente|gráfica de $y=\sin x$]] y se transforma:

1. $B$ comprime o estira horizontalmente la onda y determina su periodo.
2. $h=C/B$ la desplaza horizontalmente.
3. $A$ la estira verticalmente; si $A<0$, además la refleja respecto de su línea media.
4. $D$ la desplaza verticalmente y fija la línea alrededor de la cual oscila.

## Resumen de parámetros

| Parámetro | Efecto geométrico |
|---|---|
| $A$ | Amplitud $|A|$. Si $A<0$, reflexión vertical respecto de la línea media. |
| $B$ | Periodo $T=\frac{2\pi}{|B|}$. Un $|B|$ mayor comprime horizontalmente la gráfica. |
| $C$ | Interviene en el desplazamiento, pero no es por sí solo el desplazamiento. En la forma $Bx-C$, se tiene $h=\frac{C}{B}$. |
| $D$ | Línea media $y=D$ y desplazamiento vertical. |

## Ejemplos

> [!ejemplo] Lectura de una función transformada
> Para
> $$
> f(x)=2\sin(3x-\pi)+1
> =2\sin\left(3\left(x-\frac{\pi}{3}\right)\right)+1,
> $$
> se obtiene
> $$
> |A|=2,\qquad
> T=\frac{2\pi}{3},\qquad
> h=\frac{\pi}{3},\qquad
> y=D=1,
> $$
> y el recorrido es $[-1,3]$.

## Contraejemplos y casos frontera

> [!contraejemplo] El desplazamiento no siempre es $C$
> En $A\sin(Bx-C)+D$, el desplazamiento horizontal es $C/B$. Solo puede leerse directamente como $h$ después de factorizar:
> $$
> Bx-C=B\left(x-\frac{C}{B}\right).
> $$

> [!contraejemplo] La fórmula de amplitud no se traslada a la tangente
> En $A\tan(Bx-C)+D$, el periodo es $\pi/|B|$, pero la función continúa teniendo recorrido $\mathbb{R}$ y no tiene amplitud, máximos ni mínimos.

## Propiedades

- La forma $A\cos(Bx-C)+D$ tiene la misma amplitud, periodo, línea media y regla de desplazamiento que la forma con seno.
- Los valores máximos y mínimos de una sinusoidal son, respectivamente, $D+|A|$ y $D-|A|$.
- El parámetro de fase no es único: desplazar una función un número entero de periodos no cambia su gráfica.
- El signo de $B$ puede absorberse en otros parámetros usando las simetrías de seno y coseno; suele preferirse una representación con $B>0$.

## Conexiones

- Depende de: [[Gráficas de seno, coseno y tangente|gráficas de seno, coseno y tangente]], [[Radianes|radianes]] y transformaciones elementales de funciones.
- Permite construir: modelos periódicos, lectura de gráficas y resolución de ecuaciones trigonométricas transformadas.
- Aparece en: la comprobación de la [[09 Diario/2026-09-01 - Sesión de estudio|sesión del 01-09]] y los ejercicios de [[08 Recursos/Trigonometría - 250 ejercicios - versión 2.pdf|250 ejercicios de trigonometría]].

## Preguntas de recuperación

1. En $A\sin(Bx-C)+D$, ¿cómo se obtienen amplitud, periodo, desplazamiento, línea media y recorrido?
2. ¿Por qué el desplazamiento horizontal es $C/B$ y no necesariamente $C$?
3. Reconstruye un periodo de $2\sin(3x-\pi)+1$ señalando cinco puntos característicos.

## Fuente y validación

Nota creada por el tutor IA el 2026-09-01 a partir de la recuperación del estudiante en la [[09 Diario/2026-09-01 - Sesión de estudio|sesión del 01-09]] y contrastada con [OpenStax, *Precálculo 2ed*, §6.1](https://openstax.org/books/prec%C3%A1lculo-2ed/pages/6-1-graficos-de-las-funciones-seno-y-coseno). **Pendiente de validación por el estudiante**.
