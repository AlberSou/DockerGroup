# Ejercicio 1 - trabajo con imágenes / Enol
## Servidor web
1. Arranca un contenedor que ejecute una instancia de la imagen php:7.4-apache , que se
llame web y que sea accesible desde un navegador en el puerto 8000.
> ![1](Caps/Ejercicio%201/1.1.PNG)
> ```
> docker run -d --name web2 -p 8000:8000 php:7.4-apache
> ```


2. Colocar en el directorio raíz del servicio web ( /var/www/html ) un sitio web donde figure el nombre de los componentes del grupo <br>

3. Colocar en ese mismo directorio raíz un archivo llamado mes.php que muestre el nombre
del mes actual. Ver la salida del script en el navegador <br>
> ![1](Caps/Ejercicio%201/2.1.PNG)
> ![1](Caps/Ejercicio%201/2.2.1.PNG)


4. Borrar el contenedor
> ```
> docker rm web2
> ```
<br>

## Servidor de base de datos

<br>
Arrancar un contenedor que se llame bbdd y que ejecute una instancia de la imagen
mariadb para que sea accesible desde el puerto 3306.
Antes de arrancarlo visitar la página del contenedor en Docker Hub y establecer las variables
de entorno necesarias para que:
La contraseña de root sea root .
Crear una base de datos automáticamente al arrancar que se llame prueba .
Crear el usuario invitado con la contraseña invitado .
Entregar un documento con los siguientes pantallazos, y los comandos empleados para resolver
cada apartado: <br>

* Pantallazo que desde el navegador muestre el fichero index.html . <br>
* Pantallazo que desde un navegador muestre la salida del script mes.php .<br>
> ![1](Caps/Ejercicio%201/2.3.PNG)
* Pantallazo donde se vea el tamaño del contenedor web después de crear los dos ficheros.<br>
> ![1](Caps/Ejercicio%201/3.4.PNG)
> ```
> docker ps -a -s
> ```
* Pantallazo donde desde un cliente de base de datos (instalado en tu ordenador) se pueda
observar que hemos podido conectarnos al servidor de base de datos con el usuario creado
y que se ha creado la base de datos prueba ( show databases ). El acceso se debe realizar
desde el ordenador que tenéis instalado docker, no hay que acceder desde dentro del
contenedor, es decir, no usar docker exec . <br> 
> ![1](Caps/Ejercicio%201/3.2.PNG)
> ![1](Caps/Ejercicio%201/3.5.PNG)

* Pantallazo donde se comprueba que no se puede borrar la imagen mariadb mientras el contenedor bbdd está creado.
> ![1](Caps/Ejercicio%201/3.3.PNG)
> ```
> docker rmi mariadb
> ```



