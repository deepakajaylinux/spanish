===============
Mysqlserver
===============

sinopsis
------------

Este módulo actúa como facilitador para instalar mysql-servidor con la versión actualizada a través de apt-get. Si el servidor mysql ya existe en su equipo, se comprueba la disponibilidad de módulo recién actualizado.

Ayuda Comando
---------------------

El comando help guía a los usuarios en cuanto a la metodología en uso y también acerca de las acciones que se pueden realizar en virtud de estos módulos. También describe los nombres alternativos para mysql-server. El comando para el uso de la opción de ayuda se da a continuación

.. code-block:: bash

	ptconfigure mysql-server help

Este comando hace que los usuarios sean conscientes de su propósito y también sobre el comando utilizado para instalar el servidor mysql.
La captura de pantalla que figura a continuación muestra un pictograma sobre el comando ayuda.

.. code-block:: bash


 kevell@corp:/# ptconfigure MysqlServer help
 ******************************


  This command allows you to install the MySQL Server. Currently only
  Mysql Workbench, the Database management GUI provided by Oracle for
  Mysql.

  MysqlServer, mysql-server, mysqlserver

        - install
        Install some Mysql Server Tools through apt-get.
        example: ptconfigure mysql-server install

  Notes, during mysql install a root password will be set. First, it'll look
  for the parameter --mysql-root-pass, if this is not set, it'll look in the
  ptconfigure config for a mysql-default-root-pass setting, and failing both of
  those it will just set the password for root to ptconfigure.

 ------------------------------
 End Help
 ******************************

instalación
------------

El comando utilizado para instalar el servidor MySQL es la siguiente.

.. code-block:: bash

	ptconfigure mysql-server install

Durante la instalación, se produce el siguiente proceso
----------------------------------------------------------------

* Este módulo ayuda a instalar algunas herramientas para el servidor MySQL a través de apt-get.
* Inicialmente una contraseña de root se establecerá.
* Durante la instalación, se buscará un parámetro de la raíz del pase --mysql.
* Si la raíz de paso --mysql no está disponible, buscará la config ptconfigure para la configuración de la raíz del pase-mysql por defecto.
* En el caso de los dos pasos mencionados anteriormente no se, se procederá al establecer contraseña de root para ptconfigure.

Opciones adicionales
--------------------------

Veamos acerca de las opciones adicionales que intervienen en la instalación del servidor mysql.

.. cssclass:: table-bordered

 +------------------------+--------------------------------------+------------+--------------------------------------+
 | Parámetros             | Parámetro Alternativa                | Opciones   | Comentarios                          |
 +========================+======================================+============+======================================+
 |Install MySQL Server?   | En el lugar del MySQL Server estos   | Y(Yes)     | Si el usuario desea continuar el     |
 |(Y/N)                   | nombres alternativos pueden ser      |            | proceso de instalación se puede      |
 |                        | utilizados: MySQLServer,             |            | introducir como Y.                   |
 |                        | mysql-server, mysqlserver.           |            |                                      |
 +------------------------+--------------------------------------+------------+--------------------------------------+
 |Install MySQL Server?   | En el lugar del MySQL Server estos   | N(No)      | Si el usuario desea abandonar el     |
 |(Y/N)                   | nombres alternativos pueden ser      |            | proceso de instalación se puede      |
 |                        | utilizados: MySQLServer,             |            | introducir como N.                   |
 |                        | mysql-server, mysqlserver.|          |            |                                      |
 +------------------------+--------------------------------------+------------+--------------------------------------+

La siguiente captura de pantalla le da una presentación gráfica sobre el proceso de instalación.


.. code-block:: bash



 kevell@corp:/# ptconfigure mysql-server install 
 Install MySQL Server? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         MySQL Server!        * 
 ******************************* 
 Reading package lists... 
 Building dependency tree... 
 Reading state information... 
 The following packages were automatically installed and are no longer required: 
  libboost-filesystem1.54.0 libboost-program-options1.54.0 
  libboost-thread1.54.0 libgoogle-perftools4 libpcrecpp0 libsnappy1 
  libtcmalloc-minimal4 libunwind8 mongodb-clients 
 Use 'apt-get autoremove' to remove them. 
 The following NEW packages will be installed: 
  debconf-utils 
 0 upgraded, 1 newly installed, 0 to remove and 3 not upgraded. 
 Need to get 57.4 kB of archives. 
 After this operation, 157 kB of additional disk space will be used. 
 Get:1 http://archive.ubuntu.com/ubuntu/ trusty/main debconf-utils all 1.5.51ubuntu2 [57.4 kB] 
 Fetched 57.4 kB in 14s (4,097 B/s) 
 Selecting previously unselected package debconf-utils. 
 (Reading database ... 380784 files and directories currently installed.) 
 Preparing to unpack .../debconf-utils_1.5.51ubuntu2_all.deb ... 
 Unpacking debconf-utils (1.5.51ubuntu2) ... 
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ... 
 Setting up debconf-utils (1.5.51ubuntu2) ... 
 [Pharaoh Logging] Adding Package debconf-utils from the Packager Apt executed correctly 
 Creating /tmp/ptconfigure-temp-script-12002365099.sh 
 chmod 755 /tmp/ptconfigure-temp-script-12002365099.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-12002365099.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-12002365099.sh 
 Temp File /tmp/ptconfigure-temp-script-12002365099.sh Removed 
 [Pharaoh Logging] Package mysql-client from the Packager Apt is already installed, so not installing 
 [Pharaoh Logging] Package mysql-server from the Packager Apt is already installed, so not installing 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 

 Single App Installer: 
 -------------------------------------------- 
 MysqlServer: Success 
 ------------------------------ 
 Installer Finished 
 ****************************** 


Si el servidor MySQL está ya existe en su máquina, entonces se lanza un mensaje al usuario, ya que ya está instalado. La siguiente captura de pantalla representa el proceso de garantizar:


.. code-block:: bash

 kevell@corp:/# ptconfigure mysql-server install
 Install MySQL Server? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         MySQL Server!        *
 *******************************
 [Pharaoh Logging] Package debconf-utils from the Packager Apt is already installed, so not installing
 Creating /tmp/ptconfigure-temp-script-23889189196.sh
 chmod 755 /tmp/ptconfigure-temp-script-23889189196.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-23889189196.sh Permissions
 Executing /tmp/ptconfigure-temp-script-23889189196.sh
 Temp File /tmp/ptconfigure-temp-script-23889189196.sh Removed
 [Pharaoh Logging] Package mysql-client from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package mysql-server from the Packager Apt is already installed, so not installing
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 MysqlServer: Success
 ------------------------------
 Installer Finished
 ******************************




Beneficios
------------

* Durante la instalación del servidor mysql, se instala con la versión actualizada.
* Asegura antes de instalar, y compruebe la disponibilidad de módulos.
* En el caso de los nuevos módulos incluidos en la versión actualizada, se instalará de forma individual el módulo que falta.
* Comprueba la disponibilidad de funciones de la biblioteca en el servidor mysql.
