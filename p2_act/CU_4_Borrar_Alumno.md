# Borrar_Alumno

**ID:** *04*

**Breve descripción:** El usuario podrá borrar únicamente un solo alumno a la vez.

**Actores principales:** Usuario (Profesor).

**Actores Secundarios:** Alumnos.

**Precondiciones:**

 1. El alumno a borrar ya tiene que estar añadido al sistema.

**Flujo principal:**

 1. El caso de uso empieza cuando se accede en el menú a la opción: *Borrar_Alumno*.
 2. Después nos pedirá la opción de borrar por DNI o apellido al alumno.
 3. Debemos de introducir dicho DNI o Apellido por terminal.

**Postcondiciones:**

 * Si existen dos alumnos con el mismo apellido, solo se podrá borrar por DNI.
 * Una vez borremos un alumno, se mostrará por terminal: *Alumno borrado correctamente*.

**Flujos alternativos:**

 3.a. Si no existe el alumno o se ha introducido el DNI / Apellido de manera incorrecta el sistema dará error de borrado.
