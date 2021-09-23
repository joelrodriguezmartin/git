Joel Rodriguez Martín
2º DAW

Tarea 2: Manipulación de repositorios en Git

Indice
Introducción:	1
Configuración de git:	1
Creación de un repositorio:	2
Comprobar el estado del repositorio:	2
Realizando commits:	3
Modificación de ficheros:	3
Historial:	4
Introducción:
En la siguiente tarea crearemos y manipularemos repositorios en Git.

Configuración de git:
En primer lugar cambiaremos la configuración de git para definir nombre de usuario, correo y activar el coloreado. Después comprobamos la configuración:



Creación de un repositorio:
A continuación crearemos un repositorio llamado dpl y mostraremos su contenido:

Comprobar el estado del repositorio:
En primer lugar comprobamos el estado el repositorio utilizando el comando “git status”A continuación creamos un fichero de índice en nuestro repositorio y volvemos a comprobar el estado. Finalmente añadimos el fichero a la zona de intercambio y volvemos a comprobar el estado.











Realizando commits: 
Ahora realizaremos un commit de los cambios al fichero índice con un mensaje personalizado: 

Modificación de ficheros: 
A continuación modificamos el fichero índice, cambiando sus datos. Con los cambios realizados utilizamos el comando “git diff” para ver las diferencias en el fichero y hacemos commit de los cambios: 

Historial: 
Finalmente haremos uso del historial para mostrar los cambios del repositorio. Luego haremos cambios al mensaje del último commit y volveremos a mostrar los cambios: 

