# Crear y administrar grupos de seguridad

Los principales temas que vamos a tratar son como crear una cuenta de grupo y, a continuación, a modificar sus propiedades, veremos cómo asignarle miembros, cómo eliminarlos e incluso cómo eliminar al propio grupo.

Crear una cuenta de grupo de seguridad:

Si lo que queremos es crear un nuevo grupo, deberemos volver a la herramienta Usuarios y equipos de Active Directory.

Como en ocasiones anteriores, cuando se abra la ventana Usuarios y equipos de Active Directory, buscaremos en el panel de la izquierda el contenedor en el que queramos guardar el nuevo grupo. En este caso, volveremos a usar el contenedor Users, que ya utilizamos para las cuentas de usuario.

Después haremos clic con el botón derecho del ratón sobre el contenedor. En el menú de contexto que aparece, elegiremos Nuevo > Grupo.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/d/d01.jpg)

Veremos que aparece la ventana Nuevo objeto: Grupo. En ella, rellenaremos el nombre que queremos darle a la cuenta de grupo que estamos creando (Nombre de grupo).

Por defecto, el nombre que escribamos se utilizará para completar el campo Nombre de grupo (anterior a Windows 2000). También, en el apartado de Ámbito de grupo estará seleccionado en la opción Global y en el apartado Tipo de grupo estará seleccionado la opción Seguridad que es la que queremos en esta ocasión.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/d/d02.jpg)

Ahora ya podremos encontrar la nueva cuenta entre los objetos del contenedor Users.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/d/d03.jpg)

#### Modificar valores en las cuentas de los grupos:

Como en ocasiones anteriores, podemos volver a la herramienta Usuarios y equipos de Active Directory siempre que necesitemos ajustar las propiedades de las cuentas de grupos.

Cuando se abra la ventana, haremos clic con el botón derecho del ratón sobre el grupo que queremos modificar. En el menú de contexto que aparece elegimos Propiedades.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/d/d04.jpg)

Aparece la ventana titulada Propiedades:, seguido del nombre de la cuenta elegida. Aquí disponemos de multitud de características de la cuenta, organizadas en 4 solapas diferentes.

Como puedes ver, en la solapa General, además de poder cambiar el Nombre de grupo (anterior a Windows 2000), la Descripción y el Correo electrónico donde se recibirán incidencias relacionadas con el grupo, también podemos modificar el Ámbito del grupo y el Tipo de grupo.

Desde la solapa Miembros, elegiremos los usuarios, equipos o grupos que son miembros del grupo que estamos editando. Para verlo en detalle, dedicaremos más adelante un apartado completo a este aspecto.

Utilizaremos la solapa Miembro de, para hacer que este grupo sea, a su vez, miembro de un grupo distinto. Como en el caso anterior, estudiaremos este aspecto con más detalle en un apartado más adelante.

Y por último, la solapa Administrado por, nos permite delegar la administración de este grupo en otro usuario diferente.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/d/d05.jpg)


#### Añadir miembros a un grupo:

Ya hemos visto cómo convertir a un usuario en miembro de un grupo desde la propia cuenta de usuario. Sin embargo, si necesitamos añadir varios usuarios, será mucho más cómodo hacerlo desde el propio grupo.

Para añadir un nuevo miembro a un grupo, deberemos abrir la ventana Propiedades de dicho grupo y elegir la solapa Miembros.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/d/d06.jpg)

Aparecerá la ventana Seleccione Usuarios, Contactos, Equipos, Cuentas de servicio o Grupos.

Si ya conocemos los nombres de las cuentas que vamos a incluir, sólo tendremos que escribirlos en el cuadro titulado Escriba los nombres de objeto que desea seleccionar. Sin embargo, lo más probable es que prefiramos elegirlos de una lista. En ese caso, haremos clic sobre el botón Opciones Avanzadas.

Si tenemos idea de los primeros caracteres que tienen las cuentas de usuario que estamos buscando, podemos escribirlos a continuación de Empieza con (en la lista desplegable también podemos elegir una búsqueda exacta, pero resulta menos flexible).

Lo más sencillo es dejarlo todo en blanco. A continuación, hacemos clic en Buscar ahora.
Veremos que en el cuadro Resultado de la búsqueda aparecen todos los elementos que podemos seleccionar. Sólo queda elegir los que queramos. Cuando terminemos, hacemos clic sobre Aceptar.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/d/d07.jpg)

La ventana Seleccione Usuarios, Contactos, Equipos, Cuentas de servicio o Grupos vuelve a su aspecto normal y muestra los nombres de las cuentas que hemos elegido. Podemos repetir el proceso tantas veces como sean precisas para seleccionar las cuentas que necesitemos.

Cuando acabemos, volveremos a hacer clic en Aceptar.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/d/d08.jpg)

De vuelta en la ventana Propiedades, veremos que ya aparecen los nuevos miembros.

Ya podemos cerrar la ventana.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/d/d09.jpg)


#### Eliminar miembros de un grupo:

Para eliminar a cualquiera de los miembros de un grupo, basta con volver a la ventana Propiedades de dicho grupo y elegir, de nuevo, la solapa Miembros.

A continuación, elegiremos el usuario que queremos que deje de ser miembro del grupo. Después de hacerlo, aparecerá un mensaje para confirmar que estamos seguros de la eliminación.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/d/d10.jpg)

Para terminar, sólo tenemos que hacer clic sobre el botón Sí. Y hacemos clic sobre el botón Quitar.


#### Convertir a un grupo en miembro de otro grupo:

Convirtiendo a un grupo en miembro de otro grupo, éste heredará todos sus permisos. Y por lo tanto, también sus miembros. De este modo, podemos crear una estructura jerárquica de grupos, evitando repetir en unos grupos la asignación de permisos que hayamos configurado en otros.

Para que un grupo sea miembro de otro grupo, basta con volver a la ventana Propiedades de dicho grupo y elegir la solapa Miembro de.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/d/d11.jpg)

Esto hará que se muestre una ventana titulada Seleccionar Grupos, casi idéntica a la ventana Seleccione Usuarios, Contactos, Equipos, Cuentas de servicio o Grupos que vimos más arriba.

Como antes, podríamos hacer clic, directamente, sobre el botón Opciones avanzadas y hacer una búsqueda o elegir el grupo de la lista completa.

Sin embargo, para aprender un modo diferente de manejar esta ventana, supondré que sabemos cómo empieza el nombre del grupo que buscamos. En ese caso, bastará con escribirlo en el cuadro de texto Escriba los nombres de objeto que desea seleccionar.

Después, haremos clic sobre el botón Comprobar nombres.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/d/d12.jpg)

Si existe más de un nombre de grupo que comienza por los mismos caracteres, se mostrará una ventana titulada Nombres múltiples encontrados. En ella, seleccionamos el grupo correcto y pulsamos el botón Aceptar.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/d/d13.jpg)

De vuelta en la ventana Seleccionar Grupos, comprobamos que ya aparece el grupo elegido. Para completar la selección, hacemos clic sobre el botón Aceptar.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/d/d14.jpg)

De este modo, habremos conseguido que el grupo elegido aparezca en la lista Miembro de. Sólo nos queda volver a hacer clic sobre el botón Aceptar para completar la tarea.

#### Conseguir que un grupo deje de ser miembro de otro:

Para realizar la operación contraria a la anterior, es decir, lograr que un grupo deje de ser miembro de otro grupo, sólo hay que volver a la ventana Propiedades de dicho grupo y elegir la solapa Miembro de. Una vez ahí, elegimos el grupo que queremos eliminar.

A continuación, basta con hacer clic sobre el botón Quitar.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/d/d15.jpg)

Al hacerlo, aparecerá un mensaje para confirmar que estamos seguros de la eliminación. Para continuar, sólo tenemos que hacer clic sobre el botón Sí. Al volver a la ventana de propiedades, comprobaremos que el grupo ya no aparece.

#### Eliminar grupos:

No es frecuente que se eliminen grupos en un dominio. Sin embargo, en ocasiones podemos necesitar reestructurar el esquema de nuestra red y puede resultar interesante distribuir las cuentas de una forma diferente a como lo habíamos hecho hasta ese momento. En ese escenario, será muy útil crear nuevos grupos y eliminar los que ya teníamos.

Como en ocasiones anteriores, podemos volver a la herramienta Usuarios y equipos de Active Directory siempre que necesitemos ajustar las propiedades de las cuentas de grupos.

Después, hacemos clic con el botón derecho sobre el grupo que queremos eliminar. En el menú de contexto que aparece elegimos la opción Eliminar.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/d/d16.jpg)

Aparecerá un mensaje para confirmar que estamos seguros de la eliminación. Si estamos conformes, hacemos clic en el botón Sí.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/d/d17.jpg)
