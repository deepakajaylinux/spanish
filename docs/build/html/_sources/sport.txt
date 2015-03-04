========
Port
========

sinopsis
-------------

Puerto certificar para comprobar el estado de los puertos y los servicios. Este módulo ayuda a comprobar el servicio portuario bajo ptconfigure. Este módulo es el más cómodo con Ubuntu y CentOS.

Ayuda Comando
--------------------

Este comando ayuda a guiar al usuario sobre el módulo de puerto. Esto es adecuado para todo tipo de gente de TI.

.. code-block:: bash

          ptconfigure port help

El comando help muestra una breve lista de los comandos integrados en el módulo de puerto.

.. code-block:: bash

	kevell@corp:/# ptconfigure Port  help
	******************************


	  This command allows you to test the status of ports and services running on them

	  Port, port

        - is-responding
        Test if a port is responding
        example: ptconfigure port is-responding --port-number="25"

        - process
        See which process is using a port
        example: ptconfigure port process --port-number="25"

	------------------------------
	End Help
	******************************

anfitrión local
------------------

Cuando el usuario quiere comprobar el estado del puerto de host local entonces puede pedir a la dirección IP del usuario. La siguiente captura de pantalla y lo explicará.

.. code-block:: bash


   	kevell@corp:/# ptconfigure port process --port-number="22"

	[Pharaoh Logging] Port 22 is being used by the process sshd
	******************************


	Port Modifications:
	--------------------------------------------

	Port: Success

	------------------------------
	Port Mods Finished
	******************************

Opciones
---------------
.. cssclass:: table-bordered


 +--------------------+------------------------+--------------------------------------------+------------------------------------+
 | Parámetros         | Parámetro Alternativa  | funciones                                  | salida                             |
 +====================+========================+============================================+====================================+
 |Is-responding       | Port, port             | Prueba de puerto está respondiendo o no    | Responde al proceso de puerto      |
 +--------------------+------------------------+--------------------------------------------+------------------------------------+
 |Process             | Port, port             | Pon a prueba el estado del proceso de Port | Se mostrará el proceso de puerto|  |
 +--------------------+------------------------+--------------------------------------------+------------------------------------+


Beneficios
-------------

* El usuario puede comprobar el estado de funcionamiento actual del puerto.
* Se trata de un módulo de uso fácil.
* Consumir menos tiempo.
