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

- [PREGUNTAS](/Documentos/preguntas.md)

# Modelado de Datos

## Capitulo 9 Introducción al modelado de datos

**modelo de datos**

Un modelo de datos es un conjunto de herramientas conceptuales que permiten describir la información que es necesario administrar para un IS( Sistema de información), las relaciones existentes entre estos datos, la semántica asociada y las restricciones de consistencia.

- **Modelado conceptual**: Es desarrollado durante la etapa de adquisición de conocimiento del problema; el analista se independiza del tipo de SGBD a utilizar y, por consiguiente, del producto de mercado. Asi, el modelo conceptual se desarrolla independientemente de su implementación final.
- **Modelo logico:** El analista debe determinar el tipo de SGBD, debido a que las deciciones que debe tomar dependen de esa elección
- **Modelo fisico:** Es necesario tomar decisiones especificas. Estas últimas tienen que ver con el producto de mercado a utilizar, es decir, el SGBD específico.

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Capitulo 10 Modelado entidad relación conceptual

### Características

- **Expresividad** Capturar y presentar de la mejor forma posible la semántica de los datos del problema a resolver
- **Formalidad** Que requiere que cada elemento representado en el modelo sea preciso y bien definido, con una sola interpretación posible. Esta formalidad es comparable a la formalidad matemática.
- **Minimalidad** Caracteristeica que establece que cada elemento del modelo conceptual tiene una unica forma de representación posible y no puede expresarse mediante otros conceptos.
- **Simplicidad** que establece que el modelo debe ser fácil de entender por el cliente/usuario y el desarrollador.

### Componentes del modelo conceptual

#### Entidad 

Representa un elemento u objeto del mundo real con identidad, es decir, se diferencia unívocamente de cualquier otro objeto o cosa, incluso siendo del mismo tipo. 

Un **conjunto de entidades** es una representación que, a partir de las caracteristicas propias de cada entidad, con propiedades comunes, se resume en un núcleo.

#### Relaciones

Representan agregaciones entre dos o más entidades. Describen las dependencias o asociaciones entre dichas entidades.

Un **conjunto de relaciones** es una representación que, a partir de las características propias de cada relación existente entre dos entidades, las resume en un núcleo.

#### Atributos

Representa una propiedad básica de una entidad o relación. Es el equivalente a un campo de un registro. 

### Componentes adicionales del modelo conceptual

- **Jerarquías de generalización**
- **Subconjuntos**: es igual que una gerarquia pero no es necesario indicar la covertura
- **Atributos Compuestos** Es un atributo generado a partir de varios atributos simples
- **Identificadores** Es un atributo o conjunto de atributos que permite reconocer o distinguir a una entidad de manera univoca dentro del conjunto de entidades
    - **Simples o compuestos** El identificador es simple si esta conformado por un solo atributo y compuesto si esta conformado por varios atributos
    - **Internos o externos** Si todos los atributos que conforman su identidad pertenecen a la identidad identificada, es interno; en su defecto, es externo.

### Transformaciones para mejorar el modelo conceptual

- **Autoexplicativo** Un modelo se expresa a sí mismo si puede representarse utilizando los elementos definidos, sin necesidad de utilizar aclaraciones en lenguaje natural para expresar características.
- **Completitud** Un modelo está completo cuando todas las características del problema están contempladas en él. La forma de validar la completitud es revisar la especificación de requerimientos asociada al problema.
- **Correción** Un modelo es correcto si cada elemento en su construcción fue utilizado con propiedad. Algunos aspectos de facíl resolución en cuanto a correctitud son observar que todas las cardinalidades y coberturas se hayan expresado, haber tenido en cuenta el concepto de herencia en jerarquias, haber expresado todos los identificadores, etc.
- **Expresividad** El modelo conceptual resulta expresivo si a partir de su observación es posible darse cuenta de todos los detalles que lo involucran.
- **Extensible** El modelo conceptual resulta extensible si es fácilmente modificable para incorporar nuevos conceptos en él, resultantes de cambios en los requerimientos del problema.
- **Legibilidad** Un esquema es legible si la representación gráfica es adecuada. 
- **Minimalidad** Un esquema es minimo cuando cada concepto se representa una sola vez en el modelo. Aqui hay dos factores posibles que pueden afectar la minimalidad. Estos factores son:
    - Atributos derivados y ciclos de relaciones

<img src= 'https://i.gifer.com/origin/8c/8cd3f1898255c045143e1da97fbabf10_w200.gif' height="20" width="100%">

## Capitulo 11 Modelado entidad relación lógico

### Características del diseño lógico

El diseño lógico del modelo de datos de un problema produce como resultado un esquema lógico de dicho problema, en función de cuatro entradas.

- **Esquema conceptual** Es el resultado tangible de la etapa inmediate anterior. El esquema conceptual representa la solución, a juicio del analista, respecto del problema original. El esquema lógico a obtener debe representar la mismo información disponible en el esquema conceptual.
- **Descripción del modelo lógico a obtener** Aqui se deben definir las reglas que se aplicarán en el proceso de conversión.
- **Criterios de rendimiento de la BD** Durante la fase de diseño conceptual, se consideraron los requerimientos del usuario. No obstante, hay otro tipo de necesidades que no se pueden definir sobre el modelo conceptual. Estas necesidades tienen que ver con los requerimientos, en general, no funcionales del problema., con por ejemplo la performance de la BD.
- **Información de carga de la BD** Este concepto aparece, en cierta forma, ligado al concepto anterior. Cuando se genera el esquema lógico, el analista debe observar cada entidad e interrelación definida, y ver la probable evolución de la información contenida en esas estructuras.