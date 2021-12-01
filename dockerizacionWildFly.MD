Joel Rodriguez Martín
2º DAW

### Tarea 15: Dockerización de WildFly en Docker

## Indice
[Introducción:](#introduccion)   
[Paso 1: Creación del fichero dockerfile.](#paso1)   
[Paso 2: Uso de la nueva imagen.](#paso1)   

# Introducción:<a name="introduccion"></a>
En esta tarea vamos a realizar la dockerización de WildFly en Docker, para uso de aplicaciones en cluster.

# Paso 1: Creación del fichero dockerfile.<a name="paso1"></a>
Creamos la carpeta wildfly-config con un fichero Dockerfile dentro:   
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT15/captura1.png)<br/> 

Y de contenido le ponemos:   
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT15/captura2.png)<br/> 
A continuación contruimos la imagen, obteniendo de resultado un cofigo sha256:   
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT15/captura3.png)<br/> 
Verificamos que la imagen existe dentro de docker (es la seleccionada):   
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT15/captura4.png)<br/> 
# Paso 2: Uso de la nueva imagen.<a name="paso2"></a>
En primer lugar ejecutamos el siguiente comando para probar la imagen creada:   
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT15/captura5.png)<br/> 



Y a continuación hacemos un ps -a:   
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT15/captura6.png)<br/> 
Verificando que está arrancado.
A continuación accedemos y comprobamos que se pueda entrar a la consola de administración:   
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT15/captura7.png)<br/> 

Repositorio de github: https://github.com/joelrodriguezmartin/git
