============
Git tools
============

sinopsis
------------

Gittools es un sistema de control distribuido de versiones con un énfasis en la rapidez, integridad de los datos, y soporte para flujos de trabajo distribuidas, no lineales.

Esta instalación de ascensor módulo en versión actualizada. Durante la instalación también puede instalar gitfrom, núcleo git, gitcole, gitfrom bajo ptconfigure. La automatización es posible. Es fácil de usar con Ubuntu y CentOS.

comando Ayuda
---------------------

Este comando ayuda a guiar al usuario sobre ptconfigure. Es menos tiempo, ya que puede instalarse automáticamente. Adecuado para todo tipo de usuario. El siguiente comando ayuda ayudará al usuario para la instalación gittools. Este argumento de línea de comandos especifica el nombre de la orden sobre la que la información se va a mostrar.

.. code-block:: bash

		ptconfigure gittools help

Después de escribir el comando que muestra el uso. La captura de pantalla puede expresar la función de este comando.

.. code-block:: bash

 kevell@corp:/# ptconfigure GitTools help
 ******************************


  This command allows you to install Git and a set of common Git Tools. These include
  Git - the distributed source control manager, git Core a supplement to Git, Gitk
  which is a GUI for git, and git-cola, which is also a Git GUI.

  GitTools, gittools, git-tools

        - install
        Installs the latest version of Git Tools
        example: ptconfigure gittools install

 ------------------------------
 End Help
 ******************************


instalación
----------------

    La instalación incluye la provisión de o conexión a los servicios necesarios para hacer que el equipo instalado listo para funcionar. Es un proceso de manifiesto para instalar módulo gittools bajo ptconfigure sólo por el uso de la orden dada a continuación,

.. code-block:: bash 

		ptconfigure gittools install

Después de vitalizar el comando se catequizar entrada.

La entrada del usuario como si automáticamente se instalará gittools con la comprobación del sistema. La siguiente captura de pantalla demuestra.

.. code-block:: bash

 kevell@corp:/# ptconfigure gittools install
 Install Git Tools? (Y/N)
 y
 *******************************
 *        Pharaoh Tools        *
 *         !Git Tools!!        *
 *******************************
 [Pharaoh Logging] Package git from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package git-core from the Packager Apt is already installed, so not installing
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following packages were automatically installed and are no longer required:
  linux-headers-generic linux-image-generic
 Use 'apt-get autoremove' to remove them.
 Suggested packages:
  git-doc
 The following NEW packages will be installed:
  gitk
 0 upgraded, 1 newly installed, 0 to remove and 299 not upgraded.
 Need to get 121 kB of archives.
 After this operation, 1,250 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main gitk all 1:1.9.1-1ubuntu0.1 [121 kB]
 Fetched 121 kB in 19s (6,077 B/s)
 Selecting previously unselected package gitk.
 (Reading database ... 176395 files and directories currently installed.)
 Preparing to unpack .../gitk_1%3a1.9.1-1ubuntu0.1_all.deb ...
 Unpacking gitk (1:1.9.1-1ubuntu0.1) ...
 Processing triggers for man-db (2.6.7.1-1) ...
 Setting up gitk (1:1.9.1-1ubuntu0.1) ...
 [Pharaoh Logging] Adding Package gitk from the Packager Apt executed correctly
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following packages were automatically installed and are no longer required:
  linux-headers-generic linux-image-generic
 Use 'apt-get autoremove' to remove them.
 The following extra packages will be installed:
  libjs-jquery libjs-underscore
 Suggested packages:
  python-pyinotify python-simplejson javascript-common
 Recommended packages:
  xxdiff
 The following NEW packages will be installed:
  git-cola libjs-jquery libjs-underscore
 0 upgraded, 3 newly installed, 0 to remove and 299 not upgraded.
 Need to get 363 kB of archives.
 After this operation, 1,886 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/main libjs-jquery all 1.7.2+dfsg-2ubuntu1 [78.8 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/main libjs-underscore all 1.4.4-2ubuntu1 [45.6 kB]
 Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty/universe git-cola all 1.9.3-1 [239 kB]
 Fetched 363 kB in 1min 3s (5,679 B/s)
 Selecting previously unselected package libjs-jquery.
 (Reading database ... 176413 files and directories currently installed.)
 Preparing to unpack .../libjs-jquery_1.7.2+dfsg-2ubuntu1_all.deb ...
 Unpacking libjs-jquery (1.7.2+dfsg-2ubuntu1) ...
 Selecting previously unselected package libjs-underscore.
 Preparing to unpack .../libjs-underscore_1.4.4-2ubuntu1_all.deb ...
 Unpacking libjs-underscore (1.4.4-2ubuntu1) ...
 Selecting previously unselected package git-cola.
 Preparing to unpack .../git-cola_1.9.3-1_all.deb ...
 Unpacking git-cola (1.9.3-1) ...
 Processing triggers for man-db (2.6.7.1-1) ...
 Processing triggers for gnome-menus (3.10.1-0ubuntu2) ...
 Processing triggers for desktop-file-utils (0.22-1ubuntu1) ...
 Processing triggers for bamfdaemon (0.5.1+14.04.20140409-0ubuntu1) ...
 Rebuilding /usr/share/applications/bamf-2.index...
 Processing triggers for mime-support (3.54ubuntu1) ...
 Setting up libjs-jquery (1.7.2+dfsg-2ubuntu1) ...
 Setting up libjs-underscore (1.4.4-2ubuntu1) ...
 Setting up git-cola (1.9.3-1) ...
 [Pharaoh Logging] Adding Package git-cola from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 GitTools: Success
 ------------------------------
 Installer Finished
 ******************************

El proceso de instalación rápidamente por los siguientes pasos,

Paso 1 Install gittools ?(Y/N)

Paso 2 Si el usuario da Y, el sistema puede comprobar la versión e instalarlo

Paso 3 Si el usuario da N, salir de la instalación.

Opciones
-------------

.. cssclass:: table-bordered


 +-----------------------------+--------------------------------------+-------------+--------------------------------------------+
 | Parámetros                  | Parámetro Alternativa                | Opciones    | Comentarios                                |
 +=============================+======================================+=============+============================================+
 |Install gittools?(Y/N)       | En lugar de utilizar gittools        | Y(Yes)      | Se instalará git y un conjunto de          |
 |                             | podemos utilizar GitTools,gittools,  |             | gittools comunes bajo ptconfigure.         |
 |                             | git-tools                            |             |                                            |
 +-----------------------------+--------------------------------------+-------------+--------------------------------------------+
 |Install gittools?(Y/N)       | En lugar de utilizar gittools        | N(No)       | La salida de sistema de la instalación     |
 |                             | podemos utilizar GitTools,gittools,  |             |                                            |
 |                             | git-tools|                           |             |                                            |
 +-----------------------------+--------------------------------------+-------------+--------------------------------------------+


Beneficios
--------------

* Gittools están asociados con flujos de trabajo complejos.
* Gittools hace granular comete más fácil que cualquier otro sistema de control de versiones (VCS), ya que el usuario puede determinar que cambia  exactamente será en el próximo commit.
* Gittools para mejorar el flujo de trabajo de codificación usuario.
* Git-cola es una herramienta avanzada de Git, similar a git-gui cometió.
* Git-cola cuenta con un visor gráfico, fácil, puesta en escena interactiva, apoyo inotify.
