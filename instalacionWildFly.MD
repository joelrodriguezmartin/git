Joel Rodriguez Martín
2º DAW

### Tarea 9: Instalación de WildFly

## Indice    
[Introducción](#introduccion)      
[Paso 1: Instalación de WildFly](#paso1) 	    
[Paso 2: Arrancar WildFly:](#paso2) 	   
[Paso 3: Configurar WildFly:](#paso3)            	
[Paso 4: Acceso a WildFly:](#paso4) 	    

# Introducción:<a name="introduccion"></a>  
En este ejercicio realizaremos la instalación de WildFly


# Paso 1: Instalación de WildFly <a name="paso1"></a>  
En primer lugar actualizaremos los repositorios con “sudo apt update” y “sudo apt upgrade”.
Tras esto descargaremos WildFly con el comando wget: 
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT9/captura1.png)<br/>  

Tras esto añadimos el grupo y usuario de wildlfy, para que corra como un servicio:
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT9/captura2.png)<br/>  

Y extraemos el paquete con el comando “tar xvzf”, movemos a su ubicación y creamos enlace.
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT9/captura3.png)<br/>  
Luego le damos acceso al usuario y grupo:
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT9/captura4.png)<br/>  

# Paso 2: Arrancar WildFly:<a name="paso2"></a>  
En primer lugar:    
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT9/captura5.png)<br/>  
Podemos ver el fichero de configuración de arranque:
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT9/captura6.png)<br/>  

Y continuamos configurando el arranque:
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT9/captura7.png)<br/> 
Iniciamos el servicio, comprobamos que este arrancado y lo habilitamos para inicio automatico:
 ![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT9/captura8.png)<br/> 






# Paso 3: Configurar WildFly:<a name="paso3"></a>  
En primer lugar debemos cambiar el puerto de WildFly ya que el 8080 que aparece por defecto ya está ocupado. Utilizaremos el 8084.
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT9/captura9.png)<br/>  
Y permitiremos el tráfico en ese puerto:
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT9/captura10.png)<br/> 






# Paso 4: Acceso a WildFly:<a name="paso4"></a>  
Para empezar añadimos un usuario con el script dado por WildFly:
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT9/captura11.png)<br/> 
Luego gestionamos la consola remota en wildly.conf:
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT9/captura12.png)<br/> 



Y el fichero launch.sh: (ESTE PASO TUVE QUE DESHACERLO PORQUE PETA)
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT9/captura13.png)<br/> 
Finalmente hacemos las ultimas modificaciones:
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT9/captura14.png)<br/> 







Le añadimos esto en el nano:
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT9/captura15.png)<br/> 
Funciona:

![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT9/captura16.png)<br/> 
















Repositorio de github: https://github.com/joelrodriguezmartin/git
