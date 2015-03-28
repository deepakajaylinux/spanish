==========
Service
==========

sinopsis
----------

Este módulo facilita el estado actual del archivo en el sistema. Se puede mencionar el estado como correr o no. La automatización es posible. Este módulo especifica la configuración de su entorno. Es fácil de usar con Ubuntu y CentOS.

comando Ayuda
---------------------

Comando que se utiliza para encontrar información sobre un comando especificado Ayuda. Para obtener más información acerca de los cambios a la funcionalidad del servicio que podemos utilizar este comando ayuda. La siguiente captura de pantalla te guiará.

.. code-block:: bash

    ptconfigure Service help


.. code-block:: bash

	Kevell@corp:/# ptconfigure Service help

	******************************


	  This command allows you to view or modify service

	  Service, service

        - start
        Start a system service
        example: ptconfigure service start --service-name="apache2"

        - stop
        Stop a system service
        example: ptconfigure service restart --service-name="apache2"

        - restart
        Restart a system service
        example: ptconfigure service restart --service-name="apache2"

        - ensure-running
        Ensure a system service is running. If it is already running, dont attempt to start it
        If it is not running, start it
        example: ptconfigure service ensure-running --service-name="apache2"

        - is-running
        Checks whether a system service is running.
        example: ptconfigure service is-running --service-name="apache2"

        - run-at-reboots
        Ensure a system service will auto start on reboots.
        example: ptconfigure service run-at-reboots --service-name="apache2"

	------------------------------
	End Help
	******************************

Opciones
------------
.. cssclass:: table-bordered

 +----------------+-------------------------+---------------------------------+-----------------------------------------------------------+
 | Parámetros     | Parámetro Alternativa   | funciones                       | comandos                                                  |
 +================+=========================+=================================+===========================================================+
 |start           | Service, service        | Iniciar un servicio del sistema | ptconfigure service start –service-name=”apache2”         |
 +----------------+-------------------------+---------------------------------+-----------------------------------------------------------+
 |stop            | Service, service        | Detener un servicio de sistema  | ptconfigure service stop –service-name=”apache2”          |
 +----------------+-------------------------+---------------------------------+-----------------------------------------------------------+
 |Restart         | Service, service        | Reiniciar un servicio del       | ptconfigure service restart –service-name=”apache2”       |
 |                |                         | sistema                         |                                                           |
 +----------------+-------------------------+---------------------------------+-----------------------------------------------------------+
 |Ensure-running  | Service, service        | Garantizar un sistema de        | ptconfigure service ensure-running –service- name         |
 |                |                         | servicio se running.In caso de  | =”apache2”                                                |
 |                |                         | no correr empezar en otro no    |                                                           |
 |                |                         | intente                         |                                                           |
 +----------------+-------------------------+---------------------------------+-----------------------------------------------------------+
 |Is-running      | Service, service        | Compruebe si un servicio del    | ptconfigure service is-running –service-name=”apache2”    |
 |                |                         | sistema está en funcionamiento  |                                                           |
 |                |                         | o no funcionamiento empezar en  |                                                           |
 |                |                         | otro no intente                 |                                                           |
 +----------------+-------------------------+---------------------------------+-----------------------------------------------------------+
 |Run-at-reboots  | Service, service        | Garantizar un servicio          | ptconfigure service run-at-reboots –service-              |
 |                |                         | automático de inicio del        | name=”apache2                                             |
 |                |                         | sistema en los reinicios|       |                                                           |
 +----------------+-------------------------+---------------------------------+-----------------------------------------------------------+


El represenation pictórica de la orden de start, stop, restart, Ensure-running, Is-running and Run-at-reboots se enumeran a continuación ,

.. code-block:: bash

 kevell@corp:/# ptconfigure service start --service-name="apache2"

 [Pharaoh Logging] Starting apache2 service
 * Starting web server apache2
 * 
 ******************************


 Service Modifications:
 --------------------------------------------

 Service: Success

 ------------------------------
 Service Mods Finished
 ******************************

.. code-block:: bash

 kevell@corp:/# ptconfigure service stop --service-name="apache2"

 [Pharaoh Logging] Stopping apache2 service
 * Stopping web server apache2
 * 
 ******************************


 Service Modifications:
 --------------------------------------------

 Service: Success

 ------------------------------
 Service Mods Finished
 ******************************


.. code-block:: bash

 kevell@corp:/# ptconfigure service restart --service-name="apache2"

 [Pharaoh Logging] Restarting apache2 service
 AH00558: apache2: Could not reliably determine the server's fully qualified domain name, using 127.0.1.1. Set the 'ServerName' directive globally to suppress this message
 * Restarting web server apache2
   ...done.
 ******************************


 Service Modifications:
 --------------------------------------------

 Service: Success

 ------------------------------
 Service Mods Finished
 ******************************


.. code-block:: bash


 kevell@corp:/# ptconfigure service ensure-running --service-name="apache2"

 [Pharaoh Logging] Service apache2 is running...
 ******************************


 Service Modifications:
 --------------------------------------------

 Service: Success

 ------------------------------
 Service Mods Finished
 ******************************

.. code-block:: bash


 kevell@corp:/# ptconfigure service is-running --service-name="apache2"

 [Pharaoh Logging] Service apache2 is running...
 ******************************


 Service Modifications:
 --------------------------------------------

 Service: Success

 ------------------------------
 Service Mods Finished
 ******************************

.. code-block:: bash


 kevell@corp:/# ptconfigure service run-at-reboots --service-name="apache2"

 [Pharaoh Logging] Removing current apache2 service startup links
 Removing any system startup links for /etc/init.d/apache2 ...
   /etc/rc0.d/K09apache2
   /etc/rc1.d/K09apache2
   /etc/rc2.d/S91apache2
   /etc/rc3.d/S91apache2
   /etc/rc4.d/S91apache2
   /etc/rc5.d/S91apache2
   /etc/rc6.d/K09apache2
 [Pharaoh Logging] Adding apache2 service startup links
 Adding system startup for /etc/init.d/apache2 ...
   /etc/rc0.d/K20apache2 -> ../init.d/apache2
   /etc/rc1.d/K20apache2 -> ../init.d/apache2
   /etc/rc6.d/K20apache2 -> ../init.d/apache2
   /etc/rc2.d/S20apache2 -> ../init.d/apache2
   /etc/rc3.d/S20apache2 -> ../init.d/apache2
   /etc/rc4.d/S20apache2 -> ../init.d/apache2
   /etc/rc5.d/S20apache2 -> ../init.d/apache2
 ******************************


 Service Modifications:
 --------------------------------------------

 Service: Success

 ------------------------------
 Service Mods Finished
 ******************************




Beneficios
-------------

* El usuario puede comprobar el estado del sistema de trabajo en cualquier momento.
* Servicio proporciona para intercambiar datos entre el sistema.
* Permite la puesta en común de los recursos de la máquina
* El servicio también proporciona la función de copia de seguridad.
* Servicio proporciona un entorno de red flexible.
* Este implica la coordinación de los datos distribuidos.
