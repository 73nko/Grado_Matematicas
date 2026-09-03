---
tipo: problema
asignatura: ANA1
tema: Números reales
dificultad: inicial
estado: resuelto
fecha: 2026-08-26
repasar: false
nivel_revision: 0
ultima_revision:
proxima_revision:
tags:
  - problema
---

# ANA1 - T00 - P01 - Acotar x²-4 con módulo

## Enunciado

> [!problema] Acotar $x^2 - 4$ con módulo
> Demuestra: si $|x - 2| < 1$, entonces $|x^2 - 4| < 5$.

## Datos, hipótesis y objetivo

- Hipótesis: $|x - 2| < 1$, es decir, $x$ está en el entorno de centro $2$ y radio $1$.
- Objetivo: acotar $|x^2 - 4|$ estrictamente por $5$.
- Herramientas: multiplicatividad $|ab| = |a||b|$ y equivalencia de entorno $|u| < r \iff -r < u < r$, ambas en [[Valor absoluto|Valor absoluto]].
- Este es el gesto central de las demostraciones ε-δ (bloque P6b del [[01 Grado/Reto de preparación|Reto de preparación]]): controlar un factor con la hipótesis y acotar el otro con ella misma.

## Primer intento

## Bloqueo concreto

## Pistas solicitadas

- Pista de arranque dada con el enunciado (sesión P2-1, 2026-08-26): «factoriza $x^2 - 4$».

## Solución final

**Proposición.** Si $|x - 2| < 1$, entonces $|x^2 - 4| < 5$.

> [!demostracion] Demostración
> Factorizamos y usamos la multiplicatividad del valor absoluto:
> $$|x^2 - 4| = |(x-2)(x+2)| = |x - 2|\,|x + 2|.$$
> El primer factor está controlado por la hipótesis: $|x - 2| < 1$.
>
> Para acotar el segundo, desarrollamos la hipótesis con la equivalencia de entorno:
> $$|x - 2| < 1 \iff -1 < x - 2 < 1 \iff 1 < x < 3.$$
> Sumando $2$ en los tres miembros, $3 < x + 2 < 5$. En particular $x + 2 > 0$, luego $|x + 2| = x + 2 < 5$.
>
> Ambos factores son no negativos, así que las dos cotas estrictas se multiplican:
> $$|x^2 - 4| = |x - 2|\,|x + 2| < 1 \cdot 5 = 5. \qquad$$

## Verificación

## Idea transferible

## Error cometido

## Variación para repetir
