---
tipo: problema
asignatura: ALG1
tema: Lógica y demostraciones
dificultad: inicial
estado: resuelto
fecha: 2026-08-25
repasar: false
nivel_revision: 0
ultima_revision:
proxima_revision:
tags:
  - problema
---

# ALG1 - T00 - P02 - Suma de los primeros n naturales

## Enunciado

> [!problema] Suma de los primeros $n$ naturales
> Se define recursivamente $S_n$, para $n \geq 1$, mediante
> $$S_1 := 1, \qquad S_{n+1} := S_n + (n+1). \tag{1}$$
> La expresión informal $1 + 2 + \cdots + n$ denota $S_n$. Demuestra por inducción que para todo entero $n \geq 1$
> $$S_n = \frac{n(n+1)}{2}. \tag{2}$$

## Datos, hipótesis y objetivo

- $S_n$ solo está disponible a través de la definición recursiva (1): no se asume ningún lema sobre sumatorios.
- Herramienta: [[Principio de inducción matemática|Principio de inducción matemática]] con $n_0 = 1$.
- Objetivo: identificar $P(n)$ con precisión, verificar el caso base y deducir $P(n+1)$ de $P(n)$ usando únicamente (1) y la hipótesis inductiva.

## Primer intento

## Bloqueo concreto

## Pistas solicitadas

## Solución final

**Proposición.** Para todo entero $n \geq 1$ se tiene $S_n = \dfrac{n(n+1)}{2}$.

> [!demostracion] Demostración
> Aplicamos el principio de inducción con $n_0 = 1$ y con la propiedad
> $$P(n) : \ \text{la igualdad } S_n = \tfrac{n(n+1)}{2} \text{ es cierta.}$$
>
> **Caso base.** Por (1) se tiene $S_1 = 1$, y por otra parte $\frac{1 \cdot (1+1)}{2} = \frac{2}{2} = 1$. Ambos miembros de (2) coinciden para $n = 1$, luego $P(1)$ es verdadera.
>
> **Paso inductivo.** Sea $n \geq 1$ un entero arbitrario y supongamos que $P(n)$ es verdadera; esto es, que $S_n = \frac{n(n+1)}{2}$. Queremos deducir $P(n+1)$. Partiendo del miembro izquierdo de $P(n+1)$,
> $$
> \begin{aligned}
> S_{n+1} &= S_n + (n+1) && \text{por la definición (1)} \\
>         &= \frac{n(n+1)}{2} + (n+1) && \text{por la hipótesis inductiva} \\
>         &= (n+1)\left(\frac{n}{2} + 1\right) && \text{sacando factor común} \\
>         &= \frac{(n+1)(n+2)}{2}.
> \end{aligned}
> $$
> Como $\frac{(n+1)\big((n+1)+1\big)}{2} = \frac{(n+1)(n+2)}{2}$, lo obtenido es precisamente el enunciado $P(n+1)$. Puesto que $n \geq 1$ era arbitrario, queda probada la hipótesis (ii) del principio de inducción.
>
> Verificadas (i) y (ii), el principio garantiza que $P(n)$ es verdadera para todo entero $n \geq 1$.

## Verificación

## Idea transferible

## Error cometido

## Variación para repetir
