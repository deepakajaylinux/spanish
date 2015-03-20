=========
Behat
=========

Sinopsis
------------

Este módulo permite al usuario inicializar behat test suite. El behat ayuda en las pruebas de un script php. Pueden destacar las plantillas habilitadas y deshabilitadas. Veamos cómo init y ejecutar el teskingkamen behat.

comando Ayuda
---------------------

El comando ayuda guía al usuario en cuanto al propósito y opciones disponibles bajo un módulo. Enumera los parámetros alternativos que se utilizan en la declaración. Describe la sintaxis para inicializar y ejecutar un behat bajo la pttest. A continuación se muestra el comando utilizado para declarar ayuda:


.. code-block:: bash

	pttest behat help

La captura de pantalla siguiente muestra gráficamente sobre el funcionamiento del comando help.


.. code-block:: bash

 kevell@corp:/# pttest Behat help
 ******************************


  This command allows you to initialize a Behat test suite.

  Behat, behat

        - init, initialize
        Initialises the Behat test suite of this project
        example: pttest behat init
        example: pttest behat initialize

        - execute
        Executes the Behat test suite of this project
        example: pttest behat execute

 ------------------------------
 End Help
 ******************************


Cómo inicializar Behat 
-----------------------------

El comando usado para inicializar el behat bajo pttest se muestra:

.. code-block:: bash

	pttest behat init

or 

.. code-block:: bash

	pttest behat initialize


Después de introducir el comando anterior, ocurre el proceso de inicialización, como se muestra en la tabla siguiente.


.. cssclass:: table-bordered

 +-----------------------+----------------------------------------+------------+---------------------------------------+
 | parámetros      	 | parámetro alternativo                  | opciones   | comentarios  			       |
 +=======================+========================================+============+=======================================+
 |Initialize Behat?      | En lugar de Behat , podemos utilizar   | Y(Yes)     | Si el usuario desea continuar el      |
 |(Y/N)			 | Behat también         		  |	       | init se puede introducir como Y.      |
 +-----------------------+----------------------------------------+------------+---------------------------------------+
 |Initialize Behat?      | En lugar de Behat , podemos utilizar   | N(No)      | Si el usuario desea salir del proceso |
 |(Y/N)			 | Behat también			  |	       | init que puede introducir como N.|    |
 +-----------------------+----------------------------------------+------------+---------------------------------------+


En lugar de Behat , podemos utilizar Behat también


Finalmente el pttest behat obtiene inicializada como se muestra en la siguiente pantalla.


.. code-block:: bash

 kevell@corp:/# pttest behat init
 Initialize Behat? (Y/N) 
 Y
 *******************************
 *   Golden Contact Computing  *
 *          Behat         *
 *******************************
 Creating /tmp/ptconfigure-temp-script-72748278108.sh
 chmod 755 /tmp/ptconfigure-temp-script-72748278108.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-72748278108.sh Permissions
 Executing /tmp/ptconfigure-temp-script-72748278108.sh
 /tmp/ptconfigure-temp-script-72748278108.sh: 3: /tmp/ptconfigure-temp-script-72748278108.sh: behat: not found
 Temp File /tmp/ptconfigure-temp-script-72748278108.sh Removed
 Creating /tmp/ptconfigure-temp-script-35600300430.sh
 chmod 755 /tmp/ptconfigure-temp-script-35600300430.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-35600300430.sh Permissions
 Executing /tmp/ptconfigure-temp-script-35600300430.sh
 Temp File /tmp/ptconfigure-temp-script-35600300430.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.gcsoftshop.co.uk for more
 ******************************


 Single App Installer:
 --------------------------------------------


 Behat: Success

 ------------------------------
 Installer Finished
 ******************************


Cómo ejecutar el Behat 
---------------------------

Se muestra el comando utilizado para ejecutar el behat bajo pttest:

.. code-block:: bash

	pttest behat execute
 

Después de introducir el comando anterior, ocurre el proceso de ejecución, como se muestra en la tabla siguiente.


.. cssclass:: table-bordered 

 +-----------------------+----------------------------------------+------------+-----------------------------------------------+
 | parámetros            | parámetro alternativo                  | opciones   | comentarios                                   |
 +=======================+========================================+============+===============================================+
 |Execute Behat?         | En lugar de Behat , podemos utilizar   | Y(Yes)     | Si el usuario desea continuar el proceso de   |
 |(Y/N)                  | Behat también                          |            | ejecución se puede introducir como Y.         |
 +-----------------------+----------------------------------------+------------+-----------------------------------------------+
 |Execute Behat?         | En lugar de Behat , podemos utilizar   | N(No)      | Si el usuario desea abandonar el proceso de   |
 |(Y/N)                  | Behat también                          |            | ejecución se puede introducir como N.|        |
 +-----------------------+----------------------------------------+------------+-----------------------------------------------+


Si el usuario procede a la ejecución, el proceso de ejecución se producirá como se muestra en la siguiente captura de pantalla.


.. code-block:: bash

 kevell@corp:/# pttest behat execute
 Execute Behat? (Y/N) 
 y
 *******************************
 *   Golden Contact Computing  *
 *            Behat!           *
 *******************************
 Creating /tmp/ptconfigure-temp-script-93439425208.sh
 chmod 755 /tmp/ptconfigure-temp-script-93439425208.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-93439425208.sh Permissions
 Executing /tmp/ptconfigure-temp-script-93439425208.sh
 /tmp/ptconfigure-temp-script-93439425208.sh: 2: /tmp/ptconfigure-temp-script-93439425208.sh: behat: not found
 Temp File /tmp/ptconfigure-temp-script-93439425208.sh Removed
 Creating /tmp/ptconfigure-temp-script-97268122064.sh
 chmod 755 /tmp/ptconfigure-temp-script-97268122064.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-97268122064.sh Permissions
 Executing /tmp/ptconfigure-temp-script-97268122064.sh
 Temp File /tmp/ptconfigure-temp-script-97268122064.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.gcsoftshop.co.uk for more
 ******************************


 Single App Installer:
 --------------------------------------------


 Behat: Success

 ------------------------------
 Installer Finished
 ******************************


Beneficios
-----------

* Guía a los usuarios para identificar los errores de script php. 
* Utilizar las funciones del behat los usuarios pueden enmarcar y especificar el comportamiento de desarrollo conducido. 
* El proceso de inicialización y ejecución puede hacerse bajo este behat de pttestt. 
* Es acomodada en ambos OS ciento y así como en ubuntu. 
* Los parámetros utilizados en la declaración no son mayúsculas y minúsculas que es una ventaja añadida mientras que comparado con otros.

