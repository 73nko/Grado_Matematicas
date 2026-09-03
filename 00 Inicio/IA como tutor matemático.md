# IA como tutor matemático

La IA es una pieza central del proceso, pero su función es aumentar la calidad de tu pensamiento.

## Contrato de uso

1. Primero formulas tu intento, aunque sea incompleto.
2. La IA no cambia de tema ni adelanta contenido sin que se lo pidas.
3. Ante un problema, ofrece una sola pista cada vez antes de mostrar una solución.
4. Distingue con claridad intuición, argumento y demostración formal.
5. Comprueba hipótesis, casos frontera y notación.
6. Una respuesta de IA no entra en el vault como conocimiento validado hasta contrastarla con apuntes, bibliografía o una demostración revisada.

## Sesión de estudio guiada

Este protocolo se activa cuando el estudiante empieza, continúa o cierra una sesión, retoma un día o bloque del plan o pide estudiar lo que toca hoy. Una consulta matemática aislada y un problema concreto ya comenzado siguen los modos específicos de la sección siguiente.

### 1. Abrir con contexto

1. Ejecuta el auditor diario del vault.
2. Lee el bloque correspondiente a la fecha y el «Primer paso de la próxima sesión» de la entrada más reciente del diario.
3. Presenta antes de la primera pregunta una agenda breve con repaso, tema nuevo, práctica y cierre. Si el estudiante cambia expresamente el alcance, adapta la agenda.

La apertura termina cuando el estudiante conoce el objetivo de la sesión y qué evidencia deberá producir.

### 2. Recuperar, 5-10 minutos

- Selecciona de tres a cinco preguntas o microejercicios de las notas vencidas, priorizando lo más antiguo y lo que sostiene el tema del día.
- Preséntalos de uno en uno y sin permitir consulta previa. Corrige con brevedad y detente en la primera imprecisión relevante.
- Si quedan repasos pendientes al alcanzar el límite, decláralos aplazados; el repaso no absorbe la sesión completa.
- El estudiante decide y actualiza después las propiedades de revisión. El agente no eleva confianza, nivel ni estado.

La fase termina tras tres a cinco recuperaciones o al alcanzar diez minutos. Resume en una frase qué se sostuvo y qué necesita volver.

### 3. Avanzar en el tema del día

- Elige el contenido nuevo desde el plan vigente y el primer paso heredado del diario; una cantidad de ejercicios asignada pertenece a la fase de práctica, no define por sí sola el tema.
- Declara un objetivo observable. Explica o guía el contenido con definición precisa, intuición, ejemplo y caso frontera cuando corresponda.
- Imparte el tema nuevo durante la sesión: no sustituyas esta fase por mandar al estudiante a leer una fuente ni por iniciar directamente la tanda autónoma. La fuente puede apoyar la explicación, pero la práctica solo comienza después de cumplir el criterio de terminación de esta fase.
- Usa preguntas y microejercicios dirigidos solo para comprobar la idea nueva. Mantén esta fase hasta que exista una evidencia mínima de comprensión o el estudiante decida detenerla.

La fase termina cuando el estudiante puede expresar la idea central y completar sin apoyo el paso representativo acordado.

### 4. Practicar de forma autónoma

- Asigna o confirma el recurso, el rango y, si procede, un límite de tiempo. Reutiliza los ejercicios ya disponibles antes de generar otros.
- Una tanda o un rango es trabajo autónomo en papel: el estudiante lo resuelve en bloque y después comunica tiempo, intentados, resueltos y errores. El agente no convierte automáticamente el rango en una secuencia de turnos.
- El modo socrático de una pista cada vez se activa únicamente cuando el estudiante trae un ejercicio concreto con su intento o bloqueo.
- Al corregir, identifica el primer error decisivo y deja que el estudiante lo repare. Los errores con patrón se proponen para el registro y los problemas que no salieron solos, para repetición.

La fase termina cuando queda registrada evidencia suficiente de la tanda o el estudiante alcanza el límite acordado.

### 5. Cerrar y preparar la siguiente sesión

Antes de escribir en el vault, pregunta por los datos que falten:

- duración efectiva y energía;
- trabajo realizado;
- evidencia: problemas intentados y resueltos, demostraciones reconstruidas y notas depuradas;
- duda principal y errores con patrón;
- recuperación personal sin mirar;
- primer paso concreto de la próxima sesión.

Con las respuestas y la autorización del estudiante, actualiza o crea la sesión diaria desde su plantilla y extrae únicamente los conceptos, teoremas o problemas reutilizables. Conserva vacías las secciones personales que el agente no puede rellenar, en especial «Qué puedo recuperar sin mirar» y las demostraciones propias. Todo contenido matemático nuevo aportado por la IA queda en borrador, rojo y con fuente. El estudiante mantiene el control de confianza, nivel, fechas y dominio.

Antes de dar por cerrada la sesión, concilia cada repaso declarado como recuperado con su nota. Con la autorización del estudiante, actualiza `nivel_revision`, `ultima_revision` y `proxima_revision`; si falta autorización o evidencia, déjalo señalado explícitamente como pendiente en el diario. Ejecuta de nuevo el auditor y comprueba que ningún repaso ya cerrado siga apareciendo como vencido.

La sesión termina cuando el diario y las notas necesarias quedan actualizados y verificados, o cuando el estudiante decide explícitamente dejar ese registro pendiente.

## Modos de trabajo

### Tutor socrático

```text
Actúa como tutor socrático de [asignatura]. Trabajaremos solo [concepto].
Mi nivel actual y mi intento son: [texto].
No me des la solución completa. Haz una pregunta o proporciona una única pista que desbloquee el siguiente paso. Exige precisión en definiciones y notación.
```

### Revisor de demostraciones

```text
Revisa esta demostración línea por línea. Señala el primer salto no justificado, hipótesis no usadas, cuantificadores ambiguos y casos omitidos. No la reescribas hasta que yo intente corregirla.
[demostración]
```

### Corrector de problemas

```text
Evalúa mi solución como un profesor. Separa: planteamiento, validez lógica, cálculos, notación y claridad. Localiza el primer error decisivo y explícame por qué lo es. Después déjame corregirlo.
[enunciado e intento]
```

### Examen oral

```text
Hazme un examen oral breve sobre [tema]. Una pregunta cada vez. Alterna definición, ejemplo, contraejemplo, demostración y aplicación. No aceptes respuestas vagas. Al final, resume lagunas y propone tres ejercicios dirigidos.
```

### Generador de práctica

```text
Genera cinco ejercicios sobre [tema], graduados y sin solución visible. Deben comprobar comprensión, no repetición mecánica. Incluye al menos un caso frontera y un ejercicio que combine [concepto A] con [concepto B]. Guarda las soluciones para cuando las solicite.
```

## Antes de guardar una explicación

- [ ] ¿Puedo defender cada paso?
- [ ] ¿Las hipótesis están completas?
- [ ] ¿He probado ejemplos y casos frontera?
- [ ] ¿Sé de dónde procede el resultado?
- [ ] ¿Está escrito con mi propia comprensión?
