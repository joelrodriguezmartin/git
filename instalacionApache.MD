Joel Rodriguez Martín
2º DAW

# Tarea 5: Instalación de Apache en Linux

## Indice
[Introducción](#introduccion)    
[Paso 1 Actualización de repositorios:](#paso1)     
[Paso 2 Instalación de apache:](#paso2)   
[Paso 3 Cambio de puerto:](#paso3)   
[Paso 4 Reiniciar servicio y comprobar apps:](#paso4)    
[Paso 5 Permitir Apache a traves del cortafuegos y activarlo:](#paso5)   
[Paso 6 Comprobar que esté arrancado y acceder:](#paso6)   


### Introducción:<a name="introduccion"></a>  
En la siguiente tarea realizaremos la instalación de Apache en nuestra máquina virtual Ubuntu.  

### Paso 1 Actualización de repositorios:<a name="paso1"></a>  
Actualizamos repositorios con update y upgrade:  

![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT5/captura1.png)<br/>  






### Paso 2 Instalación de apache:<a name="paso2"></a>  
Instalamos con sudo apt install apache2 y vemos que nos da error. Esto es debido al puerto 80, ya utilizado por gitlab.  
![Captura 2](https://github.com/joelrodriguezmartin/git/blob/main/imgsT5/captura2.png)<br/>    

### Paso 3 Cambio de puerto:<a name="paso3"></a>  
Cambiamos el puerto a 8081 en ambos ficheros de configuracion  

![Captura 3](https://github.com/joelrodriguezmartin/git/blob/main/imgsT5/captura3.png)<br/>  
![Captura 4](https://github.com/joelrodriguezmartin/git/blob/main/imgsT5/captura4.png)<br/>  




### Paso 4 Reiniciar servicio y comprobar apps:<a name="paso4"></a>  

Reiniciamos el servicio apache y vemos las disponibles. Utilizaremos “Apache”  
![Captura 5](https://github.com/joelrodriguezmartin/git/blob/main/imgsT5/captura5.png)<br/>  






### Paso 5 Permitir Apache a traves del cortafuegos y activarlo: <a name="paso5"></a>  
![Captura 6](https://github.com/joelrodriguezmartin/git/blob/main/imgsT5/captura6.png)<br/>  
Permitimos a apache pasar por el cortafuegos, comprobamos si esta activo con “ufw status” y como no lo esta lo arrancamos y comprobamos otra vez

### Paso 6 Comprobar que esté arrancado y acceder:<a name="paso6"></a>  
Comprobamos  
![Captura 7](https://github.com/joelrodriguezmartin/git/blob/main/imgsT5/captura7.png)<br/>  
Y accedemos.  
![Captura 8](https://github.com/joelrodriguezmartin/git/blob/main/imgsT5/captura8.png)<br/>  

Repositorio de github: https://github.com/joelrodriguezmartin/git
