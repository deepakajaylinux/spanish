=========
PHPMD
=========

sinopsis
----------------

PHP MessDeductor es un spin-off de PHP dependen y pretende ser un PHP equivalente a la herramienta Java conocida PMD. PHPMD puede ser visto como una aplicación frontend fácil de usar para la corriente métricas medida en bruto por PHP Depend. Colateral General o GC es la gama de activos que son aceptadas, en un momento dado, como garantía en el mercado de repos por la mayoría de los intermediarios del mercado ya un tipo de interés muy similar. Esto es adecuado con Ubuntu y CentOS.

comando Ayuda
----------------------

Se necesita una base de código fuente PHPMD dado y buscar varios problemas potenciales dentro de esa fuente. PHPMD es un proyecto joven y tan sólo proporciona un conjunto limitado de reglas predefinidas, en comparación con el PMD, que detectan código de olores y posibles errores en el código fuente analizada. Pedido la sección de reglas para aprender más acerca de las reglas allimplemented. El siguiente comando ayuda guía al usuario a instalar el módulo phpmd.

.. code-block:: bash

		ptconfigure PHPMD help

La siguiente captura de pantalla vizualize sus funciones.

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPMD help
 ******************************


  This command allows you to install PHPMD from a GC Repo.

  PHPMD

        - install
        Installs the latest GC Repo version of PHPMD
        example: ptconfigure phpmd install

 ------------------------------
 End Help
 ******************************

instalación
-------------------------

Por el momento PHPMD viene con los siguientes tres procesadores:

* Xml, que formatea el informe como XML.
* Texto, formato de texto simple.
* Html, único archivo HTML con posibles problemas.

El comando utilizado para instalar el PHPMD a la máquina de los usuarios se muestra a continuación.

.. code-block:: bash


		ptconfigure PHPMD install

Después de introducir el comando anterior, el siguiente proceso se produce como se muestra en el formato de pantalla.

.. code-block:: bash

 kevell@corp:/# ptconfigure phpmd install
 Install PHP Mess Detector ? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         PHP Mess Dt.        *
 *******************************
 What is the program data directory? Found "/opt/phpmd" - use this? (Enter nothing for yes, no end slash)

 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'https://github.com/phpengine/ptconfigure-phpmd.git'  /tmp/phpmd/phpmdCloning into '/tmp/phpmd/phpmd'...
 remote: Counting objects: 356, done.
 remote: Total 356 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (356/356), 306.45 KiB | 9.00 KiB/s, done.
 Resolving deltas: 100% (239/239), done.
 Checking connectivity... done.
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************
 

 Single App Installer:
 --------------------------------------------
 PHPMD: Success
 ------------------------------
 Installer Finished
 ******************************

Opciones
------------

.. cssclass:: tabe-bordered

 +-------------------------+--------------------------------+------------+---------------------------------------------------+
 | Parámetros              | Directorio (por defecto)       | Opciones   | Comentarios                                       |
 +=========================+================================+============+===================================================+
 |Data directory           | “/opt/PHPMD”                   | Yes        | Se instalará módulo PHPMD bajo ptconfigure        |
 |(Por defecto)            |                                |            |                                                   |
 +-------------------------+--------------------------------+------------+---------------------------------------------------+
 |Data directory           | End slash                      | No         | El usuario tiene a un especifique la ruta.        |
 +-------------------------+--------------------------------+------------+---------------------------------------------------+
 |Executor directory       | “/usr/bin”                     | Yes        | Se instalará directorio ejecutor                  |
 |(Por defecto)            |                                |            |                                                   |
 +-------------------------+--------------------------------+------------+---------------------------------------------------+
 |Executor directory       | No trailing slash              | No         | El usuario da entrada como nombre del directorio| |
 +-------------------------+--------------------------------+------------+---------------------------------------------------+
  

Beneficios
------------------

ExcessivePublicCount:

Es posible que un gran número de métodos públicos y atributos declarados en una clase puede indicar la categoría de no estar funcionando como 
un mayor esfuerzo lo hará ser requerido para probar a fondo.


ExcessiveParameterList:

Listas de parámetros largos pueden indicar que un nuevo objeto debe ser creado para envolver los numerosos parámetros. Básicamente, pruebe los parámetros junto al grupo.


CyclomaticComplexity:

Complejidad se determina por el número de puntos de decisión en un método más uno para la entrada método.


superglobals:

Acceso a una variable de super-mundial directamente se considera una mala práctica. Estas variables deben ser encapsulados en los objetos que 
se proporcionan por un marco, por ejemplo.


ShortVariable:

Detecta cuando un campo, local o parámetro tiene un nombre muy corto.


LongVariable:

Detecta cuando un campo, variables formales o local se declara con un nombre largo.
