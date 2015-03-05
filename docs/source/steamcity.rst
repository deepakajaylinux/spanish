=================
Teamcity module
=================

sinopsis
------------

TeamCity es una gestión de construcción basada en Java y el servidor de integración continua. Este módulo tiene como objetivo instalar la última versión del servidor TeamCity y sus dependencias.

Ayuda Comando
--------------------

El comando de ayuda guía al usuario para proporcionar lo necesario para realizar la tarea. El comando para hacer uso de la ayuda debajo del terminal se da de la siguiente manera,

.. code-block:: bash

	ptconfigure Teamcity help

La instantánea de abajo te da una representación pictórica de comando de ayuda y aparece dos parámetros como TeamCity y TeamCity. (Los parámetros son mayúsculas y minúsculas)

.. code-block:: bash

	kevell@copy:/# ptconfigure teamcity help
	******************************


	This command allows you to install Teamcity, the popular Build Server.

	Teamcity, teamcity

        - install
        Installs Teamcity from the Jetbrains distributed native package
        example: ptconfigure teamcity install

	------------------------------
	End Help
	******************************

instalación
-------------

El comando que se utiliza para la instalación de módulo TeamCity se da a continuación,

.. code-block:: bash

	ptconfigure Teamcity install

La pantalla de abajo se explica cómo instalar el módulo TeamCity.

.. code-block:: bash


	kevell@corp:/# ptconfigure Teamcity install
	Install Teamcity? (Y/N) 
	y
	*******************************
	*        Pharaoh Tools        *
	*          ! Teamcity !        *
	*******************************
	PHP Notice:  Undefined index: version in /opt/ptconfigure/ptconfigure/src/Modules/Teamcity/Model/TeamcityUbuntu.php on line 42
	[Pharaoh Logging] Ensure module install is not checking versions
	[Pharaoh Logging] Module Java reports itself as Installed
	[Pharaoh Logging] Not installing as already installed
	Creating /tmp/ptconfigure-temp-script-82478215982.sh
	chmod 755 /tmp/ptconfigure-temp-script-82478215982.sh 2>/dev/null
	Changing /tmp/ptconfigure-temp-script-82478215982.sh Permissions
	Executing /tmp/ptconfigure-temp-script-82478215982.sh
	--2015-01-08 14:42:15--  http://download.jetbrains.com/teamcity/TeamCity-8.1.3.tar.gz
	Resolving download.jetbrains.com (download.jetbrains.com)... 54.217.236.18
	Connecting to download.jetbrains.com (download.jetbrains.com)|54.217.236.18|:80... connected.
	HTTP request sent, awaiting response... 302 Moved Temporarily
	Location: http://download-cf.jetbrains.com/teamcity/TeamCity-8.1.3.tar.gz [following]
	--2015-01-08 14:42:16--  http://download-cf.jetbrains.com/teamcity/TeamCity-8.1.3.tar.gz
	Resolving download-cf.jetbrains.com (download-cf.jetbrains.com)... 54.230.190.208, 54.230.190.220, 54.230.190.210, ...
	Connecting to download-cf.jetbrains.com (download-cf.jetbrains.com)|54.230.190.208|:80... connected.
	HTTP request sent, awaiting response... 200 OK
	Length: 551078596 (526M) [application/x-tar]
	Saving to: â€˜TeamCity-8.1.3.tar.gzâ€™
		
	 99% [                                                                                                   >  ] 60,46,771   63.3KB/s 	

Opciones
-----------

.. cssclass:: table-bordered

 +--------------------------+-------------------------+------------+-------------------------------------------------------+
 | Parámetros               | Parámetro Alternativa   | Opciones   | Comentarios                                           |
 +==========================+=========================+============+=======================================================+
 |Install Teamcity? (Y/N)   | Teamcity, teamcity      | Y(Yes)     | Si el usuario desea continuar el proceso de           |
 |                          |                         |            | instalación se puede introducir como Y.               |
 +--------------------------+-------------------------+------------+-------------------------------------------------------+
 |Install Teamcity? (Y/N)   | Teamcity, teamcity      | N(No)      | Si el usuario desea abandonar el proceso de           |
 |                          |                         |            | instalación se puede introducir como N.|              |
 +--------------------------+-------------------------+------------+-------------------------------------------------------+


Beneficios
---------------

* Instala todos los requisitos de apoyo para ejecutar el servidor TeamCity de manera eficiente
* Uso La facilidad de acceso y la instalación
* La codificación es sensible a mayúsculas.
