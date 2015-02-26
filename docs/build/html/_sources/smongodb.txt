==========
MongoDB
==========

sinopsis
-------------

Mongo DB es una base de datos orientada documento. Mongo DB evita la estructura de base de datos relacional basado en tablas tradicional a favor de php como documentos con esquemas dinámicos, por lo que la integración de los datos en ciertos tipos de aplicaciones más fácil y más rápido. Mongo DB es adecuado para trabajar con Ubuntu y CentOS.

comando Ayuda
--------------------

              Este comando puede funcionar sobre los objetivos y los comandos disponibles bajo módulo Mongo DB. También explica el comando para instalar el servidor.

.. code-block:: bash

 		ptconfigure MongoDB help

Antes de la instalación de leer este comando help explica su función

.. code-block:: bash


   kevell@corp:/# ptconfigure MongoDB help
   ******************************


  This command allows you to install the MongoDB Server. Currently only
  MongoDB Workbench, the Database management GUI provided by Oracle for
  MongoDB.

  MongoDB, mongo-db-server, mongodb-server, mongodbserver, mongodb, mongo-db

        - install
        Install MongoDB Server
        example: ptconfigure mongodb install

  Notes, during mongodb install a root password will be set. First, it'll look
  for the parameter --mongodb-root-pass, if this is not set, it'll look in the
  ptconfigure config for a mongodb-default-root-pass setting, and failing both of
  those it will just set the password for root to ptconfigure.

 ------------------------------
 End Help
 ******************************

instalación
-------------

Utilice este módulo para instalar Mongo DB en sistemas Ubuntu Linux de paquetes .deb. Mientras que Ubuntu incluye sus propios paquetes de Mongo DB, los paquetes oficiales de Mongo DB son generalmente más up-to-fecha.

.. code-block:: bash

	ptconfigure mongodb-server install

Install mongo DB server?(Y/N)

Si el usuario presta No saldrá.

Cuando el usuario da entrada como Sí automáticamente se instalarán todos depencies en pasada de raíz culo defecto y también instalar la versión actualizada. La siguiente captura de pantalla de lo explicará.

.. code-block:: bash

	kevell@corp:/# ptconfigure mongodb-server install

	Install MongoDB Server? (Y/N) 
	y
	*******************************
	*        Pharaoh Tools        *
	*         MongoDB Server!        *
	*******************************
	[Pharaoh Logging] Package mongodb-client from the Packager Apt is already installed, so not installing
	Reading package lists...
	Building dependency tree...
	Reading state information...
	The following extra packages will be installed:
	 libboost-filesystem1.54.0 libboost-program-options1.54.0
	 libboost-thread1.54.0 libgoogle-perftools4 libpcrecpp0 libsnappy1
	 libtcmalloc-minimal4 libunwind8 libv8-3.14.5 mongodb-clients
	The following NEW packages will be installed:
	 libboost-filesystem1.54.0 libboost-program-options1.54.0
	 libboost-thread1.54.0 libgoogle-perftools4 libpcrecpp0 libsnappy1
	 libtcmalloc-minimal4 libunwind8 libv8-3.14.5 mongodb-clients mongodb-server
	0 upgraded, 11 newly installed, 0 to remove and 6 not upgraded.
	Need to get 14.6 MB of archives.
	After this operation, 114 MB of additional disk space will be used.
	Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main libboost-filesystem1.54.0 amd64 1.54.0-4ubuntu3.1 [34.2 kB]
	Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main libboost-program-options1.54.0 amd64 1.54.0-4ubuntu3.1 [115 kB]
	Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main libboost-thread1.54.0 amd64 1.54.0-4ubuntu3.1 [26.5 kB]
	Get:4 http://in.archive.ubuntu.com/ubuntu/ trusty/main libpcrecpp0 amd64 1:8.31-2ubuntu2 [14.5 kB]
	Get:5 http://in.archive.ubuntu.com/ubuntu/ trusty/main libunwind8 amd64 1.1-2.2ubuntu3 [48.3 kB]
	Get:6 http://in.archive.ubuntu.com/ubuntu/ trusty/main libtcmalloc-minimal4 amd64 2.1-2ubuntu1 [104 kB]
	Get:7 http://in.archive.ubuntu.com/ubuntu/ trusty/main libgoogle-perftools4 amd64 2.1-2ubuntu1 [184 kB]
	Get:8 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libv8-3.14.5 amd64 3.14.5.8-5ubuntu2 [1,189 kB]
	Get:9 http://in.archive.ubuntu.com/ubuntu/ trusty/main libsnappy1 amd64 1.1.0-1ubuntu1 [11.2 kB]
	Get:10 http://in.archive.ubuntu.com/ubuntu/ trusty/universe mongodb-clients amd64 1:2.4.9-1ubuntu2 [9,595 kB]
	Get:11 http://in.archive.ubuntu.com/ubuntu/ trusty/universe mongodb-server amd64 1:2.4.9-1ubuntu2 [3,312 kB]
	Fetched 14.6 MB in 39s (370 kB/s)
	Selecting previously unselected package libboost-filesystem1.54.0:amd64.
	(Reading database ... 202899 files and directories currently installed.)
	
	Preparing to unpack .../libboost-filesystem1.54.0_1.54.0-4ubuntu3.1_amd64.deb ...
	Unpacking libboost-filesystem1.54.0:amd64 (1.54.0-4ubuntu3.1) ...
	Selecting previously unselected package libboost-program-options1.54.0:amd64.
	Preparing to unpack .../libboost-program-options1.54.0_1.54.0-4ubuntu3.1_amd64.deb ...
	Unpacking libboost-program-options1.54.0:amd64 (1.54.0-4ubuntu3.1) ...
	Selecting previously unselected package libboost-thread1.54.0:amd64.
	Preparing to unpack .../libboost-thread1.54.0_1.54.0-4ubuntu3.1_amd64.deb ...
	Unpacking libboost-thread1.54.0:amd64 (1.54.0-4ubuntu3.1) ...
	Selecting previously unselected package libpcrecpp0:amd64.
	Preparing to unpack .../libpcrecpp0_1%3a8.31-2ubuntu2_amd64.deb ...
	Unpacking libpcrecpp0:amd64 (1:8.31-2ubuntu2) ...
	Selecting previously unselected package libunwind8.
	Preparing to unpack .../libunwind8_1.1-2.2ubuntu3_amd64.deb ...
	Unpacking libunwind8 (1.1-2.2ubuntu3) ...
	Selecting previously unselected package libtcmalloc-minimal4.
	Preparing to unpack .../libtcmalloc-minimal4_2.1-2ubuntu1_amd64.deb ...
	Unpacking libtcmalloc-minimal4 (2.1-2ubuntu1) ...
	Selecting previously unselected package libgoogle-perftools4.
	Preparing to unpack .../libgoogle-perftools4_2.1-2ubuntu1_amd64.deb ...
	Unpacking libgoogle-perftools4 (2.1-2ubuntu1) ...
	Selecting previously unselected package libv8-3.14.5.
	Preparing to unpack .../libv8-3.14.5_3.14.5.8-5ubuntu2_amd64.deb ...
	Unpacking libv8-3.14.5 (3.14.5.8-5ubuntu2) ...
	Selecting previously unselected package libsnappy1.
	Preparing to unpack .../libsnappy1_1.1.0-1ubuntu1_amd64.deb ...
	Unpacking libsnappy1 (1.1.0-1ubuntu1) ...
	Selecting previously unselected package mongodb-clients.
	Preparing to unpack .../mongodb-clients_1%3a2.4.9-1ubuntu2_amd64.deb ...
	Unpacking mongodb-clients (1:2.4.9-1ubuntu2) ...
	Selecting previously unselected package mongodb-server.
	Preparing to unpack .../mongodb-server_1%3a2.4.9-1ubuntu2_amd64.deb ...
	Unpacking mongodb-server (1:2.4.9-1ubuntu2) ...
	Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
	Processing triggers for ureadahead (0.100.0-16) ...
	Setting up libboost-filesystem1.54.0:amd64 (1.54.0-4ubuntu3.1) ...
	Setting up libboost-program-options1.54.0:amd64 (1.54.0-4ubuntu3.1) ...
	Setting up libboost-thread1.54.0:amd64 (1.54.0-4ubuntu3.1) ...
	Setting up libpcrecpp0:amd64 (1:8.31-2ubuntu2) ...
	Setting up libunwind8 (1.1-2.2ubuntu3) ...
	Setting up libtcmalloc-minimal4 (2.1-2ubuntu1) ...
	Setting up libgoogle-perftools4 (2.1-2ubuntu1) ...
	Setting up libv8-3.14.5 (3.14.5.8-5ubuntu2) ...
	Setting up libsnappy1 (1.1.0-1ubuntu1) ...
	Setting up mongodb-clients (1:2.4.9-1ubuntu2) ...
	Setting up mongodb-server (1:2.4.9-1ubuntu2) ...
	Adding system user `mongodb' (UID 120) ...
	Adding new user `mongodb' (UID 120) with group `nogroup' ...
	Not creating home directory `/home/mongodb'.
	Adding group `mongodb' (GID 128) ...
	Done.
	Adding user `mongodb' to group `mongodb' ...
	Adding user mongodb to group mongodb
	Done.
	mongodb start/running, process 17270
	Processing triggers for libc-bin (2.19-0ubuntu6.4) ...
	Processing triggers for ureadahead (0.100.0-16) ...
	[Pharaoh Logging] Adding Package mongodb-server from the Packager Apt executed correctly
	... All done!
	*******************************
	Thanks for installing , visit www.pharaohtools.com for more
	******************************


	Single App Installer:
	--------------------------------------------
	MongoDB: Success
	------------------------------
	Installer Finished
	******************************

Opciones
------------

.. cssclass:: table-bordred

 +-------------------------+-----------------------------------------------------+-------------+--------------------------------------+
 | Parámetros              | Parámetro Alternativa                               | Opciones    | Comentarios                          |
 +=========================+=====================================================+=============+======================================+
 |Install MongoDB Server?  | En lugar de mongodb, las siguientes alternativas    | Yes         | Se instala MongoDB bajo ptconfigure  |
 |(Y/N)                    | también se pueden utilizar: MongoDB,                |             |                                      |
 |                         | mongo-db-server,mongo-db, mongodb-server, mongodb   |             |                                      |
 +-------------------------+-----------------------------------------------------+-------------+--------------------------------------+
 |Install MongoDB Server?  | En lugar de mongodb, las siguientes alternativas    | No          | sale.                                |
 |(Y/N)                    | también se pueden utilizar: MongoDB,                |             |                                      |
 |                         | mongo-db-server,mongo-db, mongodb-server, mongodb|  |             |                                      |
 +-------------------------+-----------------------------------------------------+-------------+--------------------------------------+


Beneficios
-------------

* Mongo DB es orientado documento base de datos.
* Mongo DB puede actualizada la versión más reciente.
* Durante la instalación de mongo DB todas depencies, las bibliotecas también se instala automáticamente sin tener que buscar desde la web.
* MongoDB puede almacenar el tema de negocios en el número mínimo de documentos.
* Mejoras de velocidad.
* Gran ventaja de balanceo de carga y replicación de datos cuenta con más de varios equipos para el almacenamiento de archivos.
