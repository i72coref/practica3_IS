# Administración de líderes

**ID:** *09*

**Breve descripción:** El sistema se encarga de organizar y administrar los líderes de cada grupo.

**Actores principales:** Usuario (Profesor).

**Actores Secundarios:** Alumnos.

**Precondiciones:**

1.- Es necesario introducir un alumno previamente.

**Flujo principal:**

1.- El caso de uso comienza cuando el usuario introduce o modifica un alumno el cual ha sido marcado como líder.

2.- El sistema comprueba dentro del grupo del alumno modificado/introducido si alguno de los integrantes es ya un líder o no.

3.- Si no existe un líder en el grupo del alumno modificado/introducido, se asignará dicho cargo a dicho alumno.

**Postcondiciones:**

* Si se introduce el alumno como líder, quedará modificado en los datos del sistema hasta que se realice el BackUp.

**Flujos alternativos:**

3.a En el caso de existir un líder, se mostrará un mensaje por pantalla indicando que no es posible asignar dicho cargo y se mostrará el actual líder del grupo, y en caso de que el usuario quiera asignar un nuevo líder, deberá modificarlo manualmente.
