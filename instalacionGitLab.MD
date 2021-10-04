Joel Rodriguez Martín
2º DAW

# Tarea 4: Instalación de GitLab en Linux  

## Indice  
1. [Introducción:](#introduccion)  
2. [Paso 1 Actualización de repositorios:](#paso1)  	
3. [Paso 2 Instalación de paquetes adicionales:](#paso2)  	
4. [Paso 3 Instalación de GitLab:](#paso2)	  
5. [Paso 4 Acceso:](#paso2)	  


### Introducción:<a name="introduccion"></a>  
En la siguiente tarea realizaremos la instalación de GitLab en nuestra máquina virtual Ubuntu.  

### Paso 1 Actualización de repositorios:<a name="paso1"></a>  
En primer lugar actualizamos los repositorios con apt update/upgrade:  


### Paso 2 Instalación de paquetes adicionales:<a name="paso2"></a>  
Luego instalaremos algunos paquetes necesarios para GitLab:  


### Paso 3 Instalación de GitLab:<a name="paso3"></a>  
A continuación instalamos GitLab con el shell script proporcionado por el equipo de GitLab:  
Primero:  




Después:   


Y por último ejecutamos el comando sudo gitlab-ctl reconfigure con resultado: 



### Paso 4 Acceso:<a name="paso4"></a>  
Configuramos la contraseña del root: 

Accedemos: 



Repositorio de github: https://github.com/joelrodriguezmartin/git
