==============
PTDeploy
==============

sinopsis
------------

El ptdeploy envuelve las aplicaciones de los usuarios con la implementación automatizada, construir y lanzar funciones, aplicación web de control de versiones y la infraestructura de código en PHP.

Es a aliviar los usuarios y proporciona plantillas de implementación automatizadas e instala una acumulación totalmente continua para su proyecto.

Ayuda Comando
---------------------

Si quieres saber el propósito de un módulo en particular, sólo tienes que escribir el comando de la siguiente manera:

.. code-block:: bash
	
		ptdeploy ModuleName help

este comando proporcionará el uso de ese módulo en particular y también las opciones disponibles en las acciones que se pueden realizar. La captura de pantalla se muestra bajo explica el uso del control apache módulo bajo ptdeploy usando el comando help.

.. code-block:: bash

 kevell@corp:/# ptdeploy ApacheControl help
 ******************************


  This command is part of Default Modules and handles Apache Server Control Functions.

  ApacheControl, apachecontrol, apachectl

          - start
          Start the Apache server
          example: ptdeploy apachecontrol start
          example: ptdeploy apachecontrol start --yes --guess
          example: ptdeploy apachecontrol start --yes --apache-command="apache2"

          - stop
          Stop the Apache server
          example: ptdeploy apachecontrol stop
          example: ptdeploy apachecontrol stop --yes --guess
          example: ptdeploy apachecontrol stop --yes --apache-command="apache2"

          - restart
          Restart the Apache server
          example: ptdeploy apachecontrol restart
          example: ptdeploy apachecontrol restart --yes --guess
          example: ptdeploy apachecontrol restart --yes --apache-command="apache2"

          - reload
          Reloads the Apache server configuration without restarting
          example: ptdeploy apachecontrol reload
          example: ptdeploy apachecontrol reload --yes --guess
          example: ptdeploy apachecontrol reload --yes --apache-command="apache2"

 ------------------------------
 End Help
 ******************************


El comando de ayuda también se indican los parámetros alternativos que se pueden utilizar en la declaración.



¿Por qué construir este ptdeploy
------------------------------------------

Con el fin de construir para el bienestar de la implementación, se necesitan muchos archivos a copiar de FTP u otras soluciones ad hoc. Y también gran cantidad de herramientas de automatización Empresa faltaban. Para superar estas carencias ptdeploy bajo la herramienta faraón eran acumule.

PHP tiene ptdeploy tan rubí fiils la brecha en Capistrano.

Esta herramienta es para aplicaciones de provisiones y construye a sus cajas. El usuario puede configurar aún patrón de despliegue de aplicaciones simples o complejas a su sistema con uno o dos archivos PHP o, de forma rápida patrones de despliegue amigables de configuración en la nube.

ptdeploy es modular. orientado a objetos y extensible. Así que si el usuario requiere ningún módulo extra que pueden crear y añadir los nuevos módulos en función de sus necesidades.

Este ptdeploy actúa como un contenedor en el que todos los pasos de despliegue usuarios se cubre en un solo archivo. Esto permite el uso de un solo comando para arrancar una instancia de sus aplicaciones.

Instalación
---------------

Instalación del ptdeploy se puede hacer de dos maneras posibles, dependiendo de la disponibilidad y requerimientos de los usuarios. Ellos dos formas de instalar ptdeploy son:

* Instalación ptdeploy través ptconfigure
* Instalación de la ptdeploy sin depender de ptconfigure.



Instalación ptdeploy través ptconfigure
-------------------------------------------------

Si el usuario tiene la ptconfigure en su máquina, entonces es la manera más sencilla de instalar ptdeploy utilizando el siguiente comando:

.. code-block:: bash

	sudo ptconfigure ptdeploy install --yes --guess

Instalación del ptdeploy sin depender de ptconfigure
-------------------------------------------------------------------------------

Si el usuario desea instalar el ptdeploy sin depender y utilizando el ptconfigure que pueden utilizar el siguiente comando:

.. code-block:: bash
		
	sudo apt-get install php5 git

.. code-block:: bash

	git clone https://git.pharaoh-tools.com/phpengine/ptdeploy && sudo php ptdeploy/install-silent

o

El siguiente comando es predecible para los usuarios que deseen especificar la ubicación durante la instalación.

.. code-block:: bash

	git clone https://git.pharaoh-tools.com/phpengine/ptdeploy && sudo php ptdeploy/install

Las funciones avanzadas
-------------------------

Edición de los archivos de host, los archivos de la máquina virtual, archivos de configuración, actualizaciones de bases de datos y más pueden ser automatizadas usando esto.

Mediante el uso de la capacidad de gestión de servidor remoto, los usuarios pueden automatizar despliegues en toda la infraestructura de cualquier tamaño.

La manera cómo el ptdeploy promueve su proyecto usando dapperfy
-------------------------------------------------------------------------------------------

La palabra dapperfy es un comando ptdeploy que crea algunos pilotos automáticos para su proyecto.

Utilizando el dapperfy es muy rápido, y es probablemente el mejor punto de partida.

Capify Vs Dapperfy
-------------------------

Al comparar la capify con dapperfy, es obvio decir que la dapperfy es la mejor, ya que está escrito en PHP.

El punto fuerte es que el comando ptdeploy dapperfy ofrece el conjunto estándar de los pilotos automáticos de los proyectos de los usuarios. donde el capify ofrece funciones similares al proyecto Ruby.

Cómo utilizar y módulos disponibles
-----------------------------------------------

Veamos, cómo utilizar la herramienta ptdeploy, primero, simplemente escriba como

.. code-block:: bash

		ptdeploy

este comando listará todos los nombres de los módulos que están disponibles bajo ptdeploy.

* ApacheControl - Apache Server Control
* ApacheVHostEditor - Apache Virtual Host Functions
* AppSettings - PTDeploy Application Settings
* Autopilot - PTConfigure Autopilot - User Defined Installations
* Builderfy - PTDeploy Builderfyer - Create some standard autopilots for your project
* CukeConf - Cucumber Configuration
* DBConfigure - Database Connection Configuration Functions
* DBInstall - Database Installation Management Functions
* Dapperfy - PTDeploy Dapperfyer - Automated Application Deployment autopilots for your project
* Drupal - Drupal - Integration and Templates for Drupal
* EnvironmentConfig - Environment Configuration - Configure Environments for a project
* GitClone - GitClone Source Control Clone Functions
* HostEditor - Host File Management Functions
* Invoke - SSH Invocation Functions
* Joomla - Joomla - Integration and Templates for Joomla
* LighttpdControl - Lighttpd Server Control
* Logging - Logging - Output errors to the logging
* NginxControl - Nginx Server Control
* NginxSBEditor - Nginx Server Block Functions
* ParallelSshChild - Command Execution Functions
* Project - PTDeploy Project Management Functions
* RunCommand - Execute a Command
* SFTP - SFTP Functionality
* SVN - SVN Source Control Project Checkout/Download Functions
* SystemDetection - System Detection - Detect the Running Operating System
* Templating - Templating
* Version - Versioning Functions
* Wordpress - Wordpress - Integration and Templates for Wordpress


aquí, la pantalla indica la pantalla de todos los módulos disponibles bajo ptconfigure.

.. code-block:: bash

 Comandos disponibles:
 --------------------------------------- 

 ApacheControl - Apache Server Control
 ApacheVHostEditor - Apache Virtual Host Functions
 AppSettings - PTDeploy Application Settings
 Autopilot - PTConfigure Autopilot - User Defined Installations
 Builderfy - PTDeploy Builderfyer - Create some standard autopilots for your project
 CukeConf - Cucumber Configuration
 DBConfigure - Database Connection Configuration Functions
 DBInstall - Database Installation Management Functions
 Dapperfy - PTDeploy Dapperfyer - Automated Application Deployment autopilots for your project
 Drupal - Drupal - Integration and Templates for Drupal
 EnvironmentConfig - Environment Configuration - Configure Environments for a project
 GitClone - GitClone Source Control Clone Functions
 HostEditor - Host File Management Functions
 Invoke - SSH Invocation Functions
 Joomla - Joomla - Integration and Templates for Joomla
 LighttpdControl - Lighttpd Server Control
 Logging - Logging - Output errors to the logging
 NginxControl - Nginx Server Control
 NginxSBEditor - Nginx Server Block Functions
 ParallelSshChild - Command Execution Functions
 Project - PTDeploy Project Management Functions
 RunCommand - Execute a Command
 SFTP - SFTP Functionality
 SVN - SVN Source Control Project Checkout/Download Functions
 SystemDetection - System Detection - Detect the Running Operating System
 Templating - Templating
 Version - Versioning Functions
 Wordpress - Wordpress - Integration and Templates for Wordpress

******************************



.. toctree::
   :maxdepth: 6
   

 sapachecontrol_deploy
 sapachevhosteditor_deploy
































