=============
Gitbucket
=============

sinopsis
-------------

Git es un sistema de control distribuido de versiones con un énfasis en la rapidez, integridad de datos y soporte para flujos de trabajo distribuidas, no lineales. Git es el sistema de control de versiones ampliamente adoptado para el desarrollo de software.

Directorio de trabajo Git es un repositorio de pleno derecho con la historia completa y plena capacidad de versión de seguimiento, independientemente del acceso a la red o en un servidor central.

GitBucket es la fácil instalación Github clon escrito con Scala. Proporciona una serie de características básicas siguientes:

* Público / Privado repositorio Git (acceso http solamente)
* El visor de repositorio (algunas características avanzadas como la edición de archivos en línea no se implementan)
* Buscar descarga (Código y Cuestiones)
* Wiki
* Cuestiones
* Tenedor petición / Tirar
* Notificación por correo
* Actividad línea de tiempo
* Gestión de usuarios (para administradores)
* Grupo (como Organización en Github)
* Integración LDAP
* Soporte Gravatar
* Archivo war ejecutable

Ayuda Comando
----------------------

Este comando ayuda a determinar el uso del módulo gitbucket. El usuario llega a saber acerca de las diferentes formas / formato para ejecutar este módulo. Este comando guía al usuario final a conocer el propósito de este comando. A continuación dado son el mando y la pantalla del mismo.

.. code-block:: bash
     
                ptconfigure gitbucket help

La captura de pantalla para el comando anterior se enumeran a continuación,

.. code-block:: bash

 kevell@corp:/# ptconfigure gitbucket help
 ******************************
  This command allows you to install a full Git Bucket installation on to a server
  The dependencies for GitBucket are also installed.

  GitBucket, gitbucket, git-bucket

        - install
        Installs the latest version of GitBucket on a system
        example: ptconfigure gitbucket install

 ------------------------------
 End Help
 ******************************

instalación
----------------

Cuando el usuario tiene que instalar el módulo gitbucket en máquina. El siguiente comando dado se ejecutará el proceso de instalación.
Durante la instalación, el sistema pide el directorio raíz del repositorio. El usuario tiene que definir la ruta. No hay directorio predeterminado.

.. code-block:: bash
       
                ptconfigure gitbucket install

La captura de pantalla para el comando anterior se enumeran a continuación,

.. code-block:: bash

 kevell@corp:/# ptconfigure gitbucket install
 Install Git Bucket? (Y/N)
 y
 *******************************
 *        Pharaoh Tools        *
 *         !GitBucket!        *
 *******************************
 PHP Notice:  Undefined index: version in /opt/ptconfigure/ptconfigure/src/Modules/GitBucket/Model/GitBucketUbuntu.php on line 67
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Command 'git' found
 [Pharaoh Logging] No command 'gitk' found
 [Pharaoh Logging] No command 'git-cola' found
 [Pharaoh Logging] Installing as not installed
 *******************************
 *        Pharaoh Tools        *
 *         !Git Tools!!        *
 *******************************
 PHP Warning:  file_put_contents(/opt/ptconfigure/ptconfigure/src/Modules/ptconfigureRequired/Model/../../../cleovars): failed to open stream: Permission denied in /opt/ptconfigure/ptconfigure/src/Modules/ptconfigureRequired/Model/AppConfig.php on line 115
 [Pharaoh Logging] Package git from the Packager Apt is already installed, so not installing
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
  git-core
 0 upgraded, 1 newly installed, 0 to remove and 301 not upgraded.
 Need to get 1,458 B of archives.
 After this operation, 21.5 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main git-core all 1:1.9.1-1ubuntu0.1 [1,458 B]
 Fetched 1,458 B in 1s (783 B/s)
 Selecting previously unselected package git-core.
 (Reading database ... 182763 files and directories currently installed.)
 Preparing to unpack .../git-core_1%3a1.9.1-1ubuntu0.1_all.deb ...
 Unpacking git-core (1:1.9.1-1ubuntu0.1) ...
 Setting up git-core (1:1.9.1-1ubuntu0.1) ...
 [Pharaoh Logging] Adding Package git-core from the Packager Apt executed correctly
 PHP Warning:  file_put_contents(/opt/ptconfigure/ptconfigure/src/Modules/ptconfigureRequired/Model/../../../cleovars): failed to open stream: Permission denied in /opt/ptconfigure/ptconfigure/src/Modules/ptconfigureRequired/Model/AppConfig.php on line 115
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Suggested packages:
  git-doc
 The following NEW packages will be installed:
  gitk
 0 upgraded, 1 newly installed, 0 to remove and 301 not upgraded.
 Need to get 121 kB of archives.
 After this operation, 1,250 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main gitk all 1:1.9.1-1ubuntu0.1 [121 kB]
 Fetched 121 kB in 2s (43.1 kB/s)
 Selecting previously unselected package gitk.
 (Reading database ... 182764 files and directories currently installed.)
 Preparing to unpack .../gitk_1%3a1.9.1-1ubuntu0.1_all.deb ...
 Unpacking gitk (1:1.9.1-1ubuntu0.1) ...
 Processing triggers for man-db (2.6.7.1-1) ...
 Setting up gitk (1:1.9.1-1ubuntu0.1) ...
 [Pharaoh Logging] Adding Package gitk from the Packager Apt executed correctly
 PHP Warning:  file_put_contents(/opt/ptconfigure/ptconfigure/src/Modules/ptconfigureRequired/Model/../../../cleovars): failed to open stream: Permission denied in /opt/ptconfigure/ptconfigure/src/Modules/ptconfigureRequired/Model/AppConfig.php on line 115
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libjs-jquery libjs-underscore
 Suggested packages:
  python-pyinotify python-simplejson javascript-common
 Recommended packages:
  xxdiff
 The following NEW packages will be installed:
  git-cola libjs-jquery libjs-underscore
 0 upgraded, 3 newly installed, 0 to remove and 301 not upgraded.
 Need to get 363 kB of archives.
 After this operation, 1,886 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/main libjs-jquery all 1.7.2+dfsg-2ubuntu1 [78.8 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/main libjs-underscore all 1.4.4-2ubuntu1 [45.6 kB]
 Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty/universe git-cola all 1.9.3-1 [239 kB]
 Fetched 363 kB in 13s (27.8 kB/s)
 Selecting previously unselected package libjs-jquery.
 (Reading database ... 182782 files and directories currently installed.)
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
 PHP Warning:  file_put_contents(/opt/ptconfigure/ptconfigure/src/Modules/ptconfigureRequired/Model/../../../cleovars): failed to open stream: Permission denied in /opt/ptconfigure/ptconfigure/src/Modules/ptconfigureRequired/Model/AppConfig.php on line 115
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module Java reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 Creating /tmp/ptconfigure-temp-script-15361773074.sh
 chmod 755 /tmp/ptconfigure-temp-script-15361773074.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-15361773074.sh Permissions
 Executing /tmp/ptconfigure-temp-script-15361773074.sh
 Cloning into 'gitbucket-war'...
 remote: Counting objects: 8, done.
 remote: Total 8 (delta 0), reused 0 (delta 0)
 Unpacking objects: 100% (8/8), done.
 Checking connectivity... done.
 mkdir: cannot create directory ‘/opt/gitbucket/’: Permission denied
 mv: target ‘/opt/gitbucket/’ is not a directory
 Temp File /tmp/ptconfigure-temp-script-15361773074.sh Removed
 Enter Repository Root Directory:
 /
 Program Executor Deleted if existed
 PHP Warning:  file_put_contents(/usr/bin/gitbucket): failed to open stream: Permission denied in /opt/ptconfigure/ptconfigure/src/Modules/ptconfigureRequired/Model/BaseLinuxApp.php on line 312
 chmod: cannot access ‘/usr/bin/gitbucket’: No such file or directory
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************
 

 Single App Installer:
 --------------------------------------------
 GitBucket: Success
 ------------------------------
 Installer Finished
 ******************************

Opciones
------------

.. cssclass:: table-bordered


 +---------------------------+------------------------------------+-----------+----------------------------------------------+
 | Parámetros                | Parámetro Alternativa              | Opciones  | Comentarios                                  |
 +===========================+====================================+===========+==============================================+
 |ptconfigure gitbucket      | GitBucket, gitbucket , git-bucket  | Y(Yes)    | El sistema se inicia proceso de instalación  |
 |Install                    |                                    |           |                                              |
 +---------------------------+------------------------------------+-----------+----------------------------------------------+
 |ptconfigure gitbucket      |GitBucket, gitbucket , git-bucket   | N(No)     | El sistema se inicia proceso de instalación  |
 |Install|                   |                                    |           |                                              | 
 +---------------------------+------------------------------------+-----------+----------------------------------------------+



Beneficios
--------------

* Git apoya ramificación rápida y fusión, e incluye herramientas específicas para la visualización y navegación de una historia de desarrollo 
  no lineal.
* Los repositorios pueden ser publicados a través de HTTP, FTP, rsync, o un protocolo Git más bien una toma de corriente normal, o ssh.
* Git describe como muy rápido, escalable y demostró que era un orden de magnitud más rápido que algunos sistemas de control de versiones, y ir a  buscar historial de versiones de un repositorio almacenada localmente puede ser cien veces más rápido que ir a buscar desde el servidor remoto.
* Las palabras clave en changelogs tienen hipervínculos a las páginas de emisión que corresponda, Pull Pide páginas y páginas Wiki.
* El conjunto de cambios y diferencial en los registros de cambios se enlazará con GitBucket espectador repositorio.
* Desencadenar una acumulación cuando un cambio es empujado a GitBucket utilizando un WebHook.
