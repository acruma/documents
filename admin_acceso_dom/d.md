# Requerimientos de Seguridad

#### Copias de Seguridad - Instalación del rol necesario

Antes de poder hacer copias de seguridad en el controlador de dominio, tenemos que proceder a instalar la herramienta necesaria mediante la instalación de un rol o  característica.

En realidad, se trata de un proceso muy sencillo.

Comenzamos por abrir el Administrador del servidor y, en el menú Administrar, elegir Agregar roles y características.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/d/d01.jpg)

Es importante seguir las recomendaciones del propio asistente en cuanto a asegurarnos de que la contraseña de la cuenta de Administrador es segura, que la configuración de red es correcta, que disponemos de direcciones IP estáticas y que hemos instalado las últimas actualizaciones de seguridad en el sistema operativo.

Una vez que todo sea correcto, hacemos clic en el botón Siguiente.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/d/d02.jpg)

Elegimos Instalación basada en características o en roles y hacemos clic sobre el botón Siguiente.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/d/d03.jpg)

Obtendremos una lista con los servidores de nuestra red local que ejecutan Windows Server 2016. Lógicamente, sólo se muestran los servidores que estén funcionando y se haya completado su recopilación de datos.

En nuestro caso, sólo aparece el controlador de dominio en el que estamos trabajando.

Hacemos clic sobre su entrada y, a continuación, sobre el botón Siguiente.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/d/d04.jpg)

Como hemos dicho antes, Copias de seguridad de Windows Server es una característica, lo que implica que en la etapa Seleccionar roles del servidor no tendremos que hacer nada.

Nos limitamos a hacer clic sobre el botón Siguiente.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/d/d05.jpg)

Cuando lleguemos a Seleccionar características, buscamos en la lista central la línea  con el texto Copias de seguridad de Windows Server y hacemos clic sobre su casilla de verificación.

A continuación, hacemos clic sobre el botón Siguiente.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/d/d06.jpg)

Antes de proceder con la instalación, tenemos la oportunidad de marcar la opción Reiniciar automáticamente el servidor de destino en caso necesario. Sin embargo, para el caso que nos ocupa no resulta imprescindible. S

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/d/d07.jpg)

A partir de aquí, en la parte superior de la ventana podremos ver una barra de progreso que nos mantiene informados del avance de la instalación.

Cuando la barra de progreso haya llegado al final, aparecerá bajo ella el texto Instalación correcta en MATSER-WIN.matser.local.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/d/d08.jpg)

A partir de aquí tendremos disponible la herramienta de Copias de Seguridad.

#### Copias de Seguridad - Realizar copia de seguridad

Para acceder a la herramienta, necesitaremos recurrir, como es habitual, al Administrador del servidor.

Comenzaremos haciendo clic en el menú Herramientas. Y a continuación, sobre la opción Copias de seguridad de Windows Server.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/d/d09.jpg)

En la ventana Copias de seguridad de Windows Server (local), hacemos clic sobre la opción copia de seguridad local del panel izquierdo.

Y en el panel Acciones hacemos clic sobre el enlace Hacer copia de seguridad una vez …

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/d/d10.jpg)

Esto hará que se abra la ventana Asistente para hacer copia de seguridad una vez.

Lo primero será decidir entre dos opciones:

Si hacemos una copia de seguridad siguiendo los valores elegidos en una copia de seguridad programada anterior.
Si queremos realizar una copia de seguridad con parámetros diferentes a los de la copia programada.

En el caso de la imagen siguiente, la primera opción aparece inactiva porque aún no se ha realizado ninguna copia programada. Por lo tanto, elegiremos la segunda opción.

Para continuar, haremos clic sobre el botón Siguiente.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/d/d11.jpg)

En el siguiente paso, decidiremos si la copia es del Servidor completo (incluyendo todos los volúmenes, e incluso el estado del propio sistema) o Personalizada (donde podremos excluir los volúmenes que queramos).

Nosotros elegiremos la primera opción. 

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/d/d12.jpg)

El siguiente paso consistirá en elegir un destino para la copia de seguridad. Podemos escoger entre una unidad local y una carpeta compartida en la red por otro servidor donde tengamos los permisos adecuados.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/d/d13.jpg)

El siguiente paso es continuación del anterior. Como antes hemos elegido Unidades locales, ahora indicaremos, en la lista desplegable Destino de la copia de seguridad, el volumen de destino. Si hubiésemos indicado Carpeta compartida remota, tendríamos que especificar la ubicación de dicha carpeta.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/d/d14.jpg)

Por último, el asistente nos muestra un resumen de los valores que hemos elegido hasta ahora.

Si todo es correcto, haremos clic sobre el botón Copia de seguridad.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/d/d15.jpg)

Al momento, veremos una ventana emergente que muestra la recogida de datos del sistema para la copia de seguridad. Nos limitamos a esperar a que se rellene la barra de progreso.

Si no hemos cerrado antes, al terminar aparecerá un resumen de los datos copiados. Hacemos clic sobre el botón Cerrar.

Una vez cerrado el asistente, en la ventana Copias de seguridad de Windows veremos una entrada con la copia recién realizada. Aquí irán apareciendo las diferentes copias que se vayan haciendo a lo largo del tiempo.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/d/d16.jpg)
