Joel Rodriguez Martín
2º DAW

### Tarea 17: Crear entorno LAMP y despliegue en Docker

## Indice
[Introducción:](#introduccion)   
[Paso 1: Creación del entorno de ficheros](#paso1)   
[Paso 2: Despliegue de la app](#paso2)   

# Introducción:
En esta tarea realizaremos la creación de un pseudo-entorno LAMP en Docker y desplegaremos una aplicación en PHP 

# Paso 1: Creación del entorno de ficheros
En primer lugar creamos la siguiente estructura de ficheros:   
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT17/captura1.png)<br/>  




Con esta estructura creada los contenidos de los ficheros serán los siguientes:

dbname.sql:   
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT17/captura2.png)<br/>  






index.php:   
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT17/captura3.png)<br/>  







En docker-compose.yml realizaremos un cambio al registro MYSQL_USER:   
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT17/captura4.png)<br/>  
Sustituyendo “root” colocaremos otro nombre, ya que se produce error.

Y finalmente Dockerfile:   
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT17/captura5.png)<br/>  









# Paso 2: Despliegue de la app.
Con estos ficheros ejecutaremos el comando “sudo docker-compose up -d”, lo que creara las imagenes y contenedores y los lanzara:   
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT17/captura6.png)<br/>  



Y comprobamos que la aplicación está lanzada:   
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT17/captura7.png)<br/>  
Probamos con otra app:   
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT17/captura8.png)<br/>  

Repositorio de github: https://github.com/joelrodriguezmartin/git
