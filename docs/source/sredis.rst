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
 Creating /tmp/ptconfigure-temp-script-78539017469.sh
 chmod 755 /tmp/ptconfigure-temp-script-78539017469.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-78539017469.sh Permissions
 Executing /tmp/ptconfigure-temp-script-78539017469.sh
 W: GPG error: http://packages.elasticsearch.org stable Release: The following signatures couldn't be verified because the public key is not available: NO_PUBKEY D27D666CD88E42B4
 W: GPG error: http://packages.elasticsearch.org stable Release: The following signatures couldn't be verified because the public key is not available: NO_PUBKEY D27D666CD88E42B4
 W: GPG error: http://packages.elasticsearch.org stable Release: The following signatures couldn't be verified because the public key is not available: NO_PUBKEY D27D666CD88E42B4
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free amd64 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-amd64_Packages)
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free amd64 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-amd64_Packages)
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free amd64 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-amd64_Packages)
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free amd64 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-amd64_Packages)
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free amd64 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-amd64_Packages)
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free amd64 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-amd64_Packages)
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free i386 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-i386_Packages)
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free i386 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-i386_Packages)
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free i386 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-i386_Packages)
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free i386 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-i386_Packages)
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free i386 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-i386_Packages)
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free i386 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-i386_Packages)
 W: Duplicate sources.list entry https://repo.varnish-cache.org/ubuntu/ precise/varnish-4.0 amd64 Packages (/var/lib/apt/lists/repo.varnish-cache.org_ubuntu_dists_precise_varnish-4.0_binary-amd64_Packages)
 W: Duplicate sources.list entry https://repo.varnish-cache.org/ubuntu/ precise/varnish-4.0 amd64 Packages (/var/lib/apt/lists/repo.varnish-cache.org_ubuntu_dists_precise_varnish-4.0_binary-amd64_Packages)
 W: Duplicate sources.list entry https://repo.varnish-cache.org/ubuntu/ precise/varnish-4.0 amd64 Packages (/var/lib/apt/lists/repo.varnish-cache.org_ubuntu_dists_precise_varnish-4.0_binary-amd64_Packages)
 W: Duplicate sources.list entry https://repo.varnish-cache.org/ubuntu/ precise/varnish-4.0 amd64 Packages (/var/lib/apt/lists/repo.varnish-cache.org_ubuntu_dists_precise_varnish-4.0_binary-amd64_Packages)
 W: Duplicate sources.list entry https://repo.varnish-cache.org/ubuntu/ precise/varnish-4.0 amd64 Packages (/var/lib/apt/lists/repo.varnish-cache.org_ubuntu_dists_precise_varnish-4.0_binary-amd64_Packages)
 W: Duplicate sources.list entry https://repo.varnish-cache.org/ubuntu/ precise/varnish-4.0 amd64 Packages (/var/lib/apt/lists/repo.varnish-cache.org_ubuntu_dists_precise_varnish-4.0_binary-amd64_Packages)
 W: Duplicate sources.list entry https://repo.varnish-cache.org/ubuntu/ precise/varnish-4.0 i386 Packages (/var/lib/apt/lists/repo.varnish-cache.org_ubuntu_dists_precise_varnish-4.0_binary-i386_Packages)
 W: Duplicate sources.list entry https://repo.varnish-cache.org/ubuntu/ precise/varnish-4.0 i386 Packages (/var/lib/apt/lists/repo.varnish-cache.org_ubuntu_dists_precise_varnish-4.0_binary-i386_Packages)
 W: Duplicate sources.list entry https://repo.varnish-cache.org/ubuntu/ precise/varnish-4.0 i386 Packages (/var/lib/apt/lists/repo.varnish-cache.org_ubuntu_dists_precise_varnish-4.0_binary-i386_Packages)
 W: Duplicate sources.list entry https://repo.varnish-cache.org/ubuntu/ precise/varnish-4.0 i386 Packages (/var/lib/apt/lists/repo.varnish-cache.org_ubuntu_dists_precise_varnish-4.0_binary-i386_Packages)
 W: Duplicate sources.list entry https://repo.varnish-cache.org/ubuntu/ precise/varnish-4.0 i386 Packages (/var/lib/apt/lists/repo.varnish-cache.org_ubuntu_dists_precise_varnish-4.0_binary-i386_Packages)
 W: Duplicate sources.list entry https://repo.varnish-cache.org/ubuntu/ precise/varnish-4.0 i386 Packages (/var/lib/apt/lists/repo.varnish-cache.org_ubuntu_dists_precise_varnish-4.0_binary-i386_Packages)
 deb-src http://packages.dotdeb.org squeeze all
 OK
 Ign http://in.archive.ubuntu.com trusty InRelease
 Ign http://in.archive.ubuntu.com trusty-updates InRelease
 Ign http://in.archive.ubuntu.com trusty-backports InRelease
 Hit http://in.archive.ubuntu.com trusty Release.gpg
 Get:1 http://in.archive.ubuntu.com trusty-updates Release.gpg [933 B]
 Hit http://in.archive.ubuntu.com trusty-backports Release.gpg
 Hit http://in.archive.ubuntu.com trusty Release
 Get:2 http://in.archive.ubuntu.com trusty-updates Release [62.0 kB]
 Get:3 https://repo.varnish-cache.org precise InRelease
 Hit http://in.archive.ubuntu.com trusty-backports Release
 Get:4 https://repo.varnish-cache.org precise/varnish-4.0 amd64 Packages
 Hit http://in.archive.ubuntu.com trusty/main Sources
 Get:5 https://repo.varnish-cache.org precise/varnish-4.0 i386 Packages
 Hit http://in.archive.ubuntu.com trusty/restricted Sources
 Ign http://archive.canonical.com trusty InRelease
 Hit http://in.archive.ubuntu.com trusty/universe Sources
 Get:6 https://repo.varnish-cache.org precise/varnish-4.0 Translation-en_IN
 Hit http://archive.canonical.com trusty Release.gpg
 Hit http://in.archive.ubuntu.com trusty/multiverse Sources
 Ign http://repos.zend.com server InRelease
 Hit http://repos.zend.com server Release.gpg
 Hit http://repos.zend.com server Release
 Hit http://archive.canonical.com trusty Release
 Hit http://repos.zend.com server/non-free amd64 Packages
 Hit http://in.archive.ubuntu.com trusty/main amd64 Packages
 Hit http://repos.zend.com server/non-free i386 Packages
 Hit http://archive.canonical.com trusty/partner Sources
 Hit http://in.archive.ubuntu.com trusty/restricted amd64 Packages
 Hit http://archive.canonical.com trusty/partner amd64 Packages
 Hit http://archive.canonical.com trusty/partner i386 Packages
 Hit http://in.archive.ubuntu.com trusty/universe amd64 Packages
 Hit http://in.archive.ubuntu.com trusty/multiverse amd64 Packages
 Hit http://in.archive.ubuntu.com trusty/main i386 Packages
 Ign http://archive.canonical.com trusty/partner Translation-en
 Hit http://in.archive.ubuntu.com trusty/restricted i386 Packages
 Hit http://in.archive.ubuntu.com trusty/universe i386 Packages
 Ign https://repo.varnish-cache.org precise/varnish-4.0 Translation-en_IN
 Hit http://in.archive.ubuntu.com trusty/multiverse i386 Packages
 Ign https://repo.varnish-cache.org precise/varnish-4.0 Translation-en
 Ign http://repos.zend.com server/non-free Translation-en_IN
 Hit http://in.archive.ubuntu.com trusty/main Translation-en
 Ign http://repos.zend.com server/non-free Translation-en
 Hit http://in.archive.ubuntu.com trusty/multiverse Translation-en
 Ign http://extras.ubuntu.com trusty InRelease
 Hit http://in.archive.ubuntu.com trusty/restricted Translation-en
 Hit http://extras.ubuntu.com trusty Release.gpg
 Ign http://packages.dotdeb.org squeeze InRelease
 Get:7 http://packages.dotdeb.org squeeze Release.gpg [836 B]
 Hit http://in.archive.ubuntu.com trusty/universe Translation-en
 Get:8 http://packages.dotdeb.org squeeze Release [2,287 B]
 Get:9 http://in.archive.ubuntu.com trusty-updates/main Sources [158 kB]
 Get:10 http://packages.dotdeb.org squeeze/all amd64 Packages [20.6 kB]
 Hit http://extras.ubuntu.com trusty Release
 Hit http://extras.ubuntu.com trusty/main Sources
 Hit http://extras.ubuntu.com trusty/main amd64 Packages
 Get:11 http://packages.dotdeb.org squeeze/all i386 Packages [20.6 kB]
 Hit http://extras.ubuntu.com trusty/main i386 Packages
 Ign http://extras.ubuntu.com trusty/main Translation-en_IN
 Ign http://security.ubuntu.com trusty-security InRelease
 Ign http://extras.ubuntu.com trusty/main Translation-en
 Ign http://packages.dotdeb.org squeeze/all Translation-en_IN
 Ign http://packages.elasticsearch.org stable InRelease
 Ign http://pkg.jenkins-ci.org binary/ InRelease
 Get:12 http://in.archive.ubuntu.com trusty-updates/restricted Sources [2,061 B]
 Get:13 http://security.ubuntu.com trusty-security Release.gpg [933 B]
 Ign http://packages.dotdeb.org squeeze/all Translation-en
 Ign http://packages.elasticsearch.org stable InRelease
 Get:14 http://in.archive.ubuntu.com trusty-updates/universe Sources [97.6 kB]
 Get:15 http://security.ubuntu.com trusty-security Release [62.0 kB]
 Hit http://pkg.jenkins-ci.org binary/ Release.gpg
 Ign http://packages.elasticsearch.org stable InRelease
 Get:16 http://packages.elasticsearch.org stable Release.gpg [490 B]
 Hit http://pkg.jenkins-ci.org binary/ Release
 Get:17 http://packages.elasticsearch.org stable Release.gpg [490 B]
 Get:18 http://packages.elasticsearch.org stable Release.gpg [490 B]
 Hit http://pkg.jenkins-ci.org binary/ Packages
 Hit http://packages.elasticsearch.org stable Release
 Ign http://packages.elasticsearch.org stable Release
 Get:19 http://security.ubuntu.com trusty-security/main Sources [64.8 kB]
 Hit http://packages.elasticsearch.org stable Release
 Ign http://packages.elasticsearch.org stable Release
 Hit http://packages.elasticsearch.org stable Release
 Ign http://packages.elasticsearch.org stable Release
 Get:20 http://in.archive.ubuntu.com trusty-updates/multiverse Sources [3,553 B]
 Ign http://packages.elasticsearch.org stable/main amd64 Packages/DiffIndex
 Get:21 http://in.archive.ubuntu.com trusty-updates/main amd64 Packages [406 kB]
 Ign http://packages.elasticsearch.org stable/main i386 Packages/DiffIndex
 Ign http://packages.elasticsearch.org stable/main amd64 Packages/DiffIndex
 Ign http://packages.elasticsearch.org stable/main i386 Packages/DiffIndex
 Get:22 http://security.ubuntu.com trusty-security/restricted Sources [2,061 B]
 Ign http://ppa.launchpad.net trusty InRelease
 Hit http://dl.hhvm.com trusty InRelease
 Get:23 http://security.ubuntu.com trusty-security/universe Sources [17.4 kB]
 Hit http://ppa.launchpad.net trusty Release.gpg
 Hit http://dl.hhvm.com trusty/main amd64 Packages
 Ign http://packages.elasticsearch.org stable/main amd64 Packages/DiffIndex
 Hit http://dl.hhvm.com trusty/main i386 Packages
 Hit http://ppa.launchpad.net trusty Release
 Get:24 http://security.ubuntu.com trusty-security/multiverse Sources [723 B]
 Ign http://wireframesketcher.com  InRelease
 Ign http://packages.elasticsearch.org stable/main i386 Packages/DiffIndex
 Get:25 http://security.ubuntu.com trusty-security/main amd64 Packages [200 kB]
 Hit http://wireframesketcher.com  Release.gpg
 Hit http://ppa.launchpad.net trusty/main amd64 Packages
 Hit http://wireframesketcher.com  Release
 Hit http://ppa.launchpad.net trusty/main i386 Packages
 Ign http://pkg.jenkins-ci.org binary/ Translation-en_IN
 Hit http://ppa.launchpad.net trusty/main Translation-en
 Ign http://pkg.jenkins-ci.org binary/ Translation-en
 Hit http://wireframesketcher.com  Packages
 Ign http://dl.hhvm.com trusty/main Translation-en_IN
 Ign http://dl.hhvm.com trusty/main Translation-en
 Ign http://wireframesketcher.com  Translation-en_IN
 Ign http://wireframesketcher.com  Translation-en
 Get:26 http://security.ubuntu.com trusty-security/restricted amd64 Packages [8,875 B]
 Get:27 http://security.ubuntu.com trusty-security/universe amd64 Packages [85.3 kB]
 Get:28 http://security.ubuntu.com trusty-security/multiverse amd64 Packages [1,161 B]
 Get:29 http://security.ubuntu.com trusty-security/main i386 Packages [190 kB]
 Hit http://packages.elasticsearch.org stable/main amd64 Packages
 Get:30 http://in.archive.ubuntu.com trusty-updates/restricted amd64 Packages [8,875 B]
 Hit http://packages.elasticsearch.org stable/main i386 Packages
 Get:31 http://in.archive.ubuntu.com trusty-updates/universe amd64 Packages [241 kB]
 Ign http://packages.elasticsearch.org stable/main Translation-en_IN
 Ign http://packages.elasticsearch.org stable/main Translation-en
 Hit http://packages.elasticsearch.org stable/main amd64 Packages
 Hit http://packages.elasticsearch.org stable/main i386 Packages
 Ign http://packages.elasticsearch.org stable/main Translation-en_IN
 Get:32 http://in.archive.ubuntu.com trusty-updates/multiverse amd64 Packages [9,382 B]
 Ign http://packages.elasticsearch.org stable/main Translation-en
 Get:33 http://in.archive.ubuntu.com trusty-updates/main i386 Packages [397 kB]
 Hit http://packages.elasticsearch.org stable/main amd64 Packages
 Hit http://packages.elasticsearch.org stable/main i386 Packages
 Ign http://packages.elasticsearch.org stable/main Translation-en_IN
 Ign http://packages.elasticsearch.org stable/main Translation-en
 Get:34 http://security.ubuntu.com trusty-security/restricted i386 Packages [8,846 B]
 Get:35 http://security.ubuntu.com trusty-security/universe i386 Packages [85.3 kB]
 Get:36 http://security.ubuntu.com trusty-security/multiverse i386 Packages [1,412 B]
 Hit http://security.ubuntu.com trusty-security/main Translation-en
 Hit http://security.ubuntu.com trusty-security/multiverse Translation-en
 Hit http://security.ubuntu.com trusty-security/restricted Translation-en
 Hit http://security.ubuntu.com trusty-security/universe Translation-en
 Get:37 http://in.archive.ubuntu.com trusty-updates/restricted i386 Packages [8,846 B]
 Get:38 http://in.archive.ubuntu.com trusty-updates/universe i386 Packages [241 kB]
 Get:39 http://in.archive.ubuntu.com trusty-updates/multiverse i386 Packages [9,558 B]
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
 Fetched 2,441 kB in 1min 15s (32.5 kB/s)
 Reading package lists...
 Temp File /tmp/ptconfigure-temp-script-78539017469.sh Removed
 [Pharaoh Logging] Package redis-server from the Packager Apt is already installed, so not installing
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
