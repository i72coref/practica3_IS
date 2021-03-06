# ANÁLISIS DE REQUISITOS.

### PRÁCTICA 2. INGENIERÍA DEL SOFTWARE. UCO.
> #### Realizado por:

> * Francisco Javier Córdoba Rey

> * Ángel Cañuelo Ortiz

> * Andrés López Cardenas


## Partes Interesadas:
Las partes interesadas son el **profesor** (va a usar el software), dentro de esta parte diferenciaremos profesor coordinador y ayudante; y **alumnos** (almacenaremos sus datos).

## Datos almacenados.

En el software introduciremos un máximo de _150_ alumnos, y para cada uno de ellos añadiremos:

* Nombre y apellidos.
* Dirección.
* DNI.
* Fecha de Nacimiento.
* Email.
* Curso más alto matriculado.
* Teléfono.

Y opcionalmente:

* Número de Equipo.
* Líder o no _(como máximo 1 por equipo)_.

## Requisitos Funcionales y Prioridad
* El profesor coordinador podrá cargar la información de los alumnos _(cargar Backup)_. [ **3** ]
* El Sistema guardará automaticamente los datos de los alumnos antes de Salir. [ **3** ]
* El sistema cargará los Datos de Almacenamiento de los alumnos [ **3** ]
* El usuario podrá introducir datos de alumnos manualmente. [ **2** ]
* Tendrá la opción de borrar alumno. [ **5** ]
* Tendrá la opción de mostrar datos de alumno. [ **5** ]
* Al usuario le será posible posteriormente, modificar datos de alumno en el sistema. [ **5** ]
* El profesor coordinador podrá hacer un _BackUp_ de los datos del sistema. [ **3** ]
* El usuario podrá gestionar directamente a los líderes de cada equipo [ **5** ]
* El sistema deberá buscar los alumnos y sus datos internamente para que el usuario trabaje con ellos. [ **4** ]
* Al entrar al sistema, pedirá unas credenciales para diferenciar a coordinador de ayudante. [ **1** ]


## Requistos No Funcionales y Prioridad.
* El sistema deberá mostrar la interfaz en el terminal para el usuario. [ **2** ]
* El Sistema será codificado en [C++](http://www.cplusplus.com). [ **1** ]
* Nuestro sistema será fácil y sencillo de usar para el usuario. [ **2** ]
* El sistema será eficiente. [ **2** ]
* Tendremos un sistema cerrado para 4 usuarios que tendrán sus credenciales predefinidas (2 coordinadores y 2 ayudantes). [ **3** ]
* Nuestro sistema será desarrollado para ejecutarse en el Sistema Operativo: _Linux_. [ **2** ]
* El almacenamiento del _BackUp_  será en extensión binaria _(.bin)_. [ **4** ]
* El sistema podrá almacenar como máximo _150_ alumnos. [ **4** ]
* El sistema deberá cumplir los requisitos legislativos y éticos. [ **4** ]
