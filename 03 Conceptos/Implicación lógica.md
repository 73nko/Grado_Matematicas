---
tipo: concepto
asignatura:
  - ALG1
  - ANA1
  - GEO1
tema: Lógica y demostraciones
estado: borrador
confianza: verde
repasar: true
nivel_revision: 1
ultima_revision: 2026-08-25
fecha: 2026-08-20
proxima_revision: 2026-08-28
tags:
  - concepto
---

# Implicación lógica

## Definición

> [!definicion] Implicación lógica
> La proposición $p \Rightarrow q$ es falsa únicamente cuando $p$ es verdadera y $q$ es falsa. En los demás casos es verdadera.

## Intuición

La implicación descarta una sola situación: que se cumpla la hipótesis y falle la conclusión. No afirma que $p$ sea verdadera ni que $q$ cause a $p$.

## Ejemplos

Si un entero es múltiplo de $4$, entonces es par. Aquí la hipótesis garantiza la conclusión.

## Contraejemplos y casos frontera

La recíproca no tiene por qué ser cierta: que un entero sea par no implica que sea múltiplo de $4$.

## Propiedades

- $p \Rightarrow q$ es equivalente a $\neg p \lor q$.
- Su contrarrecíproca $\neg q \Rightarrow \neg p$ es equivalente a la implicación original.
- Su negación exige que la hipótesis se cumpla y la conclusión falle.

## Conexiones

- Depende de: proposiciones, negación y tablas de verdad.
- Permite construir: demostraciones directas y por contrarrecíproco.
- Aparece en: [[04 Teoremas y demostraciones/Principio de inducción matemática|Principio de inducción matemática]] y [[05 Problemas/ALG1 - T00 - P01 - Negar una implicación|Negar una implicación]].

## Preguntas de recuperación

1. ¿En qué único caso es falsa $p \Rightarrow q$?
2. ¿Cómo se expresa usando solo negación y disyunción?
3. ¿Qué diferencia hay entre recíproca y contrarrecíproca?

## Fuente y validación

Fuente inicial: [[08 Recursos/Guia de nivelacion Matematicas.pdf|Guía de nivelación de Matemáticas]], tema 1. Borrador de referencia pendiente de contrastar con la notación de Álgebra I.
