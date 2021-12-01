Joel Rodriguez Martín
2º DAW

# Tarea 20: Balanceo de Carga en Apache

## Indice
[Introducción:	1](#introduccion)
[Paso 1: Instalacion de módulos de Apache:	1](#paso1)
[Paso 2 Modificar configuracion de Apache:	2](#paso2)
[Paso 3 Crear contenedores Docker:	2](#paso3)

### Introducción:<a name="introduccion"></a>
En esta tarea desplegaremos 4 nodos y haremos un balanceo de carga

### Paso 1: Instalacion de módulos de Apache:<a name="paso1"></a>
Instalamos los modulos necesarios con a2enmod:    
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT20/captura1.png)<br/>



### Paso 2 Modificar configuracion de Apache:<a name="paso2"></a>
Añadimos la configuración de proxy a el fichero .conf del servidor Apache:    
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT20/captura2.png)<br/>

### Paso 3 Crear contenedores Docker:<a name="paso3"></a>
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT20/captura3.png)<br/>
Configuracion de Docker para crear 4 wildflies
Y los lanzamos, comprobando desde el servidor apache que al refrescar nos mostrara un puerto diferente (balancea la carga entre los puertos):    
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT20/captura1.png)<br/>
8081    
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT20/captura1.png)<br/>
8084

Repositorio de github: https://github.com/joelrodriguezmartin/gitg
