Joel Rodriguez Martín
2º DAW

### Tarea 16: Clusterizacion de WildFly en Docker

## Indice
[Introducción:](#introduccion)   
[Paso 1: Despliegue de cluster de JBOSS con Docker.](#paso1)   

# Introducción:<a name="introduccion"></a>
En esta tarea realizaremos la clusterización de una app desplegada en WildFly usando Docker

# Paso 1: Despliegue de cluster de JBOSS con Docker.<a name="paso1"></a>
En primer lugar  modificamos la app de ejemplo. Para empezar modificamos el web.xml:   
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT16/captura1.png)<br/>  
Colocando nuestro nombre en el display name.
En segundo lugar modificamos el index jsp de la misma manera:   
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT16/captura2.png)<br/>  

E instalamos la app con mvn clean install:   
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT16/captura3.png)<br/>  

Vemos el resultado en local usando mvn clean jetty:run:   
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT16/captura4.png)<br/>  
Finalmente creamos los dos nodos con docker-compose up: 8081   
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT16/captura5.png)<br/>  



8080:   
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT16/captura6.png)<br/>  
Repositorio de github: https://github.com/joelrodriguezmartin/git
