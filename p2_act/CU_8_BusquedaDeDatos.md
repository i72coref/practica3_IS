# Búsqueda_Datos

**ID:** *08*

**Breve descripción:**
El sistema busca los datos de un alumno o un grupo.

**Actores principales:** Usuario: Profesor Coordinador o Ayudante.

**Actores Secundarios:** Alumnos.

**Precondiciones:**

1. Debe haber cargado un alumno como mínimo para usar esta función.

2. Para acceder a esta opción es necesario acceder previamente a mostrar/modificar/borrar un alumno.

3. Si se va a buscar un grupo debe de existir.

**Flujo principal:**

1. El caso de uso comienza cuando el usuario muestra/modifica/borra los datos de un alumno.

2. Dependiendo de los parámetros introducidos por el usuario se buscara internamente en nuestro sistema.

3. Se devuelve un vector de indices con las posiciones correspondientes a los elementos especificados con antelación.

**Postcondiciones:**

* Se devuelve el vector con los índices almacenados.

**Flujos alternativos:**

1.a Si no hay ningún dato se devuelve NULL.

2.a En caso de no existir el dni/apellido o grupo introducido para buscar, se devuelve NULL.
