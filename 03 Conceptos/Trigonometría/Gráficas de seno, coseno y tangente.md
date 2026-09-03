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

# Gráficas de seno, coseno y tangente

## Definición

> [!definicion] Funciones trigonométricas básicas
> En la [[Circunferencia unidad|circunferencia unidad]], $cos x$ es la coordenada horizontal y $sin x$ la vertical del punto asociado a $x$. Cuando $cos x\neq 0$, se define
> $$
> \tan x=\frac{\sin x}{\cos x}.
> $$
> Sus gráficas repiten sus valores después de un periodo fundamental: $2\pi$ para seno y coseno, y $\pi$ para tangente.

## Intuición

Al recorrer repetidamente la [[Circunferencia unidad|circunferencia unidad]], las dos coordenadas oscilan entre $-1$ y $1$. Eso produce las ondas de seno y coseno. La tangente es el cociente entre ambas coordenadas: se anula cuando el seno vale cero y crece sin cota cuando el coseno se aproxima a cero.

## Resumen esquemático

En toda la tabla, $k\in\mathbb{Z}$.

| Función | Dominio | Recorrido | Periodo fundamental | Ceros | Extremos o asíntotas | Simetría |
|---|---|---|---|---|---|---|
| $\sin x$ | $\mathbb{R}$ | $[-1,1]$ | $2\pi$ | $x=k\pi$ | Máximos: $1$ en $x=\frac{\pi}{2}+2k\pi$. Mínimos: $-1$ en $x=-\frac{\pi}{2}+2k\pi$. Sin asíntotas. | Impar: $\sin(-x)=-\sin x$. Simetría respecto del origen. |
| $\cos x$ | $\mathbb{R}$ | $[-1,1]$ | $2\pi$ | $x=\frac{\pi}{2}+k\pi$ | Máximos: $1$ en $x=2k\pi$. Mínimos: $-1$ en $x=\pi+2k\pi$. Sin asíntotas. | Par: $\cos(-x)=\cos x$. Simetría respecto del eje vertical. |
| $\tan x$ | $\mathbb{R}\setminus\left\{\frac{\pi}{2}+k\pi:k\in\mathbb{Z}\right\}$ | $\mathbb{R}$ | $\pi$ | $x=k\pi$ | No tiene máximos ni mínimos. Asíntotas verticales: $x=\frac{\pi}{2}+k\pi$. | Impar: $\tan(-x)=-\tan x$. Simetría respecto del origen. |

## Ejemplos

> [!ejemplo] Un periodo representativo
> - Para seno y coseno puede estudiarse un periodo en $[0,2\pi]$.
> - Para tangente puede estudiarse una rama completa en $\left(-\frac{\pi}{2},\frac{\pi}{2}\right)$.
> - El resto de la gráfica se obtiene trasladando horizontalmente esos fragmentos una cantidad igual a su periodo.

## Contraejemplos y casos frontera

> [!contraejemplo] La tangente no es una onda acotada
> Aunque seno, coseno y tangente son periódicas, la tangente no tiene amplitud ni recorrido acotado. Sus puntos excluidos del dominio son precisamente aquellos donde $\cos x=0$; la gráfica se aproxima a las rectas verticales correspondientes, pero nunca las corta.

## Propiedades

- Un periodo de una función $f$ es un número $T>0$ tal que $f(x+T)=f(x)$ para todo $x$ del dominio donde ambos miembros tengan sentido. El periodo fundamental es el menor periodo positivo.
- Todo múltiplo entero positivo del periodo fundamental también es un periodo.
- Seno y coseno tienen las mismas dimensiones geométricas, pero están desfasados:
  $$
  \cos x=\sin\left(x+\frac{\pi}{2}\right).
  $$
- En cada intervalo $\left(-\frac{\pi}{2}+k\pi,\frac{\pi}{2}+k\pi\right)$, la tangente es continua y estrictamente creciente.

## Conexiones

- Depende de: [[Radianes|Radianes]], [[Circunferencia unidad|circunferencia unidad]] y [[Razones trigonométricas|razones trigonométricas]].
- Permite construir: [[Transformaciones de funciones sinusoidales|transformaciones de funciones sinusoidales]], ecuaciones trigonométricas y modelos periódicos.
- Aparece en: la [[09 Diario/2026-09-01 - Sesión de estudio|sesión del 01-09]] y los ejercicios de [[08 Recursos/Trigonometría - 250 ejercicios - versión 2.pdf|250 ejercicios de trigonometría]].

## Preguntas de recuperación

1. Reconstruye dominio, recorrido, periodo y ceros de seno, coseno y tangente sin consultar la tabla.
2. ¿Por qué la tangente tiene periodo $\pi$ y asíntotas en $x=\frac{\pi}{2}+k\pi$?
3. Dibuja un periodo de cada función y justifica sus simetrías a partir de $f(-x)$.

## Fuente y validación

Nota creada por el tutor IA el 2026-09-01 a partir de la recuperación del estudiante en la [[09 Diario/2026-09-01 - Sesión de estudio|sesión del 01-09]] y contrastada con [OpenStax, *Precálculo 2ed*, §6.1](https://openstax.org/books/prec%C3%A1lculo-2ed/pages/6-1-graficos-de-las-funciones-seno-y-coseno) y [§6.2](https://openstax.org/books/prec%C3%A1lculo-2ed/pages/6-2-graficos-de-las-otras-funciones-trigonometricas). **Pendiente de validación por el estudiante**.
