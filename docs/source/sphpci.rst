===============
Phpci
===============

sinopsis
--------------

   PHPCI es una herramienta de integración continua de código abierto diseñado específicamente para ptconfigure. El usuario ha construido con la simplicidad en mente, así que mientras que no lo hace todo Jenkins puede hacer, es muy fácil de configurar y utilizar. Esta es la facilidad con Ubuntu y CentOS.

comando Ayuda
-----------------------

           Este comando ayuda a guiar al usuario a realizar determinada operación sobre módulo Phpci. Esto es adecuado para todo tipo de usuarios corporativos.

.. code-block:: bash
   
                ptconfigure PHPCI help

El comando help muestra una breve lista de los comandos integrados en el módulo Phpci. La siguiente captura de pantalla visualizarlo.

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPCI help
 ******************************


  This command allows you to install PHPCI, the popular Build Server.

  PHPCI, phpci

        - install
        Installs PHPCI through git, with its dependencies
        example: ptconfigure phpci install

        - config-default, default-config
        Installs a default config.yml file for PHPCI
        example: ptconfigure phpci config-default --yes --guess

        - install-default-database
        Installs a default database and user for PHPCI
        example: ptconfigure phpci install-default-database --yes --guess
            --mysql-admin-user="root" # guess will provide root
            --mysql-admin-pass="some-pass" # guess will provide ptconfigure

  You can install a complete local version of PHPCI with the following:

  sudo ptconfigure phpci install --yes --guess
  sudo ptconfigure phpci install-default-database --yes --guess
  sudo ptconfigure phpci config-default --yes --guess

 ------------------------------
 End Help
 ******************************


instalación
-----------------

  Este módulo ayuda a instalar phpci. El primer paso de este módulo tiene que comprobar compositor está disponible en el sistema o no. Si no está disponible en el sistema de forma automática, se instale.

.. code-block:: bash

                   ptconfigure Phpci install

Después de introducir el comando anterior, el siguiente proceso están involucrados durante el proceso de instalación como se muestra en el formato tabular,

.. cssclass:: table-bordered

 +--------------------------+---------------------------------------+-------------+--------------------------------------------------+
 | Parámetros               | Parámetro Alternativa                 | Opciones    | Comentarios                                      |
 +==========================+=======================================+=============+==================================================+
 |Install PHPCI? (Y/N)      | En lugar de PHPCI, podemos utilizar   | Y(Yes)      | Si el usuario desea continuar el proceso de      |
 |                          | phpci también.                        |             | instalación se puede introducir como Y.          |
 +--------------------------+---------------------------------------+-------------+--------------------------------------------------+
 |Install PHPCI? (Y/N)      | En lugar de PHPCI, podemos utilizar   | N(No)       | Si el usuario desea abandonar el proceso de      |
 |                          | phpci también.                        |             | instalación se puede introducir como N.|         |
 +--------------------------+---------------------------------------+-------------+--------------------------------------------------+

Si la instalación procede de usuario, durante el proceso de instalación de los siguientes pasos están involucrados,

* Construye el árbol de dependencias.
* Lee la información de estado.
* Lista outs los paquetes adicionales que se instalan automáticamente.
* Lista outs los paquetes sugeridos que está instalando.
* Lista outs los nuevos paquetes que está instalando.
* Detalles sobre el número de archivos actualizados, recién instalados, retirados y no actualizados.

Y entonces, lo hará pide aportaciones de los usuarios, tal como se representa en forma de tabla

.. cssclass:: table-bordered


 +-------------------------+-----------------------------+---------------+-------------------------------------------------------------+
 | Parámetros              | camino                      | Opciones      | Comentarios                                                 |
 +=========================+=============================+===============+=============================================================+
 |Program data directory   | “/opt/phpunit (módulo       | Y(Yes)        | Si el usuario de proceder con la instalación del directorio |
 |(Por defecto)            | correspondiente)”           |               | de datos de programa predeterminado que puede introducir    |
 |                         |                             |               | como Sí                                                     |
 +-------------------------+-----------------------------+---------------+-------------------------------------------------------------+
 |Program data directory   | específica de usuario       | N(Fin barra)  | Si el usuario desea continuar con su propio directorio de   |
 |                         |                             |               | datos del programa, pueden de entrada como N, y en la mano  |
 |                         |                             |               | especificar que poseen ubicación.                           |
 +-------------------------+-----------------------------+---------------+-------------------------------------------------------------+
 |Program executor         | “/usr/bin”                  | Yes           | Si el usuario de proceder con la instalación del directorio |
 |directory (Por defecto)  |                             |               | ejecutor programa predeterminado que puede introducir       |
 |                         |                             |               | como Sí                                                     |
 +-------------------------+-----------------------------+---------------+-------------------------------------------------------------+
 |Program executor         | específica de usuario       | N(Fin barra)  | Si el usuario desea continuar con su propio directorio      |
 |directory                |                             |               | ejecutor del programa, pueden de entrada como N, y en la    |
 |                         |                             |               | mano especificar que poseen ubicación.|                     |
 +-------------------------+-----------------------------+---------------+-------------------------------------------------------------+

La siguiente captura de pantalla representa gráficamente el proceso anteriormente descrito de la instalación.

.. code-block:: bash

 kevell@corp:/#  ptconfigure phpci install
 Install PHPCI? (Y/N)
 Y
 *******************************
 *        Pharaoh Tools        *
 *          ! PHPCI !        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libmcrypt4
 Suggested packages:
  libmcrypt-dev mcrypt
 The following NEW packages will be installed:
  libmcrypt4 php5-mcrypt
 0 upgraded, 2 newly installed, 0 to remove and 301 not upgraded.
 Need to get 77.3 kB of archives.
 After this operation, 324 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libmcrypt4 amd64 2.5.8-3.1ubuntu1 [61.9 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/universe php5-mcrypt amd64 5.4.6-0ubuntu5 [15.4 kB]
 Fetched 77.3 kB in 4s (19.1 kB/s)
 Selecting previously unselected package libmcrypt4.
 (Reading database ... 182037 files and directories currently installed.)
 Preparing to unpack .../libmcrypt4_2.5.8-3.1ubuntu1_amd64.deb ...
 Unpacking libmcrypt4 (2.5.8-3.1ubuntu1) ...
 Selecting previously unselected package php5-mcrypt.
 Preparing to unpack .../php5-mcrypt_5.4.6-0ubuntu5_amd64.deb ...
 Unpacking php5-mcrypt (5.4.6-0ubuntu5) ...
 Setting up libmcrypt4 (2.5.8-3.1ubuntu1) ...
 Setting up php5-mcrypt (5.4.6-0ubuntu5) ...
 Processing triggers for libc-bin (2.19-0ubuntu6) ...
 [Pharaoh Logging] Adding Package php5-mcrypt from the Packager Apt executed correctly
 Creating /tmp/ptconfigure-temp-script-82480901916.sh
 chmod 755 /tmp/ptconfigure-temp-script-82480901916.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-82480901916.sh Permissions
 Executing /tmp/ptconfigure-temp-script-82480901916.sh
 Temp File /tmp/ptconfigure-temp-script-82480901916.sh Removed
 Creating /tmp/ptconfigure-temp-script-43828918328.sh
 chmod 755 /tmp/ptconfigure-temp-script-43828918328.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-43828918328.sh Permissions
 Executing /tmp/ptconfigure-temp-script-43828918328.sh
 Enabling module rewrite.
 To activate the new configuration, you need to run:
  service apache2 restart
 Temp File /tmp/ptconfigure-temp-script-43828918328.sh Removed
 [Pharaoh Logging] Ensure module install is not checking versions
 sh: 1: composer: not found
 [Pharaoh Logging] Module Composer reports itself as Not Installed
 [Pharaoh Logging] Installing as not installed
 *******************************
 *        Pharaoh Tools        *
 *          Composer!         *
 *******************************
 What is the program data directory? Found "/opt/composer" - use this? (Enter nothing for yes, no end slash)
 
 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'https://github.com/phpengine/composer-phar.git'  /tmp/composer/composerCloning into '/tmp/composer/composer'...


 remote: Counting objects: 6, done.
 remote: Total 6 (delta 0), reused 0 (delta 0)
 Unpacking objects: 100% (6/6), done.
 Checking connectivity... done.
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 Creating /tmp/ptconfigure-temp-script-34508236330.sh
 chmod 755 /tmp/ptconfigure-temp-script-34508236330.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-34508236330.sh Permissions
 Executing /tmp/ptconfigure-temp-script-34508236330.sh
 #!/usr/bin/env php
 Installing block8/phpci (1.5.2)
  - Installing block8/phpci (1.5.2)
    Downloading: 100%

 Created project in phpci
 Loading composer repositories with package information
 Installing dependencies from lock file
 Warning: The lock file is not up to date with the latest changes in composer.json. You may be getting outdated dependencies. Run update to update them.
 Your requirements could not be resolved to an installable set of packages.

  Problem 1
    - The requested PHP extension ext-pdo_mysql * is missing from your system.

 Temp File /tmp/ptconfigure-temp-script-34508236330.sh Removed
 Creating /tmp/ptconfigure-temp-script-28990655696.sh
 chmod 755 /tmp/ptconfigure-temp-script-28990655696.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-28990655696.sh Permissions
 Executing /tmp/ptconfigure-temp-script-28990655696.sh
 sudo: dapperstrano: command not found
 Temp File /tmp/ptconfigure-temp-script-28990655696.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PHPCI: Success
 ------------------------------
 Installer Finished
 ******************************

Beneficios
------------

* PHPCI utiliza para instalar el archivo de configuración y la base de datos. Durante la instalación si hay algún archivo existente, 
  sobrescribir el contenido.
* La nueva versión puede actualizar automáticamente.
* Se puede aceptar el deseo del usuario en caso de instalar la base de datos.
* La integración continua es posible.
* Entorno múltiple
* Construir php con diferentes variantes como DOP, mysql, sqlite, depuración ... etc.
* Detección automática de características.
