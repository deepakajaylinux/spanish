======
Redis
======

sinopsis
----------------

Redis es un servidor de estructura de datos. En redis, en red, en memoria, y almacena las claves con durabilidad opcional. Redis es el almacén de claves y valores más popular. El nombre Redis medios remotos diccionario servidor. Redis soporta la replicación maestro-esclavo. Los datos de cualquier servidor Redis pueden replicar a cualquier número de esclavos. Esto permite Redis implementar un árbol de replicación sola raíz. Estos servicios manejar la instalación, configuración y mantenimiento de Redis en nombre del propietario de la aplicación. Este servicio le ofrece con Ubuntu y CentOS.

comando Ayuda
------------------------

El comando de ayuda conduce a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en el módulo redis. Las listas de comandos de ayuda fuera de los parámetros alternativos de redis bajo módulo ptconfigure. También describe la sintaxis para inicializar la máquina del usuario. El comando de ayuda para redis se muestra a continuación.

.. code-block:: bash

		ptconfigure redis help

La representación gráfica de la orden anterior se enumeran a continuación,

.. code-block:: bash

 kevell@corp:/# ptconfigure Redis help
 
 ******************************

 This command allows you to update Redis.
 
 Redis, redis

 - install
  Installs the latest version of redis
  example: ptconfigure redis install

 ------------------------------
 End Help
 ******************************

instalación
-----------------

La instalación de un módulo phlagrant es incluyendo controladores de dispositivos y plugins, acto de hacer el programa listo para su ejecución. Durante la instalación de este módulo se aprobó el siguiente comando.

.. code-block:: bash

 ptconfigure Phlagrant install

Después introduce el comando, el sistema puede pedir

Install Phlagrant? (Y/N)

Si el usuario da Y entonces se instalará Phlagrant. La siguiente captura de pantalla demuestran.

.. code-block:: bash


 kevell@corp:/# ptconfigure redis install

 Install Redis? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Redis!        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-45324388247.sh
 chmod 755 /tmp/ptconfigure-temp-script-45324388247.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-45324388247.sh Permissions
 Executing /tmp/ptconfigure-temp-script-45324388247.sh 

 deb-src http://packages.dotdeb.org squeeze all
 OK
 Ign http://dl.google.com stable InRelease
 Hit http://dl.google.com stable Release.gpg
 Hit http://dl.google.com stable Release
 Hit http://dl.google.com stable/main amd64 Packages
 Ign http://ppa.launchpad.net trusty InRelease
 Ign http://packages.dotdeb.org squeeze InRelease
 Ign http://extras.ubuntu.com trusty InRelease
 Ign http://security.ubuntu.com trusty-security InRelease
 Hit http://dl.google.com stable/main i386 Packages
 Ign http://ppa.launchpad.net trusty InRelease
 Ign http://in.archive.ubuntu.com trusty InRelease
 Ign http://wireframesketcher.com  InRelease
 Get:1 http://packages.dotdeb.org squeeze Release.gpg [836 B]
 Get:2 http://extras.ubuntu.com trusty Release.gpg [72 B]
 Hit http://security.ubuntu.com trusty-security Release.gpg
 Hit http://ppa.launchpad.net trusty Release.gpg
 Get:3 http://packages.dotdeb.org squeeze Release [2,287 B]
 Hit http://wireframesketcher.com  Release.gpg
 Ign http://in.archive.ubuntu.com trusty-updates InRelease
 Hit http://ppa.launchpad.net trusty Release.gpg
 Hit http://extras.ubuntu.com trusty Release
 Hit http://security.ubuntu.com trusty-security Release
 Get:4 http://packages.dotdeb.org squeeze/all amd64 Packages [20.6 kB]
 Hit http://wireframesketcher.com  Release
 Ign http://dl.google.com stable/main Translation-en_IN
 Ign http://in.archive.ubuntu.com trusty-backports InRelease
 Ign http://dl.google.com stable/main Translation-en
 Hit http://ppa.launchpad.net trusty Release
 Hit http://extras.ubuntu.com trusty/main Sources
 Hit http://wireframesketcher.com  Packages
 Hit http://security.ubuntu.com trusty-security/main Sources
 Hit http://ppa.launchpad.net trusty Release
 Hit http://in.archive.ubuntu.com trusty Release.gpg
 Hit http://extras.ubuntu.com trusty/main amd64 Packages
 Hit http://ppa.launchpad.net trusty/main amd64 Packages
 Hit http://security.ubuntu.com trusty-security/restricted Sources
 Get:5 http://in.archive.ubuntu.com trusty-updates Release.gpg [933 B]
 Get:6 http://packages.dotdeb.org squeeze/all i386 Packages [20.6 kB]
 Hit http://ppa.launchpad.net trusty/main i386 Packages
 Hit http://extras.ubuntu.com trusty/main i386 Packages
 Hit http://security.ubuntu.com trusty-security/universe Sources
 Hit http://in.archive.ubuntu.com trusty-backports Release.gpg
 Hit http://ppa.launchpad.net trusty/main Translation-en
 Hit http://security.ubuntu.com trusty-security/multiverse Sources
 Hit http://ppa.launchpad.net trusty/main amd64 Packages
 Hit http://in.archive.ubuntu.com trusty Release
 Hit http://ppa.launchpad.net trusty/main i386 Packages
 Hit http://security.ubuntu.com trusty-security/main amd64 Packages
 Get:7 http://in.archive.ubuntu.com trusty-updates Release [63.5 kB]
 Hit http://ppa.launchpad.net trusty/main Translation-en
 Hit http://security.ubuntu.com trusty-security/restricted amd64 Packages
 Hit http://security.ubuntu.com trusty-security/universe amd64 Packages
 Hit http://security.ubuntu.com trusty-security/multiverse amd64 Packages
 Ign http://wireframesketcher.com  Translation-en_IN
 Hit http://security.ubuntu.com trusty-security/main i386 Packages
 Ign http://wireframesketcher.com  Translation-en
 Hit http://security.ubuntu.com trusty-security/restricted i386 Packages
 Hit http://in.archive.ubuntu.com trusty-backports Release
 Hit http://security.ubuntu.com trusty-security/universe i386 Packages
 Ign http://packages.dotdeb.org squeeze/all Translation-en_IN
 Hit http://in.archive.ubuntu.com trusty/main Sources
 Ign http://extras.ubuntu.com trusty/main Translation-en_IN
 Ign http://packages.dotdeb.org squeeze/all Translation-en
 Hit http://security.ubuntu.com trusty-security/multiverse i386 Packages
 Hit http://in.archive.ubuntu.com trusty/restricted Sources
 Ign http://extras.ubuntu.com trusty/main Translation-en
 Hit http://security.ubuntu.com trusty-security/main Translation-en
 Hit http://in.archive.ubuntu.com trusty/universe Sources
 Hit http://security.ubuntu.com trusty-security/multiverse Translation-en
 Hit http://in.archive.ubuntu.com trusty/multiverse Sources
 Hit http://security.ubuntu.com trusty-security/restricted Translation-en
 Hit http://in.archive.ubuntu.com trusty/main amd64 Packages
 Hit http://in.archive.ubuntu.com trusty/restricted amd64 Packages
 Hit http://security.ubuntu.com trusty-security/universe Translation-en
 Hit http://in.archive.ubuntu.com trusty/universe amd64 Packages
 Hit http://in.archive.ubuntu.com trusty/multiverse amd64 Packages
 Hit http://in.archive.ubuntu.com trusty/main i386 Packages
 Hit http://in.archive.ubuntu.com trusty/restricted i386 Packages
 Hit http://in.archive.ubuntu.com trusty/universe i386 Packages
 Hit http://in.archive.ubuntu.com trusty/multiverse i386 Packages
 Hit http://in.archive.ubuntu.com trusty/main Translation-en
 Hit http://in.archive.ubuntu.com trusty/multiverse Translation-en
 Hit http://in.archive.ubuntu.com trusty/restricted Translation-en
 Hit http://in.archive.ubuntu.com trusty/universe Translation-en
 Get:8 http://in.archive.ubuntu.com trusty-updates/main Sources [189 kB]
 Get:9 http://in.archive.ubuntu.com trusty-updates/restricted Sources [2,564 B]
 Get:10 http://in.archive.ubuntu.com trusty-updates/universe Sources [107 kB]
 Get:11 http://in.archive.ubuntu.com trusty-updates/multiverse Sources [4,765 B]
 Get:12 http://in.archive.ubuntu.com trusty-updates/main amd64 Packages [488 kB]
 Get:13 http://in.archive.ubuntu.com trusty-updates/restricted amd64 Packages [9,238 B]
 Get:14 http://in.archive.ubuntu.com trusty-updates/universe amd64 Packages [261 kB]
 Get:15 http://in.archive.ubuntu.com trusty-updates/multiverse amd64 Packages [11.7 kB]
 Get:16 http://in.archive.ubuntu.com trusty-updates/main i386 Packages [477 kB]
 Get:17 http://in.archive.ubuntu.com trusty-updates/restricted i386 Packages [9,256 B]
 Get:18 http://in.archive.ubuntu.com trusty-updates/universe i386 Packages [261 kB]
 Get:19 http://in.archive.ubuntu.com trusty-updates/multiverse i386 Packages [11.9 kB]
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
 Fetched 1,941 kB in 1min 6s (29.3 kB/s)
 Reading package lists...
 Temp File /tmp/ptconfigure-temp-script-45324388247.sh Removed
 adduser: Warning: The home directory `/var/lib/redis' does not belong to the user you are currently creating.
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
   redis-tools
 The following NEW packages will be installed:
   redis-server redis-tools
 0 upgraded, 2 newly installed, 0 to remove and 363 not upgraded.
 Need to get 769 kB of archives.
 After this operation, 1,693 kB of additional disk space will be used.
 Get:1 http://packages.dotdeb.org/ squeeze/all redis-tools amd64 2:2.8.19-1~dotdeb.0 [315 kB]
 Get:2 http://packages.dotdeb.org/ squeeze/all redis-server amd64 2:2.8.19-1~dotdeb.0 [454 kB]
 Fetched 769 kB in 11s (65.4 kB/s)
 Selecting previously unselected package redis-tools.
 (Reading database ... 175243 files and directories currently installed.)
 Preparing to unpack .../redis-tools_2%3a2.8.19-1~dotdeb.0_amd64.deb ...
 Unpacking redis-tools (2:2.8.19-1~dotdeb.0) ...
 Selecting previously unselected package redis-server.
 Preparing to unpack .../redis-server_2%3a2.8.19-1~dotdeb.0_amd64.deb ...
 Unpacking redis-server (2:2.8.19-1~dotdeb.0) ...
 Processing triggers for man-db (2.6.7.1-1) ...
 Processing triggers for ureadahead (0.100.0-16) ...
 ureadahead will be reprofiled on next reboot
 Setting up redis-tools (2:2.8.19-1~dotdeb.0) ...
 Setting up redis-server (2:2.8.19-1~dotdeb.0) ...
 Starting redis-server: redis-server.
 Processing triggers for ureadahead (0.100.0-16) ...
 [Pharaoh Logging] Adding Package redis-server from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ****************************** 


 Single App Installer:
 --------------------------------------------
 Redis: Success
 ------------------------------
 Installer Finished
 ******************************

Opciones
-----------

.. cssclass:: table-bordered

 +---------------------+-----------------------------------+----------+---------------------------------------------------+
 | Parámetros          | Parámetro Alternativa             | Opciones | Comentarios                                       |
 +=====================+===================================+==========+===================================================+
 |Install Redis? (Y/N) | En lugar de utilizar redis, el    | Y(Yes)   | Si el usuario desea continuar el proceso de       |
 |                     | usuario puede utilizar Redis      |          | instalación se puede introducir como Y.           |
 +---------------------+-----------------------------------+----------+---------------------------------------------------+
 |Install Redis? (Y/N) | En lugar de utilizar redis, el    | N(No)    | Si el usuario desea abandonar el proceso de       |
 |                     | usuario puede utilizar Redis      |          | instalación se puede introducir como N.|          |
 +---------------------+-----------------------------------+----------+---------------------------------------------------+

Beneficios
-------------

* Escala automática, nodos ilimitados Redis.
* Alta disponibilidad en Ubuntu y CentOS.
* Persistencia de datos y durabilidad.
* Diario y copias de seguridad a la carta.
* Construida en el agrupamiento.
* Sensitibilidad caso.
