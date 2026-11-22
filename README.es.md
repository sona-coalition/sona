# Sona

*[English](./README.md) | **Español***

El término *Sona* se usa para describir una colección de conocimiento.

## Esquemas y Artefactos

El conocimiento se concibe como una colección de *Artefactos*. Cada Artefacto puede tener uno o más *Esquemas* que pretende satisfacer. La noción de Artefacto que satisface un Esquema generaliza muchas situaciones que se dan en el mundo, como ilustra la tabla siguiente[^1].

|Artefacto |satisface|Esquema|
|------|-----|----|
|Respuesta|responde a|Pregunta|
|Acción|completa|Tarea|
|Solución|satisface|Criterios|
|Elemento|es miembro de|Conjunto|
|Diseño|cumple|Requisitos|
|Sistema|implementa|Diseño de sistema|
|Programa|cumple|Especificación|
|Objeto|tiene tipo|Clase|
|Objeto|implementa|Interfaz|
|Objeto|implementa|Rasgo (Trait)|
|Código|pasa|Pruebas|
|Demostración|demuestra|Teorema|
|Modelo|satisface|Axiomas|

En algunos casos puede ser fácil determinar si un Artefacto satisface un Esquema. Por ejemplo, normalmente es sencillo determinar si un elemento pertenece a un conjunto o no. Sin embargo, en otros casos la situación puede ser más sutil. Podemos hablar de cuánto cumple un Diseño unos Requisitos.

## Calidad y Medida

Un Esquema consiste en una definición de *Calidad* junto con una función llamada *Medida* que determina la Calidad de un Artefacto concreto. La definición de Calidad del esquema permite comparar los resultados de la función de Medida.

## Agentes

Las Sonas no existen aisladas. Las usan y las modifican los *Agentes*. Los Agentes pueden ser:

* Humanos
* Jichi (computacionales)
* Colecciones de otros Agentes

Esta lista no pretende ser exhaustiva. En general, un Agente es cualquier cosa capaz de usar o modificar una Sona. (La palabra nombra un rol: un agente es quien asume la responsabilidad de una actividad en una Sona — en línea con el Agent de la ontología de procedencia.)

*Nota de terminología (sona#8, 2026-11-17): Agente era antes «entity»; Jichi (机气 — máquina + energía vital) nombra a los agentes computacionales donde antes se decía «computational entity»; Actividad nombra lo que antes se llamaba «work».*

## Contribuciones, Contribuyentes y Curadores

Las modificaciones de una Sona se llaman *Contribuciones*. Las Contribuciones normalmente están pensadas para mejorar la Calidad de la Sona.

Con respecto a una Sona, un Agente puede desempeñar uno de dos roles:

* *contribuyente* — quien puede
  * Proponer Contribuciones a la Sona.
* *curador* — quien puede
  * Proponer Contribuciones a la Sona
  * Aceptar y rechazar Contribuciones propuestas.

## Sonapana y Sona Personal

Las Sonas se crean dentro de una *Sonapana* — una red de Sonas. Dentro de la Sonapana, cada Agente tiene una Sona de la que es su único Curador. Es a través de esta *sona personal* que los agentes hacen y aceptan Contribuciones, mejorando así la calidad de las Sonas individuales y de la Sonapana en su conjunto. Se podría pensar en la sona personal como la huella digital del agente.

## Subsonas

Las Sonas pueden componerse de otras Sonas, que en este contexto se llaman *Subsonas*. Las Subsonas pueden usarse para separar componentes clave de una Sona global. Por ejemplo, dos Agentes Abelardo y Eloísa pueden tener cada uno una Subsona dentro de sus Sonas Personales de la que ambos actúan como Curadores.

## Privado y Público

Una Subsona que solo pueden ver los Curadores de esa Sona se llama *privada*. Las Subsonas de la Sona que no son Privadas se consideran públicas. Nótese que las partes públicas de una Sona son accesibles a los Contribuyentes de esa Sona. Las partes públicas de una Sona pueden hacerse accesibles a cualquier Agente de la Sonapana por un Contribuyente de esa Sona.

## Esquemas como Artefactos

Un Esquema puede ser un Artefacto para otro Esquema. Un Sistema puede implementar un Diseño de sistema, pero ese Diseño de sistema puede a su vez cumplir unos Requisitos de sistema.

## Más detalles

| Ruta | Qué es |
| --- | --- |
| [Estándar de actividad](./work-standard/README.md) | Cómo una organización gestiona tareas. (Su título conserva la palabra antigua por ahora; en la terminología actual el concepto es *actividad* — véase la nota de terminología más arriba.) |

[^1]: Nótese la influencia de la [Teoría de Tipos de Martin-Löf](https://www.cse.chalmers.se/~peterd/papers/MartinLöf1984.pdf).
