Joel Rodriguez Martín
2º DAW

Tarea 18: Cluster Rest Wildfly

Indice
Introducción:	1
Paso 1: Creación del entorno de ficheros	1
Paso 2: Construccion y despliegue:	3
Introducción:
En esta tarea realizaremos el despliegue de un servicio Rest en un cluster de 3 WildFly junto con un servidor phpMyAdmin y una base de datos.
Paso 1: Creación del entorno de ficheros
En primer lugar clonamos la aplicación helloworld-rs de git.
Entramos a la carpeta y realizamos la siguiente estructura de ficheros:









Añadiendo dump a la base con un fichero sql y los ficheros docker-compose y Dockerfile.
El contenido de estos ficheros sera el siguiente:
docker-compose.yml:
Le añadimos un tercer container wildfly, ademas de la base de datos y el phpmyadmin
Dockerfile:
Colocamos las opciones del widlfly






Paso 2: Construccion y despliegue:
Realizamos la construccion del war con mvn clean install con resultado:







Y luego usamos docker-compose up para desplegar los contenedores con la app. Resultado:








Y vemos la aplicación desplegada en los tres contenedores:
8086:

8087:

8088:







Además el phpmyadmin estará arrancado con la base de datos:

Repositorio de github: https://github.com/joelrodriguezmartin/git
