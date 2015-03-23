=============
Run Command
=============

sinopsis
------------

Los módulos de comando run permite a los usuarios ejecutar un comando del sistema operativo. Esto es principalmente se utiliza en piloto automático. Con este comando de ejecución el usuario puede especificar el comando, nombre del usuario y también para ejecutar el ya sea en el fondo o front-end. Vamos a ver los usos de la orden de marcha.

comando Ayuda
---------------------

El comando de ayuda describe los usos de la orden de marcha, su gran funcionalidad, sus parámetros alternativos, los comandos utilizados para ejecutar un comando y también acerca de la sintaxis para especificar el comando, nombre del usuario y también para ejecutar el ya sea en el fondo o front-end. A continuación se muestra la sintaxis utilizada para declarar el comando help.


.. code-block:: bash

	ptdeploy RunCommand help

La captura de pantalla siguiente muestra gráficamente sobre el funcionamiento del comando help.



.. code-block:: bash

 kevell@corp:/# ptdeploy RunCommand help
 ******************************


  This allows you to execute an Operating System command. This would primarily be used in an Autopilot.

  RunCommand, runcommand, run-command

        - execute
        Execute a Command
        example: ptconfigure run-command --yes --command="ls -lah /tmp" --run-as-user="ubuntu" --background

 ------------------------------
 End Help
 ******************************


Cómo usar el comando Ejecutar
--------------------------------


La sintaxis utilizada para especificar el funcionamiento comando en se muestra a continuación.


.. code-block:: bash

		ptconfigure run-command --yes --command="ls -lah /tmp" --run-as-user="ubuntu" --background


.. cssclass:: table-bordered

 +------------------------------+-----------------------------------------------+-----------------------------------------------+
 | parámetro			| función					| uso	                                        |
 +==============================+===============================================+===============================================+
 |command="ls -lah /tmp"	| Permite al usuario especificar el      	| Mediante el uso de esto, el usuario puede	|
 |				| comando y su propósito.               	| especificar su propio comando de acuerdo a	|
 |                              |                                               | sus requerimientos.                           |
 +------------------------------+-----------------------------------------------+-----------------------------------------------+
 |run-as-user="ubuntu"		| Al usar este el usuario puede especificar     | Mediante el uso de esto, el usuario puede 	|
 |				| el nombre del usuario				| especificar su usuario requerido de           |
 |                              |                                               | acuerdo a sus requerimientos.                 |
 +------------------------------+-----------------------------------------------+-----------------------------------------------+
 |" --background		| Permite al usuario especificar dónde ejecutar | Mediante el uso de esto, el usuario puede  	|
 |				| el comando en particular , ya sea             | especificar su plataforma de uso de    	|
 |				| en el fondo o en el front-end .		| acuerdo a sus requerimientos.|		|
 +------------------------------+-----------------------------------------------+-----------------------------------------------+




La sintaxis y la mesa como se describió anteriormente puede ayuda al usuario cómo utilizar el comando ejecutar.


beneficios
------------

* Los parámetros utilizados para declarar el comando help, instalación no son mayúsculas y minúsculas que es una ventaja añadida mientras que 
  comparado con otros. 
* Es acomodada en ambos OS ciento y así como en Ubuntu. 
* Los usuarios pueden especificar el comando, nombre del usuario y también para ejecutar el ya sea en el fondo o front-end. 
* El comando help guía a los usuarios en la forma de ejecutar el commando ejecutar un también su propósito.

