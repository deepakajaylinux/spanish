========
PHPVM
========

sinopsis
------------

Este módulo actúa como facilitador para la instalación y así como la actualización del vm php con la última versión. Veamos sobre el uso de este módulo y las maneras posibles de utilizar este módulo en los próximos temas.

Ayuda Comando
--------------------

El comando help guía a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en el módulo Phpvm. En él se enumeran los parámetros alternativos de módulo Phpvm. También describe la sintaxis para instalar el módulo Phpvm. El comando de ayuda para el módulo Phpvm se muestra a continuación.

.. code-block:: bash

		ptconfigure Phpvm help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda bajo Phpvm.

.. code-block:: bash

 kevell@corp:/# ptconfigure phpvm help

 ******************************


  This command allows you to update PHPVM.

  PHPVM, Phpvm, phpvm

        - install
        Installs the latest version of PHPVM
        example: ptconfigure phpvm install

 ------------------------------
 End Help
 ******************************

instalación
----------------

El comando utilizado para instalar el phpvm en la máquina de los usuarios se muestra a continuación:

.. code-block:: bash

		ptconfigure phpvm install

Después de introducir el comando anterior, el siguiente proceso se produce como se muestra en el formato tabular.

.. cssclass:: table-bordered

 +-------------------------+---------------------------------------------+-----------+-------------------------------------------------+
 | Parámetros              | Parámetro Alternativa                       | Opciones  | Comentarios                                     |
 +=========================+=============================================+===========+=================================================+
 |Install PHPVM? (Y/N)     | En lugar de phpvm, podemos utilizar PHPVM,  | Y(Yes)    | Si el usuario desea continuar el proceso de     |
 |                         | Phpvm también.                              |           | instalación se puede introducir como Y.         |
 +-------------------------+---------------------------------------------+-----------+-------------------------------------------------+
 |Install PHPVM? (Y/N)     | En lugar de phpvm, podemos utilizar PHPVM,  | N(No)     | Si el usuario desea abandonar el proceso de     |
 |                         | Phpvm también.                              |           | instalación se puede introducir como N.|        |
 +-------------------------+---------------------------------------------+-----------+-------------------------------------------------+

Si el usuario procede de la instalación, durante el proceso de instalación se describe en las listas siguientes:

* Construye el árbol de dependencias.
* Lee la información de estado.
* Lista outs los paquetes que se instalan automáticamente.
* Lista outs los nuevos paquetes que está instalando.
* Detalles sobre el número de archivos actualizados, recién instalados, retirados y no actualizados.
* Lee la lista de paquetes y muestra la lista de paquetes que ya están instalados.

La siguiente captura de pantalla representa gráficamente el proceso anteriormente descrito de la instalación.

.. code-block:: bash

 kevell@corp:/# ptconfigure phpvm install

 Install PHPVM? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         PHPVM!        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-45523327550.sh
 chmod 755 /tmp/ptconfigure-temp-script-45523327550.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-45523327550.sh Permissions
 Executing /tmp/ptconfigure-temp-script-45523327550.sh
 W: GPG error: http://packages.elasticsearch.org stable Release: The following signatures couldn't be verified because the public key is not available: NO_PUBKEY D27D666CD88E42B4
 W: GPG error: http://packages.elasticsearch.org stable Release: The following signatures couldn't be verified because the public key is not available: NO_PUBKEY D27D666CD88E42B4
 W: GPG error: http://packages.elasticsearch.org stable Release: The following signatures couldn't be verified because the public key is not available: NO_PUBKEY D27D666CD88E42B4
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free amd64 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-amd64_Packages)
 W: Duplicate sources.list entry http://repos.zend.com/zend-server/6.1/deb/ server/non-free amd64 Packages (/var/lib/apt/lists/repos.zend.com_zend-server_6.1_deb_dists_server_non-free_binary-amd64_Packages)
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
 Hit https://repo.varnish-cache.org precise InRelease
 Hit https://repo.varnish-cache.org precise/varnish-4.0 amd64 Packages
 Hit https://repo.varnish-cache.org precise/varnish-4.0 i386 Packages
 Get:1 https://repo.varnish-cache.org precise/varnish-4.0 Translation-en
 Ign http://repos.zend.com server InRelease
 Hit http://repos.zend.com server Release.gpg
 Hit http://repos.zend.com server Release
 Hit http://repos.zend.com server/non-free amd64 Packages
 Hit http://repos.zend.com server/non-free i386 Packages
 Ign http://repos.zend.com server/non-free Translation-en
 Ign http://security.ubuntu.com trusty-security InRelease
 Hit http://dl.hhvm.com trusty InRelease
 Hit http://security.ubuntu.com trusty-security Release.gpg
 Ign http://in.archive.ubuntu.com trusty InRelease
 Hit http://dl.hhvm.com trusty/main amd64 Packages
 Ign http://pkg.jenkins-ci.org binary/ InRelease
 Hit http://security.ubuntu.com trusty-security Release
 Hit http://dl.hhvm.com trusty/main i386 Packages
 Ign http://in.archive.ubuntu.com trusty-updates InRelease
 Ign https://repo.varnish-cache.org precise/varnish-4.0 Translation-en
 Hit http://security.ubuntu.com trusty-security/main Sources
 Ign http://in.archive.ubuntu.com trusty-backports InRelease
 Hit http://pkg.jenkins-ci.org binary/ Release.gpg
 Hit http://security.ubuntu.com trusty-security/restricted Sources
 Hit http://in.archive.ubuntu.com trusty Release.gpg
 Hit http://security.ubuntu.com trusty-security/universe Sources
 Hit http://in.archive.ubuntu.com trusty-updates Release.gpg
 Hit http://pkg.jenkins-ci.org binary/ Release
 Hit http://security.ubuntu.com trusty-security/multiverse Sources
 Hit http://in.archive.ubuntu.com trusty-backports Release.gpg
 Hit http://security.ubuntu.com trusty-security/main amd64 Packages
 Ign http://dl.hhvm.com trusty/main Translation-en
 Hit http://in.archive.ubuntu.com trusty Release
 Hit http://security.ubuntu.com trusty-security/restricted amd64 Packages
 Hit http://in.archive.ubuntu.com trusty-updates Release
 Hit http://security.ubuntu.com trusty-security/universe amd64 Packages
 Hit http://security.ubuntu.com trusty-security/multiverse amd64 Packages
 Hit http://in.archive.ubuntu.com trusty-backports Release
 Hit http://security.ubuntu.com trusty-security/main i386 Packages
 Hit http://in.archive.ubuntu.com trusty/main Sources
 Hit http://security.ubuntu.com trusty-security/restricted i386 Packages
 Hit http://pkg.jenkins-ci.org binary/ Packages
 Hit http://in.archive.ubuntu.com trusty/restricted Sources
 Hit http://security.ubuntu.com trusty-security/universe i386 Packages
 Hit http://in.archive.ubuntu.com trusty/universe Sources
 Hit http://security.ubuntu.com trusty-security/multiverse i386 Packages
 Hit http://in.archive.ubuntu.com trusty/multiverse Sources
 Hit http://security.ubuntu.com trusty-security/main Translation-en
 Hit http://in.archive.ubuntu.com trusty/main amd64 Packages
 Hit http://security.ubuntu.com trusty-security/multiverse Translation-en
 Hit http://in.archive.ubuntu.com trusty/restricted amd64 Packages
 Hit http://security.ubuntu.com trusty-security/restricted Translation-en
 Ign http://archive.canonical.com trusty InRelease
 Ign http://apt.newrelic.com newrelic InRelease
 Hit http://in.archive.ubuntu.com trusty/universe amd64 Packages
 Ign http://packages.elasticsearch.org stable InRelease
 Ign http://ppa.launchpad.net trusty InRelease
 Hit http://archive.canonical.com trusty Release.gpg
 Hit http://apt.newrelic.com newrelic Release.gpg
 Hit http://in.archive.ubuntu.com trusty/multiverse amd64 Packages
 Hit http://security.ubuntu.com trusty-security/universe Translation-en
 Ign http://packages.elasticsearch.org stable InRelease
 Hit http://archive.canonical.com trusty Release
 Ign http://packages.dotdeb.org squeeze InRelease
 Hit http://apt.newrelic.com newrelic Release
 Hit http://in.archive.ubuntu.com trusty/main i386 Packages
 Ign http://packages.elasticsearch.org stable InRelease
 Hit http://archive.canonical.com trusty/partner Sources
 Hit http://packages.dotdeb.org squeeze Release.gpg
 Hit http://apt.newrelic.com newrelic/non-free amd64 Packages
 Hit http://in.archive.ubuntu.com trusty/restricted i386 Packages
 Hit http://archive.canonical.com trusty/partner amd64 Packages
 Get:2 http://packages.elasticsearch.org stable Release.gpg [490 B]
 Hit http://apt.newrelic.com newrelic/non-free i386 Packages
 Hit http://packages.dotdeb.org squeeze Release
 Hit http://archive.canonical.com trusty/partner i386 Packages
 Get:3 http://packages.elasticsearch.org stable Release.gpg [490 B]
 Ign http://wireframesketcher.com  InRelease
 Hit http://packages.dotdeb.org squeeze/all amd64 Packages
 Hit http://in.archive.ubuntu.com trusty/universe i386 Packages
 Get:4 http://packages.elasticsearch.org stable Release.gpg [490 B]
 Hit http://packages.dotdeb.org squeeze/all i386 Packages
 Ign http://pkg.jenkins-ci.org binary/ Translation-en
 Hit http://in.archive.ubuntu.com trusty/multiverse i386 Packages
 Hit http://packages.elasticsearch.org stable Release
 Ign http://packages.elasticsearch.org stable Release
 Ign http://archive.canonical.com trusty/partner Translation-en
 Hit http://in.archive.ubuntu.com trusty/main Translation-en
 Hit http://packages.elasticsearch.org stable Release
 Ign http://packages.elasticsearch.org stable Release
 Hit http://ppa.launchpad.net trusty Release.gpg
 Ign http://apt.newrelic.com newrelic/non-free Translation-en
 Hit http://in.archive.ubuntu.com trusty/multiverse Translation-en
 Hit http://packages.elasticsearch.org stable Release
 Ign http://packages.elasticsearch.org stable Release
 Hit http://in.archive.ubuntu.com trusty/restricted Translation-en
 Ign http://packages.elasticsearch.org stable/main amd64 Packages/DiffIndex
 Hit http://wireframesketcher.com  Release.gpg
 Hit http://in.archive.ubuntu.com trusty/universe Translation-en
 Ign http://packages.elasticsearch.org stable/main i386 Packages/DiffIndex
 Hit http://in.archive.ubuntu.com trusty-updates/main Sources
 Hit http://in.archive.ubuntu.com trusty-updates/restricted Sources
 Hit http://ppa.launchpad.net trusty Release
 Ign http://packages.elasticsearch.org stable/main amd64 Packages/DiffIndex
 Ign http://packages.dotdeb.org squeeze/all Translation-en
 Hit http://in.archive.ubuntu.com trusty-updates/universe Sources
 Ign http://packages.elasticsearch.org stable/main i386 Packages/DiffIndex
 Hit http://in.archive.ubuntu.com trusty-updates/multiverse Sources
 Hit http://wireframesketcher.com  Release
 Get:5 http://in.archive.ubuntu.com trusty-updates/main amd64 Packages [407 kB]
 Ign http://packages.elasticsearch.org stable/main amd64 Packages/DiffIndex
 Ign http://extras.ubuntu.com trusty InRelease
 Ign http://packages.elasticsearch.org stable/main i386 Packages/DiffIndex
 Hit http://extras.ubuntu.com trusty Release.gpg
 Hit http://ppa.launchpad.net trusty/main amd64 Packages
 Hit http://extras.ubuntu.com trusty Release
 Hit http://ppa.launchpad.net trusty/main i386 Packages
 Hit http://extras.ubuntu.com trusty/main Sources
 Hit http://extras.ubuntu.com trusty/main amd64 Packages
 Hit http://extras.ubuntu.com trusty/main i386 Packages
 Hit http://ppa.launchpad.net trusty/main Translation-en
 Hit http://wireframesketcher.com  Packages
 Ign http://extras.ubuntu.com trusty/main Translation-en
 Ign http://wireframesketcher.com  Translation-en
 Get:6 http://in.archive.ubuntu.com trusty-updates/restricted amd64 Packages [8875 B]
 Get:7 http://in.archive.ubuntu.com trusty-updates/universe amd64 Packages [243 kB]
 Get:8 http://in.archive.ubuntu.com trusty-updates/multiverse amd64 Packages [11.2 kB]
 Hit http://packages.elasticsearch.org stable/main amd64 Packages
 Hit http://packages.elasticsearch.org stable/main i386 Packages
 Get:9 http://in.archive.ubuntu.com trusty-updates/main i386 Packages [399 kB]
 Ign http://packages.elasticsearch.org stable/main Translation-en
 Hit http://packages.elasticsearch.org stable/main amd64 Packages
 Hit http://packages.elasticsearch.org stable/main i386 Packages
 Ign http://packages.elasticsearch.org stable/main Translation-en
 Hit http://packages.elasticsearch.org stable/main amd64 Packages
 Hit http://packages.elasticsearch.org stable/main i386 Packages
 Ign http://packages.elasticsearch.org stable/main Translation-en
 Get:10 http://in.archive.ubuntu.com trusty-updates/restricted i386 Packages [8846 B]
 Get:11 http://in.archive.ubuntu.com trusty-updates/universe i386 Packages [243 kB]
 Get:12 http://in.archive.ubuntu.com trusty-updates/multiverse i386 Packages [11.4 kB]
 Get:13 http://in.archive.ubuntu.com trusty-updates/main Translation-en [194 kB]
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
 Fetched 1364 kB in 51s (26.6 kB/s)
 Reading package lists...
 Temp File /tmp/ptconfigure-temp-script-45523327550.sh Removed
 [Pharaoh Logging] Package apache2 from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package mysql-server from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package php5 from the Packager Apt is already installed, so not installing
 E: Could not get lock /var/cache/apt/archives/lock - open (11: Resource temporarily unavailable)
 E: Unable to lock directory /var/cache/apt/archives/
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following packages were automatically installed and are no longer required:
  gyp libc-ares-dev libc-ares2 libframework2-zend-server libicu36
  libjs-node-uuid libmcrypt4 liboci-us-locales-zend libpng3 libsqlite0
  libssl0.9.8 libv8-3.14-dev lighttpd-zend-server linux-headers-3.13.0-32
  linux-headers-3.13.0-32-generic linux-image-3.13.0-32-generic
  linux-image-extra-3.13.0-32-generic node-abbrev node-ansi node-archy
  node-async node-block-stream node-combined-stream node-cookie-jar
  node-delayed-stream node-forever-agent node-form-data node-fstream
  node-fstream-ignore node-github-url-from-git node-glob node-graceful-fs
  node-gyp node-inherits node-ini node-json-stringify-safe node-lockfile
  node-lru-cache node-mime node-minimatch node-mkdirp node-mute-stream
  node-node-uuid node-nopt node-normalize-package-data node-npmlog node-once
  node-osenv node-qs node-read node-read-package-json node-request node-retry
  node-rimraf node-semver node-sha node-sigmund node-slide node-tar
  node-tunnel-agent node-which nodejs nodejs-dev php-5.3-bcmath-zend-server
  php-5.3-bz2-zend-server php-5.3-calendar-zend-server
  php-5.3-ctype-zend-server php-5.3-curl-zend-server php-5.3-exif-zend-server
  php-5.3-fcgi-zend-server php-5.3-fileinfo-zend-server
  php-5.3-ftp-zend-server php-5.3-gd-zend-server php-5.3-gettext-zend-server
  php-5.3-imap-zend-server php-5.3-intl-zend-server php-5.3-ldap-zend-server
  php-5.3-loader-zend-server php-5.3-mbstring-zend-server
  php-5.3-mcrypt-zend-server php-5.3-oci8-zend-server
  php-5.3-pdo-mysql-zend-server php-5.3-pdo-pgsql-zend-server
  php-5.3-pgsql-zend-server php-5.3-phar-zend-server php-5.3-posix-zend-server
  php-5.3-soap-zend-server php-5.3-sockets-zend-server
  php-5.3-sqlite-zend-server php-5.3-tidy-zend-server
  php-5.3-tokenizer-zend-server php-5.3-xsl-zend-server
  php-5.3-zip-zend-server sqlite sqlite3 ttf-dejavu-core zend-server-doc
 Use 'apt-get autoremove' to remove them.
 The following packages will be REMOVED:
   php-5.3-common-extensions-zend-server php-5.3-mysql-zend-server
   php-5.3-mysqli-zend-server zend-server-php-5.3 zend-server-php-5.3-common
 The following NEW packages will be installed:
  php5-mysql
 0 upgraded, 1 newly installed, 5 to remove and 79 not upgraded.
 9 not fully installed or removed.
 [Pharaoh Logging] Adding Package php5-mysql from the Packager Apt did not execute correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PHPVM: Success
 ------------------------------
 Installer Finished
 ******************************

Beneficios
-------------

* Los parámetros utilizados en la ayuda y la instalación no son sensibles, que es una ventaja añadida, mientras que en comparación con otros.
* Es-acomodados tanto en Ubuntu y así como Cent OS.
* Este módulo se instala el phpvm en versión actualizada.
* Si el módulo ya existe en la máquina del usuario, se mostrará un mensaje, ya que ya existe.
