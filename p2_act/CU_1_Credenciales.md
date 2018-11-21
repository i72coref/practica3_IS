# Uso Credenciales

**ID:** *1*

**Breve descripción:**
El sistema debe identificar entre ayudante o coordinador a través de las credeenciales del usuario.

**Actores principales:** Coordinador y Ayudante.

**Actores Secundarios:** Alumnos.

**Precondiciones:**
 
1.- Las credenciales deben coincidir con las que tendremos en un fichero binario. 

**Flujo principal:**

1. El caso de uso comienza cuando el usuario ejecuta el porgrama.
2. El usuario introduce sus credenciales.

3. El sistema identifica si es ayudante o coordinador.

4. Dependiendo de las credeenciales se cargaŕa un menú para el ayudante y otro para el coordinador. 


**Postcondiciones:**

* Se mostrará un menú diferente dependiendo de las credenciales introducidas. 

**Flujos alternativos:**

2.a. Si las credenciales no coinciden con las del archivo binario se muestra un mensaje de error.
