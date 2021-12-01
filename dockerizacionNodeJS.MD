Joel Rodriguez Martín
2º DAW

# Tarea 19: Dockerizacion NodeJS

## Indice
[Introducción:	1](#introduccion)         
[Paso 1: Crear app de NodeJS.	1](#paso1)          
[Paso 2: Crear ficheros de Docker.	3](#paso2)          
[Paso 3: Construccion de imagen.	4](#paso3)          
[Paso 4: Ejecutar la imagen.	5](#paso4)          


### Introducción:<a name="introduccion"></a>
En esta tarea dockerizaremos NodeJS para desplegar una web.

### Paso 1: Crear app de NodeJS.<a name="paso1"></a>
En primer lugar debemos instalar npm, el manejador de paquetes de Node, usando apt-get install.
Resultado:      
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT19/captura1.png)<br/>


Luego creamos un directorio en el que estarán los ficheros y creamos la app.
En primer lugar necesitaremos un package.json con el siguiente contenido:    
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT19/captura2.png)<br/>

Con este fichero creado usamos el comando npm install:    
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT19/captura3.png)<br/>
Lo que genera el package-lock y los node-modules.





Luego creamos un fichero server.js con el siguiente contenido:     
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT19/captura4.png)<br/>
### Paso 2: Crear ficheros de Docker.<a name="paso2"></a>
A continuación creamos los ficheros necesarios de Docker. Primero el DockerFile con el contenido:    
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT19/captura5.png)<br/>




Y después un fichero .dockerignore con el contenido (que sirve para ignorar ficheros en la creacion de contenedores):    
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT19/captura6.png)<br/>
### Paso 3: Construccion de imagen.<a name="paso3"></a>
Ahora construiremos la imagen usando el comando docker build:    
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT19/captura7.png)<br/>
Comprobamos que se creo la imagen:     
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT19/captura8.png)<br/>

### Paso 4: Ejecutar la imagen.<a name="paso4"></a>
Ejecutamos con el comando docker run:    
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT19/captura9.png)<br/>

Y comprobamos que se ejecuta en el puerto pedido (en este caso 8080):    
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT19/captura10.png)<br/>
Repositorio de github: https://github.com/joelrodriguezmartin/git
