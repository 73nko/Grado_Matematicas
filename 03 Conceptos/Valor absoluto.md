---
tipo: concepto
asignatura:
  - ANA1
tema: Números reales
estado: en_progreso
confianza: rojo
repasar: true
nivel_revision: 1
ultima_revision: 2026-08-29
fecha: 2026-08-26
proxima_revision: 2026-09-01
tags:
  - concepto
---

# Valor absoluto

## Definición

> [!definicion] Valor absoluto
> Para $x \in \mathbb{R}$, el **valor absoluto** de $x$ es
> $$|x| = \begin{cases} x & \text{si } x \geq 0 \\ -x & \text{si } x < 0 \end{cases}$$
> Equivalentemente, $|x| = \max\{x, -x\} = \sqrt{x^2}$.

Las tres caracterizaciones sirven para cosas distintas: la definición por casos es la operativa (partir la recta en zonas), el máximo es cómodo en demostraciones, y $\sqrt{x^2}$ justifica el truco de elevar al cuadrado.

## Intuición

> [!intuicion] El valor absoluto es una distancia
> $|x|$ es la distancia de $x$ al origen, y $|x - a|$ es la **distancia de $x$ a $a$**. Esta lectura convierte inecuaciones en geometría:
> $$|x - a| < r \iff x \in (a - r,\, a + r)$$
> El conjunto $\{x : |x-a| < r\}$ es el **entorno** de centro $a$ y radio $r$. Toda la definición ε-δ de límite y continuidad en Análisis I es esta frase usada con disciplina.

Leer $|x|$ como "quitar el signo" funciona para calcular; leerlo como distancia es lo que escala al grado.

## Ejemplos

> [!ejemplo] De módulo a intervalo y de intervalo a módulo
> - $|2x+1| \leq 5 \iff -5 \leq 2x+1 \leq 5 \iff x \in [-3, 2]$.
> - El intervalo $(-2, 8)$ tiene centro $\frac{-2+8}{2} = 3$ y radio $8 - 3 = 5$, luego $(-2,8) = \{x : |x-3| < 5\}$.
> - $|4 - x| = |x - 4|$: el módulo no distingue el orden de la resta, porque la distancia de $x$ a $4$ y la de $4$ a $x$ son la misma.

## Contraejemplos y casos frontera

> [!contraejemplo] Donde se rompen los reflejos del instituto
> - $\sqrt{x^2} = x$ es **falso** en general: con $x = -2$, $\sqrt{4} = 2 \neq -2$. Lo correcto es $\sqrt{x^2} = |x|$.
> - $|x - 5| < 0$ no tiene solución ($\varnothing$), pero $|x-5| \leq 0$ sí: exactamente $\{5\}$. La frontera entre $<$ y $\leq$ importa.
> - $|x - 2| < a$ es vacía para **todo** $a \leq 0$: un módulo nunca es menor que algo no positivo.
> - En la triangular, la igualdad $|x+y| = |x| + |y|$ solo ocurre cuando $x$ e $y$ tienen el mismo signo (o alguno es cero); con signos opuestos es estricta: $|3 + (-3)| = 0 < 6$.

## Propiedades

Para $a > 0$ y $x, y \in \mathbb{R}$:

1. **Equivalencia de entorno**: $|u| < a \iff -a < u < a$ (un intervalo).
2. **Equivalencia exterior**: $|u| > a \iff u < -a \ \text{o}\ u > a$ (unión de dos semirrectas, nunca un intervalo).
3. **Multiplicatividad**: $|xy| = |x|\,|y|$ y $\left|\frac{x}{y}\right| = \frac{|x|}{|y|}$ si $y \neq 0$.
4. **Encaje**: $-|x| \leq x \leq |x|$ (la llave que abre la triangular).
5. **Desigualdad triangular**: $|x + y| \leq |x| + |y|$.
6. **Triangular inversa**: $\big|\,|x| - |y|\,\big| \leq |x - y|$.

Método para inecuaciones con módulo, en orden de preferencia: lectura geométrica → equivalencias 1-2 → partir en casos por los ceros de cada módulo → elevar al cuadrado (solo con ambos lados $\geq 0$).

## Conexiones

- Depende de: el orden de $\mathbb{R}$ y la noción de máximo (sin nota propia todavía).
- Permite construir: los entornos y la definición ε-δ de límite (bloque P6b del [[01 Grado/Reto de preparación|Reto de preparación]]; sin nota todavía), y las técnicas de acotación de desigualdades (P2, sesión 2).
- Aparece en: [[05 Problemas/ANA1 - T00 - P01 - Acotar x²-4 con módulo|ANA1 - T00 - P01]] — el gesto central del ε-δ —, los 12 ejercicios de la [[09 Diario/2026-08-26 - Sesión de estudio|sesión del 26-08]] y desde la primera clase de [[02 Asignaturas/1C - Análisis I/Análisis I|Análisis I]].

## Preguntas de recuperación

1. Escribe $|x - a| < r$ sin valor absoluto y di qué objeto geométrico es el conjunto solución.
2. ¿Por qué $|u| > a$ (con $a > 0$) da una unión de dos semirrectas y no un intervalo? Dibújalo.
3. Demuestra la desigualdad triangular a partir de $-|x| \leq x \leq |x|$, justificando cada paso.
4. ¿Cuándo es válido resolver $|A| < |B|$ elevando al cuadrado, y por qué?

## Fuente y validación

Nota creada por el tutor IA el 2026-08-26 a partir de la sesión P2-1 del Reto de preparación. Material de referencia: Asapchi, TEMA II (valor absoluto y entornos); Bartle-Sherbert, §2.2; Korovkin, _Desigualdades_, cap. I. **Pendiente de validación por el estudiante**: pasa a `en_progreso` cuando la trabajes y sube la confianza solo tras recuperar sin mirar.
