Joel Rodriguez Martín
2º DAW

### Tarea 8: Despliegue de servicio REST

## Indice
[Introducción:](#introduccion)	  
[Paso 1: Descarga y creación de war](#paso1)	  
[Paso 2: Solución de errores:](#paso2)	  

# Introducción:<a name="paso1"></a>
En este ejercicio intentaremos realizar el despliegue de un servicio REST en Tomcat


# Paso 1: Descarga y creación de war<a name="introduccion"></a>   
En primer lugar descargaremos el código fuente de la aplicación  de https://github.com/jpexposito/docencia/tree/master/comun/ejemplos/java/rest-service
Con el código en local ejecutamos el comando “mvn clean install” consiguiendo el siguiente resultado:
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT8/captura1.png)<br/>
Podemos ver el .war creado y que la build se ha realizado con exito.
A continuación movemos el war a la carpeta de tomcat:   
![Captura 2](https://github.com/joelrodriguezmartin/git/blob/main/imgsT8/captura2.png)<br/>










Y podemos ver que se ha desplegado la aplicación (rest-service, la ultima de la lista):    
![Captura 3](https://github.com/joelrodriguezmartin/git/blob/main/imgsT8/captura3.png)<br/>   







# Paso 2: Solución de errores:<a name="paso2"></a>
A pesar de que el programa ha desplegado eso no significa que funcione. Al ejecutarse el servicio nos encontraremos con un error 404 y al ver los logs de Tomcat encontraremos lo siguiente:
![Captura 4](https://github.com/joelrodriguezmartin/git/blob/main/imgsT8/captura4.png)<br/>
Dado que el error es del tipo “ClassNotFoundException” deducimos que falta alguna clase necesaria para la ejecución, en este caso alguna de la librería Jersey.

El primer intento de solución fue añadir las librerías del proyecto a la carpeta tomcat con el comando. Esto NO funcionó

La segunda opción fue añadir lo siguiente al pom:  
![Captura 5](https://github.com/joelrodriguezmartin/git/blob/main/imgsT8/captura5.png)<br/>  
Esto tampoco funcionó, ya que las clases de esa carpeta ya estaban incluidas.
Posteriormente observé que en el fichero web.xml se referenciaban clases que no aparecían en el pom, asi que cambiamos las clases a las incluidas en el proyecto:
![Captura 6](https://github.com/joelrodriguezmartin/git/blob/main/imgsT8/captura6.png)<br/>

Utilizando las de el repositorio “org.glassfish” en lugar de las de “com.sun”.
Con esto consegui que la clase que faltaba pasara a ser otra, javax.Filter.
Para solucionarlo añadi al pom y al webxml la dependencia a javax:
POM:
![Captura 7](https://github.com/joelrodriguezmartin/git/blob/main/imgsT8/captura7.png)<br/>


WEB:
![Captura 8](https://github.com/joelrodriguezmartin/git/blob/main/imgsT8/captura8.png)<br/>
Y con esto conseguimos que todas las clases estuvieran presentes y el error pasara a ser otro:
![Captura 9](https://github.com/joelrodriguezmartin/git/blob/main/imgsT8/captura9.png)<br/>

Nos encontramos con un ClassCastException, debido a alguna incompatibilidad entre clases.





Repositorio de github: https://github.com/joelrodriguezmartin/git
