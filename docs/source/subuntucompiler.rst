================
Ubuntu Compiler
================

sinopsis
----------

Este módulo revitalizar programa c. Ubuntu y otras distribuciones de Linux tienen repositorios de paquetes extensos de ahorrar al usuario de la molestia de la compilación. Con un único comando, se puede construir desde el código fuente como un profesional. Es la comodidad con Ubuntu y CentOS.

comando Ayuda
---------------------

Este comando ayuda a guiar al usuario acerca de Ubuntu compilador. Es menos tiempo, ya que puede instalarse automáticamente. Adecuado para el programa C.

.. code-block:: bash

		ptconfigure Ubuntucompiler help

El siguiente comando ayuda ayudará al usuario para la instalación.

.. code-block:: bash

	kevell@corp:/# ptconfigure UbuntuCompiler help
	******************************


         This allows you to Complie programs written in C Source

          UbuntuCompiler, ubuntu-compiler, ubuntucompiler

        - install
        Installs Ubuntu Compiling tools through apt-get.
        example: ptconfigure ubuntu-compiler install

	------------------------------
	End Help
	******************************

instalación
--------------

Este es un proceso perceptible para instalar el módulo compilador Ubuntu bajo ptconfigure simplemente usando el comando dado a continuación,

.. code-block:: bash

  		ptconfigure Ubuntu-compiler install

Después de dar la orden, el compilador de Ubuntu se instalará con nuevas actualizaciones.

Si la entrada del usuario como N la siguiente pantalla aparecerá.

.. code-block:: bash


 kevell@corp:/# ptconfigure ubuntu-compiler install 
 Install Ubuntu Compiler? (Y/N) 
 y
 ******************************* 
 *        Pharaoh Tools        * 
 *         Ubuntu Comp!        * 
 ******************************* 
 Reading package lists... 
 Building dependency tree... 
 Reading state information... 
 The following packages were automatically installed and are no longer required: 
  dh-apparmor libalgorithm-diff-perl libalgorithm-diff-xs-perl 
  libalgorithm-merge-perl libmail-sendmail-perl libsys-hostname-long-perl 
  po-debconf 
 Use 'apt-get autoremove' to remove them. 
 Suggested packages: 
  g++-multilib 
 The following NEW packages will be installed: 
  g++ 
 0 upgraded, 1 newly installed, 0 to remove and 3 not upgraded. 
 Need to get 1,490 B of archives. 
 After this operation, 34.8 kB of additional disk space will be used. 
 Get:1 http://archive.ubuntu.com/ubuntu/ trusty/main g++ amd64 4:4.8.2-1ubuntu6 [1,490 B] 
 Fetched 1,490 B in 1s (1,438 B/s) 
 Selecting previously unselected package g++. 
 (Reading database ... 393110 files and directories currently installed.) 
 Preparing to unpack .../g++_4%3a4.8.2-1ubuntu6_amd64.deb ... 
 Unpacking g++ (4:4.8.2-1ubuntu6) ... 
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ... 
 Setting up g++ (4:4.8.2-1ubuntu6) ... 
 update-alternatives: using /usr/bin/g++ to provide /usr/bin/c++ (c++) in auto mode 
 [Pharaoh Logging] Adding Package g++ from the Packager Apt executed correctly  

 Reading package lists... 
 Building dependency tree... 
 Reading state information... 
 The following packages were automatically installed and are no longer required: 
  dh-apparmor libmail-sendmail-perl libsys-hostname-long-perl po-debconf  
 Use 'apt-get autoremove' to remove them. 
 The following extra packages will be installed: 
  dpkg-dev make 
 Suggested packages: 
  debian-keyring make-doc 
 The following NEW packages will be installed: 
  build-essential dpkg-dev make 
 0 upgraded, 3 newly installed, 0 to remove and 3 not upgraded. 
 Need to get 850 kB of archives. 
 After this operation, 2,039 kB of additional disk space will be used. 
 Get:1 http://security.ubuntu.com/ubuntu/ trusty-security/main dpkg-dev all 1.17.5ubuntu5.3 [726 kB] 
 Get:2 http://archive.ubuntu.com/ubuntu/ trusty/main make amd64 3.81-8.2ubuntu3 [119 kB] 
 Get:3 http://archive.ubuntu.com/ubuntu/ trusty/main build-essential amd64 11.6ubuntu6 [4,838 B] 
 Fetched 850 kB in 37s (22.5 kB/s) 
 Selecting previously unselected package make. 
 (Reading database ... 393115 files and directories currently installed.) 
 Preparing to unpack .../make_3.81-8.2ubuntu3_amd64.deb ... 
 Unpacking make (3.81-8.2ubuntu3) ... 
 Selecting previously unselected package dpkg-dev. 
 Preparing to unpack .../dpkg-dev_1.17.5ubuntu5.3_all.deb ... 
 Unpacking dpkg-dev (1.17.5ubuntu5.3) ... 
 Selecting previously unselected package build-essential. 
 Preparing to unpack .../build-essential_11.6ubuntu6_amd64.deb ... 
 Unpacking build-essential (11.6ubuntu6) ... 
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ... 
 Setting up make (3.81-8.2ubuntu3) ... 
 Setting up dpkg-dev (1.17.5ubuntu5.3) ... 
 Setting up build-essential (11.6ubuntu6) ... 
 [Pharaoh Logging] Adding Package build-essential from the Packager Apt executed correctly 
 [Pharaoh Logging] Package make from the Packager Apt is already installed, so not installing 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 


 Single App Installer: 
 -------------------------------------------- 
 UbuntuCompiler: Success 
 ------------------------------ 
 Installer Finished 
 ****************************** 



opciones
-----------

.. cssclass:: table-bordered

 +-------------------------------+--------------------------------------+---------------+---------------------------------------------+
 | Parámetros                    | Parámetro Alternativa                | Opciones      | Comentarios                                 |
 +===============================+======================================+===============+=============================================+
 |Install Ubuntu Compiler? (Y/N) | UbuntuCompiler, ubuntu-compiler,     | Y(Yes)        | Si el usuario desea continuar el proceso de |
 |                               | ubuntucompiler                       |               | instalación se puede introducir como Y.     |
 +-------------------------------+--------------------------------------+---------------+---------------------------------------------+
 |Install Ubuntu Compiler? (Y/N) | UbuntuCompiler, ubuntu-compiler,     | N(No)         | Si el usuario desea abandonar el proceso de |
 |                               | ubuntucompiler                       |               | instalación se puede introducir como N.|    |
 +-------------------------------+--------------------------------------+---------------+---------------------------------------------+


Beneficios
--------------

* Arranque más rápido
* Mayor seguridad
* Cambiar el kernel de adelantarse mientras compilación
* Conveniente para el programa C
