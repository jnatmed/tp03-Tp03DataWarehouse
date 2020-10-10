
GUÍA DE LECTURA IV: Bases de datos multidimensionales

- 1.¿Qué se entiende por db multidimensional? 

R: Una base de datos multidimensional, es un datawarehouse que ofrece soluciones para la toma de decisiones, 

    + ¿Cómo se implementan?

R: La forma de implementarlo es a traves de diferentes tecnologias como ser ROLAP, MOLAP y HOLAP. Estas tecnologias ofrecen soluciones basados en esquemas del tipo ESTRELLA, COPO NIEVE o CONSTELACION DE HECHOS.

- 2.¿Qué características tienen las tablas de hechos? 

R: las tablas de hechos estan compuestas de medidas y claves, estas ultimas apuntan diferentes dimesiones. Las medidas, 
    + ¿y las de dimensiones?

R: La tabla de dimensiones representan aspectos de lo que se quiere explicar, son caracteristicas a describir de un objeto de estudio.

- 3.¿De qué depende la medida definida en una tabla de hechos?

- 4.Describa los diferentes esquemas de DW. 

R: Tenemos tres tipos de esquemas:

    * TIPO ESTRELLA: en este tipo se tiene una tabla de hecho, a partir de la cual se derivan dimensiones unicas por cada dimension, no hay ramificaciones y los atributos pueden formar una jerarquia  de orden parcial o total. 
    * TIPO COPO DE NIEVE: en este tipo, las dimensiones estan normalizadas, cada dimension puede tener relacionadas otras dimensiones conectadas a traves de llaves. Estas dimesiones describen un aspecto especifico de la dimension de la cual se produjo la especificacion.
    * TIPO CONSTELACION: la caracteristica principal es que hay mas de una tabla de hecho, las cuales comparten dimensiones entre si. 

- 5.¿Cómo puede describir la relación entre las tablas de dimensiones y el esquema copo de nieve?

R: La tabla de dimensiones representan aspectos de lo que se quiere explicar, son caracteristicas a describir de un objeto de estudio. Ahora bien, en el esquema de copo de nieve las dimensiones estan normalizadas de forma tal que se produce una ramificacion en otras tablas que explican algun aspecto de la tabla desagregada. 

- 6.¿Cuáles son los PROS y CONTRAS de un esquema copo de nieve en relación con un esquema de estrella?

|--ESQUEMA--|--PROS--|--CONTRA--|
|esquema copo de nieve|ahorra espacio|no tiene buena escalabilidad, muchos joins necesito para recuperar la informacion que necesito|
|esquema de estrella|

- 7.Dibuje un ejemplo de esquema de estrella pensando en un problema de gestión de datos obtenidos desde Twitter. 

    + ¿Qué dimensiones considera necesarias? 

    + ¿Cómo quedaría la tabla de hechos? Compartan los resultados en el Slack.

- 8.¿Qué función cumplen las jerarquías en una base de datos multidimensional? 

- 9.¿Cuál es su relación con la tabla de dimensiones? 
- 10.¿Cuales son las operaciones OLAP?
    + carga
    + refresh
    son las mas importantes
- 11.Escriba al menos 3 consultas utilizando las operaciones OLAP sobre el esquema de ejemplo del punto 7). Comparta los resultados en el Slack.
- 12.Identificar los PROS/CONTRAS de las tecnologías:
    + ROLAP, 
    + MOLAP y 
    + HOLAP.

Bibliografía sugerida:
Data Mining. Concepts and Techniques. Jiawei Han and Micheline Kamber. Capítulo 3.
