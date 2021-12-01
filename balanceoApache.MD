Joel Rodriguez Martín
2º DAW

Tarea 20: Balanceo de Carga en Apache

Indice
Introducción:	1
Paso 1: Instalacion de módulos de Apache:	1
Paso 2 Modificar configuracion de Apache:	2
Paso 3 Crear contenedores Docker:	2
Introducción:
En esta tarea desplegaremos 4 nodos y haremos un balanceo de carga
Paso 1: Instalacion de módulos de Apache:
Instalamos los modulos necesarios con a2enmod:



Paso 2 Modificar configuracion de Apache:
Añadimos la configuración de proxy a el fichero .conf del servidor Apache:
Paso 3 Crear contenedores Docker:

Configuracion de Docker para crear 4 wildflies
Y los lanzamos, comprobando desde el servidor apache que al refrescar nos mostrara un puerto diferente (balancea la carga entre los puertos):
8081
8084

Repositorio de github: https://github.com/joelrodriguezmartin/gitg
