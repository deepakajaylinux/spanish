================
MysqlTools
================

sinopsis
-----------
Este módulo tiene como objetivo la instalación de algunas herramientas que ayuda al servidor MySQL. También facilita en la instalación de la interfaz gráfica de usuario de MySQL Workbench y así como mytop herramienta de línea de comandos.

Ayuda Comando
---------------------
El comando de ayuda instruye a los usuarios en el manejo de este módulo. Además de esto, también se especifica los parámetros alternativos. El comando utilizado para la opción de ayuda se da a continuación:

.. code-block:: bash

	ptconfigure MysqlTools help

El comando de ayuda también especifica el comando utilizado para la instalación de este módulo mysqltools. Mira la captura de pantalla a continuación.

.. code-block:: bash

 kevell@corp:/# ptconfigure mysqltools help

 ******************************


  This command allows you to install some tools to help with MySQL Server. Installs the MySQL
  Workbench GUI and also the mytop Command Line Tool.

  MysqlTools, mysql-tools, mysqltools

        - install
        Installs Mysql Tools through apt-get.
        example: ptconfigure mysql-tools install

 ------------------------------
 End Help
 ******************************

instalación
-------------

Este módulo instala las herramientas de mysql que soporta el servidor mysql con la ayuda de apt-get. El comando utilizado para instalar mysqltools a su máquina se muestra a continuación:

.. code-block:: bash

	ptconfigure MysqlTools install


.. cssclass:: table-bordered

 +-----------------------+---------------------------------------------+---------------+--------------------------------------+
 | Parámetros            | Parámetro Alternativa                       | Opciones      | Comentarios                          |
 +=======================+=============================================+===============+======================================+
 |Install MySQL Tools?   | En el lugar de Herramientas Mysql estos     | Y(Yes)        | Si el usuario desea continuar el     |
 |(Y/N)                  | nombres alternativos se pueden utilizar:    |               | proceso de instalación se puede      |
 |                       | MysqlTools,mysql-tools, mysqltools.         |               | como Y.                              |
 +-----------------------+---------------------------------------------+---------------+--------------------------------------+
 |Install MySQL Tools?   | En el lugar de Herramientas Mysql estos     | N(No)         | Si el usuario desea continuar el     |
 |(Y/N)                  | nombres alternativos se pueden utilizar:    |               | proceso de instalación se puede      |
 |                       | MysqlTools,mysql-tools, mysqltools.         |               | introducir como N.|                  |
 +-----------------------+---------------------------------------------+---------------+--------------------------------------+

Si el usuario proceda de la instalación de las herramientas de mysql las siguientes operaciones se realizan durante la instalación

* Se lee la lista de paquetes.
* Construye el árbol de dependencias.
* Lee la información de estado.
* Instala los paquetes adicionales que se requieren.
* Instala los paquetes sugeridos.
* Instala los nuevos paquetes.
* Muestra el número de archivos que se actualizan, recién a instalar, eliminar y no actualizados.

La captura de pantalla como se muestra a continuación le da una presentación gráfica sobre los pasos como se explicó anteriormente.

.. code-block:: bash

 kevell@corp:/# ptconfigure mysqltools install

 Install MySQL Tools? (Y/N)
 y
 *******************************
 *        Pharaoh Tools        *
 *         MySQL Tools!        *
 *******************************
 E: Unable to correct problems, you have held broken packages.
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Some packages could not be installed. This may mean that you have
 requested an impossible situation or if you are using the unstable
 distribution that some required packages have not yet been created
 or been moved out of Incoming.
 The following information may help to resolve the situation:
 
 The following packages have unmet dependencies:
 mysql-workbench : Depends: libmysqlcppconn7 (>= 1.1.3) but it is not installabl                                                                                        e
                   Recommends: ttf-bitstream-vera but it is not going to be inst                                                                                        alled
                   Recommends: mysql-utilities but it is not going to be install                                                                                        ed
 [Pharaoh Logging] Adding Package mysql-workbench from the Packager Apt did not e                                                                                        xecute correctly
 dpkg: warning: parsing file '/var/lib/dpkg/available' near line 47586 package 'c                                                                                        leopatra':
 missing maintainer
 dpkg: warning: parsing file '/var/lib/dpkg/available' near line 47586 package 'c                                                                                        leopatra':
 missing architecture
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libconfig-inifiles-perl
 The following NEW packages will be installed:
  libconfig-inifiles-perl mytop
 0 upgraded, 2 newly installed, 0 to remove and 13 not upgraded.
 Need to get 73.8 kB of archives.
 After this operation, 288 kB of additional disk space will be used.
 Get:1 http://us.archive.ubuntu.com/ubuntu/ precise/main libconfig-inifiles-perl                                                                                         all 2.68-1 [39.6 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/universe mytop all 1.9.1-1 [34                                                                                        .1 kB]
 Fetched 73.8 kB in 7s (10.5 kB/s)
 Selecting previously unselected package libconfig-inifiles-perl.
 (Reading database ... 254866 files and directories currently installed.)
 Preparing to unpack .../libconfig-inifiles-perl_2.68-1_all.deb ...
 Unpacking libconfig-inifiles-perl (2.68-1) ...
 Selecting previously unselected package mytop.
 Preparing to unpack .../archives/mytop_1.9.1-1_all.deb ...
 Unpacking mytop (1.9.1-1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up libconfig-inifiles-perl (2.68-1) ...
 Setting up mytop (1.9.1-1) ...
 [Pharaoh Logging] Adding Package mytop from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 MysqlTools: Success
 ------------------------------
 Installer Finished
 ******************************

También se especifica el nombre de herramientas que se instalan, por ejemplo

.. code-block:: bash


 .. rubric:: mysql-server-core-5.5:amd64, mysql-server-5.5: amd64, libaio1:amd64, mysql-server:amd64.

Beneficios
-------------

* El usuario puede instalar sus herramientas requeridas compatible con el servidor mysql.
* También facilita en la instalación de la interfaz gráfica de usuario de MySQL Workbench y así como mytop herramienta de línea de comandos.
* Después de completar la instalación, será muestra las listas de herramientas que se acaba de instalar.
