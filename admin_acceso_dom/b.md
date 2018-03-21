# Se han previsto bloqueos de accesos no autorizados al dominio.

Para iniciar el proceso de configuración de las políticas de contraseña en Windows Server 2016 debemos acceder al editor de políticas de grupo y para ello contamos con las siguientes opciones. Accedemos al `Panel de control`, en la esquina superior derecha escogemos iconos pequeños. Luego `Herramientas administrativas`.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/b-acceso-dominio/1.png)

Y allí seleccionar la opción `Directiva de seguridad local`.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/b-acceso-dominio/2.png)

Una vez allí podrian darse las siguientes rutas; 

>1. Configuración del equipo

>2. Configuración de Windows

>3. Configuración de seguridad

>4. Directivas de cuenta

>5. Directiva de contraseñas.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/b-acceso-dominio/3.png)

Podemos ver que dicha política `Directiva de contraseñas` se compone de múltiples elementos como son:

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/b-acceso-dominio/4.png)
 
### Almacenar contraseñas con cifrado reversible

Esta política habilita la compatibilidad de protocolos que requieren la contraseña del usuario para el inicio de sesión.
 
Con esta política se pueden descifrar contraseñas que han sido previamente cifradas por lo cual no es recomendable su habilitación ya que algún atacante puede aprovechar su vulnerabilidad para descifrar la contraseña y acceder al equipo y con ello a los recursos compartidos.

Para realizar cualquier cambio sobre dicha política daremos doble clic sobre ella y podremos habilitarla o deshabilitarla según sea la necesidad.

![img](https://github.com/smxrlxp/dominios.html/blob/master/assets/admin_acceso_dom/b-acceso-dominio/5.png)
