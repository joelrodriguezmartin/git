Joel Rodriguez Martín
2º DAW

Tarea 1: Instalación de Git en Linux

Indice
Introducción:	1
Instalación de Git:	1
1. Instalación de Git con paquetes predeterminados:	1
2. Instalación de Git desde la fuente:	3
Configuración de Git:	5
Introducción:
En la siguiente tarea se procederá a describir los pasos necesarios para la instalación de Git en Linux. 

Instalación de Git:

1. Instalación de Git con paquetes predeterminados:
En primer lugar instalaremos Git con el administrador de paquetes de Linux.

Para empezar comprobamos si Git está instalado en nuestra versión de Linux con el comando
“git –version”:

Como podemos observar en el resultado en nuestro caso Git no estaba instalado por defecto en nuestra versión de Linux.

Procederemos a la instalación utilizando la herramienta apt de Linux, actualizando primero con el comando “sudo apt update” y luego instalandola con el comando “sudo apt install git”:

A continuación comprobamos la versión de git instalada: 
Como podemos ver en el output de la terminal la versión instalada es 2.25.1








2. Instalación de Git desde la fuente:
A continuación instalaremos Git desde la fuente.

Empezamos por comprobar la versión de Git y actualizar una vez mas el administrador de paquetes:
 
A continuacion instalamos los paquetes necesarios para Git con “sudo apt install” seguido de todos los paquetes: 
Con las dependencias instaladas creamos un directorio temporal, donde descargaremos Git, y nos movemos a él. A continuación utilizando curl descargaremos la última versión de Git obtenida en la página oficial:


Después descomprimimos el archivo tarball y nos dirigimos al directorio creado en la descompresión. 

Una vez ahí creamos e instalamos el paquete con los comandos en las capturas:



Finalmente en una nueva terminal comprobamos la versión de Git y observamos que es la deseada (2.29.3)


Configuración de Git:
Una vez realizada la instalación de Git debemos configurarlo de manera que muestre la información correcta.
Para ello utilizaremos el comando “git config –global” seguido de nuestra información, y posteriormente podemos comprobarlo con  “git config --list”
















Otra manera de cambiar la configuración es modificar el fichero de configuración de Git, que en nuestro caso haremos utilizando la herramienta nano, con el comando “nano ~/.gitconfig”.
Esto abrirá el fichero y permitirá su edición como en la captura siguiente: 



