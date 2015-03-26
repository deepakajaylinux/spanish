============
Docker
============


sinopsis
----------

Anclaje es una plataforma abierta para aplicaciones distribuidas para los desarrolladores y administradores de sistemas. Anclaje es una herramienta que puede empaquetar una aplicación y sus dependencias en un contenedor virtual que se puede ejecutar en cualquier servidor de Linux.
	
Se compone de anclaje del motor, un portátil. runtime ligero y herramienta de empaquetado. y Docker Hub, una nube de servicio para compartir aplicaciones y automatizar flujos de trabajo, Docker permite aplicaciones ser rápidamente ensamblado de componentes y elimina la fricción entre el desarrollo, QA y entornos de producción.


comando Ayuda
--------------

El comando ayuda guía a los usuarios sobre la finalidad y así como sobre las opciones que se incluyen en el módulo de estibador. Enumera los parámetros alternativos del módulo de estibador. También describe la sintaxis para instalar el módulo de estibador. El comando de ayuda para el módulo de anclaje se muestra a continuación.


.. code-block:: bash

	ptconfigure Docker help

La representación pictórica del comando anterior se enumera a continuación,

.. code-block:: bash


 kevell@corp:/# ptconfigure Docker help
 ******************************


  This command allows you to update Docker.

  Docker, docker

        - install
        Installs the latest version of Docker
        example: ptconfigure docker install

 ------------------------------
 End Help
 ******************************

Instalación
--------------


El comando utilizado para instalar el módulo de estibador en el terminal se enumera a continuación,

.. code-block:: bash

	ptconfigure docker install


El comando anterior pretende instalar la última versión de anclaje y sus dependencias. La representación pictórica del comando anterior se enumera a continuación,

.. code-block:: bash

 kevell@corp:/# ptconfigure docker install
 Install Docker? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Docker!        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-81737981568.sh
 chmod 755 /tmp/ptconfigure-temp-script-81737981568.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-81737981568.sh Permissions
 Executing /tmp/ptconfigure-temp-script-81737981568.sh
 Ign http://security.ubuntu.com trusty-security InRelease
 Ign http://ppa.launchpad.net trusty InRelease
 Ign http://extras.ubuntu.com trusty InRelease
 Ign http://packages.elasticsearch.org stable InRelease
 Ign http://in.archive.ubuntu.com trusty InRelease
 Get:1 http://security.ubuntu.com trusty-security Release.gpg [933 B]
 Hit http://ppa.launchpad.net trusty Release.gpg
 Hit http://packages.elasticsearch.org stable Release.gpg
 Get:2 http://extras.ubuntu.com trusty Release.gpg [72 B]
 Ign http://in.archive.ubuntu.com trusty-updates InRelease
 Get:3 http://security.ubuntu.com trusty-security Release [62.0 kB]
 Hit http://ppa.launchpad.net trusty Release
 Hit http://packages.elasticsearch.org stable Release
 Hit http://extras.ubuntu.com trusty Release
 Ign http://in.archive.ubuntu.com trusty-backports InRelease
 Hit http://ppa.launchpad.net trusty/main amd64 Packages
 Hit http://packages.elasticsearch.org stable/main amd64 Packages
 Hit http://extras.ubuntu.com trusty/main Sources
 Hit http://in.archive.ubuntu.com trusty Release.gpg
 Hit http://ppa.launchpad.net trusty/main i386 Packages
 Hit http://packages.elasticsearch.org stable/main i386 Packages
 Hit http://ppa.launchpad.net trusty/main Translation-en
 Hit http://extras.ubuntu.com trusty/main amd64 Packages
 Get:4 http://in.archive.ubuntu.com trusty-updates Release.gpg [933 B]
 Hit http://extras.ubuntu.com trusty/main i386 Packages
 Hit http://in.archive.ubuntu.com trusty-backports Release.gpg
 Hit http://in.archive.ubuntu.com trusty Release
 Get:5 http://in.archive.ubuntu.com trusty-updates Release [62.0 kB]
 Get:6 http://security.ubuntu.com trusty-security/main Sources [72.5 kB]
 Ign http://packages.elasticsearch.org stable/main Translation-en_IN
 Ign http://packages.elasticsearch.org stable/main Translation-en
 Ign http://extras.ubuntu.com trusty/main Translation-en_IN
 Ign http://extras.ubuntu.com trusty/main Translation-en
 Hit http://in.archive.ubuntu.com trusty-backports Release
 Hit http://in.archive.ubuntu.com trusty/main Sources
 Hit http://in.archive.ubuntu.com trusty/restricted Sources
 Hit http://in.archive.ubuntu.com trusty/universe Sources
 Hit http://in.archive.ubuntu.com trusty/multiverse Sources
 Hit http://in.archive.ubuntu.com trusty/main amd64 Packages
 Hit http://in.archive.ubuntu.com trusty/restricted amd64 Packages
 Hit http://in.archive.ubuntu.com trusty/universe amd64 Packages
 Get:7 http://security.ubuntu.com trusty-security/restricted Sources [2,061 B]
 Hit http://in.archive.ubuntu.com trusty/multiverse amd64 Packages
 Get:8 http://security.ubuntu.com trusty-security/universe Sources [17.9 kB]
 Hit http://in.archive.ubuntu.com trusty/main i386 Packages
 Hit http://in.archive.ubuntu.com trusty/restricted i386 Packages
 Get:9 http://security.ubuntu.com trusty-security/multiverse Sources [1,905 B]
 Get:10 http://security.ubuntu.com trusty-security/main amd64 Packages [222 kB]
 Hit http://in.archive.ubuntu.com trusty/universe i386 Packages
 Hit http://in.archive.ubuntu.com trusty/multiverse i386 Packages
 Hit http://in.archive.ubuntu.com trusty/main Translation-en
 Hit http://in.archive.ubuntu.com trusty/multiverse Translation-en
 Hit http://in.archive.ubuntu.com trusty/restricted Translation-en
 Hit http://in.archive.ubuntu.com trusty/universe Translation-en
 Get:11 http://in.archive.ubuntu.com trusty-updates/main Sources [184 kB]
 Get:12 http://security.ubuntu.com trusty-security/restricted amd64 Packages [8,875 B]
 Get:13 http://security.ubuntu.com trusty-security/universe amd64 Packages [88.1 kB]
 Get:14 http://security.ubuntu.com trusty-security/multiverse amd64 Packages [3,459 B]
 Get:15 http://security.ubuntu.com trusty-security/main i386 Packages [212 kB]
 Get:16 http://in.archive.ubuntu.com trusty-updates/restricted Sources [2,564 B]
 Get:17 http://in.archive.ubuntu.com trusty-updates/universe Sources [107 kB]
 Get:18 http://in.archive.ubuntu.com trusty-updates/multiverse Sources [4,484 B]
 Get:19 http://in.archive.ubuntu.com trusty-updates/main amd64 Packages [454 kB]
 Get:20 http://security.ubuntu.com trusty-security/restricted i386 Packages [8,846 B]
 Get:21 http://security.ubuntu.com trusty-security/universe i386 Packages [88.1 kB]
 Get:22 http://security.ubuntu.com trusty-security/multiverse i386 Packages [3,628 B]
 Hit http://security.ubuntu.com trusty-security/main Translation-en
 Hit http://security.ubuntu.com trusty-security/multiverse Translation-en
 Hit http://security.ubuntu.com trusty-security/restricted Translation-en
 Hit http://security.ubuntu.com trusty-security/universe Translation-en
 Get:23 http://in.archive.ubuntu.com trusty-updates/restricted amd64 Packages [9,238 B]
 Get:24 http://in.archive.ubuntu.com trusty-updates/universe amd64 Packages [259 kB]
 Get:25 http://in.archive.ubuntu.com trusty-updates/multiverse amd64 Packages [11.2 kB]
 Get:26 http://in.archive.ubuntu.com trusty-updates/main i386 Packages [444 kB]
 Get:27 http://in.archive.ubuntu.com trusty-updates/restricted i386 Packages [9,256 B]
 Get:28 http://in.archive.ubuntu.com trusty-updates/universe i386 Packages [260 kB]
 Get:29 http://in.archive.ubuntu.com trusty-updates/multiverse i386 Packages [11.3 kB]
 Hit http://in.archive.ubuntu.com trusty-updates/main Translation-en
 Hit http://in.archive.ubuntu.com trusty-updates/multiverse Translation-en
 Hit http://in.archive.ubuntu.com trusty-updates/restricted Translation-en
 Hit http://in.archive.ubuntu.com trusty-updates/universe Translation-en
 Hit http://in.archive.ubuntu.com trusty-backports/main Sources
 Hit http://in.archive.ubuntu.com trusty-backports/restricted Sources
 Hit http://in.archive.ubuntu.com trusty-backports/universe Sources
 Hit http://in.archive.ubuntu.com trusty-backports/multiverse Sources
 Hit http://in.archive.ubuntu.com trusty-backports/main amd64 Packages
 Hit http://in.archive.ubuntu.com trusty-backports/restricted amd64 Packages
 Hit http://in.archive.ubuntu.com trusty-backports/universe amd64 Packages
 Hit http://in.archive.ubuntu.com trusty-backports/multiverse amd64 Packages
 Hit http://in.archive.ubuntu.com trusty-backports/main i386 Packages
 Hit http://in.archive.ubuntu.com trusty-backports/restricted i386 Packages
 Hit http://in.archive.ubuntu.com trusty-backports/universe i386 Packages
 Hit http://in.archive.ubuntu.com trusty-backports/multiverse i386 Packages
 Hit http://in.archive.ubuntu.com trusty-backports/main Translation-en
 Hit http://in.archive.ubuntu.com trusty-backports/multiverse Translation-en
 Hit http://in.archive.ubuntu.com trusty-backports/restricted Translation-en
 Hit http://in.archive.ubuntu.com trusty-backports/universe Translation-en
 Ign http://in.archive.ubuntu.com trusty/main Translation-en_IN
 Ign http://in.archive.ubuntu.com trusty/multiverse Translation-en_IN
 Ign http://in.archive.ubuntu.com trusty/restricted Translation-en_IN
 Ign http://in.archive.ubuntu.com trusty/universe Translation-en_IN
 Fetched 2,610 kB in 1min 31s (28.5 kB/s)
 Reading package lists...
 Temp File /tmp/ptconfigure-temp-script-81737981568.sh Removed
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  aufs-tools cgroup-lite
 Suggested packages:
  btrfs-tools debootstrap lxc rinse
 The following NEW packages will be installed:
  aufs-tools cgroup-lite docker.io
 0 upgraded, 3 newly installed, 0 to remove and 181 not upgraded.
 Need to get 4,207 kB of archives.
 After this operation, 25.0 MB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/universe aufs-tools amd64 1:3.2+20130722-1.1 [92.3 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/universe docker.io amd64 1.0.1~dfsg1-0ubuntu1~ubuntu0.14.04.1 [4,111 kB]
 Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty/main cgroup-lite all 1.9 [3,918 B]
 Fetched 4,207 kB in 47s (89.1 kB/s)
 Selecting previously unselected package aufs-tools.
 (Reading database ... 195553 files and directories currently installed.)
 Preparing to unpack .../aufs-tools_1%3a3.2+20130722-1.1_amd64.deb ...
 Unpacking aufs-tools (1:3.2+20130722-1.1) ...
 Selecting previously unselected package docker.io.
 Preparing to unpack .../docker.io_1.0.1~dfsg1-0ubuntu1~ubuntu0.14.04.1_amd64.deb ...
 Unpacking docker.io (1.0.1~dfsg1-0ubuntu1~ubuntu0.14.04.1) ...
 Selecting previously unselected package cgroup-lite.
 Preparing to unpack .../cgroup-lite_1.9_all.deb ...
 Unpacking cgroup-lite (1.9) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Processing triggers for ureadahead (0.100.0-16) ...
 ureadahead will be reprofiled on next reboot
 Setting up aufs-tools (1:3.2+20130722-1.1) ...
 Setting up docker.io (1.0.1~dfsg1-0ubuntu1~ubuntu0.14.04.1) ...
 Adding group `docker' (GID 139) ...
 Done.
 docker.io start/running, process 4357
 Setting up cgroup-lite (1.9) ...
 cgroup-lite start/running
 Processing triggers for libc-bin (2.19-0ubuntu6.5) ...
 Processing triggers for ureadahead (0.100.0-16) ...
 [Pharaoh Logging] Adding Package docker.io from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Docker: Success
 ------------------------------
 Installer Finished
 ******************************


La desinstalación
--------------------


El comando utilizado para desinstalar el módulo de estibador en el terminal se enumera a continuación,

.. code-block:: bash

        ptconfigure docker uninstall

La representación pictórica del comando anterior se enumera a continuación,

.. code-block:: bash


 kevell@corp:/# ptconfigure docker uninstall
 Uninstall Docker? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Docker!        *
 *******************************
 [Pharaoh Logging] Removing Package docker.io
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following packages were automatically installed and are no longer required:
  aufs-tools cgroup-lite
 Use 'apt-get autoremove' to remove them.
 The following packages will be REMOVED:
  docker.io
 0 upgraded, 0 newly installed, 1 to remove and 181 not upgraded.
 After this operation, 24.7 MB disk space will be freed.
 (Reading database ... 195665 files and directories currently installed.)
 Removing docker.io (1.0.1~dfsg1-0ubuntu1~ubuntu0.14.04.1) ...
 docker.io stop/waiting
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 [Pharaoh Logging] Removed Package docker.io from the Packager Apt
 ... All done!
 *******************************
 Thanks for uninstalling , visit www.pharaohtools.com for more
 ******************************


 Single App Uninstaller:
 ------------------------------
 Docker: Success
 ------------------------------
 UnInstaller Finished
 ******************************




parámetros alternativos
-------------------------

Hay dos parámetros alternativos que pueden utilizarse en la línea de comandos.

Docker, docker



Beneficios
-------------

Docker trae una API para manejo de contenedores, un formato de imagen y la posibilidad de usar un registro remoto para el intercambio de envases. Este esquema beneficia tanto los desarrolladores y administradores del sistema con ventajas tales como:

Despliegue rápido de aplicaciones – contenedores incluyen los requisitos mínimo tiempo de ejecución de la aplicación, reduciendo su tamaño y permitirles desplegarse rápidamente.

Portabilidad a través de máquinas – una aplicación y todas sus dependencias pueden ser incluidos en un único contenedor que es independiente de la versión de host del kernel Linux, distribución multiplataforma o modelo de implementación. Este contenedor puede transferirse a otro equipo que ejecuta Docker y ejecutados sin problemas de compatibilidad.

Control de versiones y reutilizar – componente puede rastrear las sucesivas versiones de un contenedor, inspeccione las diferencias o regresión a las versiones anteriores. Contenedores reutilización componentes de las capas anteriores, lo cual los hace perceptiblemente ligero.

Compartir – puede usar un repositorio remoto para compartir el contenedor con los demás. Red Hat proporciona un registro para este propósito, y también es posible configurar su propio repositorio privado.

Ligera huella y sobrecarga mínima – Docker imágenes son generalmente muy pequeños, que facilita la entrega rápida y reduce el tiempo de desplegar nuevos contenedores de aplicación.
Mantenimiento simplificado – Docker reduce el esfuerzo y el riesgo de problemas con dependencias de las aplicaciones.



