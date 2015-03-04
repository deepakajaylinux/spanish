=============
PTVirtualize
=============

sinopsis
-----------

  ptvirtualize lograr gestionar el VirtualBox. Este módulo ayuda a instalar bajo ptconfigure. Directorio de datos y el directorio albacea puede especificar durante la instalación de este módulo. Este módulo es el más cómodo con Ubuntu y CentOS.

comando Ayuda
--------------------

Este comando ayuda a guiar al usuario sobre el módulo ptvirtualize. Esto es adecuado para todo tipo de personas de negocios. El comando help muestra una breve lista de los comandos integrados en el módulo ptvirtualize.

.. code-block:: bash

	Kevell@corp:/# ptconfigure ptvirtualize help
	******************************


	This command allows you to install or update ptvirtualize.

	ptvirtualize, ptvirtualize

        - install
        Installs the latest version of ptvirtualize
        example: ptconfigure ptvirtualize install

	------------------------------
	End Help
	******************************

instalación
------------

La instalación de un módulo ptvirtualize es incluyendo controladores de dispositivos y plugins, acto de hacer el programa listo para su ejecución. Durante la instalación de este módulo se aprobó el siguiente comando.

.. code-block:: bash

	ptconfigure ptvirtualize install

Después introduce el comando, el sistema puede pedir

Install ptvirtualize?(Y/N)

Si el usuario da Y entonces ptvirtualize se instalarán. La siguiente captura de pantalla demuestran.

.. code-block:: bash

	Kevell@corp:/# ptconfigure ptvirtualize install
	Install ptvirtualize ? (Y/N) 
	y
	*******************************
	*        Pharaoh Tools        *
	*          ptvirtualize         *
	*******************************
	What is the program data directory? Found "/opt/ptvirtualize" - use this? (Enter nothing for yes, no end slash)

	What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

	git clone 'https://github.com/PharaohTools/ptvirtualize.git'  /tmp/ptvirtualize/ptvirtualizeCloning into '/tmp/ptvirtualize/ptvirtualize'...
	remote: Counting objects: 4063, done.
	remote: Total 4063 (delta 0), reused 0 (delta 0)
	Receiving objects: 100% (4063/4063), 2.13 MiB | 393.00 KiB/s, done.
	Resolving deltas: 100% (2530/2530), done.
	Checking connectivity... done.
	Program Data folder populated
	Program Executor Deleted if existed
	... All done!
	*******************************
	Thanks for installing , visit www.pharaohtools.com for more
	******************************
	
	
	Single App Installer:
	--------------------------------------------
	ptvirtualize: Success
	------------------------------
	Installer Finished
	******************************

Si el usuario da N entonces saldrá de la pantalla. La siguiente captura de pantalla demuestran.

.. code-block:: bash

	kevells@corp:/# ptconfigure ptvirtualize install
	Install ptvirtualize ? (Y/N) 
	n
	******************************


	Single App Installer:
	--------------------------------------------
	ptvirtualize: Failure
	------------------------------
	Installer Finished
	******************************


opción
-----------
.. cssclass:: table-bordered


 +----------------------------+-------------------------------+-----------+-----------------------------------------------------+
 | Parámetros                 | camino                        | Opciones  | Comentarios                                         |
 +============================+===============================+===========+=====================================================+
 |Program data directory      | “/opt/ptvirtualize”           | Yes       | Se instalará ptvirtualize bajo ptconfigure          | 
 |(Por defecto)               |                               |           |                                                     |
 +----------------------------+-------------------------------+-----------+-----------------------------------------------------+
 |Program data directory      | No (End slash)                | No        | El usuario tiene a un especifique la ruta.          |
 +----------------------------+-------------------------------+-----------+-----------------------------------------------------+
 |Program executor directory  | “/usr/bin”                    | Yes       | Se instalará directorio ejecutor                    |
 |(Por defecto)               |                               |           |                                                     |
 +----------------------------+-------------------------------+-----------+-----------------------------------------------------+
 |Program executor directory  | No (End slash)                | No        | El usuario da entrada como nombre del directorio|   |
 +----------------------------+-------------------------------+-----------+-----------------------------------------------------+


Beneficios
----------

* Los usuarios de Ubuntu pueden instalar simplemente ptvirtualize del repositorio.
* La ventaja real de ptvirtualize radica en su rendimiento.
* Integración con Host OS.
* Accesibilidad velocidad.
* Gestión de caja virtual.

