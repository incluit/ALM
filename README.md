
# Instalación y Configuración de ALM

### Que es ALM?
> El software y las soluciones Micro Focus Application Lifecycle Management (ALM) permiten a equipos de todos los tamaños crear aplicaciones de alta calidad con un nivel superior de velocidad y agilidad. Combinando productos de software ALM, DevOps e integraciones de herramientas de desarrollo por medio de una API de REST abierta, un extenso ecosistema de socios y una estrategia independiente de la metodología, Micro Focus ALM aumenta la velocidad de los lanzamientos y, a la vez, equilibra la calidad de las aplicaciones y mejora la colaboración a lo largo del ciclo de vida.


## Instalación

### Pre Condiciones

#### Base de datos
Se debe tener un motor de base de datos instalado, con permisos de creación de nuevas Bases.
> ALM trabaja con **SQL Server 2005 (o superior)** u **Oracle**

#### Servicios de Windows
Deben estar corriendo los siguientes servicios

> Secondary Logon 
> Windows Management Instrumentation

o en castellano
> Inicio de sesión secundario.

![enter image description here](https://github.com/incluit/ALM/blob/master/images/prerequisites/pre1.PNG?raw=true)

> Instrumental de Administración de Windows
![
](https://github.com/incluit/ALM/blob/master/images/prerequisites/pre2.PNG?raw=true)
#### JDK or JRE
Se debe descargar e instalar el runtime de java.

Link [Jre8](http://www.oracle.com/technetwork/java/javase/downloads/jre8-downloads-2133155.html) 

### Pasos Para la instalación

Para instalar ALM, tenemos que ingresar a [microfocus](https://software.microfocus.com/es-es/solutions/software-development-lifecycle), generar una cuenta y descargar los paquetes que queramos instalar. 

Una vez que tenemos el archivo de instalación, debemos ejecutaralo

> ALM_installer.exe

Descompactará y comenzará a pedir información para la instalación

1. JDK/JRE Path
Se debe indicar cual es el path donde se encuentra el runtime d java, por ejemplo

> C:\Program Files\Java\jre1.8.0_181

2.  Seleccionar la carpeta
Se debe seleccionar cual es la carpeta donde se quiere alojar los archivos de ALM
Ejemplo:
> C:\Program Files\Micro Focus

3. Configuración del motor de base de datos
> solo hemos trabajando con SQL SERVER, pero en el caso de *oracle* la configuración sería equivalente

Se debe definir: 
a. tipo de conexión 
b. nombre del servidor de base datos 
c. Puerto de conexión a la base
d. Usuario administrador de la base
e. pass del usuario anterior

4. Selección del esquema de datos
se debe generar una nueva base de datos y un nuevo esquema para trabajarlo.
> ejemplo, db_ALM

5. Clave de licencia
Se puede tener una clave de licencia, o marcar la casilla de verificación para usar la licencia de evaluación, que permite trabajar durante 30 días

6. Seguridad
ALM usa la *Confidential Data Passphrase* para cifrar encriptar toda la información sensible.
Por seguridad, las claves deben ser de 12 a 255 caracteres.

> **Multinodos**: Como ALM se puede instalar en varios nodos, se debe tener especial cuidadon el las claves, dado que se deben replicar en cada nodo instalado

7. Usuario Administrador
Se debe definir un usuario administrador y su clave

> Nota: No usar el usuario de dominio, porque al no validar con este, las claves pueden quedar distintas y luego no recordarla

> Nota 2: La clave tener menos de 20 caracteres.

8. Usuario con el que correrá el servicio de ALM
 Se debe definir un usuario para que corra el servicio de ALM.
 > Nota: Este usuario puede ser el mismo de la persona que hace la instalación, si es un ambiente de desarrollo para un solo usuario. Sino, se recomienda crear una cuenta de dominio.

9. Selección de PATH para el repositorio
Se debe definir una ubicación en el servidor para almacenar la información generada. 

10. Mail Server
ALM viene con un servicio de *mail* para poder enviar notificaciones. Se puede delegar este servicio al IIS o no configurarlo.

Listo! **Usted a instalado ALM de forma exitosa!**

 ----
 

 
