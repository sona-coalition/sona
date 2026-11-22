# Prácticas de actividad de Sona

*[English](./README.md) | **Español***

*Cómo una organización gestiona la actividad en sus sonas, expresado en el vocabulario de [Sona](../README.es.md). Independiente de cualquier herramienta o implementación — para una realización, véase el estándar de actividad de GitHub de la coalición; la correspondencia vive en el documento de mapeo.*

*Terminología (sona#8, 2026-11-17): los conceptos son ahora **actividad** (antes «work»), **agente** (antes «entity») y **jichi** (agente computacional). El título y la ruta de este documento conservan la palabra antigua por ahora — renombrarlos es una decisión aparte, porque otros repositorios enlazan aquí.*

## Organizaciones y actividad

Una **organización** es una colección de agentes. Por ser una colección, una organización es ella misma una agente — y como cualquier agente tiene una sona personal (la colección que es enteramente suya) y puede tener más sonas para los proyectos en los que trabaja. Todos los miembros de una organización son curadores de su sona personal.

La actividad es un cambio que una organización gestiona deliberadamente, y es de dos tipos:

* La **actividad interna** modifica una de las sonas de la organización.
* La **actividad externa** cambia algo fuera de ellas — el entorno más amplio, otras sonas, otros agentes.

Una **tarea** representa un elemento de actividad interna o externa.

## Las dos aprobaciones

Estas prácticas existen para garantizar dos actos:

1. **Aprobación de la propuesta.** Antes de que empiece la actividad, la propuesta es revisada y aceptada — por una agente **distinta del proponente**.
2. **Aprobación de la actividad.** Antes de que el resultado cambie la sona (o la cosa externa), la actividad es revisada y aceptada — por una agente **distinta de quien la realizó**.

Todo lo demás es mecanismo. Una aprobación dada por el proponente no es una aprobación, es solo un clic.

## Estados de las tareas y sus guardas

Una tarea pasa por los estados `Draft`, `Proposed`, `Accepted`, `Assigned`, `InReview`, `Done`. Los estados no son puertas que restringen el movimiento; cada estado lleva una **guarda** — lo que debería ser cierto mientras una tarea está en él — comprobada en la revisión. Antes de cambiar el estado de una tarea, comprueba la guarda del estado al que la mueves.

| Estado | Guarda — lo que debería ser cierto mientras una tarea está aquí | Por qué existe el estado |
| --- | --- | --- |
| `Draft` | La tarea existe pero aún no especifica la actividad con eficacia; «hecho» puede seguir sin estar claro. | Un lugar para refinar ideas sin exponerlas como actividad planificada. |
| `Proposed` | La tarea describe completamente la actividad, incluido lo que significa «hecho». El proponente solicita la **aprobación de la propuesta**. | La cola para la primera aprobación. |
| `Accepted` | Propuesta aprobada por una agente distinta del proponente; la aprobación queda registrada. | Actividad aprobada esperando capacidad. |
| `Assigned` | La tarea tiene una contribuyente asignada, que ha empezado o está a punto de empezar. | Actividad en curso. |
| `InReview` | La asignada juzga la actividad completa y ofrece evidencia. Esperando la **aprobación de la actividad** por una agente distinta de la asignada. | La cola para la segunda aprobación. |
| `Done` | Actividad aprobada y aceptada; la sona (o la cosa externa) lo refleja. | El registro de la actividad aceptada. |

Las tareas antiguas en `Done` se archivan periódicamente para que las vistas actuales se mantengan limpias; las tareas que no se van a hacer se archivan con el motivo registrado. El borrado se reserva para tareas creadas por error o como pruebas, y solo mientras están en `Draft`.

Las decisiones que la organización toma colectivamente las ejecuta un curador, porque solo los curadores tienen el poder de cambiar la sona. Una revisión de equipo — periódica, o continua para una organización pequeña — es donde ocurren las revisiones de propuestas y de actividad; lo que importa es que cada aprobación sea real y que el registro muestre dónde ocurrió.

## Principios

1. Toda contribución está asociada al menos a una tarea.
2. Una propuesta solo se acepta tras revisión por una agente distinta del proponente.
3. Una contribución solo se acepta tras revisión por una agente distinta de la contribuyente.
4. Las tareas son transitorias: todo lo que deba persistir no puede vivir únicamente dentro de una tarea.
5. El estado de cada tarea queda registrado y es visible para toda la organización.

Una implementación de estas prácticas (por ejemplo, el estándar de actividad de GitHub) deriva sus propias reglas de estos principios; el documento de mapeo muestra la derivación.
