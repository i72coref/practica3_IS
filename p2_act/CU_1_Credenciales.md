# Uso Credenciales

**ID:** *1*

**Breve descripción:**
El sistema debe identificar entre ayudante o coordinador a través de las credeenciales del usuario.

**Actores principales:** Usuario: Profesor Coordinador o Ayudante.

**Actores Secundarios:** Alumnos.

**Precondiciones:**
 
1.- Las credenciales y deben coincidir con las que tendremos en un fichero binario. 

2.- Tendremos 5 oportunidades para introducir las credenciales de forma correcta, si fallamos saldrá del sistema.

**Flujo principal:**

1. El caso de uso comienza cuando el usuario ejecuta el porgrama.
2. Tendremos la opcion de salir del programa o introducir credenciales.

2.1. El usuario introduce sus credenciales.

2.1.1. Dependiendo de dichas credenciales, asignaremos un Rol: Ayudante o Coordinador.

**Postcondiciones:**

* Se mostrará un menú diferente dependiendo de las credenciales introducidas. 

**Flujos alternativos:**

2.1.a. Si las credenciales no coinciden con las del archivo binario se muestra un mensaje de error.
