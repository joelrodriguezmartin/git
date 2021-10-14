Joel Rodriguez Martín
2º DAW

# Tarea 5: Instalación de Apache-Tomcat en Linux

## Indice
[Introducción](#introduccion)    
[Paso 1 Actualización de repositorios](#paso1)		  
[Paso 2 Descarga de Tomcat y añadir usuario:](#paso2)		  
[Paso 3 Cambio de directorio:](#paso3)		  
[Paso 4 Configuración de Tomcat:](#paso4)	  
[Paso 5 Iniciar servicio:](#paso5)		  
[Paso 6 Cambiamos puerto y accedemos:](#paso6)		  

### Introducción:  <a name="introduccion"></a>
En esta práctica realizaremos la instalación de Tomcat en Linux  

### Paso 1 Actualización de repositorios:  <a name="paso1"></a>


![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT6/captura1.png)<br/>  
Actualizamos repositorios apt update/upgrade.  


### Paso 2 Descarga de Tomcat y añadir usuario:  <a name="paso2"></a>
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT6/captura2.png)<br/>  
Descargamos tomcat de la página de apache y creamos un usuario tomcat para usarlo.  
### Paso 3 Cambio de directorio:  <a name="paso3"></a>
Cambiamos tomcat a su directorio final y le cambiamos la propiedad al usuario tomcat:  
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT6/captura3.png)<br/>  
El primer comando extrae el paquete de tomcat en el directorio en el que estará.  
El segundo comando le pasa la propiedad al usuario tomcat.  
Y el ultimo comando renombra el directorio y crea un enlace simbólico sin número de versión.  

### Paso 4 Configuración de Tomcat:    <a name="paso4"></a>
Cambiamos el contenido del archivo de configuración al siguiente:  
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT6/captura4.png)<br/>  

### Paso 5 Iniciar servicio:  <a name="paso5"></a>
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT6/captura5.png)<br/>  
Comprobamos que el servicio está activo y lo preparamos para que arranque con Ubuntu.  



### Paso 6 Cambiamos puerto y accedemos:  <a name="paso6"></a>
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT6/captura6.png)<br/>  
Cambiamos el puerto al 8083 para evitar conflictos con GitLab y Apache.  
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT6/captura7.png)<br/>  
Comprobamos que funciona la página  


Repositorio de github: https://github.com/joelrodriguezmartin/git
