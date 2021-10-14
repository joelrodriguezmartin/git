Joel Rodriguez Martín  
2º DAW  
# Tarea 7: Despliegue de una aplicación en Tomcat  
## Indice  
[Introducción:](#introduccion)  
[Paso 1: Descarga y modificación de código:](#paso1)  
[Paso 2: Build y despliegue de la aplicación:](#paso2)  

### Introducción:<a name="introduccion"></a>
En este ejercicio realizaremos el despliegue de una aplicación sencilla en Apache Tomcat.

### Paso 1: Descarga y modificación de código:<a name="paso1"></a>  
En primer lugar descargaremos el código fuente de la aplicación de
https://github.com/jpexposito/docencia/tree/master/comun/ejemplos/java/app-web-demo  
Con el código en local le hacemos las siguientes modificaciones:<br/>  
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT7/captura1.png)<br/>
Le cambiamos el contenido al index.jsp para incluir nuestro nombre<br/>  
![Captura 2](https://github.com/joelrodriguezmartin/git/blob/main/imgsT7/captura2.png)<br/>
Le cambiamos el display-name en el archivo web.xml.<br/>  
![Captura 3](https://github.com/joelrodriguezmartin/git/blob/main/imgsT7/captura3.png)<br/>
Y le cambiamos el nombre en el pom.xml.  

### Paso 2: Build y despliegue de la aplicación:<a name="paso2"></a>    
Con el código modificado ejecutamos el comando mvn clean install para generar el archivo .war    
![Captura 4](https://github.com/joelrodriguezmartin/git/blob/main/imgsT7/captura4.png)<br/>
Ejecutamos comando.<br/>
![Captura 5](https://github.com/joelrodriguezmartin/git/blob/main/imgsT7/captura5.png)<br/>  
Y vemos el resultado.<br/>  
![Captura 6](https://github.com/joelrodriguezmartin/git/blob/main/imgsT7/captura6.png)<br/>
A continuación movemos el fichero .war a la carpeta webapps de tomcat.<br/>  
![Captura 7](https://github.com/joelrodriguezmartin/git/blob/main/imgsT7/captura7.png)<br/>
Y en el navegador accedemos a la ruta de la app (que sera el puerto de tomcat + el nombre de la  
app)<br/>  
Repositorio de github: https://github.com/joelrodriguezmartin/git
