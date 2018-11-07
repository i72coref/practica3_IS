# Modificar_Alumno

**ID:** *06*

**Breve descripción:**
El sistema permite la modificación de los datos del alumno.

**Actores principales:** Usuario (profesor).

**Actores Secundarios:** Alumnos.

**Precondiciones:**

1. Debe existir al menos un alumno cargado en el sistema para poder modificarlo.

2. Es necesario hacer una búqueda previa del alumno a modificar.

**Flujo principal:**

1. El caso de uso comienza cuando el usuario introduce la opción indicada en el menú que le permite modificar los datos del alumno.
2. Para modificar el alumno lo buscamos por su DNI / Apellidos o grupo al modificar varios.
3. El sistema debe permitir con una opción de (Si / No) en cada campo modificar o no los datos del alumno.

**Postcondiciones:**

* El sistema muestra los datos del alumno por pantalla una vez modificado.
* Los datos modificados del alumno quedan guardados en memoria principal.


**Flujos alternativos:**

1.a. En caso de no existir un alumno cargado, el sistema debe mandar un mensaje de error.
