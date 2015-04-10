==============
DBInstall
==============

Sinopsis
-------------

Dbinstall módulo ayuda en el manejo de las funciones de instalación de base de datos. Este comando utiliza para instalar una nueva base de datos. La instalación requiere acceso sudo, o tiene que ser ejecutado como root. Esto incluye la ejecución del comando rpm, o el comando miminstall del paquete de alquitrán, y también cuando se utiliza el comando dbinstall que crea una base de datos inicial.

Si bien la creación de una base de datos inicial, que ha instalado el software usted puede construir una base de datos SQL Mimer utilizando el comando dbinstall.

Acabamos de instalar una nueva base de datos en un servidor Linux (CentOS) y cuando intento conectar a la base de datos (desde el servidor) que requiere el nombre de base de datos en la cadena de conexión. Como se mencionó antes, el comando dbinstall requiere acceso sudo, o debe ser ejecutado por root. Si no se ha iniciado desde un shell contraseña sudo privilegiada se le pedirá.

Durante la sesión dbinstall, nombre de la base de datos, la ubicación de base de datos, y la contraseña del administrador de base de datos (es decir, SYSADM) debe ser especificado. También habrá opciones para instalar entornos de ejemplo, etc. Cuando se termina la sesión, una base de datos totalmente operativa está disponible - habilitado para acceso de cliente / servidor a través de TCP y arranque automático al iniciar el sistema.

Ayuda Comando
----------------------

Este comando ayuda a determinar el uso del módulo DBinstall. El usuario se llega a saber acerca de las diferentes formas / formato para ejecutar este módulo. Este comando guía al usuario final a conocer el propósito de este comando. A continuación dado son el comando y la captura de pantalla de la misma.

.. code-block:: bash
	
	ptdeploy DBInstall help

La representación gráfica de la orden anterior se muestra a continuación,

.. code-block:: bash

 kevell@corp:/# ptdeploy DBInstall help
 ******************************


  This command is part of Default Modules and handles Database Installation Functions.

  DBInstall, db-install, dbinstall

          - install
          install the database for a project. run DBConfigure first to set up users unless you already have them.
          example: ptdeploy db-install install

          - save
          save the database for a project. run DBConfigure first to set up users unless you already have them.
          example: ptdeploy db-install save

          - drop
          drop the database for a project.
          example: ptdeploy db-install drop

      
 --------------
  Wordpress Module:

  The Wordpress module extends DBInstall by adding wordpress-install

  Wordpress module adds the actions wordpress-install and wp-install to DBInstall, requiresd to allow the Post DB
  Install hooks for Wordpress, the DB restore won't work correctly without at least the url.

  ptdeploy dbinstall wordpress-install --yes --guess --hook-url=www.site.env
 ------------------------------
 End Help
 ******************************

Instalation
----------------

Cuando el usuario tiene que instalar, el usuario puede ejecutar los siguientes comandos para DBIstall. El sistema ejecutará el proceso de instalación.

.. code-block:: bash
	
	 ptdeploy dbinstall install

.. code-block:: bash


 kevell@corp:/# ptdeploy DBInstall install
 Do you want to install a database? (Y/N) 
 y
 What's the Mysql Host? Enter for 127.0.0.1 

 What's the MySQL Admin User? 

 You must enter a value. Please try again.
 What's the MySQL Admin User?

 You must enter a value. Please try again.
 What's the MySQL Admin User?
 root
 What's the MySQL Admin Password?
 root
 What's the application DB User?
 (0) **CREATE NEW USER** 
 (1) phpci 
 (2) debian-sys-maint 
 (3) phpci 
 (4) phpmyadmin 
 1
 What's the application DB Password?
 phpci_pass
 What's the application DB Name?
 Current Db's are:
 hps
 phpci
 phpmyadmin

 phpci
 Database script executed
 **************************************
 Seems Fine...Database Actions Finished
 **************************************


Save
-------

Cuando el usuario necesita para salvar a la base de datos para un proyecto, el siguiente comando dado se ejecutará el proceso.

.. code-block:: bash
	
	ptdeploy DBInstall save

.. code-block:: bash


 kevell@corp:/# ptdeploy DBInstall save
 Do you want to save a database? (Y/N) 
 y
 What's the Mysql Host? Enter for 127.0.0.1

 What's the MySQL Admin User?
 root
 What's the MySQL Admin Password?
 root
 What's the application DB Name?
 Current Db's are:
 asdf
 hps
 phpci 

 asdf
 Cannot connect with these details. Sure you want to continue? (Y/N) 
 y
 Exporting DB to /opt/db/database.sql 
 Database Dumping...
 **************************************
 Seems Fine...Database Actions Finished
 ************************************** 


Drop
----------------

Cuando el usuario necesita para dejar la base de datos para un proyecto, el siguiente comando dado se ejecutará el proceso.

.. code-block:: bash
	
	ptdeploy dbinstall drop      

.. code-block:: bash


 kevell@corp:/# ptdeploy db-install drop 

 Do you want to perform drop actions (user/db)? (Y/N) 
 y
 Do you want to drop a database? (Y/N) 
 y
 What's the Mysql Host? Enter for 127.0.0.1 

 What's the MySQL Admin User?
 root
 What's the MySQL Admin Password?
 root123
 What's the application DB Name?
 (0) karuna 
 (1) test1 
 (2) test2 
 2
 Database test2 dropped
 **************************************
 Seems Fine...Database Actions Finished
 **************************************




Parámetro Alternativa
------------------------------

Cualquiera de los tres parámetros alternativa se puede utilizar en mandamiento dbinstall, DBInstall and db-install

por ejemplo: ptdeploy DBInstall help/  ptdeploy db-install help      

Beneficios
--------------

* Se comprobará y verificará todas las dependencias para el paquete que está instalando
* Esto ejecutará dbconfigure primero para configurar los usuarios a menos que el sistema ya los tiene
* Dbinstall crea todas las bases de datos del sistema en el directorio de inicio del servidor de base de datos dada           
