# Mostrar_Alumno

**ID:** *05*

**Breve descripción:** El usuario podrá mostrar uno o varios alumnos.

**Actores principales:** Usuario: Profesor Coordinador o Ayudante.

**Actores Secundarios:** Alumnos.

**Precondiciones:**

 1. El alumno/os a mostrar ya tiene/n que estar añadidos al sistema.


**Flujo principal:**

 1. El caso de uso empieza cuando se accede en el menú a la opción: *Mostrar_Alumno*.
 2. Nos dará la opción de mostrar todos los alumnos o solo algunos.
 3. Se muestran los datos del/los alumno/s.

**Postcondiciones:**

 * Se mostrarán los datos de alumnos por el terminal (por defecto).
 * Se podrá seleccionar adicionalmente mostrar mediante fichero (markdown).
 * Si los mostramos por curso más alto, nos dará la opción de: Ascendete o descendente.
 * El líder de grupo saldrá diferenciado respecto a los demás.

**Flujos alternativos:**

2.a Si no existe el alumno o se ha introducido el DNI / Apellido de manera incorrecta el sistema mostrará un mensaje de error.

2.b Si se selecciona mostrar todos los alumnos existirán cuatro opciones:
- Ordenar por dni (Ascendente o descendente).
- Ordenar por apellidos.
- Ordenar por curso más alto (Ascendente o descendente).
- Ordenar por nombre.

2.c Si se selecciona no mostrar todos los alumnos existirán tres opciones:
- Mostrar por dni.
- Mostrar por apellidos.
- Mostrar por grupo.

3.a Si el grupo, apellido o dni no existen se muestra mensaje de error y se retorna al menú principal.
