=============
Run Command
=============

sinopsis
-----------

Los módulos de comando de ejecución permite a los usuarios para ejecutar un comando del sistema operativo. Esto principalmente se debe utilizar en un piloto automático. El uso de este orden de marcha El usuario puede especificar el comando, el nombre del usuario y también para ejecutar el ya sea en el fondo o front-end. Veamos los usos de la orden de marcha.

Ayuda Comando
--------------------

El comando de ayuda describe los usos de la orden de marcha, su funcionalidad principal, sus parámetros alternativos, los comandos que se utilizan para ejecutar un comando, y también acerca de la sintaxis para especificar el comando, el nombre del usuario y también para ejecutar el ya sea en el fondo o frontal -fin. La sintaxis utilizada para declarar el comando de ayuda se muestra a continuación.

.. code-block:: bash

		ptconfigure RunCommand help

La siguiente captura de pantalla muestra gráficamente sobre el funcionamiento de comando ayuda.

.. code-block:: bash

 kevell@corp:/# ptconfigure RunCommand help
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
---------------------------------------

La sintaxis utilizada para especificar el orden de marcha en muestra a continuación.

.. code-block:: bash

		ptconfigure run-command --yes --command="ls -lah /tmp" --run-as-user="ubuntu" --background

.. cssclass:: table-bordered

 +------------------------+------------------------------------+-------------------------+-------------------------------------------------+
 | Parámetros             | función                            | Parámetro Alternativa   | uso                                             |
 +========================+====================================+=========================+=================================================+
 |command=”ls -lah /tmp”  | Permite al usuario especificar el  | RunCommand, runcommand, | Mediante el uso de esto, el usuario puede       |
 |                        | comando y su propósito.            | run-command             | especificar su propio comando de acuerdo a sus  |
 |                        |                                    |                         | requerimientos.                                 |
 +------------------------+------------------------------------+-------------------------+-------------------------------------------------+
 |run-as-user=”ubuntu”    | Al usar este el usuario puede      | RunCommand, runcommand, | Mediante el uso de esto, el usuario puede       |
 |                        | especificar el nombre del usuario. | run-command             | especificar su usuario requerido de acuerdo a   |
 |                        |                                    |                         | sus requerimientos.                             |
 +------------------------+------------------------------------+-------------------------+-------------------------------------------------+
 |” –background           | Permite al usuario especificar     | RunCommand, runcommand, | Mediante el uso de esto, el usuario puede       |
 |                        | dónde ejecutar el comando en       | run-command             | especificar su plataforma de uso de acuerdo     |
 |                        | particular, ya sea en el fondo o   |                         | a sus necesidades.                              |
 |                        | en el front-end.|                  |                         |                                                 |
 +------------------------+------------------------------------+-------------------------+-------------------------------------------------+

Beneficios
-------------

* Los parámetros utilizados para la declaración de la ayuda de mandatos, la instalación no son sensibles, que es una ventaja añadida, mientras 
  que en comparación con otros.
* Es-acomodados tanto en OS Cent y así como en Ubuntu.
* Los usuarios pueden especificar el comando, el nombre del usuario y también para ejecutar el ya sea en el fondo o front-end.
* El comando de ayuda guía a los usuarios en la forma de ejecutar la orden de marcha una también su propósito.
