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
ultima_revision: 2026-09-03
fecha: 2026-09-02
proxima_revision: 2026-09-06
tags:
  - teorema
---

# Identidades trigonométricas de suma y diferencia

## Enunciado

> [!teorema] Identidades trigonométricas de suma y diferencia
> Para cualesquiera $\alpha,\beta\in\mathbb{R}$,
> $$
> \sin(\alpha+\beta)=\sin\alpha\cos\beta+\cos\alpha\sin\beta,
> $$
> $$
> \sin(\alpha-\beta)=\sin\alpha\cos\beta-\cos\alpha\sin\beta,
> $$
> $$
> \cos(\alpha+\beta)=\cos\alpha\cos\beta-\sin\alpha\sin\beta,
> $$
> $$
> \cos(\alpha-\beta)=\cos\alpha\cos\beta+\sin\alpha\sin\beta.
> $$
> Cuando las tangentes y los cocientes están definidos,
> $$
> \tan(\alpha+\beta)=\frac{\tan\alpha+\tan\beta}{1-\tan\alpha\tan\beta},
> $$
> $$
> \tan(\alpha-\beta)=\frac{\tan\alpha-\tan\beta}{1+\tan\alpha\tan\beta}.
> $$

## Hipótesis

- Las identidades de seno y coseno son válidas para todos los ángulos reales $\alpha$ y $\beta$.
- Las identidades escritas con tangentes exigen que $\cos\alpha\neq0$, $\cos\beta\neq0$ y $\cos(\alpha\pm\beta)\neq0$ para la operación correspondiente.

## Tesis

Las razones trigonométricas de una suma o diferencia de ángulos se expresan mediante las razones de cada ángulo por separado.

## Intuición

Sumar ángulos equivale a componer giros. El punto $P(\alpha)=(\cos\alpha,\sin\alpha)$, al girarse un ángulo $\beta$, pasa a $P(\alpha+\beta)$. La transformación mezcla sus coordenadas horizontal y vertical; al comparar las coordenadas del punto obtenido aparecen las identidades de seno y coseno.

## Estrategia de demostración

1. Girar $P(\alpha)=(\cos\alpha,\sin\alpha)$ un ángulo $\beta$ y escribir las coordenadas resultantes.
2. Identificar ese punto con $P(\alpha+\beta)$ e igualar las coordenadas.
3. Sustituir $\beta$ por $-\beta$ y usar que el coseno es par y el seno impar para obtener las fórmulas de diferencia.
4. Dividir seno entre coseno y simplificar para deducir las identidades de la tangente, conservando sus restricciones de dominio.

## Demostración propia

> [!demostracion]
>

## Dónde se usa cada hipótesis

- La parametrización de la [[Circunferencia unidad|circunferencia unidad]] permite identificar las coordenadas del punto girado con seno y coseno.
- Las condiciones sobre los cosenos garantizan que las tangentes y las divisiones empleadas en su deducción estén definidas.

## Qué falla sin ellas

Las fórmulas de seno y coseno no presentan excepciones reales. En cambio, la forma con tangentes puede dejar de tener sentido aunque la tangente del ángulo final exista: por ejemplo, $\tan(\frac{\pi}{2}+\frac{\pi}{2})=\tan\pi$ existe, pero las tangentes individuales del miembro derecho no están definidas. Si el denominador $1\mp\tan\alpha\tan\beta$ se anula, la tangente de la suma o diferencia correspondiente tampoco está definida.

## Consecuencias y conexiones

- Dependen de: [[Circunferencia unidad|circunferencia unidad]], [[Razones trigonométricas|razones trigonométricas]] y las simetrías de las [[Gráficas de seno, coseno y tangente|gráficas trigonométricas]].
- Permiten construir: las identidades de ángulo doble y mitad y la resolución de ecuaciones trigonométricas.
- Aparecen en: el cálculo exacto de $\cos15^\circ$ y $\tan15^\circ$ de la [[09 Diario/2026-09-02 - Sesión de estudio|sesión del 02-09]].

## Preguntas de recuperación

1. Reconstruye las cuatro identidades de seno y coseno y explica el patrón de signos.
2. Explica geométricamente por qué aparecen productos cruzados al sumar dos ángulos.
3. Deduce la fórmula de $\tan(\alpha-\beta)$ e indica todas sus restricciones de dominio.

## Fuente y validación

Nota creada por el tutor IA el 2026-09-02 a partir de la explicación y las comprobaciones realizadas en la [[09 Diario/2026-09-02 - Sesión de estudio|sesión del 02-09]]. Material de referencia previsto: Pearson, _Geometría y trigonometría_, bloque de identidades, y la sección 3.2 «Sum, Difference, and Cofunction Identities» del manual mostrado durante la sesión, pendiente de incorporar con sus datos bibliográficos completos. **Pendiente de validación por el estudiante**.
