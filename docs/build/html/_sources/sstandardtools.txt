==============
StandardTools
==============

sinopsis
----------------

Este módulo ayudar en la instalación de herramientas estándar en el sistema. Se puede instalar todas las herramientas como vim, zip, etc,. La automatización es posible. Especifica la estandarización de su entorno. Es fácil de usar con Ubuntu y CentOS.

comando Ayuda
---------------------

Comando que se utiliza para encontrar información sobre un comando especificado Ayuda. Para obtener más información acerca de las herramientas estándar. podemos utilizar este comando ayuda.

.. code-block:: bash

		ptconfigure StandardTools help

La siguiente captura de pantalla te guiará.

.. code-block:: bash

 kevell@corp:/# ptconfigure StandardTools help
 ******************************


  This command allows you to install a few GC recommended Standard Tools
  for productivity in your system.  The kinds of tools we found ourselves
  installing on every box we have, client or server. These include curl,
  vim, drush and zip.

  StandardTools, standard-tools, standardtools, stdtools, std-tools

        - install
        Installs some standard tools
        example: ptconfigure stdtools install

 ------------------------------
 End Help
 ******************************

instalación
------------------

  Como empresa y como personas, herramientas estándar se ha dedicado a responder a los retos de los usuarios, satisfaciendo sus necesidades y satisfacer sus objetivos de negocio. Es un proceso obvio para instalar un módulo de herramientas estándar bajo ptconfigure sólo por el uso de la orden dada a continuación,

.. code-block:: bash

                ptconfigure stdtools install

Después de introducir el comando,

Install standard tools? (Y/N)

Si el valor para el usuario como y

Entonces todas las herramientas estándar actualizados instalados.

Si el valor de usuario como N

Se saldrá de la pantalla

Las capturas de pantalla muestra esto.

.. code-block:: bash


 kevell@corp:/# ptconfigure stdtools install
 Install Standard Tools? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         Std. Tools!!        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 curl is already the newest version.
 0 upgraded, 0 newly installed, 0 to remove and 13 not upgraded.
 [Pharaoh Logging] Package curl from the Packager Apt is already installed, so not installing.
 Reading package lists...
 Building dependency tree...
 Reading state information...
 vim is already the newest version.
 0 upgraded, 0 newly installed, 0 to remove and 13 not upgraded.
 [Pharaoh Logging] Package vim from the Packager Apt is already installed, so not installing.

 Creating config file /etc/php5/mods-available/mysql.ini with new version
 php5_invoke: Enable module mysql for cli SAPI
 php5_invoke: Enable module mysql for fpm SAPI
 php5_invoke: Enable module mysql for apache2 SAPI

 Creating config file /etc/php5/mods-available/mysqli.ini with new version
 php5_invoke: Enable module mysqli for cli SAPI
 php5_invoke: Enable module mysqli for fpm SAPI
 php5_invoke: Enable module mysqli for apache2 SAPI
 
 Creating config file /etc/php5/mods-available/pdo_mysql.ini with new version
 php5_invoke: Enable module pdo_mysql for cli SAPI
 php5_invoke: Enable module pdo_mysql for fpm SAPI
 php5_invoke: Enable module pdo_mysql for apache2 SAPI
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
   php-console-table php5-mysql
 Suggested packages:
   drupal7
 Recommended packages:
  php-console-color
 The following NEW packages will be installed:
  drush php-console-table php5-mysql
 0 upgraded, 3 newly installed, 0 to remove and 13 not upgraded.
 Need to get 430 kB of archives.
 After this operation, 1,800 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main php5-mysql amd64 5.5.9+dfsg-1ubuntu4.5 [62.9 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/universe php-console-table all 1.1.6-1 [14.7 kB]
 Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty/universe drush all 5.10.0-2 [353 kB]
 Fetched 430 kB in 1min 4s (6,634 B/s)
 Selecting previously unselected package php5-mysql.
 (Reading database ... 212663 files and directories currently installed.)
 Preparing to unpack .../php5-mysql_5.5.9+dfsg-1ubuntu4.5_amd64.deb ...
 Unpacking php5-mysql (5.5.9+dfsg-1ubuntu4.5) ...
 Selecting previously unselected package php-console-table.
 Preparing to unpack .../php-console-table_1.1.6-1_all.deb ...
 Unpacking php-console-table (1.1.6-1) ...
 Selecting previously unselected package drush.
 Preparing to unpack .../drush_5.10.0-2_all.deb ...
 Unpacking drush (5.10.0-2) ...
 Processing triggers for libapache2-mod-php5 (5.5.9+dfsg-1ubuntu4.5) ...
 Processing triggers for php5-fpm (5.5.9+dfsg-1ubuntu4.5) ...
 php5-fpm stop/waiting
 php5-fpm start/running, process 5110
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up php5-mysql (5.5.9+dfsg-1ubuntu4.5) ...
 Setting up php-console-table (1.1.6-1) ...
 Setting up drush (5.10.0-2) ...
 Processing triggers for libapache2-mod-php5 (5.5.9+dfsg-1ubuntu4.5) ...
 Processing triggers for php5-fpm (5.5.9+dfsg-1ubuntu4.5) ...
 php5-fpm stop/waiting
 php5-fpm start/running, process 6189
 [Pharaoh Logging] Adding Package drush from the Packager Apt executed correctly
 Reading package lists...
 Building dependency tree...
 Reading state information...
 zip is already the newest version.
 0 upgraded, 0 newly installed, 0 to remove and 13 not upgraded.
 [Pharaoh Logging] Package zip from the Packager Apt is already installed, so not installing.
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************
 

 Single App Installer:
 --------------------------------------------
 StandardTools: Success
 ------------------------------
 Installer Finished
 ******************************

parámetros alternativos
----------------------------------

Los siguientes son los parámetros alternativos. StandardTools, herramientas estándar, standardtools, std-herramientas, stdtools.

Beneficios
-------------

* Versión actualizada de instalación disponible.
* En caso de existir, se puede sobrescribir.
* No mayúsculas y minúsculas
