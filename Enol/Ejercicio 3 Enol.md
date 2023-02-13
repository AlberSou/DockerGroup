# Ejercicio 3 - Redes / Enol
1. Crea una red bridge redbd <br>
![9](Caps/Ejercicio%203/1.1.PNG)
2. Crea un contenedor con una imagen de mariaDB que estará en la red redbd . Este
contenedor se ejecutará en segundo plano, y será accesible a través del puerto 3306. (Es
necesario definir la contraseña del usuario root y un volumen de datos persistente)
![9](Caps/Ejercicio%203/2.2.PNG)
3. Crear un contenedor con Adminer que se pueda conectar al contenedor de la BD
![9](Caps/Ejercicio%203/2.4.PNG)
4. Comprobar que el contenedor Adminer puede conectar con el contenedor mysql abriendo
un navegador web y accediendo a la URL: http://localhost:8080
![9](Caps/Ejercicio%203/2.7.PNG)
Entregar los siguientes pantallazos y los comandos empleados para resolver cada apartado:
Pantallazos donde se vean los contenedores creados y en ejecución
* Pantallazo donde se vea el acceso a la BD a través de la interfaz web de Adminer 

* Pantallazo donde se vea la creación de una BD con la interfaz web Adminer

* Pantallazo donde se entre a la consola del servidor web en modo texto y se compruebe que se ha creado la BD

* Borrar los contenedores la red y los volúmenes utilizados
