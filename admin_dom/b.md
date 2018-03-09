# Administración de cuentas de usuario y cuentas de equipos

La herramienta que nos permite administrar usuarios del dominio se llama Usuarios y equipos de Active Directory. Para ejecutarla, sólo necesitamos acceder al menú Herramientas del Administrador del Servidor. Y cuando se muestre el menú, hacemos clic sobre la opción Usuarios y equipos de Active Directory.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/b/b01.jpg)

Vemos que se abre la ventana Usuarios y equipos de Active Directory. En ella disponemos de un panel a la izquierda donde podemos ver nuestro dominio (somebooks.local) y, dentro, los diferentes contenedores de los que disponemos. Entre ellos, se encuentran Builtin y Users, los contenedores predeterminados para grupos y usuarios.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/b/b02.jpg)

#### Crear un nuevo usuario en el dominio:

Una vez elegido el contenedor donde se almacenará el nuevo usuario, sólo tenemos que hacer clic con el botón derecho del ratón sobre él. En este caso, el contenedor será Users.

En el menú de contexto que aparece, elegimos Nuevo y, a continuación, Usuario.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/b/b03.jpg)

Al hacerlo, aparecerá una nueva ventana titulada Nuevo objeto: Usuario. 

En el primer paso, tendremos que rellenar los datos del usuario: Su Nombre, Apellidos e Iniciales. Con ellos se formará el campo Nombre completo.

A continuación, escribiremos el Nombre de inicio de sesión de usuario que, en realidad, se compone de dos partes: el nombre propiamente dicho y el sufijo, que lo elegimos de una lista desplegable. Si disponemos de varios dominios en la red, en la lista aparecerá una entrada por cada uno de ellos.

Por último, el campo Nombre de inicio de sesión de usuario (anterior a Windows 2000). 

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/b/b04.jpg)

A continuación, tendremos que escribir una contraseña para el usuario, que deberá cumplir con los requerimientos de seguridad del sistema operativo. Además, en la parte inferior de la ventana disponemos de cuatro opciones que seleccionaremos a nuestro gusto.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/b/b05.jpg)

Como es habitual en todas las herramientas de configuración de Windows Server 2016, el asistente nos muestra un resumen de los datos introducidos antes de crear la cuenta de manera efectiva.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/b/b06.jpg)

Ahora ya podremos encontrar entre los usuarios la cuenta que acabamos de crear.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/b/b07.jpg)

#### Modificar valores generales de las cuentas de usuario:

Todos los ajustes de este artículo (y también del siguiente) se realizan desde la herramienta Usuarios y equipos de Active Directory. Una vez abierta la ventana, hacemos clic con el botón derecho del ratón sobre el usuario que queremos modificar. Y en el menú de contexto que aparece elegimos Propiedades.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/b/b08.jpg)

Verás que aparece una ventana titulada Propiedades, seguido del nombre del usuario que estamos editando. De forma predeterminada, estaremos situados sobre la solapa General, que contiene los datos que introdujimos en el primer paso de creación de la cuenta y otros complementarios.

Esta ventana está compuesta por 13 solapas diferentes en las que podremos modificar y administrar muchos valores de nuestra cuenta de usuario tales como pueden ser establecer horas de inicio de sesión, limitar los equipos desde los que un usuario puede iniciar sesión o averiguar de qué grupos es miembro un usuario.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/b/b09.jpg)

#### Crear una nueva cuenta de equipo en el dominio:

Para crear una cuenta de equipo, debemos volver a la herramienta Usuarios y equipos de Active Directory. Como hicimos con las cuentas de usuario, cuando se abra la ventana Usuarios y equipos de Active Directory, buscaremos en el panel de la izquierda el contenedor que nos interese. En este caso, utilizaremos el contenedor Computers. Después haremos clic con el botón derecho del ratón sobre el contenedor. En el menú de contexto que aparece, elegiremos Nuevo > Equipo.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/b/b10.jpg)

Veremos que aparece la ventana Nuevo objeto: Equipo. En ella rellenaremos los datos que nos pide.

También podremos elegir el usuario o grupo que podrá unir a este equipo al dominio, aunque, de forma predeterminada sólo lo podrán hacer los administradores.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/b/b11.jpg)

Ahora ya podremos encontrar la nueva cuenta entre los objetos del contenedor Computers.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/b/b12.jpg)

#### Modificar valores generales de las cuentas de equipo:

Igual que ocurría con las cuentas de usuario, podemos volver a la herramienta Usuarios y equipos de Active Directory en cualquier momento para ajustar las propiedades de las cuentas de equipos.

Como antes, usaremos el menú Herramientas del Administrador del Servidor y, después, Usuarios y equipos de Active Directory.

Una vez abierta la ventana, hacemos clic con el botón derecho del ratón sobre el equipo que queremos modificar. En el menú de contexto que aparece elegimos Propiedades.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/b/b13.jpg)

Aparece la ventana titulada Propiedades, seguido del nombre de la cuenta elegida. Aquí disponemos de multitud de características diferentes de la cuenta, organizadas en 7 solapas distintas.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/b/b14.jpg)

#### Restablecer cuentas de equipo:

En ocasiones, tratamos de iniciar sesión en el dominio desde un equipo cliente y recibimos un error de conexión aún después de asegurarnos de que los datos que hemos introducido son correctos.

Esto puede ocurrir porque se ha desincronizado la contraseña que introducimos con la almacenada en la Autoridad de Seguridad Local. Para resolverlo, volveremos a abrir la herramienta Usuarios y equipos de Active Directory, buscaremos la cuenta de equipo que está ocasionando los problemas y haremos clic sobre ella con el botón derecho del ratón.

En el menú de contexto que aparece, hacemos clic sobre Restablecer la cuenta. Aparecerá un cuadro de diálogo que nos pregunta si estamos seguros de reiniciar la cuenta. Cuando concluya la operación, aparecerá un nuevo mensaje indicando que la cuenta se ha restablecido correctamente.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/b/b15.jpg)
