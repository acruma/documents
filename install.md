# Instalación de Windows Server 2016 mediante interfaz gráfica

Para obtener esta imagen ISO, sólo tienes que ir hasta su página de [descarga](https://www.microsoft.com/es-es/evalcenter/evaluate-windows-server-2016) e iniciar sesión con tu cuenta Microsoft. Si no dispones de una, podrás crearla sobre la marcha.

Una vez virtualizada la imagen ISO en nuestra máquina virtual, la iniciamos y veremos como comienza a cargarse la interfaz del asistente de instalación: aparecerá la primera pantalla donde tenemos que introducir información.

Se trata de la configuración del idioma, aunque en realidad se establecen tres parámetros: El propio idioma, el formato de hora, fecha y moneda, y el tipo de teclado que vamos a utilizar.
 
![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/InstWS%20(Con%20I.%20Gr%C3%A1fica)/a01.jpg)


Con esta sencilla operación, el asistente está listo para comenzar la instalación del sistema operativo.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/InstWS%20(Con%20I.%20Gr%C3%A1fica)/a02.jpg)


Poco después, el asistente nos pedirá que seleccionemos la edición concreta de Windows Server 2016 que vamos a instalar. En esta versión de evaluación aparecen cuatro opciones:

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/InstWS%20(Con%20I.%20Gr%C3%A1fica)/a03.jpg)


Seleccionaremos la segunda opción: Windows Server 2016 Standard Evaluation (Experiencia de escritorio).

Después, el asistente nos muestra el contrato de licencia correspondiente al producto que hemos elegido en el paso anterior. Es conveniente leer atentamente las condiciones.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/InstWS%20(Con%20I.%20Gr%C3%A1fica)/a04.jpg)


En el siguiente paso, debemos indicar el tipo de instalación que realizaremos, aunque, si hemos iniciado la instalación desde el DVD de instalación (como es el caso), sólo podremos elegir la opción Personalizada: instalar solo Windows (avanzado).

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/InstWS%20(Con%20I.%20Gr%C3%A1fica)/a05.jpg)


A continuación, podemos optar por asignar todo el espacio del disco duro para la instalación de Windows Server 2016. Para ello, sólo habría que hacer clic sobre el botón Siguiente. No obstante, también tenemos diferentes opciones para configurar el disco (o los discos) que tengamos en el servidor a nuestro gusto.

En nuestro caso, asignaremos todo el espacio del disco para la instalación.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/InstWS%20(Con%20I.%20Gr%C3%A1fica)/a06.jpg)


A partir de ahí, comienza el proceso de instalación en el disco. Durante el proceso el sistema se reiniciará varias veces. 

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/InstWS%20(Con%20I.%20Gr%C3%A1fica)/a07.jpg)


Cuando concluya este proceso se producirá un nuevo reinicio y la instalación habrá concluido.

Durante la instalación, se ha creado automáticamente un usuario llamado Administrador, que será el que tenga los máximos privilegios en el equipo. Sin embargo, este usuario tan importante aún no tiene asignada una contraseña. Esta será la primera tarea que deberemos completar ahora que ya está instalado Windows Server 2016.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/InstWS%20(Con%20I.%20Gr%C3%A1fica)/a08.jpg)


Poco después llegamos a la ventana de autenticación de Windows Server 2016. Ahora no se pide directamente el nombre de usuario y la contraseña, sino que se muestra la fecha y la hora y un mensaje que indica la combinación de teclas que nos permiten iniciar sesión.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/InstWS%20(Con%20I.%20Gr%C3%A1fica)/a09.jpg)

Ahora sí, el sistema nos muestra el nombre de la cuenta Administrador y nos solicita su contraseña.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/InstWS%20(Con%20I.%20Gr%C3%A1fica)/a10.jpg)


Después de esto, la cuenta Administrador ya está funcional y lista para usarse. Nada más terminar el inicio de sesión, aparecerá en pantalla un asistente que nos permite buscar otros equipos y dispositivos en la red local.

También comienza a ejecutarse la herramienta Administrador del servidor. Este asistente aparece de forma automática cada vez que iniciamos sesión con la cuenta Administrador y nos permite realizar las principales tareas de configuración del servidor.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/InstWS%20(Con%20I.%20Gr%C3%A1fica)/a11.jpg)

