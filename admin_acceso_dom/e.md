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

##### Configuración de software 

En este apartado podremos imponer directivas sobre la instalación de software por parte del usuario.

![img](https://raw.githubusercontent.com/smxrlxp/dominios.html/master/assets/admin_acceso_dom/e/11_a.png)

##### Configuración de Windows

Aqui, podremos administrar directivas sobre;

>`Scripts` de inicios y cierres de sesión
>Configuración de seguridad 
>Redirección de carpetas
>Calidad de servicios basadas en directivas
>Impresoras implementadas

![img](https://raw.githubusercontent.com/smxrlxp/dominios.html/master/assets/admin_acceso_dom/e/11_b.png)

En este mismo apartado se encuentra la `Configuración de seguridad`

Donde podremos crear configuraciones adicionales sobre la seguridad tanto en claves públicas como en restricciones de software

![img](https://raw.githubusercontent.com/smxrlxp/dominios.html/master/assets/admin_acceso_dom/e/11_d.png)

##### Plantillas administrativas

Aqui, podremos crear plantillas para la administración en los siguientes apartados;

>Active Desktop
>Carpetas compartidas
>Componentes de Windows
>Menú de Inicio y barra de Tareas
>Panel de control
>Red
>Sistema

![img](https://raw.githubusercontent.com/smxrlxp/dominios.html/master/assets/admin_acceso_dom/e/11_c.png)

### Configuración del equipo - Directivas

##### Configuración de software

En este apartado podremos imponer directivas sobre la instalación de software por parte del equipo.

![img](https://raw.githubusercontent.com/smxrlxp/dominios.html/master/assets/admin_acceso_dom/e/10_a.png)

##### Configuración de Windows

Aqui, podremos administrar directivas sobre;

>`Scripts` de inicios y cierres de sesión
>Configuración de seguridad 
>Directivas de resoluciones de nombres
>Calidad de servicios basadas en directivas
>Impresoras implementadas

![img](https://raw.githubusercontent.com/smxrlxp/dominios.html/master/assets/admin_acceso_dom/e/10_b.png)

En este mismo apartado se encuentra la `Configuración de seguridad`

Aqui, podremos adminsitrar configuraciones extras de seguridad como pueden ser...

>Directivas de cuentas
>Directivas locales
>Registro de eventos
>Grupos Restringidos
>Servicios del sistema
>Registro
>Sistema de archivos
>Directivas de red cableada
>Firewall de Windows con seguridad avanzadas
>Directivas de Administración
>Directivas de red inalambrica
>Directivas de clave publica 
>Restricciones de software
>Control de aplicaciones
>Seguridad de IP en Active Directory
>Configuración de directiva de auditoria avanzada

![img](https://raw.githubusercontent.com/smxrlxp/dominios.html/master/assets/admin_acceso_dom/e/10_d.png)

##### Plantillas administrativas

Aqui, podremos crear plantillas para la administración en los siguientes apartados;

>Servidor
>Impresoras
>Componentes de Windows
>Menú de Inicio y barra de Tareas
>Panel de control
>Red
>Sistema

![img](https://raw.githubusercontent.com/smxrlxp/dominios.html/master/assets/admin_acceso_dom/e/10_c.png)
