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

 kevell@corp:/#ptconfigure PHPCI install
 Install PHPCI? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *          ! PHPCI !        *
 *******************************
 [Pharaoh Logging] Packages php5-mcrypt, curl from the Packager Apt are already installed, so not installing
 Creating /tmp/ptconfigure-temp-script-45785693692.sh
 chmod 755 /tmp/ptconfigure-temp-script-45785693692.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-45785693692.sh Permissions
 Executing /tmp/ptconfigure-temp-script-45785693692.sh
 Temp File /tmp/ptconfigure-temp-script-45785693692.sh Removed
 Creating /tmp/ptconfigure-temp-script-47686609771.sh
 chmod 755 /tmp/ptconfigure-temp-script-47686609771.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-47686609771.sh Permissions
 Executing /tmp/ptconfigure-temp-script-47686609771.sh
 Module rewrite already enabled
 Temp File /tmp/ptconfigure-temp-script-47686609771.sh Removed
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module Composer reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 Creating /tmp/ptconfigure-temp-script-71236381661.sh
 chmod 755 /tmp/ptconfigure-temp-script-71236381661.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-71236381661.sh Permissions
 Executing /tmp/ptconfigure-temp-script-71236381661.sh
 Installing block8/phpci (1.6.0)
   - Installing block8/phpci (1.6.0)
    Loading from cache

 Created project in phpci
 Loading composer repositories with package information
 Installing dependencies from lock file
  - Installing symfony/yaml (v2.6.4)
    Loading from cache

  - Installing block8/b8framework (1.1.9)
    Loading from cache

  - Installing ircmaxell/password-compat (v1.0.4)
    Loading from cache

  - Installing psr/log (1.0.0)
    Loading from cache

  - Installing monolog/monolog (1.12.0)
    Loading from cache

  - Installing pimple/pimple (v1.1.1)
    Loading from cache

  - Installing symfony/console (v2.6.4)
    Loading from cache

  - Installing symfony/filesystem (v2.6.4)
    Loading from cache

  - Installing symfony/config (v2.6.4)
    Loading from cache

  - Installing robmorgan/phinx (v0.4.2.1)
    Loading from cache

  - Installing swiftmailer/swiftmailer (v5.3.1)
    Loading from cache

 Generating autoload files
 Temp File /tmp/ptconfigure-temp-script-42085224634.sh Removed
 Creating /tmp/ptconfigure-temp-script-47565859655.sh
 chmod 755 /tmp/ptconfigure-temp-script-47565859655.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-47565859655.sh Permissions
 Executing /tmp/ptconfigure-temp-script-47565859655.sh
 [Pharaoh Logging] Lets begin Configuration of a Web Server for PHPCI
 [Pharaoh Logging] Lets Add our Apache VHost
 [Pharaoh Logging] Now lets restart Apache so we are serving our new application 

 Logging Starting
 Logging Complete
 Logging Starting
 Logging Complete
 <VirtualHost 127.0.0.1:80>
	ServerAdmin webmaster@localhost
	ServerName www.phpci.local
	DocumentRoot /opt/phpci/phpci/public/
	<Directory /opt/phpci/phpci/public/>
		Options Indexes FollowSymLinks MultiViews
		AllowOverride All
		Require all granted

        <IfModule mod_rewrite.c>
          RewriteEngine On
          RewriteBase /opt/phpci/phpci/public/
          RewriteCond %{REQUEST_FILENAME} !-f
          RewriteCond %{REQUEST_FILENAME} !-d
          RewriteRule . /index.php [L]
        </IfModule>

	</Directory>

 </VirtualHost>

 Assuming Okay due to yes parameter
 Site www.phpci.local already enabled
 a2ensite www.phpci.local done
 Logging Starting
 Logging Complete
 Temp File /tmp/ptconfigure-temp-script-47565859655.sh Removed
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

.. code-block:: bash

 kevell@corp:/#ptconfigure PHPCI config-default

 Install PHP CI Default Configuration? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         PHPCI Defaults        *
 *******************************
 Set non-default value for db_read_host? Default is 127.0.0.1 (Y/N) 
 n
 Set non-default value for db_write_host? Default is 127.0.0.1 (Y/N) 
 n
 Set non-default value for db_name? Default is phpci (Y/N) 
 n
 Set non-default value for db_username? Default is phpci (Y/N) 
 n
 Set non-default value for db_pass? Default is phpci_pass (Y/N) 
 n
 Set non-default value for phpci_url? Default is http://www.phpci.local (Y/N) 
 n
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ****************************** 

 Single App Installer:
 --------------------------------------------
 No Data.
 ------------------------------
 Installer Finished
 ****************************** 

.. code-block:: bash


 kevell@corp:/#ptconfigure phpci install-default-database
 Install PHPCI? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *          ! PHPCI !        *
 *******************************
 What's the MySQL Admin User?
 root
 What's the MySQL Admin Password?
 root
 Database script executed
 ******************************  

 Seems Fine...Database Actions Finished
 ******************************

 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ****************************** 

 Single App Installer:
 --------------------------------------------
 No Data.
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
