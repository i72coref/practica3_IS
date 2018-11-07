# Hacer_BackUp

**ID:** *07*

**Breve descripción:**
El sistema realiza un Back_Up

**Actores principales:** Usuario (Profesor).

**Actores Secundarios:** Alumnos.

**Precondiciones:**

1. Debe existir un fichero de tipo binario que pueda ser utilizado por el programa.

2. En el menú existe un a opción que permite al usuario seleccionar Hacer_BackUp.

**Flujo principal:**

1. El caso de uso comienza cuando el usuario selecciona la opción de *Hacer_BackUp* desde el menú principal.

2. Aparece por pantalla un mensaje para introducir el nombre que el usuario quiera darle al fichero.

3. El sistema busca el fichero binario en la ruta especificada y guarda todos los datos que se han ido introduciendo, moficando o borrando.

4. El sistema manda un mensaje una vez se han copiado todos los datos en el fichero, mostrando éxito o error.

**Postcondiciones:**

* El sistema muestra mensaje de error o éxito al terminar el BackUp.

**Flujos alternativos:**

1.a Si el usuario introduce un número que no esté dentro del rango del menú debe aparecer un mensaje de error y se debe volver a introducir una opción.


3.a En caso de existir el fichero se sobreeescribe con el nuevo nombre, y si no existe en la ruta especificada, se crea un fichero binario con el nombre introducido.
