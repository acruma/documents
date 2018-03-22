# Unir un cliente Windows 10 a un dominio Windows Server 2016

El primer paso, para comenzar a utilizar los recursos que ofrece un dominio, consiste en añadir a dicho dominio los ordenadores que puedan actuar como clientes.

En este caso, comenzaremos por un ordenador que está ejecutando Microsoft Windows 10.

Básicamente, el proceso consistirá en realizar los siguientes pasos:

- Establecer las características de red, para que coincidan con las necesidades del dominio.

- Ajustar el nombre del equipo cliente.

- Unir el equipo al dominio.

Al final del proceso, iniciaremos sesión en el equipo cliente usando una cuenta de usuario de las que ya tenemos definidas en el dominio. Con esto comprobaremos que el proceso se ha realizado correctamente.

Así es que, si estás listo, pongamos manos a la obra.

#### Configuración de la red del equipo cliente:

Para conseguir que un cliente pueda unirse a un dominio, antes deberemos asegurarnos de que las características de su configuración de red sean coincidentes con las necesidades del dominio. 

En nuestro dominio configuramos el siguiente direccionamiento:

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/a/a01.jpg)

La diferencia es que, ahora, podemos dejar habilitada la asignación automática de IP, pero debemos asegurarnos de que el Servidor DNS preferido hace referencia a la dirección IP del controlador del dominio.

En definitiva, podemos dejar una configuración como la que muestra la siguiente imagen:

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/a/a02.jpg)

#### Comprobar que la configuración de red es correcta:

Después de completar el apartado anterior, debemos comprobar que no hemos cometido ningún error. Esto es tan sencillo como abrir una ventana de comandos y hacer un ping al Servidor.

Si utilizamos el nombre del servidor en lugar de su dirección IP, no sólo estaremos comprobando que el equipo cliente está en la misma red que el servidor. También comprobaremos que la configuración DNS del cliente es correcta y que el servidor DNS del controlador de dominio está funcionando adecuadamente.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/a/a03.jpg)

Si todo es correcto, el servidor responderá y la salida será parecida a lo que muestra la imagen anterior.

#### Cambiar el nombre del equipo y unirlo al dominio:

El siguiente paso consistirá en ajustar el nombre del equipo cliente, para que coincida con un nombre de equipo definido en el dominio. Al indicar el nombre del dominio, el sistema procederá a establecer el vínculo. En el documento anterior, ya teníamos una cuenta de equipo en el dominio con el nombre Cliente01-Win10.

Para comenzar, hacemos clic, con el botón derecho del ratón, sobre el botón Inicio. En el menú que aparece, elegimos la opción Sistema.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/a/a04.jpg)

Al hacerlo, aparecerá una ventana con información del sistema. En la parte inferior, además de algunos detalles sobre el hardware del equipo, podemos encontrar su nombre. 

Para cambiar estos datos, sólo tenemos que hacer clic en el enlace Cambiar configuración. En la ventana Propiedades del sistema, haremos clic sobre el botón Cambiar, para escribir el nuevo nombre del equipo y nombre del dominio.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/a/a05.jpg)

En el campo Nombre de equipo, debemos asegurar de escribir el nombre de la cuenta del dominio. Además, en el área Miembro del, elegiremos la opción Dominio y debajo escribiremos el nombre del dominio al que queremos unir el equipo.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/a/a06.jpg)

En ese momento, Windows 10 busca en la red el dominio especificado. Si no lo encuentra, aparecerá un mensaje de aviso.

Si lo encuentra, deberemos escribir un nombre de usuario y una contraseña, perteneciente al dominio, que tenga privilegios suficientes para unir el equipo cliente.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/a/a07.jpg)

La ventana de autenticación se cierra y en su lugar aparece un mensaje indicando que el equipo se ha unido correctamente al dominio. A continuación, aparece una nueva ventana informativa indicando que deberemos reiniciar el equipo para que se apliquen los cambios, pero que antes deberemos cerrar todos los programas y guardar todos los archivos que tengamos abiertos. Cuando cerremos la ventana de Propiedades del sistema, detectará que ya no hay programas en ejecución y nos dará la oportunidad de reiniciar en ese momento.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/a/a08.jpg)
