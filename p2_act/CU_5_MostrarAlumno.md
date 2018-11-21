# Mostrar_Alumno

**ID:** *05*

**Breve descripción:** El usuario podrá mostrar uno o varios alumnos.

**Actores principales:** Usuario (Profesor).

**Actores Secundarios:** Alumnos.

**Precondiciones:**

 1. El alumno/os a mostrar ya tiene/n que estar añadidos al sistema.


**Flujo principal:**

 1. El caso de uso empieza cuando se accede en el menú a la opción: *Mostrar_Alumno*.
 2. Nos dará la opción de mostrar todos los alumnos con sus datos correspondientes.
 3. Tendremos la opción de mostrar un alumno buscando su DNI o apellido.
 4. Podremos mostar alumnos buscando su grupo.

**Postcondiciones:**

 * Se mostrarán los datos de alumnos por el terminal (por defecto).
 * Se podrá seleccionar adicionalmente mostrar mediante fichero (markdown).
 * Si mostramos los alumnos por nombre, estarán ordenados alfabeticamente.
 * Si los mostramos por curso más alto, nos dará la opción de: Ascendete o descendente.
 * El líder de grupo saldrá diferenciado respecto a los demás.

**Flujos alternativos:**

 3.a. Si no existe el alumno o se ha introducido el DNI / Apellido de manera incorrecta el sistema mostrará un mensaje de error.

4.a. Si el grupo buscado no existe, se mostrará un mensaje de error.
