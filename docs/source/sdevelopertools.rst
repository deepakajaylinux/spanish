=================
DeveloperTools
=================

sinopsis
----------
El módulo devtools hace la instalación mucho más fácil para crear un paquete siguiendo la estructura definida en los Devtools. También hace que sea más fácil para poner a prueba su paquete, a través del editor. Este módulo en un envase que tiene una excelente idea: no sólo hace que el paquete de usuario más fiable en el largo plazo, sino que también simplifica el proceso de desarrollo en forma sorprendente. Esto es conveniente en Ubuntu y CentOS.

comando Ayuda
----------------------
Devtools hace que el desarrollo conjunto de una brisa: se trabaja con las convenciones existentes para la estructura del código, añadiendo herramientas eficaces para apoyar el ciclo de desarrollo de paquetes. Con devtools, el desarrollo de un paquete llega a ser tan fácil que será el diseño predeterminado de usuario cada vez que el usuario está escribiendo una cantidad significativa de código.

.. code-block:: bash

                cleopatra devtools help

La siguiente captura de pantalla y lo explica.

.. code-block:: bash

 kevell@corp:/# cleopatra devtools help
 ******************************


  This command allows you to install a set of Developer Tools. These include
  Geany IDE, Bluefish IDE, Kompozer IDE and Emma DB Manager.

  DeveloperTools, devtools, dev-tools

        - install
        Installs the latest version of Developer Tools
        example: cleopatra devtools install

 ------------------------------
 End Help
 ******************************


instalación
--------------

    La instalación incluye la provisión de o conexión a los servicios necesarios para hacer que el equipo instalado listo para funcionar. Es un proceso de manifiesto para instalar módulo devtools bajo Cleopatra simplemente usando la orden dada a continuación,

.. code-block:: bash

 cleopatra devtools install

Después de vitalizar el comando se catequizar entrada.
Cuando la entrada de usuario como si automáticamente se istall devtools con la comprobación del sistema. Si no salir de la instalación. la siguiente captura de pantalla demuestra.

.. code-block:: bash


 kevell@corp:/$ cleopatra devtools install
 Install Developer Tools? (Y/N)
 y
 *******************************
 *        Pharaoh Tools        *
 *         Devel Tools!        *
 *******************************

 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  geany-common
 Suggested packages:
  libvte9
 The following NEW packages will be installed:
  geany geany-common
 0 upgraded, 2 newly installed, 0 to remove and 301 not upgraded.
 Need to get 3,808 kB of archives.
 After this operation, 9,872 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/universe geany-common all 1.23.1+dfsg-1 [2,709 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/universe geany amd64 1.23.1+dfsg-1 [1,100 kB]
 Fetched 3,808 kB in 4min 54s (12.9 kB/s)
 Selecting previously unselected package geany-common.
 (Reading database ... 182047 files and directories currently installed.)
 Preparing to unpack .../geany-common_1.23.1+dfsg-1_all.deb ...
 Unpacking geany-common (1.23.1+dfsg-1) ...
 Selecting previously unselected package geany.
 Preparing to unpack .../geany_1.23.1+dfsg-1_amd64.deb ...
 Unpacking geany (1.23.1+dfsg-1) ...
 Processing triggers for doc-base (0.10.5) ...
 Processing 1 added doc-base file...
 Processing triggers for hicolor-icon-theme (0.13-1) ...
 Processing triggers for gnome-menus (3.10.1-0ubuntu2) ...
 Processing triggers for desktop-file-utils (0.22-1ubuntu1) ...
 Processing triggers for bamfdaemon (0.5.1+14.04.20140409-0ubuntu1) ...
 Rebuilding /usr/share/applications/bamf-2.index...
 Processing triggers for mime-support (3.54ubuntu1) ...
 Processing triggers for man-db (2.6.7.1-1) ...
 Setting up geany-common (1.23.1+dfsg-1) ...
 Setting up geany (1.23.1+dfsg-1) ...
 Preparing to unpack .../bluefish-data_2.2.5-1_all.deb ...
 Unpacking bluefish-data (2.2.5-1) ...
 Selecting previously unselected package bluefish-plugins.
 Preparing to unpack .../bluefish-plugins_2.2.5-1_amd64.deb ...
 Unpacking bluefish-plugins (2.2.5-1) ...
 Selecting previously unselected package bluefish.
 Preparing to unpack .../bluefish_2.2.5-1_amd64.deb ...
 Unpacking bluefish (2.2.5-1) ...
 Processing triggers for hicolor-icon-theme (0.13-1) ...
 Processing triggers for shared-mime-info (1.2-0ubuntu3) ...
 Processing triggers for man-db (2.6.7.1-1) ...
 Processing triggers for gnome-menus (3.10.1-0ubuntu2) ...
 Processing triggers for desktop-file-utils (0.22-1ubuntu1) ...
 Processing triggers for bamfdaemon (0.5.1+14.04.20140409-0ubuntu1) ...
 Rebuilding /usr/share/applications/bamf-2.index...
 Processing triggers for mime-support (3.54ubuntu1) ...
 Setting up bluefish-data (2.2.5-1) ...
 Setting up bluefish-plugins (2.2.5-1) ...
 Setting up bluefish (2.2.5-1) ...
 [Pharaoh Logging] Adding Package bluefish from the Packager Apt executed correctly
 PHP Warning:  file_put_contents(/opt/cleopatra/cleopatra/src/Modules/CleopatraRequired/Model/../../../cleovars): failed to open stream: Permission denied in /opt/cleopatra/cleopatra/src/Modules/CleopatraRequired/Model/AppConfig.php on line 115
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 DeveloperTools: Success
 ------------------------------
 Installer Finished
 ******************************

Opciones
-------------
.. cssclass:: table-bordered


 +-------------------------+-------------------------------------+-------------+-----------------------------------------+
 | Parámetros              | alternativos de parámetros          | Opción      | Comentarios                             |
 +=========================+=====================================+=============+=========================================+
 |Install devtools?(Y/N)   | En lugar de utilizar devtools       | Y           | Se instalará editor de base de          |
 |                         | podemos utilizar DeveloperTools,    |             | datos y devtools bajo cleopatra         |
 |                         | DevTools, dev-tools                 |             |                                         |
 +-------------------------+-------------------------------------+-------------+-----------------------------------------+
 |Install devtools?(Y/N)   | En lugar de utilizar devtools       | N           | La salida de sistema de la instalación  |
 |                         | podemos utilizar DeveloperTools,    |             |                                         |
 |                         | DevTools, dev-tools|                |             |                                         |
 +-------------------------+-------------------------------------+-------------+-----------------------------------------+

Beneficios
-------------

* Facilitar el proceso de desarrollo de paquetes
* Ayuda a liberar su paquete en el medio natural
* Que sea fácil de instalar y editor de base de datos.
* Depuración rápida
* On-the-Fly Estilo Cambios - para los cambios de estilo rápidas, el usuario ni siquiera necesita usar un editor de texto. El usuario puede 
  inspeccionar el particular  elemento de la página para determinar que se están aplicando estilos.

