# Se han implementado y verificado directivas de grupo.

Pulsando `Windows + R` abrimos la opción de ejecutar. Escribimos `gpmc.msc` y pulsamos enter. Esto nos llevará a `Administración de directivas de grupo`. Abrimos el "bosque" elegido, y vamos a "Dominios" y alli seleccionamos le dominio en cuestión.

![img](https://raw.githubusercontent.com/smxrlxp/dominios.html/master/assets/admin_acceso_dom/e/1.png)

Si hacemos click derecho sobre el dominio podremos crear una nueva directiva de grupo. `Crear un GPO en este dominio y vincularlo aquí...`

![img](https://raw.githubusercontent.com/smxrlxp/dominios.html/master/assets/admin_acceso_dom/e/3.png)

Le añadimos un nombre y aceptamos. Nos saltará un aviso, que aceptaremos tambien.

![img](https://raw.githubusercontent.com/smxrlxp/dominios.html/master/assets/admin_acceso_dom/e/4.png)
![img](https://raw.githubusercontent.com/smxrlxp/dominios.html/master/assets/admin_acceso_dom/e/5.png)

Haciendo click derecho sobre la directiva que queramos podremos editarla pulsando en `Editar`.

![img](https://raw.githubusercontent.com/smxrlxp/dominios.html/master/assets/admin_acceso_dom/e/6.png)

Dentro de la GPO encontraremos directivas para `Usuarios` y `Equipos`.

En cada una de estas directivas encontraremos tres carpetas principales

>Configuración de software
>Configuración de Windows
>Plantillas Administrativas

![img](https://raw.githubusercontent.com/smxrlxp/dominios.html/master/assets/admin_acceso_dom/e/7.png)

### Configuración de usuario - Directivas

##### Configuración de software .....

![img](https://raw.githubusercontent.com/smxrlxp/dominios.html/master/assets/admin_acceso_dom/e/11_a.png)

##### Configuración de Windows .....

![img](https://raw.githubusercontent.com/smxrlxp/dominios.html/master/assets/admin_acceso_dom/e/11_b.png)

En este mismo apartado se encuentra la `Configuración de seguridad` .....

![img](https://raw.githubusercontent.com/smxrlxp/dominios.html/master/assets/admin_acceso_dom/e/11_d.png)

##### Plantillas administrativas .....

![img](https://raw.githubusercontent.com/smxrlxp/dominios.html/master/assets/admin_acceso_dom/e/11_c.png)

### Configuración del equipo - Directivas

##### Configuración de software .....

![img](https://raw.githubusercontent.com/smxrlxp/dominios.html/master/assets/admin_acceso_dom/e/10_a.png)

##### Configuración de Windows .....

![img](https://raw.githubusercontent.com/smxrlxp/dominios.html/master/assets/admin_acceso_dom/e/10_b.png)

En este mismo apartado se encuentra la `Configuración de seguridad` .....

![img](https://raw.githubusercontent.com/smxrlxp/dominios.html/master/assets/admin_acceso_dom/e/10_d.png)

##### Plantillas administrativas .....

![img](https://raw.githubusercontent.com/smxrlxp/dominios.html/master/assets/admin_acceso_dom/e/10_c.png)
