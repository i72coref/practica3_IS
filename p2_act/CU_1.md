# Interfaz por terminal

**ID:** *01*

**Breve descripción:**
La visualización y utilización del software será mediante la terminal de Linux.

**Actores principales:** Usuario (Profesor).

**Actores Secundarios:** Alumnos.

**Precondiciones:**
El sistema se usará un sistema operativo basado en GNU/Linux.

**Flujo principal:**

1. El caso de uso comienza cuando el usuario ejecuta el programa.
2. El programa se abre en una ventana de terminal.
3. Para seleccionar una opción debemos de introducir por teclado el numero indicado.


**Postcondiciones:**
* El programa no recoge ningun argumento.
* Cada vez que seleccionemos una opción, se limpiará el terminal con los datos de la opción anterior.

**Flujos alternativos:**
1.a. En caso de que el programa esté corrupto o no haya memoria disponible en el sistema no se abrirá.
3.a. Si introduce un número fuera del rango establecido para seleccionar, se vuelve a pedir un numero dentro del rango.
