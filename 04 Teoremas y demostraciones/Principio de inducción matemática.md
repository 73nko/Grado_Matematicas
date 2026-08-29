---
tipo: teorema
asignatura:
  - ALG1
  - ANA1
tema: Lógica y demostraciones
estado: borrador
confianza: verde
repasar: true
nivel_revision: 2
ultima_revision: 2026-08-29
fecha: 2026-08-20
proxima_revision: 2026-09-05
tags:
  - teorema
---

# Principio de inducción matemática

## Enunciado

> [!teorema] Principio de inducción matemática
> Sea $P(n)$ una proposición definida para todo entero $n \geq n_0$. Si $P(n_0)$ es verdadera y, para todo $k \geq n_0$, de $P(k)$ se deduce $P(k+1)$, entonces $P(n)$ es verdadera para todo $n \geq n_0$.

## Hipótesis

1. Caso base: $P(n_0)$.
2. Paso inductivo: para todo $k \geq n_0$, $P(k) \Rightarrow P(k+1)$.

## Tesis

$P(n)$ se cumple para cada entero $n \geq n_0$.

## Intuición

El caso base pone en marcha la cadena y el paso inductivo garantiza que cada caso alcanzado conduce al siguiente.

## Estrategia de demostración

Identificar con precisión $P(n)$, comprobar el primer índice permitido y, en el paso inductivo, separar la hipótesis $P(k)$ de la conclusión $P(k+1)$.

## Demostración propia

> [!demostracion]
>

## Dónde se usa cada hipótesis

- El caso base evita que el argumento sea una cadena sin punto de inicio.
- El paso inductivo propaga la propiedad entre enteros consecutivos.

## Qué falla sin ellas

Un paso inductivo correcto sin caso base no demuestra que ningún caso sea verdadero. Un caso base aislado no permite alcanzar los casos posteriores.

## Consecuencias y conexiones

- Usa [[03 Conceptos/Implicación lógica|Implicación lógica]] en el paso inductivo.
- Es una técnica transversal para identidades, desigualdades y propiedades definidas sobre los naturales.

## Fuente y validación

Fuente inicial: [[08 Recursos/Guia de nivelacion Matematicas.pdf|Guía de nivelación de Matemáticas]], tema 1, y Sominski, _Método de inducción matemática_, §1–4. Borrador pendiente de contraste con la formulación del profesorado.
