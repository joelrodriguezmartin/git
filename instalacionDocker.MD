Joel Rodriguez Martín
2º DAW

### Tarea 13: Instalación de Docker

## Indice
[Introducción:](@introduccion)   
[Paso 1: Instalar Docker:](@paso1)
[Paso 2: Trabajar con imagenes de Docker:](@paso2)
[Paso 3: Administrar contenedores de Docker:](@paso3)

# Introducción:<a name="introduccion"></a>  
En esta tarea realizaremos la instalación de Docker en Linux.
# Paso 1: Instalar Docker:<a name="paso1"></a>  
En primer lugar actualizamos paquetes con apt update y upgrade.
A continuación instalamos algunos paquetes previos, para permitir que apt use paquetes a traves de https:
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT13/captura1.png)<br/>  
Y luego añadimos la clave de GPG para el repositorio de Docker:
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT13/captura2.png)<br/>  
Añadimos el repositorio de docker a las fuentes de apt:
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT13/captura3.png)<br/>  












Y volvemos a hacer update, comprobando luego que la instalación se va a hacer desde el repositorio recien agregado:
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT13/captura4.png)<br/>  
E instalamos docker:
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT13/captura5.png)<br/>  

Y comprobamos que funciona:
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT13/captura6.png)<br/>  
# Paso 2: Trabajar con imagenes de Docker:<a name="paso2"></a>  
Para empezar comprobamos si podemos acceder y descargar de DockerHub usando hello-world:
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT13/captura7.png)<br/>  
# Paso 3: Administrar contenedores de Docker:<a name="paso3"></a>  
Comprobamos los contenedores activos con docker ps(activos), ps -a(todos) y ps-l(ultimo creado), a demás de images(muestra la nueva y la anterior de la que se derivó):
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT13/captura8.png)<br/>  

Repositorio de github: https://github.com/joelrodriguezmartin/git
