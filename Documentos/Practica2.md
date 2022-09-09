## Practica 2

### 1 - INTRODUCCIÓN AL MODELADO CONCEPTUAL, LÓGICO y FÍSICO.

#### Parte 1 Modelo Logico
- [Ejercicio 1](#ejercicio-1-logico)
- [Ejercicio 2](#ejercicio-2-logico)
- [Ejercicio 3](#ejercicio-3-logico)
- [Ejercicio 4](#ejercicio-4-logico)
- [Ejercicio 5](#ejercicio-5-logico)
- [Ejercicio 6](#ejercicio-6-logico)
- [Ejercicio 7](#ejercicio-7-logico)
- [Ejercicio 8](#ejercicio-8-logico)
- [Ejercicio 9](#ejercicio-9-logico)
- [Ejercicio 10](#ejercicio-10-logico)
- [Ejercicio 11](#ejercicio-11-logico)
- [Ejercicio 12](#ejercicio-12-logico)
#### Parte 2 Modelo Fisico
- [Ejercicio 1](#ejercicio-1-fisico)
- [Ejercicio 2](#ejercicio-2-fisico)
- [Ejercicio 3](#ejercicio-3-fisico)
- [Ejercicio 4](#ejercicio-4-fisico)
- [Ejercicio 5](#ejercicio-5-fisico)
- [Ejercicio 6](#ejercicio-6-fisico)
- [Ejercicio 7](#ejercicio-7-fisico)
- [Ejercicio 8](#ejercicio-8-fisico)

**Para cada ejercicio realizar el correspondiente modelo conceptual, pasaje al modelo lógico y pasaje al modelo físico**

### Ejercicio 1 Logico
Se debe modelar la información necesaria para una Inmobiliaria de la ciudad de La Plata

Es necesario modelar la información de clientes y empleados de la inmobiliaria. De ambos se conoce D.N.I, nombre, apellido, dirección detallada y número de pasaporte. Además de los empleados se conoce el número de legajo, el cual no se repite entre diferentes empleados y el área donde trabaja cada uno. Los empleados pueden ir rotando de área a lo largo del tiempo y es necesario modelar por las distintas áreas que pasó un empleado. De las áreas se conoce código único de área, descripción, teléfonos y ubicación. De cada cliente, además, se debe almacenar sexo, nacionalidad y los inmuebles de los que es dueño. Un cliente no puede trabajar en la inmobiliaria

La inmobiliaria maneja diferentes inmuebles de los cuales se conoce dirección detallada, código único de inmueble, cantidad de ambientes, si posee balcón, si posee lavadero, cantidad de baños, si se alquila, se vende o ambas cosas, precio de venta y precio de alquiler, tipo de inmueble (casa, duplex, depto,...).

Debe quedar registrado todo alquiler y venta que realiza la inmobiliaria detallando, para los alquileres inmueble, cliente, fechas de inicio y fin de alquiler, empleado que alquiló y precio. De las ventas se registran fecha y hora de venta, cliente, empleado que vendió la
propiedad, precio de venta y comisión de venta

**Nota:** tenga en cuenta que podría pedirse promedio de ventas de un semestre del año,
vendedor más exitoso del año, tipo de inmueble más alquilado o más vendido entre otros

### Ejercicio 2 Logico

Se desea modelar la información necesaria para una red social. La red social permite a los usuarios compartir imágenes de diferentes temáticas y realizar comentarios sobre las mismas. De los usuarios se registran: nombre y apellido, usuario en la red social (que es único), clave de acceso y cuentas de correo electrónico, dirección detallada y un teléfono de contacto. En la red social, los usuarios pueden subir imágenes, o bien comentar, descargar o compartir una publicación (imagen/es) de otros usuarios vinculados. Cuando dos usuarios se vinculan, se debe almacenar información de este vínculo, fecha y hora, tipo de vínculo y opcionalmente una descripción estandarizada en la red social que indica de donde se conocen (lugar de vínculo). En la misma fecha y hora el mismo usuario no podrá generar dos vínculos. De las imágenes se debe almacenar: fecha y hora de publicación, temática de la imagen, título, usuario que realiza el posteo y el nombre del archivo correspondiente, además de un conjunto de palabras claves que caracterizan la imagen. Un usuario no puede subir dos imágenes con título idéntico.De las temáticas se registra un nombre único y una descripción asociada. De las imágenes se debe poder determinar los usuarios que compartieron la imagen o la descargaron, indicando fecha y hora y si la compartió o descargó. Así mismo, los usuarios pueden realizar comentarios en la red social, se debe almacenar un texto, la fecha y hora de creación del comentario, que imagen comentó o a que comentario respondió. Un comentario podría ser respuesta a otro comentario existente. Un usuario no podrá realizar dos comentarios en la misma fecha y hora.

### Ejercicio 3 Logico

Se desea modelar una base de datos para el manejo de una unidad del servicio penitenciario (cárcel en lenguaje coloquial). En la unidad trabajan empleados de los cuales se conoce nombres, apellidos, dirección completa, legajo (único), D.N.I, teléfonos y el área donde trabaja. Cada empleado puede trabajar en una única área a la vez pero puede a lo largo del tiempo trabajar en las diferentes áreas, se debe modelar el historial de áreas en donde ha trabajado un empleado. Existen dos tipos de áreas, las áreas administrativas y los pabellones. En las áreas administrativas trabajan solo empleados administrativos y en los pabellones solo empleados penitenciarios. Un empleado administrativo no puede ser penitenciario. Además de los empleados penitenciarios es necesario conocer el número de matrícula el cual es único. Los empleados administrativos pueden tener uno o varios títulos. De los internos se conoce, nombre, apellido, apodo, número de causa (puede ser compartida por varios internos), listado estandarizados de delitos en esa causa y D.N.I. Los internos son alojados en pabellones, es necesario conocer el pabellón donde se encuentra un interno. Si un interno es movido a otro pabellón debe quedar registrado el historial. De los pabellones se conoce, número único de pabellón, ubicación, cantidad máxima de internos y una descripción. Las áreas administrativas tienen un número único y una descripción. Por último es necesario registrar los posibles incidentes ocurridos en la unidad detallando fecha y hora del incidente, internos involucrados, descripción del incidente el pabellón donde ocurrió y el penitenciario responsable.

### Ejercicio 4 Logico

Se desea modelar el manejo de la información referente a una casa de comidas. De los clientes se conoce D.N,I, apellidos, teléfonos, dirección detallada, mail y cuit. La casa vende diferentes platos de los que se conoce código único, precio actual y descripción. Cuando un cliente llama, se le toma el pedido, el cual puede estar formado por uno o varios productos. Debe quedar registro de la fecha y hora que se realizó el llamado, la fecha y hora de entrega del pedido, el precio total y los precios que fue vendido cada producto. Los repartos se realizan por zonas, conociéndose de cada zona el número único de zona y el costo de envío hasta esa zona. Es necesario poder obtener el costo de envío de un pedido dado.

Por otro lado, debemos modelar la reposición de materia prima con la que se elaboran los platos. Cada plato está formado por varios productos de los que se conoce código, descripción, precio actual, proveedor,stock y cantidad mínima. Se realizan compras de productos a proveedores de los cuales se conoce nro único de proveedor, D.N.I, nombre, apellido y razón social (único). Por cada compra debemos poder obtener los productos involucrados, el proveedor, la fecha, la hora y el precio al que se compró cada producto

**NOTA:** tenga en cuenta que se podría pedir: obtener los productos que conforman cada plato como así también aquellos pedidos que fueron entregados, los pedidos que fueron rechazados, pedidos mayores a $10000 y los pedidos que se encuentran pendientes, entre otras estadísticas y consultas

### Ejercicio 5 Logico

Se desea modelar la información necesaria para una cadena de tiendas de indumentaria. De cada tienda se desea almacenar: la razón social, su dirección completa, un teléfono de contacto, instagram y facebook de la misma (si posee). Las tiendas están conformadas por un grupo de empleados y un supervisor a cargo de la misma. De los empleados se registran: DNI, C.U.I.T, nombre, apellido, fecha de nacimiento, dirección, uno o varios teléfonos de contacto, fecha de ingreso, cantidad de hijos y estado civil. Las tiendas están divididas en sectores de trabajo: personal,proveedores, ventas, entre otros. De cada sector se registra nombre, descripción y un código único relativo a la tienda, el mismo código de sector puede estar en varias tiendas. Cada empleado está asignado a un sector determinado pero con el transcurso del tiempo va cambiando de sector; se debe poder determinar lo/s sectores por los que pasó un empleado en orden cronológico. Cada empleado trabaja en una y solo una tienda. El supervisor sólo podrá estar a cargo de una tienda. De los productos que se comercializan en las tiendas se debe registrar: tipo de producto, marca, modelo, talle, descripción, color, precio de venta y el stock del mismo en la tienda y un código único de producto. Por último, se deben registrar las ventas realizadas, indicando fecha, número de ticket fiscal, empleado que efectúa la venta, el/los productos involucrados y el total de la misma.

**NOTAS:**

- El supervisor es un empleado de la tienda que se desempeña como tal.
- Tenga en cuenta que el stock de un producto y el precio de venta del producto podrían variar en las diferentes tiendas.
- Se debe poder consultar la información mediante diferentes alternativas: marca y/o modelo más vendidos, tipo de productos más vendidos, entre otras

### Ejercicio 6 Logico

Se debe modelar la información necesaria para un vivero muy importante de la ciudad.

Resulta indispensable conocer la información de los empleados y clientes del vivero. De ambos se registra: D.N.I, C.U.I.T, apellido, nombre, teléfonos de contacto, email si posee y dirección detallada. En particular para los empleados debe registrarse además: fecha de ingreso, fecha de nacimiento, cantidad de hijos y un número único de empleado. De los clientes, se registra además el código único de cliente. El vivero ofrece diferentes artículos para jardinería: plantas, herramientas, macetas, sustratos entre otros. De todos ellos se registra un número único de artículos, precio, tamaño, nombre, stock y descripción. Se deben registrar las ventas realizadas. De cada venta se registra fecha, hora, cliente y el empleado que se encarga de realizar la venta, además se deben registrar el/los artículos vendidos y un número de ticket fiscal. De los artículos vendidos se debe almacenar precio de venta y cantidad vendida. El cliente puede abonar las compras en efectivo, con débito o crédito. Si abona con débito o crédito, debe quedar registro del número de tarjeta, banco y entidad que la emite (visa, mastercard,..). Del banco y entidad emisora se registra un nombre único y descripción. Si el pago es con crédito se debe registrar además la cantidad de cuotas en que realizó el pago. (Tenga en cuenta que la tarjeta se debe poder reutilizar en otros pagos y con otro nro de cuotas). Si abona en efectivo se deberá dejar constancia de esto.

### Ejercicio 7 Logico
Se desea modelar la información necesaria para el tratamiento de pacientes con COVID-19

Es necesario representar tanto a los pacientes que han contraído el virus como a los médicos que atienden los casos.Tanto para los médicos como para los pacientes es necesario almacenar: D.N.I, número de pasaporte (si poseen), dirección detallada, nombre, apellido y edad. Para los pacientes se debe almacenar además, una descripción de enfermedades preexistentes e información referente al episodio de contagio y además cantidad de dosis de la vacuna anti covid. Tenga en cuenta que hay pacientes que pueden contagiarse más de una vez, por lo tanto tendrán más de un episodio. De cada episodio, se registra: número único de episodio, fecha de detección, síntomas y médicos que llevaron a cabo la atención. Los síntomas pueden variar entre los diferentes episodios sabiendo que cada síntoma tiene un código único y una descripción asociada. Para los médicos es necesario almacenar además, el código de matrícula, especialidades y sala en la que atiende. Un médico puede rotar de salas y es necesario modelar el historial de rotaciones de cada médico. De la sala se conoce, número de sala (único), piso y capacidad. De las especialidades se almacena un nombre único y descripción. Es necesario que se almacene la nota promedio obtenida por el médico en cada especialidad. Tenga en cuenta que un médico también puede contagiarse COVID-19 y su modelo debe
permitir representar esto.

**Nota:** Podría pedirse médico que tiene máximo de atenciones por covid, médico que no atendió más de 10 pacientes, paciente con más contagios, entre otros

### Ejercicio 8 Logico

Se desea modelar la información necesaria para una empresa dedicada a la realización de eventos gastronómicos al aire libre. Para cada evento se alquilan cierta cantidad de lugares donde el inquilino podrá vender productos comestibles o bien¿ utilizarlo para difundir su actividad, además se brindan servicios tales como electricidad, agua corriente y demás, si el inquilino lo requiere. De los lugares se registra: número único, descripción, m2, ubicación, distancia a la puerta de acceso al predio, precio por día. De los servicios en cambio se registra: nombre único, descripción y precio del servicio. De cada evento se registra: nombre del evento, fecha y hora de inicio, dirección del evento, duración del evento y el staff de personas encargadas de la organización y difusión del evento. De cada integrante del staff se debe registrar: DNI, nombre completo, dirección detallada, fecha de nacimiento, correo electrónico, teléfonos de contacto y el rol que cumple dentro del evento. De los inquilinos se registran: DNI, nombre completo, dirección detallada, teléfonos de contacto, razón social (si el inquilino representa a una empresa), y tipo de gastronomía (si vende comestibles). Además, se debe registrar información de los alquileres: fecha, hora, quien es el inquilino, el evento al que corresponde el alquiler y el o los lugares que alquila y en caso de que alquile servicios los servicios alquilados. Nota: El nombre del evento no se podrá repetir en una misma fecha y hora de inicio. Tenga en cuenta que debe poder determinar el costo de todos los alquileres (valor al que se alquila o alquiló cada lugar o servicio), actuales e histórico.

### Ejercicio 9 Logico

Se debe modelar la información correspondiente para la gestión de personal y proyectos de una empresa de software con sede en la ciudad de la plata. La empresa se encuentra dividida en diferentes áreas, de cada una de ellas se conoce: nombre del área (único), un código de área único y una descripción de las funciones de la misma. Los empleados de la empresa corresponden a un área de la empresa pudiendo prestar servicios en uno o varios proyectos. De cada empleado se conoce: DNI, CUIT, fecha de nacimiento, cantidad de hijos, fecha de ingreso, una descripción de lo/s título/s si posee, dirección detallada, uno o varios teléfonos de contacto y el área en la que se desempeña. Cada área cuenta con un gerente encargado de la misma que forma parte de los empleados de la empresa. Todos los empleados pueden rotar dentro de las áreas de la empresa, se debe poder determinar todos los empleados que trabajaron en una determinada área en orden cronológico, del mismo modo todos los gerentes que tuvo un área. La empresa además lleva adelante varios proyectos, de cada proyecto se conoce: nombre único, fecha de comienzo, fecha estimada de finalización, costo estimado, tipo de proyecto y los empleados que intervienen en su realización. Cuando un empleado es asignado a un proyecto se debe indicar fecha inicio, fecha de fin opcional, cargo que desempeñará dentro del proyecto, cantidad de horas dedicadas. De los tipos de proyecto se conoce: nombre único del tipo y una descripción asociada. Además se tiene estandarizado los posibles cargos a asumir dentro de un proyecto, de cada cargo se almacena: código único, nombre y una descripción del mismo. Tenga en cuenta que podría consultarse cuántos empleados se desempeñan con cargo programador, o bien cuántos proyectos de tipo x finalizaron este año.

### Ejercicio 10 Logico

Se debe modelar la información necesaria para una herramienta que permita realizar el seguimiento de tareas que desempeña determinada empresa en sus proyectos. La herramienta debe permitir almacenar información básica de cada proyecto, el conjunto de tareas que involucra el proyecto e información sobre los empleados que se desempeñan implementando las tareas o bien coordinando proyectos y los servicios necesarios para cada proyecto. De los empleados se registran DNI, apellido, nombre, fecha nacimiento, dirección detallada, email y teléfono de contacto. Además, para cada empleado se debe registrar un nombre de usuario y clave para utilizar la herramienta. De cada proyecto se registra un código único, un título, descripción, fechas de inicio y finalización, el presupuesto asignado, quien es el empleado coordinador del proyecto y si requiere servicios externos información de los mismos, indicando además fecha de inicio y fin del servicio. Cada proyecto se divide en tareas, de cada tarea se registra: número único de tarea, nombre, descripción, tipo de tarea, porcentaje realizado, fecha de inicio y fecha de fin de la misma, estado de la tarea (pendiente, ejecución, finalizada, cerrada, etc), empleado que cargó la tarea y empleado asignado para realizarla (si posee). Además, la tarea puede tener uno o varios empleados seguidores de la misma, se debe dejar registro de los seguidores de cada tarea. Las tareas se pueden dividir en varias subtareas, se debe registrar para cada tarea la o las tareas que la componen. De los servicios externos se registra: código de servicio, nombre,costo y la empresa que lo brinda. El código de servicio es relativo a la empresa, es decir no se repite dentro de la empresa. De las empresas se detalla razón social, teléfonos de contacto y dirección detallada de la misma. Tenga en cuenta que ese servicio podría ser utilizado posteriormente en otro proyecto. La herramienta debe permitir realizar estadísticas tales como cuáles son las tareas en determinado estado, que empleado tiene más tareas asignadas, cuales son las tareas de un determinado proyecto, entre otras

### Ejercicio 11 Logico

Se trata de modelar la información de clientes de una peluquería. De cada cliente debe modelarse la información personal: nombre, apellido, fecha de nacimiento, DNI, dirección y teléfonos, además de una descripción si es alérgico a algún componente químico. De cada cliente se tiene una ficha, la misma permite determinar las atenciones que se le realizaron al cliente. De cada atención se debe registrar fecha de atención, que peluquero lo atendió, si se le realizó tratamiento detalle del o los mismos. Se deberá indicar para cada tratamiento aplicado que componentes se utilizaron (en caso de ser necesario) y cantidad de cada componente. Existen diferentes tratamientos. Los tratamientos se identifican por su nombre, y además se registra una descripción, precio, duración y los componentes necesarios para el mismo (algunos tratamientos pueden no requerir componentes), indicando cantidad sugerida por cada componente. De los componentes se registra código único de componente, nombre, marca que lo fabrica. De cada peluquero se registran: DNI, apellido, nombre, domicilio detallado, teléfono de contacto. Tenga en cuenta que el valor de los tratamientos varía, se debe poder determinar cuánto pagó un cliente x, por el tratamiento y en una fecha determinada. El cliente puede abonar la atención en efectivo, con débito o crédito, debiéndose registrar el modo de pago. Si abona con débito o crédito, debe quedar registro del número de tarjeta (número único), código de seguridad, banco y entidad que la emite (visa, mastercard,..). Si el pago es con crédito se debe registrar además la cantidad de cuotas en que realizó el pago. Los nombres de entidades emisoras y bancos son únicos.
**Nota:** tenga en cuenta que la tarjeta se puede usar en n pagos y en diferente cantidad de cuotas en cada caso

### Ejercicio 12 Logico
Se debe modelar la información necesaria para la gestión de un colegio de la ciudad de La Plata, el mismo cuenta con tres niveles de enseñanza: jardín de infantes, primaria y secundaria. Se debe almacenar información de los alumnos indicando: nombre, apellido, DNI, fecha de nacimiento, dirección detallada, teléfonos, descripción de alergias(si posee), si es celíaco, diabético o intolerante a la lactosa y el nivel de enseñanza que se encuentra. De los alumnos se conoce además información de sus tutores, indicando: DNI, nombre, apellido, teléfonos de contacto, email, dirección detallada, si permite contactar por WhasthApp (nro de telefono para WhasthApp) y vínculo con el alumno. Además, los alumnos de jardín y primaria pueden tener personas autorizadas a retirarlos, de estos se almacena la misma información que la de los tutores. Si un alumno es retirado se debe dejar constancia de fecha y hora de retiro, alumno y el tutor o persona autorizada que lo retira. El colegio brinda servicio de catering para sus alumnos, para ello cuenta con un menú diario de platos donde se almacena: día de la semana, costo del menú de ese día, descripción de posibles platos y una opción de plato para celíacos. Diariamente se debe dejar constancia de los alumnos que consumieron el menú diario, indicando alumno, fecha y menú consumido. Además se debe registrar información relacionada a los pagos realizados al colegio indicando: fecha y hora, tutor que abona, a que alumno/s corresponde el pago, monto, la forma de pago con la que realiza el mismo y qué concepto está pagando: si es un pago de catering o de matrícula o bien si es un pago de cuota mensual (se debe almacenar número de cuota y año que abona). Si el pago se realiza con tarjeta de débito o crédito se debe dejar constancia de: nro. de tarjeta, código de seguridad, entidad emisora de la tarjeta (Visa, Mastercard,...), banco de la tarjeta y cantidad de cuotas en las que realiza el pago. (Tenga en cuenta que la tarjeta se debe poder reutilizar en otros pagos y en otra nro de cuotas)

#### Parte 2 Modelo Fisico

Para cada ejercicio plantear el correspondiente pasaje al modelo lógico y al modelo físico. Convenciones para el modelo físico:

- Subrayar con una línea las claves primarias.
- Denotar como fk a las claves externas.
- Denotar atributos opcionales con el signo de interrogación (p. ej., b3?)

### Ejercicio 1 Fisico

![](/Img/0.png)

### Ejercicio 2 Fisico

![](/Img/1.png)

### Ejercicio 3 Fisico

![](/Img/2.png)

### Ejercicio 4 Fisico

![](/Img/3.png)

### Ejercicio 5 Fisico

![](/Img/4.png)

### Ejercicio 6 Fisico

![](/Img/5.png)

### Ejercicio 7 Fisico

![](/Img/6.png)

### Ejercicio 8 Fisico

![](/Img/7.png)