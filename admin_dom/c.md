# Se ha centralizado la información personal de los usuarios del dominio mediante el uso de perfiles móviles y carpetas personales.

### Crear la carpeta contenedora para los perfiles

Para crear la carpeta contenedora, comenzaremos por abrir el Explorador de archivos.

![imagen](https://github.com/smxrlxp/dominios.html/blob/master/assets/c/1.png)

Después, nos desplazamos hasta el lugar donde queremos crear la carpeta compartida. Una vez allí, hacemos clic con el botón derecho del ratón sobre cualquier espacio libre del área de trabajo.

![imagen](https://github.com/smxrlxp/dominios.html/blob/master/assets/c/2.png)

Así, creamos una nueva carpeta y, a continuación, le damos el nombre que queramos.

### Cambiar los permisos para dar el control a los usuarios de un grupo.

Una vez creada la carpeta contenedora, debemos cambiar sus permisos para que los usuarios del grupo que hemos elegido puedan tener todo el control sobre ella.

Para lograrlo, comenzamos por hacer clic con el botón derecho del ratón sobre ella.

![imagen](https://github.com/smxrlxp/dominios.html/blob/master/assets/c/3.png)

Cuando aparezca la ventana Propiedades: Nombre_Carpeta hacemos clic en la solapa Compartir.

![imagen](https://github.com/smxrlxp/dominios.html/blob/master/assets/c/4.png)

En la ventana Uso compartido avanzado, que aparece a continuación, hacemos clic en Compartir esta carpeta.

![imagen](https://github.com/smxrlxp/dominios.html/blob/master/assets/c/5.png)

A continuación, aparece la ventana Seleccionar Usuarios, Equipos, Cuentas de servicio o Grupos. Aquí podemos actuar de varias formas, por ejemplo, escribiendo el principio del nombre del grupo con el que queremos compartir la carpeta…

![imagen](https://github.com/smxrlxp/dominios.html/blob/master/assets/c/6.png)

Al cerrarse la ventana, volvemos a la ventana Permisos de Perfiles. Nos aseguramos de que está seleccionado el grupo seleccionado...

![imagen](https://github.com/smxrlxp/dominios.html/blob/master/assets/c/7.png)

También podemos evitar que accedan a la carpeta el resto de los usuarios.

![imagen](https://github.com/smxrlxp/dominios.html/blob/master/assets/c/8.png)

Después de esto, ya podemos cerrar todas las ventanas….

### Cambiar el lugar donde el usuario o los usuarios guardan su perfil

A partir de ahora es cuando realmente vamos a crear el perfil móvil. Para conseguirlo, volveremos a la consola Usuarios y equipos de Active Directory y localizamos la cuenta (o cuentas) a la que queremos asignar el perfil móvil. Cuando la localicemos, haremos clic con el botón derecho del ratón sobre ella.

![imagen](https://github.com/smxrlxp/dominios.html/blob/master/assets/c/9.png)

En la ventana de propiedades de la cuenta, hacemos clic sobre la solapa Perfil. En ella, debemos dar valor al cuadro de texto Ruta de acceso al perfil. El contenido seguirá el siguiente formato:

`\\servidor\carpeta_compartida\nombre_usuario`

![imagen](https://github.com/smxrlxp/dominios.html/blob/master/assets/c/10.png)

Y... Listo!
