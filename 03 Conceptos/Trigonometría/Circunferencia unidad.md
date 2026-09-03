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
ultima_revision: 2026-09-01
fecha: 2026-08-31
proxima_revision: 2026-09-04
tags:
  - concepto
---

# Circunferencia unidad

## Definición

> [!definicion] Circunferencia unidad
> La circunferencia unidad es
> $$
> S^1=\{(x,y)\in\mathbb{R}^2:x^2+y^2=1\}.
> $$
> Si un ángulo $\theta$ se mide desde el semieje positivo de las abscisas, en sentido antihorario, el punto correspondiente es
> $$
> P(\theta)=(\cos\theta,\sin\theta).
> $$

## Intuición

El coseno es la coordenada horizontal y el seno la vertical. El cuadrante determina sus signos; el ángulo de referencia permite recuperar sus valores absolutos comparando con un ángulo agudo del primer cuadrante.

## Ejemplos

> [!ejemplo] Valores notables del primer cuadrante
>
> | $\theta$ | $0$ | $\frac{\pi}{6}$ | $\frac{\pi}{4}$ | $\frac{\pi}{3}$ | $\frac{\pi}{2}$ |
> |---|---:|---:|---:|---:|---:|
> | $\cos\theta$ | $1$ | $\frac{\sqrt3}{2}$ | $\frac{\sqrt2}{2}$ | $\frac12$ | $0$ |
> | $\sin\theta$ | $0$ | $\frac12$ | $\frac{\sqrt2}{2}$ | $\frac{\sqrt3}{2}$ | $1$ |
>
> Los valores de $30^\circ$ y $60^\circ$ se obtienen de un triángulo equilátero partido por su altura; los de $45^\circ$, de un triángulo rectángulo isósceles.

## Contraejemplos y casos frontera

> [!contraejemplo] Los ejes no pertenecen a ningún cuadrante
> En los ejes alguna coordenada es cero: por ejemplo, para $\theta=\frac{\pi}{2}$, $P=(0,1)$. Por eso no basta una regla de signos de cuadrantes para decidir si una razón está definida.

## Propiedades

- Signos de $(\cos\theta,\sin\theta)$: I $(+,+)$, II $(-,+)$, III $(-,-)$, IV $(+,-)$.
- El ángulo de referencia $\alpha\in[0,\frac{\pi}{2}]$ es el ángulo agudo entre el lado terminal y el eje horizontal. Seno y coseno conservan los valores absolutos de $\alpha$ y toman el signo del cuadrante.
- Los ángulos que difieren en una vuelta completa determinan el mismo punto:
  $$
  P(\theta+2k\pi)=P(\theta),\qquad k\in\mathbb{Z}.
  $$
- La ecuación $x^2+y^2=1$ produce la [[Identidades pitagóricas trigonométricas|identidad pitagórica trigonométrica]].

## Conexiones

- Depende de: [[Radianes|Radianes]] y la ecuación cartesiana de una circunferencia.
- Permite construir: las [[Razones trigonométricas|razones trigonométricas]], sus signos y las gráficas periódicas.
- Aparece en: la [[09 Diario/2026-08-31 - Sesión de estudio|sesión de trigonometría del 31-08]] y el bloque activo del [[01 Grado/Reto de preparación|Reto de preparación]].

## Preguntas de recuperación

1. ¿Qué significan geométricamente $\cos\theta$ y $\sin\theta$ en la circunferencia unidad?
2. Reconstruye los valores de seno y coseno de $30^\circ$, $45^\circ$ y $60^\circ$ sin usar una tabla memorizada.
3. ¿Cómo se usa el ángulo de referencia para hallar los valores y signos en los cuatro cuadrantes?

## Fuente y validación

Nota creada por el tutor IA el 2026-08-31 a partir de la sesión de trigonometría y del plan de trabajo del [[01 Grado/Reto de preparación|Reto de preparación]]. **Pendiente de validación por el estudiante**.
