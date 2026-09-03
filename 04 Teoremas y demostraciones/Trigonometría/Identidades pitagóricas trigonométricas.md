---
tipo: teorema
asignatura:
  - ANA1
  - GEO1
tema: Trigonometría
estado: borrador
confianza: rojo
repasar: true
nivel_revision: 1
ultima_revision: 2026-09-01
fecha: 2026-08-31
proxima_revision: 2026-09-04
tags:
  - teorema
---

# Identidades pitagóricas trigonométricas

## Enunciado

> [!teorema] Identidades pitagóricas trigonométricas
> Para todo $\theta\in\mathbb{R}$,
> $$
> \sin^2\theta+\cos^2\theta=1.
> $$
> Si además $\cos\theta\neq0$,
> $$
> 1+\tan^2\theta=\sec^2\theta.
> $$
> Si además $\sin\theta\neq0$,
> $$
> 1+\cot^2\theta=\csc^2\theta.
> $$

## Hipótesis

- En la identidad básica, $P(\theta)=(\cos\theta,\sin\theta)$ pertenece a la [[Circunferencia unidad|circunferencia unidad]].
- Para dividir por $\cos^2\theta$, se exige $\cos\theta\neq0$.
- Para dividir por $\sin^2\theta$, se exige $\sin\theta\neq0$.

## Tesis

La identidad básica relaciona seno y coseno. Las otras dos son consecuencias algebraicas de ella y de las definiciones de las [[Razones trigonométricas|razones trigonométricas]].

## Intuición

La primera identidad es la ecuación $x^2+y^2=1$ de la circunferencia unidad escrita con $x=\cos\theta$ e $y=\sin\theta$. Las identidades de tangente y cotangente no son resultados independientes: se obtienen cambiando la escala mediante una división.

## Estrategia de demostración

1. Sustituir $P(\theta)=(\cos\theta,\sin\theta)$ en $x^2+y^2=1$.
2. Dividir la identidad básica por $\cos^2\theta$ y reconocer $\tan\theta$ y $\sec\theta$.
3. Dividir la identidad básica por $\sin^2\theta$ y reconocer $\cot\theta$ y $\csc\theta$.

## Demostración propia

> [!demostracion]
>

## Dónde se usa cada hipótesis

- La pertenencia a la circunferencia unidad justifica $\cos^2\theta+\sin^2\theta=1$.
- Las condiciones $\cos\theta\neq0$ y $\sin\theta\neq0$ permiten dividir y coinciden con los dominios de las razones que aparecen.

## Qué falla sin ellas

En $\theta=\frac{\pi}{2}+k\pi$ no están definidas $\tan\theta$ ni $\sec\theta$. En $\theta=k\pi$ no están definidas $\cot\theta$ ni $\csc\theta$. La identidad básica sí sigue siendo válida en todos esos ángulos.

## Consecuencias y conexiones

- Permiten hallar una razón trigonométrica a partir de otra, con el signo decidido por el cuadrante.
- Son la herramienta básica para simplificar expresiones, conservando siempre el dominio de la expresión original.
- Se trabajaron en la [[09 Diario/2026-08-31 - Sesión de estudio|sesión de trigonometría del 31-08]] y se usarán en la próxima sesión.

## Fuente y validación

Nota creada por el tutor IA el 2026-08-31 a partir de la sesión de trigonometría y del plan de trabajo del [[01 Grado/Reto de preparación|Reto de preparación]]. **Pendiente de validación por el estudiante**; la sección «Demostración propia» se deja sin rellenar.
