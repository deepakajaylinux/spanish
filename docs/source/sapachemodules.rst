================
ApacheModules
================

Sinopsis
-----------

Este módulo facilita a instalar los módulos de Apache. En él se especifica la configuración de su entorno. Es posible comprobar la disponibilidad de los módulos. Es cómodo en Ubuntu así como en Cent OS.

comando Ayuda
---------------------

Este comando ayuda explica sobre el propósito de un módulo en particular. La sintaxis para la instalación se representa bajo el comando de ayuda. También se enumeran los parámetros alternativos que se pueden utilizar para la declaración. El comando de ayuda es fácil de manejar por el usuario final. El comando siguiente guía al usuario sobre el uso de este módulo.

.. code-block:: bash

	 cleopatra apache modules help

Después de dar el comando, el comando listará las opciones de ayuda. Las siguientes capturas de pantalla darán efecto visual para el uso de este módulo.

.. code-block:: bash

 kevell@corp:/# cleopatra ApacheModules help
 ******************************


  This command is part of Core and provides you  with a method by which you can configure Application Settings.
  You can configure default application settings, ie: mysql admin user, host, pass

  ApacheModules, apachemods, apache-modules, apachemodules

        - install
        Installs common apache Modules
        example: cleopatra apache-modules install

 ------------------------------
 End Help
 ******************************

instalación
-------------

La instalación no es un proceso difícil de instalar este módulo bajo Cleopatra por la mera utilización de la orden dada a continuación,

.. code-block:: bash

	Install apache-modules install

Después de dar la orden de que le preguntará,

.. code-block:: bash

	Install Apache module? (Y/N)

	Si le das una entrada como 'Y', se ha instalado correctamente el módulo.

	Si le das una entrada como 'N', entonces saldrá de la instalación.


Las siguientes capturas de pantalla darán efecto visual para la instalación de este módulo.

.. code-block:: bash

 kevell@corp:/#  cleopatra apache-modules install
 Install Apache Modules? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Apache Mods!        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
  libxml2-dev
 0 upgraded, 1 newly installed, 0 to remove and 229 not upgraded.
 Need to get 630 kB of archives.
 After this operation, 2,928 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main libxml2-dev amd64 2.9.1+dfsg1-3ubuntu4.4 [630 kB]
 Fetched 630 kB in 2min 38s (3,990 B/s)
 Selecting previously unselected package libxml2-dev:amd64.
 (Reading database ... 181481 files and directories currently installed.)
 Preparing to unpack .../libxml2-dev_2.9.1+dfsg1-3ubuntu4.4_amd64.deb ...
 Unpacking libxml2-dev:amd64 (2.9.1+dfsg1-3ubuntu4.4) ...
 Processing triggers for man-db (2.6.7.1-1) ...
 Setting up libxml2-dev:amd64 (2.9.1+dfsg1-3ubuntu4.4) ...
 [Pharaoh Logging] Adding Package libxml2-dev from the Packager Apt executed correctly
 Creating /tmp/cleopatra-temp-script-11435369770.sh
 chmod 755 /tmp/cleopatra-temp-script-11435369770.sh 2>/dev/null
 Changing /tmp/cleopatra-temp-script-11435369770.sh Permissions
 Executing /tmp/cleopatra-temp-script-11435369770.sh
 Enabling module rewrite.
 To activate the new configuration, you need to run:
  service apache2 restart
 Temp File /tmp/cleopatra-temp-script-11435369770.sh Removed
 Creating /tmp/cleopatra-temp-script-95277456152.sh
 chmod 755 /tmp/cleopatra-temp-script-95277456152.sh 2>/dev/null
 Changing /tmp/cleopatra-temp-script-95277456152.sh Permissions
 Executing /tmp/cleopatra-temp-script-95277456152.sh
 Considering dependency filter for deflate:
 Module filter already enabled
 Module deflate already enabled
 Temp File /tmp/cleopatra-temp-script-95277456152.sh Removed
 Creating /tmp/cleopatra-temp-script-1351048337.sh
 chmod 755 /tmp/cleopatra-temp-script-1351048337.sh 2>/dev/null
 Changing /tmp/cleopatra-temp-script-1351048337.sh Permissions
 Executing /tmp/cleopatra-temp-script-1351048337.sh
 Considering dependency setenvif for ssl:
 Module setenvif already enabled
 Considering dependency mime for ssl:
 Module mime already enabled
 Considering dependency socache_shmcb for ssl:
 Enabling module socache_shmcb.
 Enabling module ssl.
 See /usr/share/doc/apache2/README.Debian.gz on how to configure SSL and create self-signed certificates.
 To activate the new configuration, you need to run:
   service apache2 restart
 Temp File /tmp/cleopatra-temp-script-1351048337.sh Removed
 [Pharaoh Logging] Package libapache2-mod-php5 from the Packager Apt is already installed, so not installing
 Creating /tmp/cleopatra-temp-script-89813944614.sh
 chmod 755 /tmp/cleopatra-temp-script-89813944614.sh 2>/dev/null
 Changing /tmp/cleopatra-temp-script-89813944614.sh Permissions
 Executing /tmp/cleopatra-temp-script-89813944614.sh
 Module php5 already enabled
 Temp File /tmp/cleopatra-temp-script-89813944614.sh Removed
 [Pharaoh Logging] Restarting apache2 service
 Output of config test was:
 apache2: Syntax error on line 214 of /etc/apache2/apache2.conf: Could not open configuration file /etc/apache2/httpd.conf: No such file or 
 directory 
 Action 'configtest' failed.
 The Apache error log may have more information.
 * Restarting web server apache2
   ...fail!
 * The apache2 configtest failed.
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ****************************** 


 Single App Installer:
 --------------------------------------------
 ApacheModules: Success
 ------------------------------
 Installer Finished
 ****************************** 


opción
-------

.. cssclass:: table-bordered


 +---------------------------+---------------------------------------------------+-----------------+-----------------------------------------+
 | Parámetros	             | parámetros alternativos                           | Necesario       | Comentario                              |
 +===========================+===================================================+=================+=========================================+
 |Install Apache             | En lugar de utilizar ApacheModules también        | Y(Yes)          | Si el usuario da entrada como sí, va a  |
 |Module? (Y/N)              | podemos utilizar apachemods, apache-module,       |                 | instalar el módulo.                     |
 |                           | apachemodules                                     |                 |                                         |
 +---------------------------+---------------------------------------------------+-----------------+-----------------------------------------+
 |Install Apache             | En lugar de utilizar ApacheModules también        | N(No)           | Si el usuario da entrada como no,       |
 |Module? (Y/N)              | podemos utilizar apachemods, apache-module,       |                 | se cierra.                              |
 |                           | apachemodules|                                    |                 |                                         |
 +---------------------------+---------------------------------------------------+-----------------+-----------------------------------------+


Beneficios
-------------

* El módulo es una ayuda a Link con Cleopatra.
* Durante la instalación de los módulos de Apache, será aceptar los archivos de configuración.
* Si los archivos de configuración no están disponibles en el sistema de este módulo se instalará automáticamente.