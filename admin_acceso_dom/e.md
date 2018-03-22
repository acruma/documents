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
