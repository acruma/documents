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
