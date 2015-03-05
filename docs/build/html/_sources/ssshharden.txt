=============
SshHarden
=============

sinopsis
----------

Este módulo ayuda a la creación y modificación sshhardens. El endurecen ssh facilita las funciones de seguridad de las cuentas de usuarios de SSH.

Ayuda Comando
--------------------

El comando de ayuda conduce a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en el módulo endurecen SSH. Las listas de comandos de ayuda fuera de los parámetros alternativos de endurecer SSH. También se describe la sintaxis para utilizar endurecen SSH para Securify. El comando de ayuda para SSH endurecen es la siguiente.

.. code-block:: bash

	ptconfigure SshHarden help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda bajo SSH Harden.

.. code-block:: bash

	Kevell@corp:/# ptconfigure SshHarden help
	
	******************************


        This command allows you to modify create or modify sshhardens

	SshHarden, sshharden, ssh-harden

        - securify
        Add some security to your SSH accounts
        example: ptconfigure ssh-harden securify

	------------------------------
	End Help
	******************************


Securify
-----------

El comando utilizado para securifying la cuenta de los usuarios a través de SSH endurecen SSH se muestra a continuación:

.. code-block:: bash

	ptconfigure ssh-harden securify

Después de introducir el comando como se da por encima de la instalación de Ssh endurecimiento comienza como se muestra en el formato tabular.

.. cssclass:: table-bordered

 +-------------------------+----------------------------------------+------------+--------------------------------------------------+
 | Parámetros              | Parámetro Alternativa                  | Opciones   | Comentarios                                      |
 +=========================+========================================+============+==================================================+
 |Install Ssh Hardening?   | En lugar de Ssh Hardening, las         | Y(Yes)     | Si el usuario desea continuar el proceso de      |
 |(Y/N)                    | siguientes alternativas también se     |            | instalación se puede introducir como Y.          |
 |                         | pueden utilizar: SshHarden, sshharden, |            |                                                  |
 |                         | ssh-harden.                            |            |                                                  |
 +-------------------------+----------------------------------------+------------+--------------------------------------------------+
 |Install Ssh Hardening?   | En lugar de Ssh Hardening, las         | N(No)      | Si el usuario desea abandonar el proceso de      |
 |(Y/N)                    | siguientes alternativas también se     |            | instalación se puede introducir como N.          |
 |                         | pueden utilizar: SshHarden, sshharden, |            |                                                  |
 |                         | ssh-harden.|                           |            |                                                  |
 +-------------------------+----------------------------------------+------------+--------------------------------------------------+

Si el usuario continúa la instalación de Ssh endurecen que permite securifying la cuenta ssh de los usuarios consigue iniciado. Mientras se produce el proceso de ejecución, la configuración sshd es modificado que no permite ssh root login y así como de configuración sshd es modificado que desautoriza contraseña basada ssh login. finalmente, se reinicia el servicio ssh y mostrar los resultados de terminadas las modificaciones Ssh Harden. La siguiente captura de pantalla explica el proceso mencionado anteriormente pictóricamente.

.. code-block:: bash

	Kevell@corp:/# ptconfigure ssh-harden securify
	
	Install Ssh Hardening? (Y/N) 
	y
	[Pharaoh Logging] [File] Reading File /etc/ssh/sshd_config
	PHP Notice:  Undefined index: searchline in /opt/ptconfigure/ptconfigure/src/Modules/File/Model/FileAllOS.php on line 175
	[Pharaoh Logging] [File] Reading File /etc/ssh/sshd_config
	[Pharaoh Logging] [File] Reading File /etc/ssh/sshd_config
	PHP Notice:  Undefined index: searchline in /opt/ptconfigure/ptconfigure/src/Modules/File/Model/FileAllOS.php on line 149
	[Pharaoh Logging] [File] Writing File /etc/ssh/sshd_config
	[Pharaoh Logging] /etc/ssh/sshd_config modified to disallow root ssh login
	[Pharaoh Logging] [File] Reading File /etc/ssh/sshd_config
	PHP Notice:  Undefined index: searchline in /opt/ptconfigure/ptconfigure/src/Modules/File/Model/FileAllOS.php on line 175
	[Pharaoh Logging] [File] Reading File /etc/ssh/sshd_config
	[Pharaoh Logging] [File] Reading File /etc/ssh/sshd_config
	PHP Notice:  Undefined index: searchline in /opt/ptconfigure/ptconfigure/src/Modules/File/Model/FileAllOS.php on line 149
	[Pharaoh Logging] [File] Writing File /etc/ssh/sshd_config
	[Pharaoh Logging] /etc/ssh/sshd_config modified to disallow password based ssh login
	[Pharaoh Logging] Restarting ssh service
	ssh stop/waiting
	ssh start/running, process 17375
	******************************


	SshHarden Modifications:
	--------------------------------------------

	Ssh Hardening: Success

	------------------------------
	SshHarden Mods Finished
	******************************

Beneficios
------------

* Este Ssh actos endurecen como un potenciador que permite las funciones de seguridad de las cuentas de usuarios de SSH.
* Los parámetros utilizados en ayuda y securifying, las operaciones de instalación no son sensibles, que es una ventaja añadida, mientras que en  comparación con otros.
* Este módulo permite la modificación de ssh config endurecen que prohíbe ssh root de usuario, contraseña basada ssh login.
