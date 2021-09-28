
Joel Rodriguez Martín
2º DAW

# Tarea 3: Manipulación avanzada de repositorios en Git

## Indice
1. [Introducción](#introduccion)  
2. [Preparación](#preparacion)    
3. [Ejercicio 1](#ejercicio1)  
4. [Ejercicio 2](#ejercicio2)    
5. [Ejercicio 3](#ejercicio3)    
6. [Ejercicio 4](#ejercicio4)     
7. [Ejercicio 5](#ejercicio5)   
8. [Ejercicio 6](#ejercicio6)   
9. [Ejercicio 7](#ejercicio7)   
10. [Ejercicio 8](#ejercicio8)   
11. [Ejercicio 9](#ejercicio9)   



### Introducción <a name="introduccion"></a>
En la siguiente tarea utilizaremos comandos mas avanzados de git.

### Preparación: <a name="preparacion"></a>
Para la realización de las tareas primero clonaremos un repositorio remoto y trabajaremos sobre él.    
![Captura 1](https://github.com/joelrodriguezmartin/git/blob/main/imgsT3/captura1.png)<br/>








### Ejercicio 1: <a name="ejercicio1"></a>
Las tareas serán:
    • Mostrar el historial de cambios del repositorio.   
    • Crear la carpeta capitulos y crear dentro de ella el fichero capitulo1.txt con el siguiente texto.   
    • “Git es un sistema de control de versiones ideado por Linus Torvalds.”  
    • Añadir los cambios a la zona de intercambio temporal.   
    • Hacer un commit de los cambios con el mensaje Añadido capítulo 1.   
    • Volver a mostrar el historial de cambios del repositorio.   
Los comandos utilizados serán los siguientes: 
Se puede observar como en el historial se añade un commit con el mensaje utilizado.
![Captura 2](https://github.com/joelrodriguezmartin/git/blob/main/imgsT3/captura2.png)<br/>



### Ejercicio 2: <a name="ejercicio2"></a>
Las tareas serán:
    • Crear el fichero capitulo2.txt en la carpeta capitulos con el siguiente texto.   
    • “El flujo de trabajo básico con Git consiste en: 1- Hacer cambios en el repositorio. 2- Añadir los cambios a la zona de intercambio temporal. 3- Hacer un commit de los cambios.”  
    • Añadir los cambios a la zona de intercambio temporal.   
    • Hacer un commit de los cambios con el mensaje Añadido capítulo 2.   
    • Mostrar las diferencias entre la última versión y dos versiones anteriores.   
Los comandos utilizados fueron los siguientes:  

![Captura 3](https://github.com/joelrodriguezmartin/git/blob/main/imgsT3/captura3.png)<br/>

Con el comando diff podemos ver las diferencias entre el primer commit y el actual


### Ejercicio 3: <a name="ejercicio3"></a>
Los objetivos serán:
    • Crear el fichero capitulo3.txt en la carpeta capitulos con el siguiente texto.   
    • “Git permite la creación de ramas lo que permite tener distintas versiones del mismo proyecto y trabajar de manera simultanea en ellas.”  
    • Añadir los cambios a la zona de intercambio temporal.   
    • Hacer un commit de los cambios con el mensaje Añadido capítulo 3.   
    • Mostrar las diferencias entre la primera y la última versión del repositorio.   
Los comandos utilizados fueron los siguientes:  
![Captura 4](https://github.com/joelrodriguezmartin/git/blob/main/imgsT3/captura4.png)<br/>













Hacemos cambios y utilizamos el historial para recoger el codigo hash de un commit.  

![Captura 5](https://github.com/joelrodriguezmartin/git/blob/main/imgsT3/captura5.png)<br/>












Y utilizamos el codigo hash con el comando diff para ver las diferencias entre la version actual y el commit que queremos.














### Ejercicio 4: <a name="ejercicio4"></a>
Las tareas objetivo eran las siguientes:
    • Añadir al final del fichero indice.txt la siguiente línea:   
    • “Capítulo 5: Conceptos avanzados”  
    • Añadir los cambios a la zona de intercambio temporal.   
    • Hacer un commit de los cambios con el mensaje Añadido capítulo 5 al índice..   
    • Mostrar quién ha hecho cambios sobre el fichero indice.txt.   
Los comandos usados fueron:  
![Captura 6](https://github.com/joelrodriguezmartin/git/blob/main/imgsT3/captura6.png)<br/>
Utilizamos el comando annotate para ver los cambios en un fichero.




### Ejercicio 5: <a name="ejercicio5"></a>
El objetivo era:
    • Crear una nueva rama bibliografia y mostrar las ramas del repositorio.  
Los comandos usados fueron:  
![Captura 7](https://github.com/joelrodriguezmartin/git/blob/main/imgsT3/captura7.png)<br/>









### Ejercicio 6: <a name="ejercicio6"></a>
Los objetivos eran: 
    • Crear el fichero capitulos/capitulo4.txt y añadir el texto siguiente:   
    • “En este capítulo veremos cómo usar GitHub para alojar repositorios en remoto.”  
    • Añadir los cambios a la zona de intercambio temporal.   
    • Hacer un commit con el mensaje “Añadido capítulo 4.”   
    • Mostrar la historia del repositorio incluyendo todas las ramas.   
Los comandos usados fueron:  
![Captura 8](https://github.com/joelrodriguezmartin/git/blob/main/imgsT3/captura8.png)<br/>








### Ejercicio 7: <a name="ejercicio7"></a>
Los objetivos eran:
    • Cambiar a la rama bibliografia.   
    • Crear el fichero bibliografia.txt y añadir la siguiente referencia:   
    • “Chacon, S. and Straub, B. Pro Git. Apress.”    
    • Añadir los cambios a la zona de intercambio temporal.   
    • Hacer un commit con el mensaje “Añadida primera referencia bibliográfica.”   
    • Mostrar la historia del repositorio incluyendo todas las ramas.   

Los comandos utilizados fueron:  
![Captura 9](https://github.com/joelrodriguezmartin/git/blob/main/imgsT3/captura9.png)<br/>
Hacemos commits en la nueva rama



### Ejercicio 8: <a name="ejercicio8"></a>
En este ejercicio haremos lo siguiente:
    • Fusionar la rama bibliografia con la rama master.   
    • Mostrar la historia del repositorio incluyendo todas las ramas.   
    • Eliminar la rama bibliografia.   
    • Mostrar de nuevo la historia del repositorio incluyendo todas las ramas.   
Los comandos fueron los siguientes:  
![Captura 10](https://github.com/joelrodriguezmartin/git/blob/main/imgsT3/captura10.png)<br/>







### Ejercicio 9: <a name="ejercicio9"></a>
Las tareas eran las siguientes: 
    • Crear la rama bibliografia.   
    • Cambiar a la rama bibliografia.   
    • Cambiar el fichero bibliografia.txt para que contenga las siguientes referencias:   
    • “Scott Chacon and Ben Straub. Pro Git. Apress.  
    • Ryan Hodson. Ry’s Git Tutorial. Smashwords (2014)”  
    • Cambiar a la rama master.   
    • Cambiar el fichero bibliografia.txt para que - contenga las siguientes referencias:   
    • “Chacon, S. and Straub, B. Pro Git. Apress.  
    • Loeliger, J. and McCullough, M. Version control with Git. O’Reilly.”  
    • Añadir los cambios a la zona de intercambio temporal y hacer un commit con el mensaje “Añadida nueva referencia bibliográfica.”   
    • Fusionar la rama bibliografia con la rama master.   
    • Resolver el conflicto dejando el fichero bibliografia.txt con las referencias:   
    • “Chacon, S. and Straub, B. Pro Git. Apress.  
    • Loeliger, J. and McCullough, M. Version control with Git. O’Reilly.”  
    • Añadir los cambios a la zona de intercambio temporal y hacer un commit con el mensaje “Resuelto conflicto de bibliografía.”   
    • Mostrar la historia del repositorio incluyendo todas las ramas.   














Empezaremos por hacer los cambios de la rama bibliografia.  
![Captura 11](https://github.com/joelrodriguezmartin/git/blob/main/imgsT3/captura11.png)<br/>














Luego hacemos los cambios en la rama principal  
![Captura 12](https://github.com/joelrodriguezmartin/git/blob/main/imgsT3/captura12.png)<br/>

















Y finalmente solucionamos el conflicto y comprobamos el historial.  
![Captura 13](https://github.com/joelrodriguezmartin/git/blob/main/imgsT3/captura13.png)<br/>
