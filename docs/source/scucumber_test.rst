============
Cucumber
============


Sinopsis
------------

Este módulo ayuda al usuario a iniciar y ejecutar el paquete de pruebas de pepino. Veamos cómo inicializar y ejecutar el paquete de pruebas de pepino en los próximos temas.


comando Ayuda
--------------------

El comando ayuda guía al usuario en cuanto al propósito y opciones disponibles bajo un módulo. Enumera los parámetros alternativos que se utilizan en la declaración. Describe la sintaxis para inicializar y ejecutar el pepino bajo el pttest. A continuación se muestra el comando utilizado para declarar ayuda:


.. code-block:: bash

	pttest cucumber help

La captura de pantalla siguiente muestra gráficamente sobre el funcionamiento del comando help.


.. code-block:: bash

 kevell@corp:/# pttest cucumber help
 ******************************


  This command allows you to initialize a Cucumber test suite.

  Cucumber, cucumber

        - init, initialize
        Initialises the Cucumber test suite of this project
        example: pttest cucumber init
        example: pttest cucumber initialize

        - execute
        Executes the Cucumber test suite of this project
        example: pttest cucumber execute

 ------------------------------
 End Help
 ******************************


Cómo inicializar pepino 
-----------------------------------

El comando usado para inicializar el pepino en pttest se muestra:

.. code-block:: bash

	pttest cucumber init

or 

.. code-block:: bash

	pttest cucumber initialize

Después de introducir el comando anterior, ocurre el proceso de inicialización, como se muestra en la tabla siguiente.



.. cssclass:: table-bordered

 +-----------------------------+--------------------------------------+-----------+---------------------------------------+
 | parámetros		       | parámetro alternativo                | opciones  | comentarios			          |
 +=============================+======================================+===========+=======================================+
 |Initialize Cucumber? (Y/N)   | En vez de pepino , podemos utilizar  | Y(Yes)	  | Si el usuario desea continuar el init |
 | 			       | el pepino también                    | 	  | se puede introducir como Y.           |
 +-----------------------------+--------------------------------------+-----------+---------------------------------------+
 |Initialize Cucumber? (Y/N)   | En vez de pepino , podemos utilizar  | N(No) 	  | Si el usuario desea salir del proceso |
 | 			       | el pepino también                    | 	  | init que puede introducir como N.|    |
 +-----------------------------+--------------------------------------+-----------+---------------------------------------+


Finalmente consigue inicializado el pepino pttest como se muestra en la siguiente pantalla.



.. code-block:: bash


 kevell@corp:/# pttest cucumber init
 Initialize Cucumber? (Y/N) 
 Y
 *******************************
 *   Golden Contact Computing  *
 *          Cucumber         *
 *******************************
 Creating /tmp/ptconfigure-temp-script-81470621814.sh
 chmod 755 /tmp/ptconfigure-temp-script-81470621814.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-81470621814.sh Permissions
 Executing /tmp/ptconfigure-temp-script-81470621814.sh
 Temp File /tmp/ptconfigure-temp-script-81470621814.sh Removed
 Creating /tmp/ptconfigure-temp-script-65310697385.sh
 chmod 755 /tmp/ptconfigure-temp-script-65310697385.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-65310697385.sh Permissions
 Executing /tmp/ptconfigure-temp-script-65310697385.sh
 Temp File /tmp/ptconfigure-temp-script-65310697385.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.gcsoftshop.co.uk for more
 ******************************


 Single App Installer:
 --------------------------------------------


 Cucumber: Success

 ------------------------------
 Installer Finished
 ******************************


Cómo ejecutar el pepino 
----------------------------------------

The command used for executing the cucumber under pttest is shown:

.. code-block:: bash

pttest cucumber execute

Después de introducir el comando anterior, ocurre el proceso de ejecución, como se muestra en la tabla siguiente.

.. cssclass:: table-bordered

 +-----------------------------+--------------------------------------+-----------+-------------------------------------------+
 | parámetros                  | parámetro alternativo                | opciones  | comentarios                               |
 +=============================+======================================+===========+===========================================+
 |Execute Cucumber? (Y/N)      | En vez de pepino , podemos utilizar  | Y(Yes)    | Si el usuario desea continuar el proceso  |
 |                             | el pepino también                    |           | de ejecución se puede introducir como Y.  |
 +-----------------------------+--------------------------------------+-----------+-------------------------------------------+
 |Execute Cucumber? (Y/N)      | En vez de pepino , podemos utilizar  | N(No)     | Si el usuario desea abandonar el proceso  |
 |                             | el pepino también                    |           | de ejecución se puede introducir como N.| |
 +-----------------------------+--------------------------------------+-----------+-------------------------------------------+



Si el usuario procede a la ejecución, el proceso de ejecución se producirá como se muestra en la siguiente pantalla.



beneficios
------------


* Es acomodada en ambos OS ciento y así como en ubuntu. 
* Los parámetros utilizados en la declaración no son mayúsculas y 
  minúsculas que es una ventaja añadida mientras que comparado con otros. * Este pepino permite a los usuarios para iniciar y ejecutar el paque  te de pruebas de pepino.

