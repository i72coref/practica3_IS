# Cargar BackUp.

El usuario Coordinador escoge la opción de Cargar BackUp. Hacemos un bucle LOOP para en el caso que la ruta sea incorrecta, 
la vuelva a pedir.
Tenemos dentro un ALT, si la ruta está correctamente, se muestra un mensaje de carga correcto; 
en caso contrario se muestra un mensaje de error y se vuelve arriba del bucle.

# Hacer BackUp.

El usuario Coordinador, selecciona la opción de hacer BackUp, el sistema pregunta por el nombre del fichero, el usuario la introduce.
Se busca dicho fichero en la ruta del profesor, cuando se encuentra se pide a la agenda el vector 
de los alumnos para almacenarlo en el fichero.
Tendremos un ALT para mostrar un mensaje de guardado Exitoso en caso de que se guarde correctamente, 
y uno de error en caso contrario. 
Al final tenemos un ALT: se muestra un mensaje de guardado exitoso en caso de que se almacene de forma correcta el fichero, 
y en caso contrario se muestra un mensaje de error como anteriormente.

# Guardar Alumnos.

Una vez que el usuario decide que quiere salir del sistema en el menu. 
El Sistema llama a la funcion de guardado, en la que se accede al vector de alumnos de la agenda 
y se sobre-escriben los datos existentes en el fichero del profesor. Tenemos al final un ALT para 
salir si se ha guardado correctamente o mostrar un mensaje de error en caso de que el guardado no haya sido exitoso.


# Cargar Almacenamiento.

El usuario introduce sus credenciales y se confirman. Una vez antes de cargar el menu desde el Sistema, 
tenemos un ALT para cargar todos los Datos de los alumnos, si el fichero con dichos datos se encuentra, 
se carga, y sino se muestra un mensaje de error.

# Gestión de Líderes.

Una vez que introducimos que un alumno es Lider de grupo, o modificamos uno al que le ponemos que lo es. 
Se inicia la gestión de lideres con la agenda, buscando internamente los alumnos de este grupo.
Creamos un LOOP para recorrer el grupo del alumno, para comprobar si en este grupo ya hay un lider 
(no se puede tener más de un lider por grupo).
Cremaos un ALT para que en el caso de que exista un lider se devuelva un mensaje de error, y en el caso contrario 
(no hay lider) se asigna el cargo al miembro mencionado al principio.

# Modificar_Alumno.

Una vez que el Usuario escoge si va a Buscar al Alumno a Modificar por DNI, 
Apellidos o Grupo, empieza nuestro Diagrama de Secuencia a cobrar complejidad. 
Tenemos un ALT general por si el dato es igual a grupo, en caso contrario tenemos otro ALT por si el 
Dato es igual a apellido, y si no se da ninguna de estas dos, ya sabemos que es igual a DNI.

- Si el Dato es igual a Grupo entramos en el primer ALT, y la Opción para modificar por Grupo. 
Tenemos un nuevo ALT para comprobar si existe el grupo introducido, en caso afirmativo: la agenda nos devuelve que existe 
y tenemos un bucle LOOP para que vaya desde el primer hasta el último integrante de dicho grupo, 
y un nuevo bucle ALT para modificar o no cada campo... en el caso de que modificar sea SÍ, se introduce el dato, 
se almacena y se pide el siguiente....; en caso negativo: devuelve un mensaje de error.

- Si el Dato es igual a Apellido, entramos en la segunda opción del primer ALT general, y creamos otro ALT por si el dato fuese DNI, 
pero como es apellido, nos quedamos en la primera opción de este. Una vez dentro tenemos otro ALT por si el apellido existe, 
en caso afirmativo la agenda nos devuelve que existe y tenemos un bucle LOOP para que vaya desde el primer hasta el último 
integrante de dicho grupo, y un nuevo bucle ALT para modificar o no cada campo... en el caso de que modificar sea SÍ, 
se introduce el dato, se almacena y se pide el siguiente....; en caso negativo: devuelve un mensaje de error.

- Si el Dato es igual a DNI, es la subopción del ALT creado para Apellido, repetimos el proceso anterior, 
creamos un ALT por si el DNI existe: y dentro de este un bucle LOOP para que vaya desde el primer dato hasta 
el ultimo pregundado si modificar o no, se crea un ALT para comprobar si modificar es SÌ o NO, en el caso de 
que modificar sea SÍ, se introduce el dato, se almacena y se pide el siguiente.... En el caso que el DNI no exista,
devolvemos un mensaje de error.

# Login

El usuario hace un intento de login con el Sistema que le pide las credenciales, creamos un bucle LOOP para que 
pida las credenciales entre 1 y 5 veces en caso de que no las introduzca correctamente.
Creamos un ALT para que el usuario elija la opción de introducir las credenciales o Salir del Sistema, 
si elige la primera opción entra en un ALT.
Dentro de este ALT, se comprueban que concuerdan con las que tenemos almacenadas en un fichero binario, 
pudiendo acceder a ellas gracias a la ruta en profesor. Si se han encontrado asigna rol al usuario. En el caso contrario, 
se devuelve un mensaje de error. Despues cargamos el Menú en función del ROL ya especificado.

# Borrar Alumno. 

Una vez que el usuario introduce que se va a borrar Alumno, se busca el alumno en la agenda según los parametros introducidos, 
retornando un vector de índices con los alumnos encontrados o NULL en caso contrario.
Creamos un ALT en caso de que el retorno sea igual a NULL, se muestra un mensaje de alumno no encontrado, 
en caso contrario, tenemos un bucle LOOP en el que eliminamos el indice n encontrado, 
restructuramos el vector y mostramos un mensaje de alumno borrado correctamente.

# Buscar_Alumno

Una vez que se llama a una función del sistema (Modificar, Eliminar, Mostrar). En nuestra agenda creamos un 
vector de indices apuntando a NULL.
Dependiendo del tipo de Dato pasado, hacemos un ALT para diferenciarlos, y dentro de cada caso, creamos un bucle LOOP 
que compara el dato pasado por el usuario con todos los elemenos del vector de alumnos (agenda), si coincide se 
almacena el indice del alumno en el vector de índices, y si no coincide se queda a NULL como estaba al principio.
Al final acabamos devolviendo el vector de índices.

# Introducir_alumno

Cuando el usuario escoge la opción de introducir alumno, se pregunta por el número de alumnos que se quiere introducir, 
y hay un bucle LOOP y un ALT para controlar que el usuario no pueda introducir mas de 150 alumnos en total.
Dentro hay otro LOOP que llega hasta el número de alumnos que se quiere introducir, y dentro de el:
-Para los datos que son obligatorios hay otro LOOP y ALT, que pedira el dato y siguirá un esquema do-while que controlará
que no se dejen en blanco.
-Para los que no son obligatorios tan solo se pide el dato y se almacena, aunque sea en blanco.

# Hacer BackUp.

El usuario, coordinador o ayudante, selecciona la opción de cargar un Back_Up introduciendo el número correspondiente a dicha opción según el menú principal. 
A continuación, se le pide al usuario la ruta del fichero donde se encuentra el back_up: (Ejemplo: /dir/backup.txt)
La clase profesor se encargará de buscar el fichero en la ruta especificada: si lo encuentra, se sobreeescribe con los nuevos datos modificados o borrados, en caso contrario, se crea un fichero con el nombre especificado y se guardan los datos en ese fichero. 
Para poder acceder a estos alumnos que se van a guardar es necesario acceder a la agenda en la cual se encuentra el vector de alumnos, con tdos los alumnos del sistema. La agenda devolverá un vector auxiliar igual que el de los alumnos el cual será copiado al fichero del back_up.
Si todo ocurre de forma exitosa, se mostrará un mensaje de éxito, en caso contrario, se muestra mensaje de error. Para ambos casos, una vez se muestyre el mensaje, se vuelve a retornar al menú principal.

# Mostrar Alumno

Comienza cuando el usuario (Coordinador o ayudante) selecciona desde el menú principal la opción de Mostrar Alumno introduciendo para ello el número correspondiente a dicha opción.
El sistema accede a la agenda para poder acceder al vector con los datos de los alumnos cargados. Ahora se le pregunta al usuario si quiere mostrar todos los alumnos o solo algunos.

1.- Si escoge la opción de mostrar todos los alumnos, le aparecen otras 4 opciones para elegir mediante las cuales podrá ordenar la forma en la que se muestran los alumnos, las opciones son: 
 - por dni
 - por nombre
 - por curso más alto
 - por apellidos
Como tenemos dos formas que son de ordenar enteros y otras dos son de cadenas, hemos incluido en dos OPT cada grupo, es decir, por un lado tenemos la ordenación por dni o curso más alto, y por otro la ordenación por nombre o apellidos. Para ello se crea un vector auxiliar copiado del de los alumnos y se ordenará este vector desde la clase Agenda.
Solo en el caso de que se escoja la opción de ordenar por dni o curso más alto, volverán a aparecerle dos opciones al usuario, si lo quiere ordenar de forma ascendente o descendente. En caso contrario, las cadenas se ordenan de forma automática alfabéticamente.
Para mostrar todos los datos de un alumno, utilizamos el LOOP para mostrar cada dato del alumno, mostrando resaltado el nombre de líder en caso de que el alumno lo sea, y este bucle se repitirá hasta recorrer el vector de alumnos.


2.- Si el usuario escoge mostrar solo algunos alumnos, se le dará la opción de mostrar buscando por un dni, buscando un grupo o buscando por apellidos.
Para ello, hemos usado la función de buscar, a la cual le pasaremos (dependiendo de la opción escogida por el alumno) como parámetros el dato a buscar y el tipo de dato.

Esta función nos devuelve un vector con los alumnos encontrados y a continuación mostramos con un LOOP los datos de todos los alumnos con esas coincidencias. Si no se encuentra a nadie con los datos introducidos a buscar, se muestra un mensaje.

Una vez terminemos de mostrar los alumnos con sus datos, ya sea la opción 1 o 2, se carga de nuevo el menú principal y se muestra por pantalla al usuario.
