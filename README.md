# Principios de diseño

## Principio de Sencillez

- McIlroy	***Rule of Simplicity***	Design for simplicity; add complexity only where you must.
- McIlroy	***Rule of Clarity***	Clarity is better than cleverness.
- Durand	***Indescriptive Naming***	Programs should be written for people to read, and only incidentally for machines to execute
- Meyer	***Class Name rule***	El nombre de una clase siempre debe ser:
  - Un sustantivo, posiblemente calificado.
  - (Sólo para una clase diferida que describe una propiedad estructural) un adjetivo.

## Principio de Minimización

- Raymond	***La perfección (en diseño)*** se alcanza no cuando ya no hay nada que agregar, sino cuando ya no hay nada que quitar.	
- Durand	***Premature Optimization***	la optimización prematura es la raíz de todos los males

## Principio de Uniformidad

## Principio de Unicidad

- Durand	***Duplication***	No lo repitas ( DRY ) y también mantenlo simple, estúpido (KISS)
- ThomasHunt	***No te repitas.***	Cada pieza de conocimiento debe de tener una única e inequívoca representación dentro de un sistema.
- Meyer	***Symbolic Constant principle***	"No utilice una constante manifiesta, distinta de los elementos cero de la básica operaciones, en cualquier construcción que no sea una declaración constante simbólica"

## Principio de Modularidad

- Dijkstra	***Separación de Asuntos***	centrar la atención en algún aspecto": no significa ignorar los demás aspectos, es simplemente hacer justicia al hecho de que desde el punto de vista de este aspecto, el otro es irrelevante. Se trata de tener una mentalidad única y múltiple simultáneamente
- Larman	***Information Expert***	Assign responsibility to the class that has the information needed to fulfill it
- Meyer	***Class Consistency principle***	Todas las características de una clase deben pertenecer a una sola abstracción bien identificada.
- ThomasHunt	***Las abstracciones viven más que los detalles.***	Invertir en abstracción, no en la implementación. Las abstracciones pueden sobrevivir.
- McIlroy	***Rule of Modularity***	Write simple parts connected by clean interfaces.
- McIlroy	***Rule of Separation***	Separate policy from mechanism; separate interfaces from engines.
- Larman	***Indirection***	Assign the responsibility to an intermediate object to mediate between other components or services so that they are not directly coupled.
- Larman	***Pure Fabrication***	a class that does not represent a concept in the problem domain, specially made up to achieve low coupling, high cohesion, and the reuse potential thereof derived
- Martin	***Common Closure Principle***	Classes that change together are packaged together.
- Martin	***Common Reuse Principle***	Classes that are used together are packaged together.

## Principio del Problema

- ThomasHunt	***Usa un glosario del proyecto.***	Crea y mantén una única fuente de todos los términos y vocabulario específico de un proyecto.
- ThomasHunt	***Programa cerca del dominio***	Diseña y programa usando el mismo lenguaje usado por el usuario.
- McIlroy	***Rule of Representation***	Fold knowledge into data so program logic can be stupid and robust.
- Raymond	***Las estructuras de datos inteligentes y el código burdo funcionan mucho mejor que en el caso inverso.***	
- Meyer	***Linguistic Modular Units principle***	Los módulos deben corresponder a unidades sintácticas en el idioma utilizado.
- Meyer	***Class Elicitation principle***	La elicitación de clase es un proceso dual: sugerencia de clase, rechazo de clase.

## Principio de la Solución

- ThomasHunt	***Separa las vistas de los modelos.***	Gana flexibilidad a bajo coste diseñando tu aplicación en términos de modelos y vistas.
- Larman	***Controller***	should be used to deal with all system events of a use case, and may be used for more than one use case.
- Larman	***Creator***	
  - "Assign class B the responsibility to create object A if one, or preferably more, of the following apply:
    - Instances of B contain or compositely aggregate instances of A
    - Instances of B record instances of A
    - Instances of B closely use instances of A
    - Instances of B have the initializing information for instances of A and pass it on creation"

## Principio de Jerarquía

- Dijkstra	***Programación Estructurada***	
  - simplemente con la combinación de tres estructuras básicas, es suficiente para expresar cualquier función computable
  - programs flow from top to bottom following a hierarchical model"
- Parnas	***Hierarchical Structure***	The existence of the hierarchical structure assures us that we can "prune" off the upper levels of the tree and start a new tree on the old trunk. If we had designed a system in which the "low level" modules made some use of the "high level" modules, we would not have the hierarchy, wewouldfind it much harder to remove portions of the system, and "level" would not have much meaning in the system.
- Martin	***Acyclic Dependency Principle***	The dependency graph of packages must have no cycles.

## Principio de Interfaz

- McIlroy	***Rule of Least Surprise***	In interface design, always do the least surprising thing.
- McIlroy	***Rule of Silence***	When a program has nothing surprising to say, it should say nothing.
- Meyer	***Command-Query Separation principle***	Las funciones no deberían producir efectos secundarios abstractos.

## Principio de Ocultación

- Parnas	***Ocultación de Información***	Every module in the second decomposition is characterized by its knowledge of a design decision which it hides from all others. Its interface or definition was chosen to reveal as little as possible about its inner workings

## Principio de Cohesión

- Constantine	***Cohesion*** 	refers to the degree to which the elements inside a module belong together
- Larman	***High Cohesion***	to keep objects appropriately focused, manageable and understandable
- Martin	***Principio de responsabilidad única***	un objeto solo debería tener una única razón para cambiar.
- ThomasHunt	***Elimina los efectos entre cosas no relacionadas.***	Los componentes de un diseño son autónomos, independientes y tienen un único propósito bien definido.

## Principio de Acoplamiento

- Constantine	***Coupling*** 	is the degree of interdependence between software modules
- Larman	***Low Coupling***	Coupling is a measure of how strongly one element is connected to, has knowledge of, or relies on other elements
- Durand	***Tight Coupling***	Los módulos estrechamente acoplados son difíciles de reutilizar y también difíciles de probar
- ThomasHunt	***Minimiza el acoplamiento entre módulos.***	Evita el acoplamiento debido al código “tímido” y aplica la Ley de Demeter.

## Principio de Granularidad

## Principio de Autoprotección

- ThomasHunt	***Diseña con contratos.***	Recurre a los contratos para documentar y comprobar que el código hace realmente lo que tiene que hacer.
- ThomasHunt	***Usa afirmaciones para prevenir lo imposible.***	Las afirmaciones validan tu hipótesis. Úsalas para proteger el código de un mundo desconocido.
- ThomasHunt	***Usa excepciones para los problemas excepcionales.*** 	El abuso del uso de excepciones pueden convertir tu aplicación en poco legible y sotenible. Usa las excepciones para casos excepcionales.
- ThomasHunt	***No se puede escribir el software perfecto.***	Protege el código y a los usuarios de errores inevitables.
- Meyer	***Disciplined Exception Handling principle***	Sólo existen dos respuestas legítimas a una excepción que ocurre durante la ejecución de una rutina:
  - R1 •Reintentar: intenta cambiar las condiciones que llevaron a la excepción y ejecutar la rutina nuevamente desde el inicio.
  - R2 •Falla (también conocida como pánico organizado): limpiar el entorno, finalizar la llamada e informar la falla a la persona que llama.
  Además, las excepciones resultantes de algunas señales del sistema operativo (caso E3 de la clasificación de excepciones) pueden, en casos raros, justificar una respuesta de falsa alarma: determinar que la excepción es inofensiva y retomar la ejecución de la rutina donde comenzó."

## Principio de Clasificación

- Meyer	***Single Choice principle***	"Siempre que un sistema de software deba soportar un conjunto de alternativas, uno y sólo un módulo del sistema debe conocer su lista exhaustiva"
- Larman	***Polymorphism***	responsibility for defining the variation of behaviors based on type is assigned to the type for which this variation happens

## Principio de Especialización

- Meyer	***Taxomania rule***	Cada heredero debe introducir una característica, redeclarar una característica heredada o agregar una cláusula invariante
- Meyer	***“Is-a” rule of inheritance***	No haga que una clase B herede de una clase A a menos que de alguna manera pueda argumentar que se puede ver cada instancia de B también como una instancia de A.
- Meyer	***Rule of change***	No utilice la herencia para describir una relación percibida "es-un" si es posible que sea necesario cambiar los componentes del objeto correspondientes en tiempo de ejecución.
- Meyer	***Polymorphism rule***	La herencia es apropiada para describir una relación percibida "es-un" si entidades o componentes de estructura de datos del tipo más general pueden necesitar unirse a objetos del tipo más especializado.

## Principio de Sustitución

- Martin	***Principio de sustitución de Liskov***	Los objetos de un programa deberían ser reemplazables por instancias de sus subtipos sin alterar el correcto funcionamiento del programa

## Principio de Extensibilidad

- Martin	***Principio de abierto/cerrado***	Las entidades de software deben estar abiertas para su extensión, pero cerradas para su modificación.
- Meyer	***Open-Closed principle***	Los módulos deben estar abiertos y cerrados.
- Larman	***Protected Variations***	protects elements from the variations on other elements (objects, systems, subsystems) by wrapping the focus of instability with an interface and using polymorphism to create various implementations of this interface
