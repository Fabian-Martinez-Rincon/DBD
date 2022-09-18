<h1 align="center"> 💿 Diseño de Base de Datos</h1>

<p><img width="250" align='right' src="https://media.giphy.com/media/xUA7aQfR9hhgU78KDC/giphy.gif"></p>

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
  - [Resolver las Jerarquias]()
  - [Resolver Atributos compuestos]()
  - [Resolver Atributos Polivalentes]()

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


**Dejo todas las entidades.**

<table >
<tr>
<td>  <div align="center">Conceptual</div> </td> <td> <div align="center" >Logico</div> </td>
</tr>

 <tr>
<td> <img  width="340" src="./Img/Logico/1.png"> </td> <td><img  width="390" src="./Img/Logico/Conversion.PNG"></td>
</tr>
 
</table>



En las siguientes tres, no puedo eliminar al padre, tengo las otras dos posibilidades, no puedo dejar solo a los hijos eliminando al padre.
- **Total Superpuesta (T, S):** 
- **Parcial Exclusiva (P, E):** 
- **Parcial Superpuesta (P, S):** 


## Resolver Atributos compuestos
## Resolver Atributos Polivalentes