=========
Newrelic
=========

Sinopsis
----------------

NewRelic utiliza para supervisar el servidor. La colaboración entre los diferentes roles ofrece muchos beneficios. La combinación de una base común de código, integración continua, técnicas de prueba impulsada y despliega automatizados, entre otras cosas, exponer problemas, en el código de aplicación, infraestructura o de configuración, antes porque el software no está "tirado por encima del muro" ?? de operaciones en la final de la codificación. Despliegues automatizados y entornos de producción estandarizadas, aspectos clave de DevOps, hacen despliegues predecible y la gente libre de tareas repetitivas de rutina para ir a hacer cosas más creativas. El NewRelic se siente cómodo con Ubuntu y CentOS.

Comando Ayuda
----------------------

El comando de ayuda conduce a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en los módulos NewRelic. Las listas de comandos de ayuda fuera de los parámetros alternativos de NewRelic bajo módulo ptconfigure. También describe la sintaxis para la detección de la máquina del usuario. El comando de ayuda para NewRelic se muestra a continuación.

.. code-block:: bash

		ptconfigure newrelic help

La sintaxis para el comando de ayuda no entre mayúsculas y minúsculas, que añade una ventaja para este módulo. La siguiente captura de pantalla a visualizar al usuario sobre el comando de ayuda bajo NewRelic.

.. code-block:: bash

 kevell@corp:/# ptconfigure NewRelic help
 ******************************

 "‚This command allows you to update Newrelic.
 "‚"‚NewRelic, newrelic, Newrelic

 "‚- install
 "‚Installs the latest version of ptconfigure
 "‚example: ptconfigure newrelic install

 ------------------------------
 End Help
 ******************************

instalación
-------------------

Estos procedimientos de instalación son para los administradores de sistemas. Esta sección incluye información sobre la compatibilidad y requisitos, instrucciones básicas sobre cómo instalar y configurar ptconfigure a información más detallada.

Antes de la instalación, el usuario tiene que seguir:

1. Asegúrese de que su sistema cumple con los requisitos de compatibilidad y PHP de New Relic.

2. Si aún no tienes una cuenta nueva reliquia, cree una.

3. A partir de la nueva configuración de cuenta Relic, copiar su información de clave de licencia.

4. Siga los procedimientos de instalación de agentes, tanto para la extensión de PHP y el demonio proxy local.

5. Realice los ajustes de configuración para el agente y, opcionalmente, el demonio de proxy.

6. Cambie el nombre de la aplicación por defecto de un nombre significativo.

7. Reinicie Apache o su programa de acogida PHP (como php-pies por minuto), según corresponda.

8. Si no hay datos aparece después de unos minutos, consulte Resolución de problemas de instalación.

.. code-block:: bash

 kevell@corp:/# ptconfigure newrelic install

 Install NewRelic? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         NewRelic!        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-97361213995.sh
 chmod 755 /tmp/ptconfigure-temp-script-97361213995.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-97361213995.sh Permissions
 Executing /tmp/ptconfigure-temp-script-97361213995.sh
 --2015-01-28 13:05:04--  https://download.newrelic.com/548C16BF.gpg
 Resolving download.newrelic.com (download.newrelic.com)... 50.31.164.159
 Connecting to download.newrelic.com (download.newrelic.com)|50.31.164.159|:443... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: 1682 (1.6K) [application/octet-stream]
 Saving to: Ã¢â‚¬ËœSTDOUTÃ¢â‚¬â„¢

 100%[=======================================================================================================>] 1,682       --.-K/s   in 0s      

 2015-01-28 13:05:07 (27.9 MB/s) - written to stdout [1682/1682]
 
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
 OK
 Ign http://security.ubuntu.com trusty-security InRelease
 Get:1 http://security.ubuntu.com trusty-security Release.gpg [933 B]
 Get:2 http://security.ubuntu.com trusty-security Release [62.0 kB]
 Get:3 http://security.ubuntu.com trusty-security/main Sources [64.8 kB]
 Ign http://archive.canonical.com trusty InRelease
 Ign http://packages.dotdeb.org squeeze InRelease
 Ign http://ppa.launchpad.net trusty InRelease
 Get:4 http://security.ubuntu.com trusty-security/restricted Sources [2,061 B]
 Hit http://archive.canonical.com trusty Release.gpg
 Hit http://packages.dotdeb.org squeeze Release.gpg
 Get:5 http://security.ubuntu.com trusty-security/universe Sources [17.4 kB]
 Hit http://archive.canonical.com trusty Release
 Hit http://packages.dotdeb.org squeeze Release
 Hit http://archive.canonical.com trusty/partner Sources
 Hit http://packages.dotdeb.org squeeze/all amd64 Packages
 Hit http://archive.canonical.com trusty/partner amd64 Packages
 Hit http://packages.dotdeb.org squeeze/all i386 Packages
 Ign http://wireframesketcher.com  InRelease
 Hit http://archive.canonical.com trusty/partner i386 Packages
 Get:6 http://security.ubuntu.com trusty-security/multiverse Sources [723 B]
 Get:7 https://repo.varnish-cache.org precise InRelease
 Get:8 http://security.ubuntu.com trusty-security/main amd64 Packages [200 kB]
 Get:9 https://repo.varnish-cache.org precise/varnish-4.0 amd64 Packages
 Hit http://ppa.launchpad.net trusty Release.gpg
 Get:10 https://repo.varnish-cache.org precise/varnish-4.0 i386 Packages
 Get:11 https://repo.varnish-cache.org precise/varnish-4.0 Translation-en_IN
 Ign http://archive.canonical.com trusty/partner Translation-en
 Ign http://packages.elasticsearch.org stable InRelease
 Ign http://in.archive.ubuntu.com trusty InRelease
 Ign http://packages.elasticsearch.org stable InRelease
 Ign http://in.archive.ubuntu.com trusty-updates InRelease
 Ign http://packages.elasticsearch.org stable InRelease
 Ign http://packages.dotdeb.org squeeze/all Translation-en_IN
 Ign http://in.archive.ubuntu.com trusty-backports InRelease
 Get:12 http://packages.elasticsearch.org stable Release.gpg [490 B]
 Ign http://packages.dotdeb.org squeeze/all Translation-en
 Hit http://in.archive.ubuntu.com trusty Release.gpg
 Get:13 http://packages.elasticsearch.org stable Release.gpg [490 B]
 Get:14 http://packages.elasticsearch.org stable Release.gpg [490 B]
 Hit http://packages.elasticsearch.org stable Release
 Ign http://packages.elasticsearch.org stable Release
 Get:15 http://in.archive.ubuntu.com trusty-updates Release.gpg [933 B]
 Hit http://packages.elasticsearch.org stable Release
 Ign http://packages.elasticsearch.org stable Release
 Hit http://in.archive.ubuntu.com trusty-backports Release.gpg
 Hit http://wireframesketcher.com  Release.gpg
 Hit http://packages.elasticsearch.org stable Release
 Ign http://packages.elasticsearch.org stable Release
 Hit http://in.archive.ubuntu.com trusty Release
 Ign http://packages.elasticsearch.org stable/main amd64 Packages/DiffIndex
 Get:16 http://in.archive.ubuntu.com trusty-updates Release [62.0 kB]
 Ign http://packages.elasticsearch.org stable/main i386 Packages/DiffIndex
 Ign https://repo.varnish-cache.org precise/varnish-4.0 Translation-en_IN
 Hit http://ppa.launchpad.net trusty Release
 Ign https://repo.varnish-cache.org precise/varnish-4.0 Translation-en
 Hit http://wireframesketcher.com  Release
 Ign http://packages.elasticsearch.org stable/main amd64 Packages/DiffIndex
 Hit http://ppa.launchpad.net trusty/main amd64 Packages
 Ign http://packages.elasticsearch.org stable/main i386 Packages/DiffIndex
 Hit http://ppa.launchpad.net trusty/main i386 Packages
 Hit http://ppa.launchpad.net trusty/main Translation-en
 Ign http://packages.elasticsearch.org stable/main amd64 Packages/DiffIndex
 Hit http://in.archive.ubuntu.com trusty-backports Release
 Ign http://packages.elasticsearch.org stable/main i386 Packages/DiffIndex
 Hit http://wireframesketcher.com  Packages
 Hit http://in.archive.ubuntu.com trusty/main Sources
 Hit http://in.archive.ubuntu.com trusty/restricted Sources
 Get:17 http://security.ubuntu.com trusty-security/restricted amd64 Packages [8,875 B]
 Hit http://in.archive.ubuntu.com trusty/universe Sources
 Get:18 http://security.ubuntu.com trusty-security/universe amd64 Packages [85.3 kB]
 Ign http://pkg.jenkins-ci.org binary/ InRelease
 Ign http://extras.ubuntu.com trusty InRelease
 Hit http://in.archive.ubuntu.com trusty/multiverse Sources
 Hit http://in.archive.ubuntu.com trusty/main amd64 Packages
 Hit http://extras.ubuntu.com trusty Release.gpg
 Hit http://pkg.jenkins-ci.org binary/ Release.gpg
 Hit http://in.archive.ubuntu.com trusty/restricted amd64 Packages
 Hit http://extras.ubuntu.com trusty Release
 Hit http://in.archive.ubuntu.com trusty/universe amd64 Packages
 Hit http://extras.ubuntu.com trusty/main Sources
 Hit http://in.archive.ubuntu.com trusty/multiverse amd64 Packages
 Hit http://in.archive.ubuntu.com trusty/main i386 Packages
 Ign http://repos.zend.com server InRelease
 Hit http://repos.zend.com server Release.gpg
 Hit http://repos.zend.com server Release
 Hit http://repos.zend.com server/non-free amd64 Packages
 Hit http://pkg.jenkins-ci.org binary/ Release
 Hit http://repos.zend.com server/non-free i386 Packages
 Hit http://in.archive.ubuntu.com trusty/restricted i386 Packages
 Hit http://extras.ubuntu.com trusty/main amd64 Packages
 Hit http://pkg.jenkins-ci.org binary/ Packages
 Hit http://extras.ubuntu.com trusty/main i386 Packages
 Hit http://in.archive.ubuntu.com trusty/universe i386 Packages
 Hit http://in.archive.ubuntu.com trusty/multiverse i386 Packages
 Ign http://wireframesketcher.com  Translation-en_IN
 Hit http://in.archive.ubuntu.com trusty/main Translation-en
 Get:19 http://security.ubuntu.com trusty-security/multiverse amd64 Packages [1,161 B]
 Get:20 http://security.ubuntu.com trusty-security/main i386 Packages [190 kB]
 Hit http://dl.hhvm.com trusty InRelease
 Ign http://wireframesketcher.com  Translation-en
 Hit http://dl.hhvm.com trusty/main amd64 Packages
 Hit http://dl.hhvm.com trusty/main i386 Packages
 Hit http://in.archive.ubuntu.com trusty/multiverse Translation-en
 Ign http://extras.ubuntu.com trusty/main Translation-en_IN
 Ign http://repos.zend.com server/non-free Translation-en_IN
 Hit http://in.archive.ubuntu.com trusty/restricted Translation-en
 Ign http://extras.ubuntu.com trusty/main Translation-en
 Ign http://repos.zend.com server/non-free Translation-en
 Hit http://in.archive.ubuntu.com trusty/universe Translation-en
 Get:21 http://in.archive.ubuntu.com trusty-updates/main Sources [158 kB]
 Ign http://apt.newrelic.com newrelic InRelease
 Get:22 http://apt.newrelic.com newrelic Release.gpg [198 B]
 Get:23 http://apt.newrelic.com newrelic Release [3,364 B]
 Ign http://dl.hhvm.com trusty/main Translation-en_IN
 Get:24 http://apt.newrelic.com newrelic/non-free amd64 Packages [9,582 B]
 Ign http://dl.hhvm.com trusty/main Translation-en
 Ign http://pkg.jenkins-ci.org binary/ Translation-en_IN
 Get:25 http://apt.newrelic.com newrelic/non-free i386 Packages [9,623 B]
 Ign http://pkg.jenkins-ci.org binary/ Translation-en
 Ign http://apt.newrelic.com newrelic/non-free Translation-en_IN
 Ign http://apt.newrelic.com newrelic/non-free Translation-en
 Hit http://packages.elasticsearch.org stable/main amd64 Packages
 Hit http://packages.elasticsearch.org stable/main i386 Packages
 Ign http://packages.elasticsearch.org stable/main Translation-en_IN
 Ign http://packages.elasticsearch.org stable/main Translation-en
 Hit http://packages.elasticsearch.org stable/main amd64 Packages
 Hit http://packages.elasticsearch.org stable/main i386 Packages
 Ign http://packages.elasticsearch.org stable/main Translation-en_IN
 Ign http://packages.elasticsearch.org stable/main Translation-en
 Hit http://packages.elasticsearch.org stable/main amd64 Packages
 Get:26 http://in.archive.ubuntu.com trusty-updates/restricted Sources [2,061 B]
 Get:27 http://security.ubuntu.com trusty-security/restricted i386 Packages [8,846 B]
 Get:28 http://in.archive.ubuntu.com trusty-updates/universe Sources [97.6 kB]
 Hit http://packages.elasticsearch.org stable/main i386 Packages
 Get:29 http://security.ubuntu.com trusty-security/universe i386 Packages [85.3 kB]
 Ign http://packages.elasticsearch.org stable/main Translation-en_IN
 Ign http://packages.elasticsearch.org stable/main Translation-en
 Get:30 http://in.archive.ubuntu.com trusty-updates/multiverse Sources [3,553 B]
 Get:31 http://in.archive.ubuntu.com trusty-updates/main amd64 Packages [406 kB]
 Get:32 http://security.ubuntu.com trusty-security/multiverse i386 Packages [1,412 B]
 Hit http://security.ubuntu.com trusty-security/main Translation-en
 Hit http://security.ubuntu.com trusty-security/multiverse Translation-en
 Hit http://security.ubuntu.com trusty-security/restricted Translation-en
 Hit http://security.ubuntu.com trusty-security/universe Translation-en
 Get:33 http://in.archive.ubuntu.com trusty-updates/restricted amd64 Packages [8,875 B]
 Get:34 http://in.archive.ubuntu.com trusty-updates/universe amd64 Packages [241 kB]
 Get:35 http://in.archive.ubuntu.com trusty-updates/multiverse amd64 Packages [9,382 B]
 Get:36 http://in.archive.ubuntu.com trusty-updates/main i386 Packages [397 kB]
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
 Fetched 2,420 kB in 2min 58s (13.6 kB/s)
 Reading package lists...
 Temp File /tmp/ptconfigure-temp-script-97361213995.sh Removed
 dpkg: error processing package zend-server-php-5.3 (--configure):
 subprocess installed post-installation script returned error exit status 2
 Errors were encountered while processing:
 zend-server-php-5.3
 E: Sub-process /usr/bin/dpkg returned an error code (1)
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following packages were automatically installed and are no longer required:
 gyp libc-ares-dev libc-ares2 libjs-node-uuid libv8-3.14-dev
  linux-headers-3.13.0-32 linux-headers-3.13.0-32-generic
  linux-image-3.13.0-32-generic linux-image-extra-3.13.0-32-generic
  node-abbrev node-ansi node-archy node-async node-block-stream
  node-combined-stream node-cookie-jar node-delayed-stream node-forever-agent
  node-form-data node-fstream node-fstream-ignore node-github-url-from-git
  node-glob node-graceful-fs node-gyp node-inherits node-ini
  node-json-stringify-safe node-lockfile node-lru-cache node-mime
  node-minimatch node-mkdirp node-mute-stream node-node-uuid node-nopt
  node-normalize-package-data node-npmlog node-once node-osenv node-qs
  node-read node-read-package-json node-request node-retry node-rimraf
  node-semver node-sha node-sigmund node-slide node-tar node-tunnel-agent
  node-which nodejs nodejs-dev ttf-dejavu-core
 Use 'apt-get autoremove' to remove them.
 The following NEW packages will be installed:
  newrelic-sysmond
 0 upgraded, 1 newly installed, 0 to remove and 69 not upgraded.
 1 not fully installed or removed.
 Need to get 1,914 kB of archives.
 After this operation, 4,780 kB of additional disk space will be used.
 Get:1 http://apt.newrelic.com/debian/ newrelic/non-free newrelic-sysmond amd64 2.0.2.111 [1,914 kB]
 Fetched 1,914 kB in 4min 33s (6,991 B/s)
 Selecting previously unselected package newrelic-sysmond.
 (Reading database ... 280715 files and directories currently installed.)
 Preparing to unpack .../newrelic-sysmond_2.0.2.111_amd64.deb ...
 Unpacking newrelic-sysmond (2.0.2.111) ...
 Processing triggers for ureadahead (0.100.0-16) ...
 Setting up zend-server-php-5.3 (6.1.0+b1177) ...
 Module php5 already enabled
 Module rewrite already enabled
 Site zendserver_gui already enabled
 X-Powered-By: PHP/5.3.26 ZendServer/6.1.0
 Content-type: text/html

 ERROR: "/usr/sbin/apache2ctl" -S 2>&1 returned with error
 Setting up newrelic-sysmond (2.0.2.111) ...

 *********************************************************************
 *********************************************************************
 ***
 ***  Can not start the New Relic Server Monitor until you insert a
 ***  valid license key in the following file:
 ***
 ***     /etc/newrelic/nrsysmond.cfg
 ***
 ***  You can do this by running the following command as root:
 ***
 ***     nrsysmond-config --set license_key=<your_license_key_here>
 ***
 ***  No data will be reported until the server monitor can start.
 ***  You can get your New Relic key from the 'Configuration' section
 ***  of the 'Support' menu of your New Relic account (accessible at
 ***  https://rpm.newrelic.com).
 ***
 *********************************************************************
 *********************************************************************
 
 Processing triggers for ureadahead (0.100.0-16) ...
 [Pharaoh Logging] Adding Package newrelic-sysmond from the Packager Apt executed correctly
 Enter Your Licence Key:
                            
 Creating /tmp/ptconfigure-temp-script-5830489845.sh
 chmod 755 /tmp/ptconfigure-temp-script-5830489845.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-5830489845.sh Permissions
 Executing /tmp/ptconfigure-temp-script-5830489845.sh
 Error: no value specified for license_key

 *********************************************************************
 *********************************************************************
 ***
 ***  Can not start the New Relic Server Monitor until you insert a
 ***  valid license key in the following file:
 ***
 ***     /etc/newrelic/nrsysmond.cfg
 ***
 ***  You can do this by running the following command as root:
 ***
 ***     nrsysmond-config --set license_key=<your_license_key_here>
 ***
 ***  No data will be reported until the server monitor can start.
 ***  You can get your New Relic key from the 'Configuration' section
 ***  of the 'Support' menu of your New Relic account (accessible at
 ***  https://rpm.newrelic.com).
 ***
 *********************************************************************
 *********************************************************************
 
 Temp File /tmp/ptconfigure-temp-script-5830489845.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 NewRelic: Success
 ------------------------------
 Installer Finished
 ******************************

Opciones
---------------

.. cssclass:: table-bordered

 +--------------------+-------------------------------------------+--------------+----------------------------------------+
 | Parámetros         | Parámetro Alternativa                     | Opciones     | Comentarios                            |
 +====================+===========================================+==============+========================================+
 |Install newrelic?   | En lugar de utilizar newrelic el usuario  | Y(Yes)       | Comienza la instalación de NewRelic    |
 |(Y/N)               | puede utilizar NewRellic, Newrelic        |              | bajo ptconfigure                       |
 +--------------------+-------------------------------------------+--------------+----------------------------------------+
 |Install newrelic?   | En lugar de utilizar newrelic el usuario  | N(No)        | Finalizando la instalación             |
 |(Y/N)               | puede utilizar NewRellic, Newrelic|       |              |                                        |
 +--------------------+-------------------------------------------+--------------+----------------------------------------+


Beneficios
-------------

ventajas técnicas
----------------------------

* Entrega de software continua
* Problemas menos complejos para fijar
* Una resolución más rápida de problemas
* Comodidades con Ubuntu y CentOS
* Sensitibilidad caso

ventajas para la empresa
------------------------------

* Una entrega más rápida de características
* Entornos operativos más estables
* Más tiempo disponible para agregar valor (en lugar de fijar / mantener)