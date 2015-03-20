========
PhpUnit
========

sinopsis
----------

PHPUnit es un framework de pruebas de unidad para el lenguaje de programación PHP en tesingkamen. Es un ejemplo de la arquitectura para marcos de prueba de unidad que se originó con php test suite Inicializa y llegó a ser popular con pttest.


Funciona de dos maneras. Son init y ejecutar. Es valioso para trabajar con Ubuntu y centos.


comando Ayuda
---------------

El comando help conduce a los usuarios sobre la finalidad y así como sobre las opciones que están incluidas en los módulos de Phpunit. El comando ayuda enumera los parámetros alternativos de Phpunit debajo del módulo pttest. También describe la sintaxis para inicializar la máquina del usuario. A continuación se muestra el comando help de phpunit.


.. code-block:: bash
	
	pttest phpunit help

La sintaxis para el comando de ayuda no mayúsculas y minúsculas que añade una ventaja para este módulo. La siguiente captura de pantalla visualizar al usuario sobre el comando de ayuda en la detección de sistemas.



.. code-block:: bash

 kevell@corp:/# pttest PHPUnit help
 ******************************


  This command allows you to initialize a PHPUnit test suite.

  PHPUnit, phpunit

        - init, initialize
        Initialises the PHPUnit test suite of this project
        example: pttest phpunit init
        example: pttest phpunit initialize

        - execute
        Executes the PHPUnit test suite of this project
        example: pttest phpunit execute

 ------------------------------
 End Help
 ******************************


parámetros alternativos
---------------------------

En lugar de utilizar phpunit el usuario puede utilizar los siguientes parámetros de alternativa.


PHPUnit,  phpunit


inicializar
--------------

Inicializa la suite phptest de este proyecto. Esto puede indicar al usuario que la escritura de uso común para configurar carga automática para las clases que han de analizarse. El comando init es como sigue:


.. code-block:: bash

	pttest phpunit init

¿Después de introducir el sistema puede cuestionar como inicializar PHPUnit? S/N. Esto puede explicarse por the following screenshot.


.. code-block:: bash

 kevell@corp:/# pttest phpunit init
 Initialize PHPUnit? (Y/N) 
 Y
 *******************************
 *   Golden Contact Computing  *
 *          PHPUnit         *
 *******************************
 Creating /tmp/ptconfigure-temp-script-79746566500.sh
 chmod 755 /tmp/ptconfigure-temp-script-79746566500.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-79746566500.sh Permissions
 Executing /tmp/ptconfigure-temp-script-79746566500.sh
 Temp File /tmp/ptconfigure-temp-script-79746566500.sh Removed
 Creating /tmp/ptconfigure-temp-script-57284647129.sh
 chmod 755 /tmp/ptconfigure-temp-script-57284647129.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-57284647129.sh Permissions
 Executing /tmp/ptconfigure-temp-script-57284647129.sh
 Temp File /tmp/ptconfigure-temp-script-57284647129.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.gcsoftshop.co.uk for more
 ******************************


 Single App Installer:
 --------------------------------------------


 PHPUnitInit: Success

 ------------------------------
 Installer Finished
 ******************************


Execute
-------------

Esta ejecución ayuda al usuario a ejecuta PHPUnit test suite de pttest. Pueden ejecutar programas para un sistema en un proceso por lotes sin interacción humana, o un usuario puede escribir comandos en una sesión interactiva del intérprete. Se utiliza el siguiente comando para ejecutar phpunit.


.. code-block:: bash

	pttest phpunit execute

Después de escribir el comando una pregunta. Se pueden visualizar en la siguiente imagen.



.. code-block:: bash

 kevell@corp:/# pttest phpunit execute
 Execute PHPUnit? (Y/N) 
 Y
 *******************************
 *   Golden Contact Computing  *
 *          PHPUnit         *
 *******************************
 Creating /tmp/ptconfigure-temp-script-23757829034.sh
 chmod 755 /tmp/ptconfigure-temp-script-23757829034.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-23757829034.sh Permissions
 Executing /tmp/ptconfigure-temp-script-23757829034.sh
 /tmp/ptconfigure-temp-script-23757829034.sh: 3: /tmp/ptconfigure-temp-script-23757829034.sh: phpunit: not found
 Temp File /tmp/ptconfigure-temp-script-23757829034.sh Removed
 Creating /tmp/ptconfigure-temp-script-85280710426.sh
 chmod 755 /tmp/ptconfigure-temp-script-85280710426.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-85280710426.sh Permissions
 Executing /tmp/ptconfigure-temp-script-85280710426.sh
 Temp File /tmp/ptconfigure-temp-script-85280710426.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.gcsoftshop.co.uk for more
 ******************************


 Single App Installer:
 --------------------------------------------


 PHPUnitExec: Success

 ------------------------------
 Installer Finished
 ******************************


Opciones
--------------


.. cssclass:: table-bordered

 +------------------------------+-----------------------+--------------------------------------------------+
 | parámetros			| opciones		| comentarios	                           	   |
 +==============================+=======================+==================================================+
 |Initialize Phpunit? (Y/N)	| Yes			| phpunit pueda ser inicializada pttest.           |
 +------------------------------+-----------------------+--------------------------------------------------+
 |Execute Phpunit? (Y/N)	| Yes			| Phpunit se puede ejecutar bajo pttest.           |
 +------------------------------+-----------------------+--------------------------------------------------+
 |Initialize Phpunit/Execute 	| No			| Se puede salir de la pantalla  		   |
 |Phpunit? (Y/N)|		|			|					 	   |
 +------------------------------+-----------------------+--------------------------------------------------+
 


beneficios
----------

* PHPUnit fue creado con la opinión de que cuanto antes de que se detectan sus errores de código, más rápido se pueden arreglarlos.  
* Al igual que todos los marcos pruebas unidad PHPUnit utiliza afirmaciones para verificar que el comportamiento de la unidad de código 
  bajo prueba se comporta como se esperaba. 
* PHPUnit puede enviar los resultados de la prueba en un número de diferentes formatos como xml. 
* Phpunit puede ser una caso sin sensibilidad. 
* Phpunit comodidades con Ubuntu y centOS.
