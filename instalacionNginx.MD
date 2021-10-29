Joel Rodriguez Martín
2º DAW

### Tarea 11: Instalación de Nginx

## Indice
[Introducción:](#introduccion)       	
[Paso 1: Instalar Nginx](#paso1)       		
[Paso 1: Aplicar ajustes al firewall](#paso2)       	
[Paso 3: Comprobar servidor web:](#paso3)       	
[Paso 4: Configurar bloques de servidor:](#paso4)       	

# Introducción:<a name="introduccion"></a>
En esta práctica realizaremos la instalación del servidor Nginx en Ubuntu.

# Paso 1: Instalar Nginx<a name="paso1"></a>
Actualizamos paquetes con apt update e instalamos nginx:   
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT11/captura1.png)<br/>

# Paso 2: Aplicar ajustes al firewall<a name="paso2"></a>
Enumeramos las configuraciones:  
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT11/captura2.png)<br/>













Permitimos Nginx HTTP:  
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT11/captura3.png)<br/>














# Paso 3: Comprobar servidor web:<a name="paso3"></a>
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT11/captura4.png)<br/>
Comprobamos que el servidor está inactivo, esto es debido al puerto al que esta asignado por defecto.  
# Paso 4: Configurar bloques de servidor:<a name="paso4"></a>
Primero creamos un directorio para nuestro dominio y le damos permisos y propiedad:  
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT11/captura5.png)<br/>









A continuacion creamos una página de ejemplo con nano con el siguiente contenido:  
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT11/captura6.png)<br/>

Y cambiamos la configuración para acceder a un puerto disponible (85):  
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT11/captura7.png)<br/>

Luego habilitamos el archivo haciendo un enlace entre él y el directorio sites-enabled:  
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT11/captura8.png)<br/>

Ahora modificamos nginx.conf para evitar problemas de memoria (descomentamos la linea de bucket size):  

![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT11/captura9.png)<br/>
Comprobamos que el servidor está corriendo:  
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT11/captura10.png)<br/>

Y la página:  
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT11/captura11.png)<br/>

Repositorio de github: https://github.com/joelrodriguezmartin/git
