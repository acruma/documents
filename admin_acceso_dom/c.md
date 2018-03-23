# Controlar el acceso a recursos locales y en la red

Lo primero que tenemos que tener en cuenta sería diferenciar correctamente entre compartir recursos y dar permisos a estos recursos. Cuando nosotros compartimos un recurso con algún usuario o con el grupo: Todos, no significa que algún miembro de ese grupo: Todos, pueda tener acceso a ese recurso, ya que antes necesitamos configurar los permisos. De forma inversa, si un usuario tiene los permisos en un recurso pero no se le ha compartido este recurso, no podrá acceder.

Para administrar todos los recursos usaremos la herramienta de Administrador del servidor. En el panel de la izquierda, seleccionaremos Servicios de archivos y de almacenamiento. Y por último, entraremos en el menú de Recursos compartidos.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/c/c00.jpg)

Crear un recurso compartido:

Ahora procederemos a crear nuestro primer recurso compartido. Nosotros en primer lugar vamos a crear la carpeta llamada Recursos en la que todos los usuarios y grupos del dominio tendrán acceso. En la pantalla de Recursos compartidos seleccionaremos en TAREAS y hacemos click en Nuevo recurso compartido.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/c/c01.jpg)

Nos aparece un asistente para crearlo y procedemos a seguir los pasos indicados:

En primer lugar seleccionamos Recurso compartido SMB - Rápido.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/c/c02.jpg)

En el segundo paso seleccionamos la ruta del recurso creado.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/c/c03.jpg)

Seguiremos asignando un nombre al recurso y opcionalmente, una descripción.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/c/c04.jpg)

Este paso es clave para nuestro recurso ya que va a ser el que certifique a quien va a ser compartido y los permisos que va a tener cada usuario o grupo respecto este recurso. En este caso no lo editaremos porque esta va a ser la carpeta que contenga a los diferentes recursos por lo que este recurso estará compartido con todos.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/c/c05.jpg)

Por último, confirmamos los cambios realizados y ya tendremos nuestro primer recurso.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/c/c06.jpg)

Creación de diferentes recursos compartidos para la comprobación con cliente:

Hemos creado 4 recursos compartidos diferentes para comprobar diferentes situaciones respecto a un usuario:

Primera situación:

La primera de estas situaciones será crear un nuevo recurso que hemos llamado Sergio y que queremos configurar como la carpeta principal del usuario Smxrlxp.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/c/c07.jpg)

La creamos siguiendo los pasos anteriormente explicados pero ahora nos detendremos en el apartado de permisos. Para configurarlos de manera en que solo tenga acceso a esta carpeta Sergio y el administrador del servidor, lo haremos de la siguiente manera:

Hacemos click en Personalizar permisos.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/c/c08.jpg)

En la pestaña de Permisos, hacemos click en Deshabilitar herencia. De esta forma podremos eliminar todos los permisos de la pestaña Permisos y de la pestaña Compartir. 

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/c/c09.jpg)

Cuando hayamos eliminado todos los permisos anteriores procederemos a crear los permisos que nos hacen falta según la situación que queremos que se de. En primer lugar configuraremos los permisos de acceso  en el recurso creado. Para ello nos situamos en la pestaña Compartir y pulsamos en Agregar.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/c/c10.jpg)

Hacemos click en Seleccionar una entidad de seguridad.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/c/c11.jpg)

En el recuadro blanco añadimos (como ya aprendimos en el documento anterior) al usuario o grupo al que queramos asignarle permisos y pulsamos en Aceptar.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/c/c12.jpg)

Le asignamos los permisos que le queramos dar. En este caso tendrá Control total ya que será su carpeta personal.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/c/c13.jpg)

Hacemos los mismos pasos pero con el usuario Administrador. Y de esta forma quedarán los permisos de acceso.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/c/c14.jpg)

De la misma forma lo hacemos en la pestaña Permisos. Quedará como muestra la siguiente imagen. Como ya hemos dicho para que se apliquen correctamente los permisos el usuario o grupo tiene que configurarse en la pestaña Permisos y en la pestaña Compartir.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/c/c15.jpg)

De esta forma ya habremos creado el recurso que pretendíamos.


Segunda situación: 

En esta segunda situación el recurso se llamará Alumnos en la que nuestros dos usuarios Smxrlxp y Acruma tendrán control total.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/c/c16.jpg)

Estos son los permisos dados:

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/c/c17.jpg)

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/c/c18.jpg)

Tercera situación:

Ahora crearemos un recurso exclusivo para nuestro usuario Acruma, en la que solo él y el administrador tendrán control total.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/c/c19.jpg)

Estos son los permisos dados:

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/c/c20.jpg)

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/c/c21.jpg)

Cuarta situación:

Por último, crearemos un recurso al que puedan compartir archivos profesores con alumnos.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/c/c22.jpg)

En este caso en la pestaña Compartir le daríamos Control total a los dos grupos.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/c/c23.jpg)

Pero en la pestaña Permisos modificaremos los permisos del grupo Alumnos para que estos solo puedan leer y ejecutar los archivos de este recurso.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/c/c24.jpg)

De esta forma quedarán establecidos los permisos:

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/c/c25.jpg)

En el último caso hemos establecido diferentes permisos en la diferentes pestañas para el mismo grupo. Esto os puede causar alguna confusión pero nuestro servidor siempre escogerá la opción más restrictiva de las dos por lo que en este caso se ajustará a los permisos dados en la pestaña Permisos.

Comprobaciones:

Para finalizar, haremos las comprobaciones desde el nuestro usuario Smxrlxp conectado como cliente. Como podemos ver en la imagen, accederemos a  los recursos entrando en el explorador de archivos, en el apartado Red.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/c/c26.jpg)

En nuestro primer caso, creamos el recurso llamado Sergio que tenía Control total para el usuario Smxrlxp por lo que podremos crear carpetas y archivos como podemos ver.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/c/c27.jpg)

En el segundo caso creamos el recurso llamado Alumnos en el que todos los usuarios pertenecientes a este grupo tendrán control total.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/c/c28.jpg)

En el tercer caso, creamos el recurso llamado Mateo que tenía Control total para el usuario Acruma por lo que en este caso que estamos intentando acceder desde el usuario Smxrlxp nos aparece un mensaje en el que nos dice que no tenemos permisos para acceder a este recurso.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/c/c29.jpg)

Por último, creamos el recurso llamado Profesores-Alumnos. En este caso como podemos ver, podemos acceder al recurso y leer los archivos pero no podemos crear nada ya que nuestro usuario pertenece al grupo Alumnos y este solo tiene permisos de acceso y lectura.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/c/c30.jpg)
