# Introducir datos

**ID:** *03*

**Breve descripción:** En cualquier momento el usuario puede introducir nuevos alumnos.

**Actores principales:** Usuario (Profesor).

**Actores Secundarios:** Alumnos.

**Precondiciones:**

1. Cuando se introduce un alumno se deben introducir obligatoriamente el DNI, Nombre, Teléfono, E-mail corporativo, dirección, curso mas alto de matriculación, y, de forma opcional, el equipo y el líder, pudiendo dejar estos 2 últimos campos en blanco.
2. Los datos se introducen únicamente de forma manual por teclado.

**Flujo principal:**

1. El caso de uso comienza cuando el usuario escoge del menú principal la opción de "introducir datos".

2. Se pregunta cuántos alumnos de desea introducir.

3. El programa pide el DNI, nombre,...,del alumno campo por campo.

4. Si se ha llegado al número de alumnos que se desea introducir se sale al menú, sino se introduce otro alumno.

**Postcondiciones:**

* Al finalizar se muestra un mensaje con el número de alumnos en el sistema.

* Los alumnos quedan guardados en memoria principal hasta que se hace el backup.

**Flujos alternativos:**

2.a Si se desea introducir mas de 150 alumnos en total o ningún alumno se muestra un error, y se pide de nuevo el número de alumnos que se desea introducir.

3.a  Si se deja en blanco algún campo obligatorio se muestra un error y se pide de nuevo el dato.
