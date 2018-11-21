# Búsqueda_Datos

**ID:** *08*

**Breve descripción:**
El sistema busca los datos de un alumno o un grupo.

**Actores principales:** Usuario (Profesor).

**Actores Secundarios:** Alumnos.

**Precondiciones:**

1. Debe haber cargado un alumno como mínimo para usar esta función.

2. Para acceder a esta opción es necesario acceder previamente a mostrar/modificar/borrar un alumno.

**Flujo principal:**

1. El caso de uso comienza cuando el usuario muestra/modifica/borra los datos de un alumno.

2. Cuando selecciona una de las tres opciones anteriores el usuario introduce el apellido o dni por el que quiere filtrar.

3. Los datos seleccionados aparecen por pantalla.

**Postcondiciones:**

* El sistema muestra por pantalla los datos del alumno.

**Flujos alternativos:**

1.a Si no hay ningún dato cargado aparece mensaje de error indicando que no hay datos en el sistema.

2.a En caso de no existir el dni/apellido introducido para buscar, se muestra que no existe nadie con esos datos y se retorna para volver a introducir uno de los dos datos.
