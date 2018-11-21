# Uso Credenciales

**ID:** *1*

**Breve descripción:**
El sistema debe identificar entre ayudante o coordinador a través de las credeenciales del usuario.

**Actores principales:** Coordinador y Ayudante.

**Actores Secundarios:** Alumnos.

**Precondiciones:**
 
1.- Las credenciales y el Rol deben coincidir con las que tendremos en un fichero binario. 

**Flujo principal:**

1. El caso de uso comienza cuando el usuario ejecuta el porgrama.
2. Tendremos la opcion de salir del programa o introducir credenciales.
2.1. El usuario introduce sus credenciales y su Rol (coordinador o ayudante).
2.1.1. Dependiendo del Rol, cargaremos un menú para el coordinador y otro para el ayudante.

**Postcondiciones:**

* Se mostrará un menú diferente dependiendo de las credenciales introducidas. 

**Flujos alternativos:**

2.1.a. Si las credenciales no coinciden con las del archivo binario se muestra un mensaje de error.
