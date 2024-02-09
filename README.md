<div align="center">

[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/Nomadiix/DBD)
[![GitHub stars](https://img.shields.io/github/stars/Nomadiix/DBD)](https://github.com/FabianMartinez1234567/DBD/stargazers/)
[![GitHub repo size in bytes](https://img.shields.io/github/repo-size/Nomadiix/DBD)](https://github.com/Nomadiix/DBD)
 </div>

<h1 align="center"> 💿 Diseño de Base de Datos </h1>

<br>


<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

> [!IMPORTANT]
> Todas las preguntas van a estar justificadas segun el libro [Introducción a las Bases de Datos](/Introducción%20a%20las%20Bases%20de%20Datos%20-%20Bertone-Thomas.pdf) y mi sentido común


<div align='center'>

# Finales 

![](https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExd2lpd3A1emYyajVvOGV2MjBjZmF6N2FvNGUxMno1dHltZWp1NnJhciZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/Wkr0EKIsWitJm/giphy.gif)

</div>

> [!NOTE]  
> Es un recopilatorio de preguntas, algunas pueden que esten bien y otras mal porque depende de la interpretación o justificación de cada uno, en este caso vamos a tratar justificar todo en base al libro

## Temario de Preguntas

- [Diagramas Conceptuales](#archivos)
- [Consultas](#consultas)

> [!TIP]
> La strat del final este es responder 7/10 preguntas, porque tenes margen para errarle en 2 preguntas :D

---

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