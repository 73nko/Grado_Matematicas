# Sistema de estudio

El objetivo del vault no es acumular apuntes. Es convertir cada tema en conocimiento recuperable y aplicable.

## Ciclo por tema

1. **Mapa previo, 10-15 min.** Lee títulos, definiciones y resultados. Escribe qué crees que aprenderás.
2. **Clase o estudio guiado.** Crea una nota con [[90 Plantillas/Plantilla - Clase|Plantilla - Clase]]. Distingue hechos, intuiciones, dudas y ejemplos.
3. **Extracción, dentro de 24 h.** Separa los conceptos y teoremas que merezcan notas propias. Una nota, una idea central.
4. **Recuperación activa.** Cierra los apuntes y reconstruye definiciones, hipótesis y argumentos.
5. **Problemas.** Intenta antes de consultar pistas. Registra los fallos que puedan repetirse.
6. **Síntesis.** Explica el tema de memoria y conecta sus ideas con otros temas o asignaturas.
7. **Revisión espaciada.** Revisa aproximadamente a 1, 3, 7, 21, 45, 90 y 180 días siguiendo la escalera de repaso. Ajusta el intervalo según el dominio real.

## Escalera de repaso

El repaso espaciado funciona con `repasar`, `nivel_revision`, `ultima_revision` y `proxima_revision`, junto con el panel [[07 Revisiones/Repasos.base|Repasos]]. La vista **Para hoy** está embebida en [[00 Inicio/Inicio|Inicio]]: lo que aparece ahí es el trabajo de repaso del día.

Programa conceptos y teoremas nucleares que quieras poder reconstruir o aplicar. No programes notas de referencia o navegación. Los problemas permanecen fuera por defecto y solo entran cuando `estado: repetir` y `repasar: true`.

1. Para cada nota que aparezca, intenta la recuperación sin mirar: responde sus preguntas de recuperación, reconstruye la demostración o repite el problema.
2. Pon `ultima_revision` en hoy y registra tú el resultado:
   - **Bien recuperado**: avanza un nivel y programa el intervalo nuevo.
   - **Imprecisión**: conserva o reduce el nivel y usa `ámbar`.
   - **Fallo**: vuelve a nivel 0, usa `rojo` y programa mañana.
3. Los niveles son `0 → 1 día`, `1 → 3`, `2 → 7`, `3 → 21`, `4 → 45`, `5 → 90` y `6 → 180`.
4. Marca `estado: dominado` solo cuando puedas demostrar el criterio de dominio; ningún intervalo ni agente lo decide automáticamente.

La vista **Sin programar** avisa de notas elegibles que se quedaron sin fecha. Un problema pendiente con `repasar: false` no es una fuga.

## Criterio de dominio

No marques un concepto como dominado solo por reconocerlo. Debes poder:

- Enunciar la definición con precisión.
- Producir un ejemplo y un contraejemplo.
- Explicar por qué es útil.
- Conectarlo con al menos otra idea.
- Resolver un problema nuevo donde intervenga.

Para un teorema, además:

- Identificar cada hipótesis y dónde se usa.
- Reconstruir la estrategia de la demostración.
- Explicar qué falla al retirar una hipótesis relevante.

## Semáforo

- `rojo`: no puedo reconstruirlo sin mirar.
- `ámbar`: entiendo la idea, pero fallo en precisión o aplicación.
- `verde`: puedo explicarlo y aplicarlo sin apoyo.

El semáforo mide recuperación, no familiaridad.
