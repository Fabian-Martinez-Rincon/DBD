
<div align='center'>

# Finales 

![](https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExd2lpd3A1emYyajVvOGV2MjBjZmF6N2FvNGUxMno1dHltZWp1NnJhciZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/Wkr0EKIsWitJm/giphy.gif)

</div>

> [!NOTE]  
> Es un recopilatorio de preguntas, algunas pueden que esten bien y otras mal porque depende de la interpretación o justificación de cada uno, en este caso vamos a tratar justificar todo en base al libro

## Temario de Preguntas

- [Modelado](#modelado)
- [Consultas](#consultas)
- [Seguridad e Integridad de los Datos]()

> [!TIP]
> Responder todo, ya fuee

---

### Sacado del libro

![image](https://github.com/Fabian-Martinez-Rincon/Fabian-Martinez-Rincon/assets/55964635/1db36f21-78a1-4acb-ba6b-36e39ac6d926)

Las funciones de agregación en una consulta



- [ ] a) Pueden ir en el SELECT
- [ ] b) Pueden ir en el WHERE
- [ ] c) Pueden ir en el HAVING
- [ ] d) Pueden aparecer sin otros atributos en el select
- [ ] e) Todas son correctas
- [ ] f) A, C y D son correctas
- [ ] g) A, B y C son correctas
- [ ] h) A y C son correctas

<details><summary>👀 Respuesta</summary>

- Falta responder

En el SELECT si, en el WHERE no

</details>

---

Un checkPoint en hambientes concurrentes

- [ ] a) Solo se genera si se utiliza el protocolo de HDE
- [ ] b) Solo se genera si se utiliza el protocolo de dos fases
- [ ] c) Se aplica en el protocolo de doble paginación
- [ ] d) Se coloca siempre entre dos transacciones, cuando ninguna esta activa
- [ ] e) Todas las anteriores
- [ ] f) Algunas de las anteriores
- [ ] g) Ninguna de las anteriores

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---


La propiedad de aislamiento

- [ ] a) No se aplica en un ambiente concurrente
- [ ] b) Se aplica en un ambiente concurrente
- [ ] c) No se aplica en un ambiente monousuario
- [ ] d) Se aplica en un ambiente monousuario
- [ ] e) Algunas de las anteriores
- [ ] f) Ninguna de las anteriores

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

Se tiene una jerarquia total exclusiva en el modelo conceptual. Al pasar dicho modelo al logico se debe decidir que hacer con la misma

- [ ] a) Se puede dejar solo al padre
- [ ] b) Se puede dejar solo a los hijos
- [ ] c) Se puede dejar todas las entidades
- [ ] d) Todas las anteriores son validas
- [ ] e) Algunas de las anteriores son validas
- [ ] f) No tengo datos suficientes para responder

<details><summary>👀 Respuesta</summary>

> [!IMPORTANT]
> En la foto de donde lo saque estaba corregida

- Todas las anteriores son validas

</details>

---

Una dependencia multivaluada

- [ ] a) Puede generar repetición innecesaria de información
- [ ] b) Genera repetición de información si no es una dependencia multivaluada trivial
- [ ] c) Genera repetición innecesaria de información
- [ ] d) Todas las anteriores son correctas
- [ ] e) Algunas de las anteriores son correctas  
- [ ] f) Ninguna de las anteriores es correcta

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

Un esquema fisico que no tiene dependencias parciales esta en:

- [ ] a) 3FN
- [ ] b) 5FN
- [ ] c) 2FN
- [ ] d) 1FN
- [ ] e) 4FN
- [ ] f) BCNF
- [ ] g) Todas las anteriores
- [ ] h) Algunas de las anteriores
- [ ] i) Ninguna de las anteriores

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

Suponga que tiene tablas

- Alumnos = (idAlumno, nombre, edad)
- Materias = (idMateria, nombre, año)
- Inscribe = (idAlumno, idMateria)

Indique cual sentencia AR muestra al alumno con las materias en las que se inscribió.

Como referencia

P proyeccción, S selección, I Intersección, R renombre


- [ ] a) Pnombre (alumnos |x| materias |x| inscribe)
- [ ] b) Pnombre (alumnos) |x| Pnombre (materias)
- [ ] c) Pnombre (alumnos) |x| Pnombre (materias) |x| inscribe
- [ ] d) Palumnos.nombre, materias.nombre (alumnos |x| materias)
- [ ] e) Ninguna de las anteriores

<details><summary>👀 Respuesta</summary>

> [!IMPORTANT]
> En la foto de donde lo saque estaba corregida

- Ninguna de las anteriores

</details>

---

La siguiente consulta SQL: SELECT * FROM B INNER JOIN A ON (A.id = B.id)

- [ ] a) Retorna solo las filas de A que tengan coincidencia con las filas de B en el atributo id.
- [ ] b) Retorna solo las filas de B que no tengan coincidencia con las filas de A en el atributo id.
- [ ] c) Proyecta solo las columnas de A
- [ ] d) Retorna todas las filas de B
- [ ] e) Proyecta solo las columnas de B
- [ ] f) Hay más de una respuesta correcta
- [ ] g) Todas las anteriores son correctas
- [ ] h) Ninguna de las anteriores es correcta

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

La función de agregación SUM de SQL:

- [ ] a) Requiere de una cláusula GROUP BY.
- [ ] b) Calcula el máximo para una columna de la tabla.
- [ ] c) Cuenta los valores distintos para una fila de la tabla
- [ ] d) Se puede utilizar en la clausula HAVING sin utilizar un GROUP BY
- [ ] e) Hay más de una opcion válida 
- [ ] f) Todas las anteriores son correctas
- [ ] g) Ninguna de las anteriores es correcta

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

La operación de proyección en Álgebra Relacional:

- [ ] a) Es un operador binario
- [ ] b) Es un operador unitario
- [ ] c) Es equivalente a la clausula "Where" de SQL
- [ ] d) Es equivalente a la clausula "Order By" de SQL
- [ ] e) Puede proyectar elementos repetidos
- [ ] f) Hay más de una opción valida
- [ ] g) Todas las opciones anteriores son válidas
- [ ] h) Ninguna de las opciones anteriores es válida

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

Si una entrada en el registro bitácora tiene el siguiente formato: "\<T1, dato, valor anterior, valor nuevo>"

- [ ] a) Utiliza bitácora con modificación diferida
- [ ] b) Utiliza el protocolo de hora de hora de entrada
- [ ] c) Utiliza bítacora con modificación inmediata
- [ ] d) Utiliza el protocolo de página en la sombra
- [ ] e) Hay más de una opción valida
- [ ] f) Todas las opciones anteriores son válidas
- [ ] g) Ninguna de las opciones anteriores es válida

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

Dada una transacción T1 que obtiene un bloqueo exclusivo sobre el dato D1 y otra transacción T2 que obtiene un bloque exclusivo sobre el dato D2, entonces:

- [ ] a) T1 no deberá esperar a que T2 libere el dato si desea leer D2
- [ ] b) T2 no deberá esperar a que T1 libere el dato si desea leer D1
- [ ] c) T1 no debera esperar a que T2 libere el dato para poder escribir D2
- [ ] d) T2 no deberá esperar a que T1 libere el dato para poder escribir D1
- [ ] e) T1 deberá esperar a que T2 libere el dato si desea leer D2
- [ ] f) T2 deberá esperar a que T1 libere el dato si desea leer D1
- [ ] g) Hay más de una opción valida
- [ ] h) Todas las opciones anteriores son válidas
- [ ] i) Ninguna de las opciones anteriores es válida

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

Una jerarquía con cobertura Parcial y Exclusiva (P, E), al pasar al modelo lógico:

- [ ] a) No es posible dejar solamente las entidades hijas
- [ ] b) No se puede quitar la entidad generalizadora
- [ ] c) Se deja la jerarquia completa sin relacionar las entidades que la componen
- [ ] d) No se realiza cambio alguno
- [ ] e) Hay más de una opción válida
- [ ] f) Todas las opciones anteriores son válidas
- [ ] g) Ninguna de las opciones anteriores es válida

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

Una relación entre dos entidades en un modelo conceptual:

- [ ] a) Puede no tener cardinalidad
- [ ] b) No puede contener un atributo opcional polivalente
- [ ] c) No puede contener un atributo compuesto monovalente
- [ ] d) No debe contener atributos
- [ ] e) No puede contener más de un atributo opcional monovalente
- [ ] f) Puede contener un atributo identificador
- [ ] g) Hay más de una opción válida 
- [ ] h) Todas las opciones anteriores son válidas
- [ ] i) Ninguna de las opciones anteriores es válida

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

Un identificador compuesto de una entidad en el modelo conceptual, cuando se realiza el pasaje al logico relacional:


- [ ] a) Se debe transformar debido a que el modelo lógico relacional no acepta este tipo de identificadores
- [ ] b) Se deja sin modificación alguna
- [ ] c) Se debe separar en distintos atributos y uno de ellos será elegido identificador de la entidad
- [ ] d) Se elimina del modelo lógico relacional
- [ ] e) Hay más de una opción válida
- [ ] f) Todas las opciones anteriores son válidas
- [ ] g) Ninguna de las opciones anteriores es válida


<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

Una clave foránea en el modelo físico

- [ ] a) No puede ser opcional
- [ ] b) No acepta valores repetidos
- [ ] c) Puede ser clave primaria y foránea al mismo tiempo y en la misma tabla
- [ ] d) Hay más de una opción válida
- [ ] e) Todas las opciones anteriores son válidas
- [ ] f) Ninguna de las opciones anteriores es válida

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

En el algebra Relacional la expresión A U B

- [ ] a) Requiere que A y B contengan la misma cantidad de elementos
- [ ] b) Requiere que el esquema de B se encuentre contenido en el esquima de A
- [ ] c) Requiere que el esquima de A se encuentre contenido en el esquema de B
- [ ] d) Hay más de una opción valida
- [ ] e) Todas las opciones anteriores son válidas
- [ ] f) Ninguana de las opciones anteriores es válida

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

¿Cuál de las siguientes afirmaciones es cierca acerca de la normalización de base de datos?

- [ ] a) La normalización es el proceso de agregar redundancia a una base de datos para mejorar la eficiencia de las consultas
- [ ] b) La normalización es el proceso de eliminar la redundancia en una base de datos para evitar problemas de inconsistencia de datos
- [ ] c) La normalización es el proceso de crear copias de seguridad de una base de datos para protegerla de pérdidas de datos
- [ ] d) La normalización es el proceso de cifrar los datos en una base de datos para proteger su confidencialidad
- [ ] e) Todas las opciones anteriores son verdaderas
- [ ] f) Algunas de las opciones anteriores son verdaderas
- [ ] g) Ninguna de las opciones anteriores es verdadera

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

¿Cuál de las siguientes afirmaciones es verdadera sobre el modelo Entidad-Relación(ER)?

- [ ] a) El modelo ER es un modelo lógico que se enfoca en la implementación física de la base de datos
- [ ] b) Las entidades en el modelo ER representan relaciones entre los datos
- [ ] c) Las relaciones en un modelo ER representan vínculos entre las entidades
- [ ] d) El modelo ER no incluye atributos para las entidades y relaciones
- [ ] e) Todas las opciones anteriores son verdaderas
- [ ] f) Algunas de las opciones anteriores son verdaderas
- [ ] g) Ninguna de las opciones anteriores es verdadera

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

¿Cuál de las siguientes técnicas es útil para optímizar consultas SQL en una base de datos?

- [ ] a) Usar subconsultas en lugar de productos de tablas
- [ ] b) Evitar el uso de índices para las claves primarias
- [ ] c) Usar funciones de agregación en lugar de GROUP BY
- [ ] d) Usar el operador LIKE en lugar de igualdad para comparaciones de cadenas
- [ ] e) Todas las opciones anteriores son verdaderas
- [ ] f) Algunas de las opciones anteriores son verdaderas
- [ ] g) Ninguna de las opciones anteriores es verdadera

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

¿Cuál de las siguientes afirmaciones es verdadera sobre el modelo lógico relacional?

- [ ] a) Se pueden tener atributos compuestos
- [ ] b) Se pueden tener atributos derivados
- [ ] c) No se pueden tener identificadores compuestos
- [ ] d) Se pueden tener atributos polivalentes
- [ ] e) Todas las opciones anteriores son verdaderas
- [ ] f) Algunas de las opciones anteriores son verdaderas
- [ ] g) Ninguna de las opciones anteriores es verdadera

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

¿Cuál de las siguientes afirmaciones es cierta acerca de la integridad referencial en una base de datos relacional?

- [ ] a) La integridad referencial garantiza que cada registro en una tabla tenga un valor único en su clave primaria.
- [ ] b) La integridad referencial asegura que los valores en una tabla sean válidos en referencia a otra tabla.
- [ ] c) La integridad referencial solo se aplica a las tablas que tienen una clave foránea.
- [ ] d) La integridad referencial no es necesaria en una base de datos relacional.
- [ ] e) Todas las opciones anteriores son verdaderas
- [ ] f) Algunas de las opciones anteriores son verdaderas
- [ ] g) Ninguna de las opciones anteriores es verdadera

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

Un atributo derivado posee información disponible en una entidad. Si esa información no estuviera sería posible aún calcularla. Entonces

- [ ] a) Contiene información redundante y puede quitarse del modelo
- [ ] b) Contiene información redundante y debe quitarse del modelo 
- [ ] c) No contiene información redundante y debe dejarse en el modelo 
- [ ] d) No contiene información redundante
- [ ] e) Todas las anteriores son correctas
- [ ] f) Algunas de las anteriores son correctas
- [ ] g) Ninguna de las anteriores es correcta

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

¿Cuáles de las siguientes cláusulas son necesarias para una consulta de selección de datos en SQL?

- [ ] a) SELECT
- [ ] b) FROM
- [ ] c) WHERE
- [ ] d) Todas las anteriores
- [ ] e) Algunas de las anteriores
- [ ] f) Ninguna de las anteriores

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

¿Qué afirmación describe mejor la relacion entre la cantidad de tuplas o filas generadas por las cláusulas LEFT JOIN e INNER JOIN en una consulta SQL?

- [ ] a) Generan igual cantidad de tuplas o filas
- [ ] b) LEFT JOIN genera menos cantidad de tuplas o filas que INNER JOIN
- [ ] c) LEFT JOIN genera más cantidad de tuplas o filas que INNER JOIN
- [ ] d) LEFT JOIN puede generar igual cantidad de tuplas o filas que INNER JOIN
- [ ] e) Todas las anteriores son correctas
- [ ] f) Algunas de las anteriores son correctas
- [ ] g) Ninguna de las anteriores es correcta

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

¿Cuál de las siguientes afirmaciones es verdadera acerca de las tablas en una base de datos?

- [ ] a) Tienen una clave primaria
- [ ] b) No pueden tener claves candidatas
- [ ] c) Deben tener al menos una clave foránea
- [ ] d) No pueden tener claves foráneas
- [ ] e) Todas las anteriores son correctas
- [ ] f) Algunas de las anteriores son correctas
- [ ] g) Ninguna de las anteriores es correcta

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

¿Qué significa la condición de idempotencia en el contexto de las transacciones en una base de datos?

- [ ] a) Garantiza que una transacción se pueda ejecutar varias veces con el mismo resultado
- [ ] b) Garantiza que una transacción que ha fallado se pueda ejecutar varias veces con el mismo resultado
- [ ] c) Garantiza que una transacción que se ha registrado de transacciones se pueda ejecutar varias veces con el mismo resultado
- [ ] d) Todas las anteriores son correctas
- [ ] e) Algunas de las anteriores son correctas
- [ ] f) Ninguna de las anteriores es correcta

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

Una jerarquia con cobertura Parcial y Exclusiva (P, E), al pasar al modelo lógico:

- [ ] a) Es posible dejar solamente las entidades hijas
- [ ] b) Se puede quitar la entidad generalizadora
- [ ] c) Se deja la jerarquia completa sin relacionar las entidades que la componen
- [ ] d) No se realiza cambio alguno
- [ ] e) Hoy más de una opción válida
- [ ] f) Todas las opciones anteriores son válidas
- [ ] g) Ninguna de las opciones anteriores es válida

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

Una relación entre dos entidades en un modelo conceptual:

- [ ] a) Puede no tener cardinalidad
- [ ] b) No puede contener un atributo opcional polivalente
- [ ] c) No puede contener un atributo compuesto monovalente
- [ ] d) No debe contener atributos
- [ ] e) Puede contener más de un atributo opcional monovalente
- [ ] f) Puede contener un atributo identificador
- [ ] g) Hay más de una opción válida
- [ ] h) Todas las opciones anteriores son válidas
- [ ] i) Ninguna de las opciones anteriores es válida

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

Una clave foránea en una tabla del modelo físico

- [ ] a) No puede ser opcional
- [ ] b) No acepta valores repetidos
- [ ] c) No es clave primaria en ninguna tabla del modelo físico
- [ ] d) Hay mas de una opción válida
- [ ] e) Todas las opciones anteriores son válidas
- [ ] f) Ninguna de las opciones anteriores es válida

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

En el algebra Relacional la expresión A U B

- [ ] a) Requiere que A y B contengan la misma cantidad de elementos
- [ ] b) Requiere que el esquema de B se encuentre contenido en el esquema de A
- [ ] c) Requiere que el esquema de A se encuentre contenido en el esquema de B
- [ ] d) Hay más de una opción válida
- [ ] e) Todas las opciones anteriores son válidas
- [ ] f) Ninguna de las opciones anteriores es válida

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

La función de agregación AVG de SQL:

- [ ] a) Requiere de una cláusula GROUP BY.
- [ ] b) Calcula el máximo para una columna de la tabla.
- [ ] c) Cuenta los valores distintos para una fila de la tabla
- [ ] d) Se puede utilizar en la clausula HAVING sin utilizar un GROUP BY
- [ ] e) Hay más de una opcion válida
- [ ] f) Todas las anteriores son correctas
- [ ] g) Ninguna de las anteriores es correcta

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

La operación de diferencia (-) en Álgebra Relacional:

- [ ] a) Es un operador binario
- [ ] b) Es un operador unitario
- [ ] c) Es equivalente a la clausula "Where" de SQL
- [ ] d) Es equivalente a la clausula "Order By" de SQL
- [ ] e) Puede proyectar elementos repetidos
- [ ] f) Hay más de una opción válida
- [ ] g) Todas las opciones anteriores son válidas
- [ ] h) Ninguna de las opciones anteriores es válida

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

El algebra relacional

- [ ] a) Es un lenguaje de consultas teorico de BD relacional que define como hacer las operaciones de manipulacion de datos
- [ ] b) Es un lenguaje de consultas teorico de BD entidad relación que define como hacer las operaciones de manipulación de datos
- [ ] c) Es un lenguaje de consultas teorico de BD relacional que define solamente el resultado esperado en la respuesta 
- [ ] d) Es un lenguaje de consultas teorico de BD entidad relación que define solamente el resultado esperado en la respuesta.

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

La clausula EXIST en SQL

- [ ] a) Solo se aplica en una operación de consulta
- [ ] b) Necesita necesariamente una subconsulta
- [ ] c) No utiliza en el select que la contiene una función de agregación
- [ ] d) Todas las anteriores
- [ ] e) Algunas de las anteriores
- [ ] f) Ninguna de las anteriores

<details><summary>👀 Respuesta</summary>  

- Falta responder

</details>

---

La clausula DELETE en SQL

- [ ] a) Es una clausula de definicion de datos
- [ ] b) Es una clausula de manipulacion de datos
- [ ] c) Puede alcanzar el estado Cometido
- [ ] d) Todas las anteriores
- [ ] e) Ninguna de las anteriores

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

Una transacción que alcanza el espacio de fallada

- [ ] a) Puede volver a activarse
- [ ] b) Puede alcanzar el estado Abortada
- [ ] c) Puede alcanzar el estado Cometido
- [ ] d) Todas las anteriores
- [ ] e) Ninguna de las anteriores

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

Ante dos transacciones concurrentes que generan un problema de integridad contra la BD

- [ ] a) Es preferible que haya un deadlock a tener inconsistencia
- [ ] b) Es preferible que haya inconsistencia si el deadlock produce inanición
- [ ] c) Es preferible que haya inconsistencia antes que tener deadlock
- [ ] d) Todas las anteriores
- [ ] e) Ninguna de las anteriores

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

Un atributo derivado

- [ ] a) Representa un dato que está presente de otra forma en el modelo
- [ ] b) Puede estar en el modelo logico
- [ ] c) Puede estar en el modelo fisico
- [ ] d) Hay más de una opción válida
- [ ] e) Todas las opciones anteriores son válidas
- [ ] f) Ninguna de las opciones anteriores es válida

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

Un atributo polivalente sobre el modelo conceptual

- [ ] a) Indica que el atributo esta formado por varios atributos simples
- [ ] b) Indica que el atributo puede tener multiples valores, pero no puede ser nulo
- [ ] c) Indica que el atributo puede tener multiples valores, pero debe aceptar ser nulo
- [ ] d) Todas las anteriores son correctas
- [ ] e) Algunas de las anteriores son correctas
- [ ] f) Ninguna de las anteriores es correcta

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

Una relación del modelo lógico cuando se pasa al fisico

- [ ] a) Siempre se convierte en tabla
- [ ] b) En algún caso puede no convertirse en tabla
- [ ] c) No se convierte en tabla
- [ ] d) Todas las anteriores son correctas
- [ ] e) Algunas de las anteriores son correctas
- [ ] f) Ninguna de las anteriores es correcta

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

Una jerarquia parcial superpuesta, donde el padre tiene tres hijos, cuando se convierte al modelo fisico

- [ ] a) Puede quedar solo el padre
- [ ] b) Puede quedar solo los hijos
- [ ] c) Puede quedar todo con relaciones es un
- [ ] d) Todas las anteriores son correctas
- [ ] e) Algunas de las anteriores son correctas
- [ ] f) Ninguna de las anteriores es correcta

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

Un identificador simple de una tabla

- [ ] a) Puede ser un atributo con valor nulo
- [ ] b) Puede ser un atributo polivalente
- [ ] c) Puede ser un atributo derivado
- [ ] d) Todas las anteriores son correctas
- [ ] e) Algunas de las anteriores son correctas
- [ ] f) Ninguna de las anteriores es correcta

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

Un identificador de una entidad sobre el modelo lógico, cuando dicha entidad se convierte en tabla sobre el fisico

- [ ] a) Puede ser clave primaria
- [ ] b) Puede ser clave candidata
- [ ] c) Puede ser clave secundaria
- [ ] d) Todas las anteriores son correctas
- [ ] e) Algunas de las anteriores son correctas
- [ ] f) Ninguna de las anteriores es correcta

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

Una clave primaria en el esquema fisico de una BD

- [ ] a) Puede haber sido clave candidata
- [ ] b) No ha sido clave candidata
- [ ] c) Ha sido identificador en el esquema lógico
- [ ] d) No ha sido identificador en el esquema conceptual
- [ ] e) Ninguna de las anteriores

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

Para la construcción del modelo ER-Conceptual, es necesario

- [ ] a) Contar con la definición del DBMS a utilizar
- [ ] b) Contar con la descripción detallada de las necesidades de usuario
- [ ] c) Contar con un DBA experimentado en el DBMS a utilizar
- [ ] d) Todas las anteriores son correctas
- [ ] e) Ninguna de las anteriores

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

Un ciclo de entidades

- [ ] a) Representa una solución donde se repite información
- [ ] b) Debe ser quitado del modelo logico
- [ ] c) Aparece en el modelo fisico y repite información
- [ ] d) Todas las anteriores son correctas
- [ ] e) Ninguna de las anteriores

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

Una entidad en el esquema fisico

- [ ] a) No puede tener atributos polivalentes
- [ ] b) No puede tener atributos compuestos
- [ ] c) Tiene al menos un identificador
- [ ] d) Puede tener más de un identificador
- [ ] e) Algunas de las anteriores
- [ ] f) Ninguna de las anteriores

<details><summary>👀 Respuesta</summary>

> [!IMPORTANT]
> En la foto de donde lo saque estaba corregida

- Ninguna de las anteriores

</details>


---

Una relación recursiva en el esquema lógico

- [ ] a) Solo tiene un identificador
- [ ] b) Puede tener más de un identificador
- [ ] c) Puede tener más de un atributo
- [ ] d) No puede tener atributos con cardinalidad máxima N
- [ ] e) Algunas de las anteriores
- [ ] f) Ninguna de las anteriores

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

Un ciclo de relaciones en el esquema conceptual

- [ ] a) Puede generar redundancia
- [ ] b) Si genera redundacia, luego debe eliminar el ciclo del proceso d(se corta)
- [ ] c) Siempre es entre 4 o más entidades
- [ ] d) Algunas de las anteriores
- [ ] e) Ninguna de las anteriores

<details><summary>👀 Respuesta</summary>

> [!IMPORTANT]
> En la foto de donde lo saque estaba corregida

- Puede generar redundancia

</details>

---

Un atributo derivado 

- [ ] a) Puede ser clave
- [ ] b) Puede tener valor nulo
- [ ] c) Puede ser polivalente
- [ ] d) Todas las anteriores son correctas
- [ ] e) Ninguna de las anteriores

<details><summary>👀 Respuesta</summary>

- Falta responder

</details>

---

La operación de proyección en Álgebra Relacional

- [ ] a) Es un operador binario
- [ ] b) Es un operador unitario
- [ ] c) Es equivalente a la clausula "Where" de SQL
- [ ] d) Es equivalente a la clausula "Order By" de SQL
- [ ] e) Puede proyectar elementos repetidos
- [ ] f) Hay más de una opción válida
- [ ] g) Todas las opciones anteriores son válidas
- [ ] h) Ninguna de las opciones anteriores es válida

<details><summary>👀 Respuesta</summary>

> [!IMPORTANT]
> En la foto de donde lo saque estaba corregida

- Es un operador unitario

</details>

---

Dada una transacción T1 que obtiene un bloqueo exclusivo sobre el dato D1 y otra transacción T2 que obtiene un bloqueo exclusivo sobre el dato D2, entonces:

- [ ] a) T1 no deberá esperar a que T2 libere el dato si desea leer D2
- [ ] b) T2 no deberá esperar a que T1 libere el dato si desea leer D1
- [ ] c) T1 no debera esperar a que T2 libere el dato para poder escribir D2
- [ ] d) T2 no deberá esperar a que T1 libere el dato para poder escribir D1
- [ ] e) T1 deberá esperar a que T2 libere el dato si desea leer D2
- [ ] f) T2 deberá esperar a que T1 libere el dato si desea leer D1
- [ ] g) Hay más de una opción valida
- [ ] h) Todas las opciones anteriores son válidas
- [ ] i) Ninguna de las opciones anteriores es válida

<details><summary>👀 Respuesta</summary>

> [!IMPORTANT]
> En la foto de donde lo saque estaba corregida

- Hay más de una opción valida

</details>

---

¿Cuál de las siguientes afirmaciones es verdadera sobre el modelo lógico relacional?

- [ ] a) Se pueden tener atributos compuestos
- [ ] b) Se pueden tener atributos derivados
- [ ] c) No se pueden tener identificadores compuestos
- [ ] d) Se pueden tener atributos polivalentes
- [ ] e) Todas las opciones anteriores son verdaderas
- [ ] f) Algunas de las opciones anteriores son verdaderas
- [ ] g) Ninguna de las opciones anteriores es verdadera

<details><summary>👀 Respuesta</summary>

> [!IMPORTANT]
> En la foto de donde lo saque estaba corregida

- Se pueden tener atributos derivados

</details>

---

Si en una consulta SQL se utiliza la cláusula GROUP BY

- [ ] a) Se debe utilizar la cláusula HAVING
- [ ] b) Se puede indicar la condición del grupo en la cláusula WHERE
- [ ] c) Se debe utilizar al menos una función de agregación
- [ ] d) Todas las anteriores
- [ ] e) Algunas de las anteriores
- [ ] f) Ninguna de las anteriores

<details><summary>👀 Respuesta</summary>

> [!IMPORTANT]
> En la foto de donde lo saque estaba corregida

- Se debe utilizar al menos una función de agregación

</details>

---

En algebra relacional la empresa A |x| B da el mismo resultado que:

- [ ] a) A x B
- [ ] b) A x B si entre las tablas A y B no hay atributo común
- [ ] c) B |x| A
- [ ] d) Todas las anteriores
- [ ] e) Ninguna de las anteriores

<details><summary>👀 Respuesta</summary>

> [!IMPORTANT]
> En la foto de donde lo saque estaba corregida

- B |x| A

</details>

---

En el algebra relacional la expresión A - B

- [ ] a) Requiere que A y B contengan la misma cantidad de elementos
- [ ] b) Requiere que el esquema de B se encuentre contenido en el esquema de A
- [ ] c) Requiere que el esquema de A se encuentre contenido en el esquema de B
- [ ] d) Hay más de una opción válida
- [ ] e) Todas las opciones anteriores son válidas
- [ ] f) Ninguna de las opciones anteriores es válida

<details><summary>👀 Respuesta</summary>

> [!IMPORTANT]
> En la foto de donde lo saque estaba corregida

ESTA CORREGIDA COMO ERROR

- Hay más de una opción válida 

</details>

---

La función de agregación SUM() de SQL:

- [ ] a) Necesita de una cláusula GROUP BY
- [ ] b) Calcula el máximo para una columna de la tabla
- [ ] c) Puede contar los valores distintos para una fila de la tabla
- [ ] d) Se puede utilizar en la clausula HAVING sin utilizar un GROUP BY 
- [ ] e) Hay más de una opcion válida
- [ ] f) Todas las anteriores son correctas
- [ ] g) Ninguna de las anteriores es correcta

<details><summary>👀 Respuesta</summary>

> [!IMPORTANT]
> En la foto de donde lo saque estaba corregida

- Ninguana de las anteriores es correcta

</details>

---

Una clave candidata en una tabla del modelo físico

- [ ] a) Es un atributo o conjunto de atributos que juntos se pueden repetir dentro de la misma tabla.
- [ ] b) Es un atributo o conjunto de atributos que juntos conforman un atributo opcional
- [ ] c) No puede estar conformada por más de un atributo
- [ ] d) Puede estar conformada por más de un atributo opcional
- [ ] e) Puede estar conformada por más de un atributo monovalente obligatorio
- [ ] f) Hay más de una opción válida
- [ ] g) Todas las opciones anteriores son válidas
- [ ] h) Ninguna de las opciones anteriores es válida

<details><summary>👀 Respuesta</summary>

> [!IMPORTANT]
> En la foto de donde lo saque estaba corregida

- Puede estar conformada por más de un atributo monovalente obligatorio

</details>

---

![image](https://github.com/Fabian-Martinez-Rincon/Fabian-Martinez-Rincon/assets/55964635/b751577b-60e9-48d5-a8d6-b9a9eb7b13da)


---

## Preguntas del ostin

Los profes dijeron que solo estudiemos de las preguntas con fotos

---

Cuál de las siguientes afirmaciones es cierta acerca de la normalización de base de datos?

- [ ] a) La normalización es el proceso de agregar redundancia a una base de datos para mejorar la eficiencia en las consultas
- [ ] b) La normalización es el proceso de eliminar la redundancia en una base de datos para evitar problemas de inconsistencia de datos.
- [ ] c) La normalización es el proceso de crear copias de seguridad de una base de datos para protegerla de pérdidas de datos.
- [ ] d) La normalización es el proceso de cifrar los datos en una base de datos para proteger su confidencialidad.
- [ ] e) Todas las opciones anteriores son verdaderas.
- [ ] f) Algunas de las opciones anteriores son verdaderas.
- [ ] g) Ninguna de las opciones anteriores es verdadera.

<details><summary>👀 Respuesta</summary>

- b) La normalización es el proceso de eliminar la redundancia en una base de datos para evitar problemas de inconsistencia de datos.

</details>

---

¿Cuál de las siguientes afirmaciones es verdadera sobre el modelo Entidad-Relación (ER)?

- [ ] a) El modelo ER es un modelo lógico que se enfoca en la implementación física de la base de datos.
- [ ] b) Las entidades en el modelo ER representan relaciones entre los datos.
- [ ] c) Las relaciones en un modelo ER representan vínculos entre las entidades.
- [ ] d) El modelo ER no incluye atributos para las entidades y relaciones.
- [ ] e) Todas las opciones anteriores son verdaderas.
- [ ] f) Algunas de las opciones anteriores son verdaderas.
- [ ] g) Ninguna de las opciones anteriores es verdadera.

<details><summary>👀 Respuesta</summary>

- c) Las relaciones en un modelo ER representan vínculos entre las entidades.

</details>

---

¿Cuál de las siguientes técnicas es útil para optimizar consultas SQL en una base de datos?

- [ ] a) Usar subconsultas en lugar de productos de tablas.
- [ ] b) Evitar el uso de índices para las claves primarias.
- [ ] c) Usar funciones de agregación en lugar de GROUP BY.
- [ ] d) Usar el operador LIKE en lugar de igualdad para comparaciones de cadenas.
- [ ] e) Todas las opciones anteriores son verdaderas.
- [ ] f) Algunas de las opciones anteriores son verdaderas.
- [ ] g) Ninguna de las opciones anteriores es verdadera.

<details><summary>👀 Respuesta</summary>

- Lo unico que sabemos es que NINGUNA esta puesta como mal en el parcial, alguna tiene que ser

</details>

---

¿Cuál de las siguientes afirmaciones es verdadera sobre el modelo lógico relacional?

- [ ] a) Se pueden tener atributos compuestos.
- [ ] b) Se pueden tener atributos derivados.
- [ ] c) No se pueden tener identificadores compuestos.
- [ ] d) Se pueden tener atributos polivalentes.
- [ ] e) Todas las opciones anteriores son verdaderas.
- [ ] f) Algunas de las opciones anteriores son verdaderas.
- [ ] g) Ninguna de las opciones anteriores es verdadera.

<details><summary>👀 Respuesta</summary>

- Se pueden tener atributos derivados

</details>

---

¿Cuál de las siguientes afirmaciones es cierta acerca de la integridad referencial en una base de datos relacional?

- [ ] a) La integridad referencial garantiza que cada registro en una tabla tenga un valor único en su clave primaria.
- [ ] b) La integridad referencial asegura que los valores en una tabla sean válidos en referencia a otra tabla.
- [ ] c) La integridad referencial solo se aplica a las tablas que tienen una clave foránea.
- [ ] d) La integridad referencial no es necesaria en una base de datos relacional.
- [ ] e) Todas las opciones anteriores son verdaderas.
- [ ] f) Algunas de las opciones anteriores son verdaderas.
- [ ] g) Ninguna de las opciones anteriores es verdadera.

<details><summary>👀 Respuesta</summary>

- Sabemos que algunas no es

</details>

---

Ya me canse de escribir

![WhatsApp Image 2024-02-09 at 14 50 14](https://github.com/Fabian-Martinez-Rincon/Fabian-Martinez-Rincon/assets/55964635/efe8f812-9826-4525-a2cf-2f59cd0054b4)
![WhatsApp Image 2024-02-09 at 14 50 14 (3)](https://github.com/Fabian-Martinez-Rincon/Fabian-Martinez-Rincon/assets/55964635/fbe76e26-5866-4b2b-91ee-f5ba8035c611)
![WhatsApp Image 2024-02-09 at 14 50 14 (2)](https://github.com/Fabian-Martinez-Rincon/Fabian-Martinez-Rincon/assets/55964635/d73e2c07-1757-4a57-8c81-3240fc70e47c)
![WhatsApp Image 2024-02-09 at 14 50 14 (1)](https://github.com/Fabian-Martinez-Rincon/Fabian-Martinez-Rincon/assets/55964635/dbe3da57-94ee-4fd9-adfc-255daf6cef8a)

![WhatsApp Image 2024-02-09 at 14 50 15 (2)](https://github.com/Fabian-Martinez-Rincon/Fabian-Martinez-Rincon/assets/55964635/36af06e9-50c5-4b58-9816-4c7241325b97)
![WhatsApp Image 2024-02-09 at 14 50 14 (14)](https://github.com/Fabian-Martinez-Rincon/Fabian-Martinez-Rincon/assets/55964635/fa1352ed-a85e-49b4-984f-a41a42ba9300)
![WhatsApp Image 2024-02-09 at 14 50 14 (13)](https://github.com/Fabian-Martinez-Rincon/Fabian-Martinez-Rincon/assets/55964635/cdcec387-c0e9-447c-a490-1d7e090581f1)
![WhatsApp Image 2024-02-09 at 14 50 14 (12)](https://github.com/Fabian-Martinez-Rincon/Fabian-Martinez-Rincon/assets/55964635/738340b7-320e-469b-ba59-3024006ed3ba)
![WhatsApp Image 2024-02-09 at 14 50 14 (11)](https://github.com/Fabian-Martinez-Rincon/Fabian-Martinez-Rincon/assets/55964635/0f69779b-46ef-4c1c-a995-a4d9f870c2ab)
![WhatsApp Image 2024-02-09 at 14 50 14 (10)](https://github.com/Fabian-Martinez-Rincon/Fabian-Martinez-Rincon/assets/55964635/64508d80-b09b-42cd-aa7b-da5d8b05c4f4)
![WhatsApp Image 2024-02-09 at 14 50 14 (6)](https://github.com/Fabian-Martinez-Rincon/Fabian-Martinez-Rincon/assets/55964635/b41d662f-607d-4c7c-b3e2-8cda5d15b1a2)
![WhatsApp Image 2024-02-09 at 14 50 14 (4)](https://github.com/Fabian-Martinez-Rincon/Fabian-Martinez-Rincon/assets/55964635/aad173fd-2dde-499f-967a-e4cb73e8dc9c)
![WhatsApp Image 2024-02-09 at 14 50 14 (2)](https://github.com/Fabian-Martinez-Rincon/Fabian-Martinez-Rincon/assets/55964635/503f64e0-dc0c-432e-a1bf-178d6c0321fd)
![WhatsApp Image 2024-02-09 at 14 50 15 (6)](https://github.com/Fabian-Martinez-Rincon/Fabian-Martinez-Rincon/assets/55964635/2aa849f1-0f35-4c2f-91d1-3050cd99b1ab)
![WhatsApp Image 2024-02-09 at 14 50 15 (3)](https://github.com/Fabian-Martinez-Rincon/Fabian-Martinez-Rincon/assets/55964635/fe789d3a-9605-4c3d-8ab2-1d84a685294d)
