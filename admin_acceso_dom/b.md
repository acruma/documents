# Se han previsto bloqueos de accesos no autorizados al dominio.

Para iniciar el proceso de configuración de las políticas de contraseña en Windows Server 2016 debemos acceder al editor de políticas de grupo y para ello contamos con las siguientes opciones. Accedemos al `Panel de control`, en la esquina superior derecha escogemos iconos pequeños. Luego `Herramientas administrativas`.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/b/1.png)

Y allí seleccionar la opción `Directiva de seguridad local`.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/b/2.png)

Una vez allí podrian darse las siguientes rutas; 

>1. Configuración del equipo

>2. Configuración de Windows

>3. Configuración de seguridad

>4. Directivas de cuenta

>5. Directiva de contraseñas.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/b/3.png)

Podemos ver que dicha política `Directiva de contraseñas` se compone de múltiples elementos como son:

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/b/4.png)
 
### Almacenar contraseñas con cifrado reversible

Esta política habilita la compatibilidad de protocolos que requieren la contraseña del usuario para el inicio de sesión.
 
Con esta política se pueden descifrar contraseñas que han sido previamente cifradas por lo cual no es recomendable su habilitación ya que algún atacante puede aprovechar su vulnerabilidad para descifrar la contraseña y acceder al equipo y con ello a los recursos compartidos.

Para realizar cualquier cambio sobre dicha política daremos doble clic sobre ella y podremos habilitarla o deshabilitarla según sea la necesidad.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/b/5.png)

### Exigir historial de contraseñas

Con esta política determinamos la cantidad de nuevas contraseñas deben estar asociadas a la cuenta antes de poder usar de nuevo la contraseña antigua. El usar la misma contraseña de forma seguida puede resultar en una fallo de seguridad dentro de nuestra gestión ya que esta será más vulnerable a un ataque de fuerza bruta.

El valor por defecto es 10 lo cual indica que hasta dentro de 10 cambios de contraseñas nuevas podremos usar la contraseña actual.

Podemos configurar el rango de veces entre 0 y 24 pero el objetivo, a nivel de seguridad, es establecer la mayor cantidad de veces posibles.

Para su edición daremos doble clic sobre la política y editaremos los valores según sean necesarios.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/b/6.png)

### La contraseña debe cumplir los requisitos de complejidad

Esta es una de las políticas más vitales para llevar a cabo una excelente configuración de políticas de contraseñas ya que acá definiremos los niveles de complejidad que deben ser obligatorios aplicar a la contraseña asignada por el usuario.
 
Con esta política indicamos la serie de requisitos a ser aplicados durante la creación de la contraseña como:

>La contraseña no debe contener el samAccountName (Nombre de cuenta del usuario) o el DisplayName
>(Nombre desplegado) sin importar si son mayúsculas o minúsculas.
>Recomendable que posea los siguientes atributos:
>Longitud mínima de 8 caracteres.
>Contener caracteres especiales como ,!, $, #, %.
>Incluir números.
>Incluir letras mayúsculas y minúsculas.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/b/7.png)

### Longitud mínima de la contraseña

Con esta política indicamos la cantidad mínima de caracteres que debe contener la contraseña para que sea aceptada por el sistema.

Allí podremos establecer valores entre 1 y 14 pero si dejamos el valor en 0 significa que el usuario ingresara sin contraseña. El valor por defecto en Windows Server 2016 es de 7 caracteres.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/b/8.png)

### Vigencia máxima de la contraseña

Esta política nos permite definir la cantidad de tiempo, en días, en las cuales la contraseña caducará y será necesario forzar al usuario a cambiarla por una nueva siguiendo las políticas configuradas. El valor por defecto es 42 días.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/b/9.png)

### Vigencia mínima de la contraseña

Indica el tiempo en el cual una contraseña puede ser usada antes de que el usuario decida modificarla. Allí podremos establecer tiempos entre 0 y 998 días.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/b/10.png)


Otra de las políticas a nivel de seguridad primordiales en Windows Server 2016 es la del bloqueo de cuentas ya que a través de ella podremos definir si un usuario no autorizado está intentando acceder al sistema y esto lo logramos configurando dicha política para que después de tres intentos fallidos la cuenta sea bloqueada por lo cual deben recurrir al administrador para su desbloqueo.

Allí tenemos la posibilidad de configurar los siguientes parámetros:

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/b/11.png)

### Duración del bloqueo de cuenta

Esta política nos perite definir la cantidad de tiempo en la cual la cuenta involucrada permanecerá bloqueada y este tiempo se expresa en minutos en un rango entre 1 y 99.999 minutos; Si establecemos el valor cero (0) solo un administrador podrá desbloquear dicha cuenta.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/b/12.png)

### Restablecer el bloqueo de cuenta después de

Con esta política definimos la cantidad de tiempo en minutos que deben pasar antes que el contador de intento de inicio de sesión este en cero para intentar nuevamente acceder a la cuenta.

Allí podremos definir un valor entre 1 y 99.999 minutos.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/b/13.png)

### Umbral de bloqueo de cuenta

Esta es la política que nos permite llevar un control especial en términos de seguridad ya que allí definiremos la cantidad de intentos de inicio de sesión fallidos antes de que la cuenta sea bloqueada.

Es importante anotar que si dicho valor está en cero la cuenta no será bloqueada por lo cual esa opción no es recomendable. Allí podremos definir un valor entre 0 y 999. Esta política es la principal en esta sección ya que una vez bloqueada por intentos de sesión fallidos solo un administrador tendrá el derecho para deshabilitarla.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/b/14.png)
