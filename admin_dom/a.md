# Instalar un dominio básico desde la interfaz gráfica

La instalación de un dominio en Windows Server se divide en dos subtareas: primero tendremos que instalar el rol Servicios de dominio de Active Directory en el servidor y después convertiremos el servidor en un controlador de dominio.

#### Instalar el rol Servicios de dominio de Active Directory:

La instalación de roles y características de Windows Server 2016, se realiza desde la herramienta Administrador del servidor. Lo normal es que se abra automáticamente al iniciar sesión con la cuenta de Administrador, pero si la has cerrado, puedes encontrarla, fácilmente, haciendo clic sobre el botón Inicio.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/a/a01.jpg)

Una vez abierta la ventana del Administrador del servidor, comenzaremos haciendo clic sobre el enlace Agregar roles y características de la página principal de la ventana.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/a/a02.jpg)

Al hacerlo, se iniciará el Asistente para agregar roles y características. Es importante seguir las recomendaciones del propio asistente.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/a/a03.jpg)

Elegimos Instalación basada en características o en roles y hacemos clic sobre el botón Siguiente.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/a/a04.jpg)

El siguiente paso será elegir la opción: Seleccionar un servidor del grupo de servidores. De esta forma, obtendremos una lista con los servidores de nuestra red local que ejecutan Windows Server 2016. En nuestro caso, sólo aparece el servidor en el que estamos trabajando.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/a/a05.jpg)

En la siguiente etapa, tendremos que elegir el servicio o servicios que queremos instalar. Seleccionamos la opción: Servicios de dominio de Active Directory.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/a/a06.jpg)

Al hacerlo, el asistente nos muestra un aviso indicando que los servicios elegidos dependen de otros roles y características que necesitaremos instalar también de forma complementaria.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/a/a07.jpg)

Al volver a la ventana del asistente, comprobamos que la línea Servicios de dominio de Active Directory ya aparece seleccionada. Hacemos clic sobre el botón Siguiente.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/a/a08.jpg)

Después de seleccionar los roles, el asistente nos ofrece la posibilidad de instalar características. Nos limitamos a hacer clic sobre el botón Siguiente.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/a/a09.jpg)

Después de esto, aparece una pantalla informativa que debemos leer atentamente. Cuando estemos seguros de haber entendido toda la información, haremos clic en el botón Siguiente.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/a/a10.jpg)

Antes de proceder con la instalación, marcamos la opción Reiniciar automáticamente el servidor de destino en caso necesario. Al hacerlo aparece un cuadro de diálogo que nos advierte de que al marcar la opción, pueden producirse reinicios sin notificaciones previas. Lo marcamos. Por último, en la pantalla que resumen de la instalación, podemos comprobar los distintos roles y características que van a instalarse.Hacemos clic sobre el botón Instalar.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/a/a11.jpg)

Cuando termine la instalación, aparecerá un enlace con el texto: Promover este servidor a controlador de dominio. Es ahora el momento de pasar a la segunda subtarea.


#### Convertir el servidor en un controlador de dominio:

Después de realizar la instalación del rol Servicios de dominio de Active Directory, bastaría con hacer clic sobre el enlace: Promover este servidor a controlador de dominio de la última pantalla del asistente. Así iniciaremos la promoción.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/a/a12.jpg)

Al hacerlo, se abrirá la ventana del Asistente para configuración de Servicios de dominio de Active Directory.

En la primera pantalla, deberemos indicar el tipo de operación que queremos implementar. Lógicamente, como en este caso estamos partiendo de una situación en la que no disponemos de infraestructura previa, la opción que deberemos elegir es la última. 

Cuando lo hagamos, en la parte inferior se nos solicitará el dominio raíz para el nuevo bosque. Si disponemos de un dominio registrado en Internet, aquí incluiremos el nombre de dicho dominio. Sin embargo, de momento supondremos que no es así y terminaremos nuestro dominio en .local (p. ej. ejemplo.local).

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/a/a13.jpg)

En el siguiente paso (Opciones del controlador de dominio) indicamos el nivel de funcionalidad del controlador. Si no tenemos en la red controladores de dominio que ejecuten versiones más antiguas de Windows Server, deberemos elegir Windows Server 2016. 

Bajo el epígrafe: Especificar capacidades del controlador de dominio, indicaremos que el equipo también actuará como ‘Servidor de Sistema de nombres de Dominio (DNS)’.

Por último, antes de cambiar de página, deberemos escribir la contraseña del modo de restauración de servicios de directorio (DSRM).

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/a/a14.jpg)

En el siguiente paso nos limitaremos a hacer clic sobre el botón Siguiente, ya que no se encuentra un Servidor DNS principal, como nos dice advierte el mensaje que aparece.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/a/a15.jpg)

A continuación, en el paso Opciones adicionales, el asistente sugiere un nombre NetBIOS para el dominio raíz del bosque. Lógicamente, podemos aceptar el nombre que nos propone o indicar cualquier otro.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/a/a16.jpg)

Después de esto, en el apartado Rutas de acceso, el asistente nos pregunta dónde queremos almacenar los archivos de trabajo de Active Directory. Como en nuestro caso no hay otra opción, haremos clic en Siguiente.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/a/a17.jpg)

En el apartado Revisar opciones, como cabe esperar, el asistente muestra un resumen del proceso de instalación. Si todo es correcto, basta con hacer clic sobre el botón Siguiente.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/a/a18.jpg)

Por último, en el apartado Comprobación de requisitos, se verifica que el sistema cumple todas las condiciones para convertirse en un controlador de dominio.

Como puedes ver en la imagen siguiente, pueden aparecer algunos avisos, como el que nos informa de que no puede crearse una delegación para el servidor DNS que estamos a punto de instalar, pero no supondrán ningún problema. También pueden aparecer errores que impidan la instalación del controlador de dominio.
Como en nuestro sistema no han aparecido errores, podemos hacer clic sobre el botón Instalar para completar la operación.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/a/a19.jpg)

Al finalizar la instalación, el servidor se reiniciará automáticamente.

Cuando finalmente se nos solicite la contraseña de la cuenta Administrador, veremos que la cuenta aparece precedida del nombre NetBios del dominio (en este caso, MATSER). Esta es la primera constatación de que todo ha sido correcto.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/a/a20.jpg)

Para finalizar, podremos asegurarnos de que todo el proceso ha sido correcto, observando la pantalla de propiedades del equipo. Una de las formas más sencilla de conseguirlo consiste en abrir la ventana del Explorador de archivos.

Una vez en ella, nos dirigimos al panel izquierdo de la ventana y hacemos clic, con el botón derecho del ratón, sobre el elemento Este equipo. En el menú desplegado seleccionamos Propiedades.

Al hacerlo, conseguimos que se muestre la ventana Sistema. En ella podremos comprobar que los valores de los campos Nombre completo del equipo y Dominio son correctos.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/a/a21.jpg)
