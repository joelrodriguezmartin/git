Joel Rodriguez Martín
2º DAW

# Tarea 18: Cluster Rest Wildfly

## Indice    
[Introducción:	1](#introduccion)    
[Paso 1: Creación del entorno de ficheros	1](#paso1)    
[Paso 2: Construccion y despliegue:	3](#paso2)   

### Introducción:<a name="introduccion"></a>
En esta tarea realizaremos el despliegue de un servicio Rest en un cluster de 3 WildFly junto con un servidor phpMyAdmin y una base de datos.


### Paso 1: Creación del entorno de ficheros<a name="paso1"></a>
En primer lugar clonamos la aplicación helloworld-rs de git.   
Entramos a la carpeta y realizamos la siguiente estructura de ficheros:    
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT18/captura1.png)<br/>








Añadiendo dump a la base con un fichero sql y los ficheros docker-compose y Dockerfile.   
El contenido de estos ficheros sera el siguiente:   
docker-compose.yml:   
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT18/captura2.png)<br/>
Le añadimos un tercer container wildfly, ademas de la base de datos y el phpmyadmin   
Dockerfile:   
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT18/captura3.png)<br/>
Colocamos las opciones del widlfly






### Paso 2: Construccion y despliegue:<a name="paso2"></a>
Realizamos la construccion del war con mvn clean install con resultado:   
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT18/captura4.png)<br/>







Y luego usamos docker-compose up para desplegar los contenedores con la app. Resultado:   
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT18/captura5.png)<br/>








Y vemos la aplicación desplegada en los tres contenedores:   
8086:   
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT18/captura6.png)<br/>
8087:   
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT18/captura7.png)<br/>
8088:   
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT18/captura8.png)<br/>






Además el phpmyadmin estará arrancado con la base de datos:   
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT18/captura10.png)<br/>

Repositorio de github: https://github.com/joelrodriguezmartin/git
