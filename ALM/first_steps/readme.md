## ALM
Una vez que tenemos ALM instalado, tenemos diferentes herramientas para trabajar.

Para esto, tenemos que acceder al servidor y seleccionar 

> Para acceder al server, debemos ir a http://< nombre del servidor >: puerto /qcbin
> Por ejemplo:
	> http://localhost:8081/qcbin


![
](https://github.com/incluit/ALM/blob/master/images/fiststeps/1.PNG?raw=true)

### Site Administrator
Dentro del sitio administrador, crearemos los proyectos, usuarios, etc

#### Creando proyectos
Los proyectos son un conjunto de Requerimientos, casos de prueba, etc etc Todo aquello necesario para trabajar con CI/CD.

![
](https://github.com/incluit/ALM/blob/master/images/fiststeps/2.PNG?raw=true)

Una vez que accedimos al sitio de Administrador, seleccionamos el botón de crear nuevo proyecto

![
](https://github.com/incluit/ALM/blob/master/images/fiststeps/3.PNG?raw=true)

Definimos un nombre y un dominio. 

![
](https://github.com/incluit/ALM/blob/master/images/fiststeps/4.PNG?raw=true)

Definimos la conexión y el servidor donde querramos crear la suite de testing

![
](https://github.com/incluit/ALM/blob/master/images/fiststeps/5.PNG?raw=true)

Paso siguiente, debemos asociar usuarios al proyecto. 
Esto permite que después puedan crear requerimientos, casos de prueba, etc

![
](https://github.com/incluit/ALM/blob/master/images/fiststeps/6.PNG?raw=true)

Luego, debemos seleccionar las extensiones que tendrá habilitado el proyecto.

![
](https://github.com/incluit/ALM/blob/master/images/fiststeps/7.PNG?raw=true)

Por último, nos ofrece un resumen de lo seleccionado anteriormente, y debemos proceder a crear el proyecto
> **Importante**: No debemos olvidar activar el proyecto!

![
](https://github.com/incluit/ALM/blob/master/images/fiststeps/8.PNG?raw=true)

----
## Generando Casos de testing
Una vez generado el proyecto, debemos ingresar con la herramienta de cliente, para poder crear casos de prueba.

Para esto, tenemos que acceder al server,  y seleccionar aLM Desktp Client.

	> http://localhost:8081/qcbin


![
](https://github.com/incluit/ALM/blob/master/images/fiststeps/1.PNG?raw=true)

No nos preocupemos si se demora en abrir....

![
](https://github.com/incluit/ALM/blob/master/images/fiststeps/9.PNG?raw=true)

Una vez que accedemos, vemos a la izquierda el árbol de opciones, al centro los elementos según la opción del árbol y a la derecha las opciones del elemento seleccionado en el centro.

![
](https://github.com/incluit/ALM/blob/master/images/fiststeps/10.png?raw=true)

Para crear un nuevo test, debemos ir a **Testing --> test plan --> (botón derecho) new test**

Esto desplegará una nueva ventana para colocar los datos del test case

![
](https://github.com/incluit/ALM/blob/master/images/fiststeps/11.PNG?raw=true)

Una vez creado el caso, tenemos que diseñar los pasos o "Steps"

![
](https://github.com/incluit/ALM/blob/master/images/fiststeps/12.PNG?raw=true)


![
](https://github.com/incluit/ALM/blob/master/images/fiststeps/13.PNG?raw=true)

por último, tenemos que asociar el test a uno más requerimientos 

![
](https://github.com/incluit/ALM/blob/master/images/fiststeps/14.PNG?raw=true)

![
](https://github.com/incluit/ALM/blob/master/images/fiststeps/15.PNG?raw=true)

#### Creando requerimientos
Además de administrar los test, podemos crear requerimientos.
Para esto, tenemos que recorrer el árbol e ir a requirements y agregar uno nuevo
![
](https://github.com/incluit/ALM/blob/master/images/fiststeps/rq0.PNG?raw=true)

![
](https://github.com/incluit/ALM/blob/master/images/fiststeps/rq1.PNG?raw=true)

Luego, estos requerimientos pueden mapearse con los casos de prueba
