
- [Condiciones de aprobación](/Documentos/condiciones.md)
- [Modelo conceptual](#modelo-conceptual)
  - [Entidad](#entidad)
  - [Relación](#relación)
  - [Relación reculsiva](#relación-reculsiva)
  - [Atributo](#atributo)
  - [Atributo compuesto](#atributo-compuesto)
  - [Identificador](#identificador)
  - [Cardinalidades en los atributos](#cardinalidades-en-los-atributos)
  - [Cardinalidades en las relaciones](#cardinalidades-en-las-relaciones)
  - [Identificador compuesto](#identificador-compuesto)
  - [Identificador externo](#identificador-externo)
  - [Gerarquias de generalizacion](#gerarquias)
- [Modelo Logico](#modelo-logico)
  - [Resolver las Jerarquias](#resolver-las-jerarquias)
    - [Dejar Todas las entidades](#dejo-todas-las-entidades)
    - [Dejar solo al Padre](#dejar-solo-al-padre)
    - [Dejar solo a los hijos](#dejar-solo-a-los-hijosesta-opcion-solo-la-puedo-cuando-tengo-t-e)
  - [Resolver Atributos compuestos](#resolver-atributos-compuestos)
  - [Resolver Atributos Polivalentes](#resolver-atributos-polivalentes)
- [Modelo Fisico](#modelo-fisico)
  - [Conversion de Entidades](#conversion-de-entidades)
  - [Conversion de Relaciones](#conversion-de-relaciones)
    - [Ejemplo 1 (0, 1) a (1, 1)](#ejemplo-1-0-1-a-1-1)
    - [Ejemplo 2 (1, 1) a (1, 1)](#ejemplo-2-1-1-a-1-1)
    - [Ejemplo 3 (0, 1) a (0, 1)](#ejemplo-3-0-1-a-0-1)
    - [Ejemplo 4 (1, 1) a (0/1, N)](#ejemplo-4-1-1-a-01-n)
    - [Ejemplo 5 (0, 1) a (0/1, N)](#ejemplo-5-0-1-a-01-n)
    - [Ejemplo 6 (0/1, N) a (0/1, N)](#ejemplo-6-01-n-a-01-n)
- [Algebra Relacional](#algebra-relacional)
  - [Selección σp (T) ](#selección)
  - [Proyección πa1, … an (T)](#proyección)
  - [Unión T1 ∪ T2](#unión)
  - [Intersección T1 ∩ T2](#intersección)
  - [Producto cartesiano T1 × T2](#producto-cartesiano)
  - [Producto natural T1 \|×\| T2](#producto-natural)
  - [Diferencia T1 – T2](#diferencia)
  - [División T1 % T2](#división)
  - [Renombre ρT (Table)](#renombre)
  - [Asignación Α ⇐ Consulta](#asignación)


# Modelo conceptual
## Entidad


<p><img width="200" align='right' src="./Img/Diagramas/Entidad.png"></p>

Es un elemento u objeto del mundo real que queremos representar. Partimos de un problema/dominio, este va a tener distintos elementos/objetos a representar y los representamos en el modelo conceptual a partir de una entidad.

---

## Relación

Nos representan las dependencias que tenemos entre dos o mas entidades, si una relacion une dos entidades, hablamos de una relacion binaria. Si une tres entidades, hablamos de una relacion ternaria y asi sucesivamente. El nombre descriptivo en la relacion **R1** no es una buena practica ya que podemos representar distintas dependencias con una misma relación (y genera ambigüedad)

<p><img src="./Img/Diagramas/Relacion.png"></p>

---
## Relación reculsiva
Relacion que une dos entidades particulares del mismo conjunto. En este caso, materias esta relacionada con si misma. Por ejemplo R1 = 'es correlativa de', estariamos diciendo que una materia es correlativa de otra materia.

<p><img width="400"  src="./Img/Diagramas/Recursiva.png"></p>

---
## Atributo

<p><img align='right' width="200"   src="./Img/Diagramas/Atributo.png"></p>

Un atributo representa una propiedad basica de una entidad o relacion. Un atributo es equivalente a un campo de un registro

---
## Atributo compuesto

<p><img align='right' width="300"   src="./Img/Diagramas/Atributo Compuesto.png"></p>

Un atributo compuesto representa a un atributo generado a partir de una combinacion de varios atributos simples 

<br>
<br>

---

## Identificador
<p><img align='right' width="200"   src="./Img/Diagramas/Identificador.png"></p>

Un identificador es un atributo o un conjunto de atributos que permite reconocer o distinguir a una entidad de matenar univoca dentro del conjunto de entidades. 
- Tota entidad tiene un atributo identificador 
- Los atributos identificadores son unicamente atributos de entidades.
- Si yo encuentro un valor en mi entidad cuyo valor es unico, si o si, estoy obligado a marcarlo como atributo identificador

---
## Cardinalidades en los atributos

Los atributos, tienen asociado el concepto de cardinalidad. Cuando se define un atributo se debe indicar si es o no obligatorio y si puede tomar mas de un valor (Polivalente). En el primer parametro tenes la cardinalidad minima, y en segundo, tenes la cardinalidad maxima. 

<p><img align='right' width="200"  src="./Img/Diagramas/Atributo.png"></p>

- **Cardinalidad (1,1)** Monovalente obligatior. La cardinalidad existe y esta presenta, pero solamente en este caso no se debe indicar en forma explicita.

<p><img align='right' width="200"   src="./Img/Diagramas/Monovalente.png"></p>

- **Cardinalidad (0,1)** Monovalente obligatiorio, el '0' significa que puede tomar ningun valor 

<p><img align='right' width="200"   src="./Img/Diagramas/Polivalente.png"></p>

- **Cardinalidad (0, N)** Polivalente no obligatorio

<p><img align='right' width="200"   src="./Img/Diagramas/PolivalenteObligatorio.png"></p>

- **Cardinalidad (1, N)** Polivalente Obligatorio

---
## Cardinalidades en las relaciones
Me indica el nivel de correspondencia que hay entre las dos entidades que une la relacion. Se debe definir el nivel minimo de correspondencia (cardinalidad minima), y el nivel maximo de correspondecia (cardinalidad maxima)

La cardinalidad minima, me indica que puede inscribirse a como minimo a 0 cursadas y como maximo N, es lo mismo de ambos lados.

- Toda relacion tiene cardinalidad.
<p><img  src="./Img/Diagramas/CardinalidadesRelaciones.png"></p>

---

## Identificador compuesto

<p><img align='right' width="300" src="https://user-images.githubusercontent.com/55964635/190878428-1451518b-a901-46f5-85d2-5901a9cde948.png"></p>

Los identificadores compuestos, estan formados por varios atributos simples.

- La fecha y hora, puede repetirse en distintos examen
- Mi DNI puede repetirse en varios examenes
- Pero lo que no se puede repetir son los dos anteriores a la vez

---
## Identificador externo
- Para tener un atributo identificador externo, si o si, las dos entidades tienen que estar relacionadas
- Para que una entidad, pueda ser identificada, tiene que ser una entidad devil (tener cardinalidad 1,1)

<p><img  width="500" src="https://user-images.githubusercontent.com/55964635/190878612-4c773e60-ad9f-4c10-89f2-7c6c917147ed.png"></p>


En este caso, me indica que copia, va a ser identificado con el nro de copia , mas el identificador que me traigo de libro (que seria ISBN). 
Por lo tanto, copia va a ser identificado con nro de copia + ISBN. \
De esto puedo deducir que nro de copia se puede repetir para distintos libros pero este + el ISBN no.

---
## Gerarquias

## Generalizacion
Cuando tenemos entidades que tienen caracteristicas y propiedades comunes, podemos crear una entidad padre que junte las caracteristicas comunes, y a partir de esa entidad padre, podemos generar varias entidades hijas. Cada atributo hijo puede tener sus propios atributos/relaciones.

![image](https://user-images.githubusercontent.com/55964635/190879035-413ecd9d-bd98-4648-86aa-19476997e1b9.png)
- El primer parametro (T o P) lo que me esta indicando en el caso de que sea total es que no existe una persona que no sea (alumno, docente o graduado). 
- Si fuera parcial, lo que me esta indicando, es lo contrario, que la suma de los elementos de los hijos, no necesariamente dan la totalidad de los elementos del padre. Podrian haber personas que no sean (alumnos, docentes o graduados).
- Segundo parametro (S o P), si es exclusiva, significa que los elementos en los hijos nunca se van a superponer, en este caso una persona es (o un alumno, o un docente, o un graduado, nunca una persona, puede ser las dos a la vez)
- Que sea superpuesta, es lo contrario, una persona puede ser alumno, docente y graduado a la vez


Coberturas
- (T, E) Total Esclusiva
- (T, S) Total SuperPuesta
- (P, E) Parcial Esclusiva
- (P, S) Parcial SuperPuesta

---
## Subconjuntos  
Caso especial de las jerarquias de generalizacion, donde se tiene una generalizacion de la que se desprende solamente una especializacion. No es necesario indicar la cobertura para los subconjuntos.


---


# Modelo Logico

## Resolver las Jerarquias
- **Total Exclusiva (T, E):** Tengo tres posibilidades, dejar los padres y los hijos (dejar todo), dejar solo los hijos eliminando al padre o dejar solo al padre, eliminando a los hijos.

En las siguientes tres, no puedo eliminar al padre, tengo las otras dos posibilidades, no puedo dejar solo a los hijos eliminando al padre.
- **Total Superpuesta (T, S):** 
- **Parcial Exclusiva (P, E):** 
- **Parcial Superpuesta (P, S):** 


### **Dejo todas las entidades.**

- Usualmente cuando dejamos todas las entidades, aparecen las relaciones **esUn**
- Recordar que no podemos tener nombres repetidos ni de entidades, ni de relaciones. (Por eso el **esUn1**)
- Tengo que mirar si los hijos tienen identificador propio, si el hijo tiene, no estoy obligado a bajar el identificador del padre. Pero si el hijo, no posee identifificador propio, estoy obligado a bajar el identificador del padre, tal y como se muestra en la imagen.
- **La cardinalidad de las relaciones:** del lado del padre, siempre va a tener **(0, 1)** y del lado del hijo, siempre va a ser **(1, 1)**



<table >
<tr>
<td>  <div align="center">Conceptual</div> </td> <td> <div align="center" >Logico</div> </td>
</tr>

 <tr>
<td> <img  width="400" src="./Img/Logico/1.png"> </td> <td><img  width="400" src="./Img/Logico/Conversion.PNG"></td>
</tr>
 
</table>


---


### **Dejar solo al padre**

- Si dejo solo al padre, los atributos de los hijos tendran que pasar al padre (porque sino perderia esa informacion)
- **Que pasa cuando paso los atributos de los hijos al padre?** Esos atributos se vuelven opcionales. 
- Los identificadores, pasan a ser atributos opcionales

<table >
<tr>
<td>  <div align="center">Conceptual</div> </td> <td> <div align="center" >Logico</div> </td>
</tr>

 <tr>
<td> <img  width="400" src="./Img/Logico/1.png"> </td> <td><img  width="400" src="./Img/Logico/2.PNG"></td>
</tr>
 
</table>


--- 

### **Dejar solo a los hijos(Esta opcion solo la puedo cuando tengo (T, E))**

- Los atributos del padre bajan a los hijos

<table >
<tr>
<td>  <div align="center">Conceptual</div> </td> <td> <div align="center" >Logico</div> </td>
</tr>

 <tr>
<td> <img  width="400" src="./Img/Logico/1.png"> </td> <td><img  width="900" src="./Img/Logico/3.PNG"></td>
</tr>
 
</table>

--- 


## Resolver Atributos compuestos

Para resolver los atributos compuestos, tengo dos formas.
- Todos los atributos simples que conforman el atributo compuesto, bajan a la entidad
- O dejo un unico atributo que me deje un atributo simple
- Cual es la mejor opcion? Todo depende del dominio que este modelando, si yo estoy modelando un dominio cuya direccion sea un campo que es muchas veces consultado, no me conviene modelarlo todo en un atributo, porque en direccion, voy a tener que separar los datos (ya que estan todos en un atributo) y esa tarea es demasiado pesada para lo que necesitamos. En cambio si lo resolvemos como atributos individuales, tengo todos los datos mas a mano, sin necesitad de procesar nada de informacion extra.
- Si estoy modelando un dominio cuya direccion es solo un dato mas, puedo ponerlo todo en un solo atributo

<table >
<tr>
<td>  <div align="center">Sólo los atributos individuales
</div> </td> <td> <div align="center" >Todo en un solo atributo</div> </td>
</tr>

 <tr>
<td> <img  width="400" src="./Img/Logico/4.PNG">


 </td> <td><img  width="400" src="./Img/Logico/5.PNG"></td>
</tr>
 
</table>

## Resolver Atributos Polivalentes

Para resolver los atributos polivalentes se debe agregar una entidad y una interaccion.

- Siempre conviene poner cardinalidad (0, n) de ambos lados, (podria poner cardinalidad (1, 1) y que sea una entidad devil en funcion del dominio que tengo que resolver, si hacemos esto, vamos a tener que usar un identificar exteno)

<table align = 'center'>
<tr><td><img width="300" src="./Img/Logico/6.PNG"></td></tr>

 <tr>
 <td>
<img  width="700" src="./Img/Logico/7.PNG">
</td>
</tr>
 
</table>

---

# Modelo Fisico

## Conversion de entidades
Tota entidad de mi modelo logico termina siendo una tabla 

<table align = 'center'>
 <tr>
 <td>
<img  width="300" src="./Img/Fisico/1.PNG">


</td>
</tr>
 
</table>

**Alumno** = (`dni`, nombres, calle, nro, piso?, dpto?)

## Conversion de relaciones

Analizar las cardinalidades de mi relacion.

- Una relacion puede o no ser una tabla.
- Que la relacion sea una tabla o no, depende de la cardinalidad de la relacion.

### Ejemplo 1 (0, 1) a (1, 1)

Cuando tenemos esta cardinalidad, la relacion no se convierte en tabla. Ahora tengo que mantener la relacion entre `A` y `B` y no perder informacion. Lo que hago es pasar el identificador de `A` hacia `B`. Pasamos el identificador de `A` porque este, tiene cardinalidad minima cero. Y puede no estar relacionada. En caso contrario de `B` que si esta relacionada.

Si paso el identificador de `B` hacia `A` en algunos casos puedo llegar a tener un identificador nulo.

<img  src="./Img/Fisico/2.PNG">

- `B` = (`idB`, idA (fk), atB)
- `A` = (`idA`, atA)
- `at` = atributo simple
- `fk:` es la clave que yo utilizo para relacionarme con la entidad en mi modelo logico.

### Ejemplo 2 (1, 1) a (1, 1)

- La relacion no se convierte en tabla
En este caso tengo `A` relacionado con `B` y tengo relacionado 1 a 1 de ambos lados. Es este caso, es indistinto, pasar el identificador del lado de `A` o pasar el identificador del lado de `B`

<img  src="./Img/Fisico/3.PNG">

- `B` = (`idB`, idA (fk), atB)
- `A` = (`idA`, atA)

O tambien podria ser

- `B` = (`idB`, atB)
- `A` = (`idA`, idB(fk), itA)

### Ejemplo 3 (0, 1) a (0, 1)

Nada me asegura, ni que `A` este relacianda con `B` ni que `B` este relaciando con `A`. Esto quiere decir, que pasar un identificador para cualquiera de los lados para mantener las relaciones, ya no me sirve.


<img  src="./Img/Fisico/4.PNG">

En este caso, estoy obligado a convertir la relacion en tabla.

- `B` = (`idB`, atB)
- `A` = (`idA`, atA)
- `R` = (`idA`, idB)  o  `R` = (idA, `idB`) Estos dos datos, van a tomar valores cuando ambos esten relacionadas

### Ejemplo 4 (1, 1) a (0/1, N)

Lo que se hace aca es pasar siempre el identificador de la cardinalidad que tiene maxima `N`, pasar el identificador hacia la entidad que tiene cardinalidad (1, 1)

- Esto me asegura de que el identificador de B toma un unico valor, porque `A` esta relacionado solo una vez con `B`

<img  src="./Img/Fisico/5.PNG">

- `A` = (`idA`, idB(fk), atA)
- `B` = (`idB`, atB)


- Que pasa cuando en una entidad tengo mas de un atributo identificador? Cuando paso esos identificadores a tablas, eso se llama clave candidata, en este caso, tenemos que elegir solo un atributo identificador.


### Ejemplo 5 (0, 1) a (0/1, N)

En este caso, estoy obligado a que la relacion se comvierta a tabla, porque no importa que identificador quiera pasar, siempre voy a tener perdida de informacion, ya que en la primera cardinalidad, puede tomar valor cero y lo mismo pasa para la otra entidad.

<img  src="./Img/Fisico/6.PNG">

Cuando mi relacion se convierte en tabla, se lleva los atributos identificadores de las dos entidades que relaciona.

- Por que la clave primaria de la tabla va a ser id de A y no de B? Porque la id de A no se va a repetir. Porque en nuestra relacion, a lo suma un A, se relaciona con un B, esto me esta indicando que no se va a repetir.
- `A` = (`idA`, atA)
- `B` = (`idB`, atB)
- `R` = (`idA`, idB)

### Ejemplo 6 (0/1, N) a (0/1, N)
Si o si en este caso, la relacion siempre es tabla. 
Cuando tenemos una relacion N a N, la relacion se convierte en tabla, se lleva los identificadores como todas las relaciones. Pero ambas, son claves primarias, porque yo me aseguro de que lo que no se va a repetir en mi relacion es idA + idB conjuntamente (Los dos valores juntos no se van a repetir)

<img  src="./Img/Fisico/7.PNG">

- `A` = (`idA`)
- `B` = (`idB`, atB)
- `R` = (`idA`,`idB`, atR)

En caso de que ambos ids se repitan estando juntas, vamos a tener que marcar a atR para poder identificar a R


### Ejemplo 7 Recursivas

Las relaciones recursivas se manejas de igual forma que una relacion binaria, solo que se llama a si misma

<img width="500" src="./Img/Fisico/8.PNG">

- **R12 =** (Codigo Materia, Codigo Materias Correlativa) Como no puedo tener dos atributos con el mismo nombre, lo que hago es renombrar

---

# Algebra Relacional

## Selección
<p><img src="./Img/Practica 3/1.png"></p>

## Proyección
<p><img src="./Img/Practica 3/2.png"></p>

## Unión
<p><img src="./Img/Practica 3/3.png"></p>

## Intersección
<p><img src="./Img/Practica 3/4.png"></p>

## Producto cartesiano
<p><img src="./Img/Practica 3/5.png"></p>

## Producto natural
<p><img src="./Img/Practica 3/6.png"></p>

## Diferencia
<p><img src="./Img/Practica 3/7.png"></p>

## División
<p><img src="./Img/Practica 3/8.png"></p>

## Renombre
<p><img src="./Img/Practica 3/1.png"></p>

## Asignación
