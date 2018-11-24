# Cargar Backup

**ID:** *02*

**Breve descripción:**
En cualquier momento se podrá cargar un fichero el cual contiene los ditintos datos de los alumnos.

**Actores principales:** Usuario: Profesor Coordinador o Ayudante.

**Actores Secundarios:** Alumnos.

**Precondiciones:**

1. Para poder cargar un backup el usuario tiene que tener un backup con el formato correcto, en un fichero binario.
2. El fichero debe existir en la ruta especificada.

**Flujo principal:**

1. El caso de uso comienza cuando el usuario selecciona la opción de "Cargar backup".
2. El programa pide la ruta del backup, por defecto será la misma carpeta del software. 
3. Se cargan los datos del fichero en memoria.

**Postcondiciones:**

* Se muestra un mensaje informando que el proceso se ha realizado con éxito.


**Flujos alternativos:**

2.a En caso de no encontrar el fichero especificado saltará un error, y después se pedirá de nuevo el nombre de la ruta del backup.

3.a Si el fichero está corrupto se lanza un mensaje de error.
