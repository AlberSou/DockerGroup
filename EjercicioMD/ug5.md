## Docker- Dockerfile

#### Creamos una servidor que sirva un sitio con gninx.
- Lo pirmero será entrar en el root para evitarnos los sudo por cada comando.
![](../Capturas/g51.png)
- Creamos la carpeta build
![](../Capturas/g52.png)
- Ahora le daré permisos para todos y la cambiaré al usuario que usaremos en dockerfile
![](../Capturas/g53.png)
![](../Capturas/g54.png)
- Me meto en la carpeta y mediante un fichero de texto le indicaré la plantilla
![](../Capturas/g55.png)
- Tengo aqui mi html

![](../Capturas/g58.png)
- Usare la imagen httpd:2,4, copiare mi html a hdocs y lo colocaré en el puerto 80
- Creamos la imagen.
![](../Capturas/g57.png)
- Y ahora la subiremos, iniciaremos sesion
![](../Capturas/g59.png)
- y ahora la subimos
![](../Capturas/g510.png)
- Como vemos se subió sin problema
![](../Capturas/g511.png)
- Me la descargaré yo de nuevo
![](../Capturas/g512.png)
- Creo un contenedor con dicha imagen
![](../Capturas/g513.png)
- Y aqui está!
![](../Capturas/g514.png)

