Joel Rodriguez Martín
2º DAW

Tarea 19: Dockerizacion NodeJS

Indice
Introducción:	1
Paso 1: Crear app de NodeJS.	1
Paso 2: Crear ficheros de Docker.	3
Paso 3: Construccion de imagen.	4
Paso 4: Ejecutar la imagen.	5
Introducción:
En esta tarea dockerizaremos NodeJS para desplegar una web.
Paso 1: Crear app de NodeJS.
En primer lugar debemos instalar npm, el manejador de paquetes de Node, usando apt-get install.
Resultado:


Luego creamos un directorio en el que estarán los ficheros y creamos la app.
En primer lugar necesitaremos un package.json con el siguiente contenido:

Con este fichero creado usamos el comando npm install:

Lo que genera el package-lock y los node-modules.





Luego creamos un fichero server.js con el siguiente contenido: 

Paso 2: Crear ficheros de Docker.
A continuación creamos los ficheros necesarios de Docker. Primero el DockerFile con el contenido:





Y después un fichero .dockerignore con el contenido (que sirve para ignorar ficheros en la creacion de contenedores):

Paso 3: Construccion de imagen.
Ahora construiremos la imagen usando el comando docker build:

Comprobamos que se creo la imagen: 


Paso 4: Ejecutar la imagen.
Ejecutamos con el comando docker run:

Y comprobamos que se ejecuta en el puerto pedido (en este caso 8080):

Repositorio de github: https://github.com/joelrodriguezmartin/git
