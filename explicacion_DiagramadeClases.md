# Diagrama de Clases.

En nuestro Sistema vamos a trabajar con tres Clases principalmente: *Alumno, Agenda y Profesor.*
La Agenda recibe agregación de la clase Alumno (un alumno solo tiene 1 agenda, y la agenda puede recibir de 0 a n alumnos. La clase Agenda está relacionada a su vez con la clase Profesor (una agenda puede tener de 1 a n profesores y un profesor solo tiene una agenda). En cada clase tenemos un conjunto de atributos privados y de funciones públicas:

 - ALUMNO: 

  **Atributos** (**-**): dni, telefono, nombre, apellido, curso, fecha de nacimiento, email, direccion, lider...

  **Funciones** (**+**): Sabiendo que las funciones **SET()** asignan a cada alumno el dato que recibe, y las **GET()** devuelven el dato. Tenemos las siguientes: setDNI, setNombre, setApellidos, setCurso, setFechadeNacimiento, setEmail, setDireccion, setCursoMasAlto, setLider... getDNI, getNombre, getApellidos, getCurso, getFechadeNaciemiento, getEmail, getDireccion, getCursoMasAlto, getLider... con los datos correspondientes.

 - AGENDA 

 **Atributos** (**-**): tendremos un vector con los N alumnos del sistema de tipo: Alumno. vectordealumnos_.

  **Funciones** (**+**): 
- setAlumnos(): asigna a cada alumno los Datos, recibiendo uno auxiliar. 
- GetAlumnos(): devuelve el vector de alumnos y lo muestra. 
- GestiondeLideres(): comprueba que en el grupo que se quiera introducir un lider ya exista o no, uno.
- BorrarAlumno: borra a un alumno buscandolo por su grupo, dni o apellido. 
- BuscarAlumno(): busca a un alumno por su dni, apellido o grupo. 
- Modificar alumno(): modifica a un alumno buscado por su dni, apellido o grupo, teniendo en cada campo la opción de modificar (Si/No). 
- Introducir alumno(): agrea un nuevo alumno al vector de alumnos, introduciendo todos sus datos.
- Ordenar(): ordena lo que veremos por pantalla de manera ascendente o descendente.

 - PROFESOR:

 **Atributos** (**-**): tiene su nombre de usuario, necesario para loguearse al sistema, su rol (asignado en funcion de su nombre de usuario) y un ptrAgenda.

  **Funciones** (**+**): 
- Login(): compara los datos introducidos por el profesor con los que tendremos en un fichero binario. Devuele un número en funcion de si los a introducido correctamente y el rol que tendrá.
- getUsuario(): coge el usuario del profesor.
- HacerBackUp(): le da la opción al Coordinador de hacer un BackUp de los Datos del Sistema en un fichero.
- Cargar BackUp(): le da la opción al Coordinador de volcar en el sistema los Datos de los Alumnos almacenados en un fichero.
- Cargar Fichero Almacenamiento(): una vez que el profesor se loguea en el sistema se carga directamente un fichero con los datos de los alumnos de almacenamiento.
- Guardar Fichero Almacenamiento(): una vez que el profesor desee salir del sistema, se guardan automaticamente los datos de los alumnos almacenados en el programa.
- Asignar Ptr(): le asigna memoria al puntero para acceder a la agenda desde el profesor.
- Liberar Ptr: libera la memoria del puntero.
