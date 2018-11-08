## ALM Synchronizer 
ALM Sync está compuesto por dos elementos, un server y un cliente.

El server, debe ser instalado en el mismo cliente que el ALM Server, sino no habrá conectividad entre los ellos.

### ALM Synchornizer Server
Para instalar ALM, tenemos que ingresar a  [microfocus](https://software.microfocus.com/es-es/solutions/software-development-lifecycle), generar una cuenta y descargar los paquetes que queramos instalar.

Una vez que tenemos el archivo de instalación, debemos ejecutaralo

> setup.exe

Debemos seguir con los pasos de una instalación común....

![
](https://github.com/incluit/ALM/blob/master/images/Synchronizer/0.PNG?raw=true)

debemos aceptar la licencia..
![
](https://github.com/incluit/ALM/blob/master/images/Synchronizer/1.PNG?raw=true)

Seleccionar donde se deberá instalar el server del sync
![
](https://github.com/incluit/ALM/blob/master/images/Synchronizer/2.PNG?raw=true)

Nos informa el resumen y se instala.
![
](https://github.com/incluit/ALM/blob/master/images/Synchronizer/3.PNG?raw=true)

Nos informa el resumen..
![
](https://github.com/incluit/ALM/blob/master/images/Synchronizer/4.PNG?raw=true)
> Importante, el server no se puede re instalar, se debe borrar e instalar nuevamente

#### Configuración 
Una vez que se terminó la instalación y sin decirnos nada, se lanza el programa de configuración.

![
](https://github.com/incluit/ALM/blob/master/images/Synchronizer/5.PNG?raw=true)

Lo primero que debemos indicar es la versión de ALM. Para este ejemplo, estamos trabajando con **ALM 12.60**
![
](https://github.com/incluit/ALM/blob/master/images/Synchronizer/6.PNG?raw=true)

Luego, nos pide un usuario para que corra el server de sincronización. Este usuario, no tiene porqué ser el mismo que el usado en la instalación de ALM. 
Además, si queremos que corra con *local system*, debemos dejar vacíos los campos.

![
](https://github.com/incluit/ALM/blob/master/images/Synchronizer/7.PNG?raw=true)

Paso siguiente, nos indicará que instalará una base de datos. 
En este caso, no utilizará una DB de nuestra arquitectura, sino que instalará un **postgreSQL** local

![
](https://github.com/incluit/ALM/blob/master/images/Synchronizer/8.PNG?raw=true)

por último, nos informará que está corriendo correctamente.
![
](https://github.com/incluit/ALM/blob/master/images/Synchronizer/9.PNG?raw=true)

---

### ALM Synchronizer Client
Luego de instalar el Server, debemos continuar con el Cliente
El server será quien haga la conexión entre ALM y lo que reciba desde y hacia sus clientes.
El Servicio de Cliente, será quien registre las conexiones entre los distintos **endpoints** 
Ejemplo: 
> ALM <--> JIRA
> ALM <--> TFS

Debemos descargar el archivo de instalación de micro focus también, y ejecutarlo

> ALM_Synchronizer_Client_12.60.msi

![
](https://github.com/incluit/ALM/blob/master/images/Synchronizer/c0.PNG?raw=true)

Nos pedirá aceptar la licencia...

![
](https://github.com/incluit/ALM/blob/master/images/Synchronizer/c1.PNG?raw=true)

El lugar de instalación... 

![
](https://github.com/incluit/ALM/blob/master/images/Synchronizer/c2.PNG?raw=true)

y por ultimo la confirmación.

![
](https://github.com/incluit/ALM/blob/master/images/Synchronizer/c3.PNG?raw=true)

Una vez que tenemos esto, podemos ejecutar el programa **ALM Sync Client**

Donde nos van a pedir, 
> Nombre del server: si está trabajando en el mismo server, debe poner el nombre del server, *no localhost*
> Puerto: el puerto por defecto del Sync Server es 7064
> Si es la primera vez que abre el cliente, debe loguearse con el usuario *admin* sin password
> 

![
](https://github.com/incluit/ALM/blob/master/images/Synchronizer/c4.PNG?raw=true)

Una vez que estamos conectados, podemos generar nuevos links
![
](https://github.com/incluit/ALM/blob/master/images/Synchronizer/c5.png?raw=true)

