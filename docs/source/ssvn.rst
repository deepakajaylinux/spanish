=======
SVN
=======

sinopsis
------------

Este módulo ayuda a los usuarios a instalar la última versión de SVN en Ubuntu. Subversion (a menudo abreviado SVN, después de que el nombre del comando svn) es un sistema de control de versiones de software y control de revisiones distribuido como software libre bajo la licencia Apache. [1] Los desarrolladores usar Subversion para mantener las versiones actuales e históricas de archivos como el código fuente, web páginas y documentación. Su objetivo es ser un sucesor en su mayoría compatibles con la Concurrent Versions System ampliamente utilizado (CVS). Veamos cómo este módulo facilita en instalación, desinstalación, asegurando la subversión en ubuntu.

Ayuda Comando
---------------------

El comando help guía a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en el SVN. En él se enumeran los parámetros alternativos de subversion. También describe la sintaxis para instalar, desinstalar, asegurando la subversion. El comando de ayuda para el módulo de SVN se muestra a continuación.

.. code-block:: bash
	
		ptconfigure svn help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda en virtud de subversion.

.. code-block:: bash

 kevell@corp:/# ptconfigure svn help
 ******************************


  This command allows you to install the latest available SVN in the Ubuntu
  repositories.

  SVN, svn

        - install
        Installs the latest available (In your package manager) version of SVN
        example: ptconfigure svn install

        - ensure
        Ensures SVN is installed
        example: ptconfigure svn ensure

        - uninstall
        Installs the latest version of SVN
        example: ptconfigure svn uninstall

 ------------------------------
 End Help
 ******************************

instalación
---------------

El comando utilizado para instalar el SVN para el ubuntu se muestra a continuación.

.. code-block:: bash
		
		ptconfigure svn install

Después de introducir el comando anterior, las siguientes operaciones se produce como se muestra en forma de tabla.

.. cssclass:: table-bordered

 +-----------------------+-----------------------------------+-----------+------------------------------------------------+
 | Parámetros            | Parámetro Alternativa             | Opciones  | Comentarios                                    |
 +=======================+===================================+===========+================================================+
 |Install SVN? (Y/N)     | En lugar de SVN, podemos utilizar | Y(Yes)    | Si el usuario desea continuar el proceso de    |
 |                       | svn también.                      |           | instalación se puede introducir como Y.        |
 +-----------------------+-----------------------------------+-----------+------------------------------------------------+
 |Install SVN? (Y/N)     | En lugar de SVN, podemos utilizar | N(No)     | Si el usuario desea abandonar el proceso de    |
 |                       | svn también.                      |           | instalación se puede introducir como N.|       |
 +-----------------------+-----------------------------------+-----------+------------------------------------------------+

Si el usuario continúa el proceso de instalación, durante la ejecución de la instalación produce el siguiente proceso:

* Lee las listas de paquetes.
* Construye el árbol de dependencias.
* Lee la información de estado.
* Enumera a cabo paquetes adicionales instalados.
* Enumera nuevos paquetes instalados.
* Número de archivos actualizados, recién instalados, retirados, sin actualizar.
* Por último, la instalación de SVN se completó. La siguiente captura de pantalla que muestra sobre el proceso de instalación de SVN en ubuntu.

.. code-block:: bash

 kevell@corp:/# ptconfigure svn install
 Install SVN? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         !Subversion!        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libserf-1-1 libsvn1
 Suggested packages:
  subversion-tools db5.3-util
 The following NEW packages will be installed:
  libserf-1-1 libsvn1 subversion
 0 upgraded, 3 newly installed, 0 to remove and 8 not upgraded.
 Need to get 1,240 kB of archives.
 After this operation, 4,701 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main libserf-1-1 amd64 1.3.3-1ubuntu0.1 [42.2 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main libsvn1 amd64 1.8.8-1ubuntu3.1 [917 kB]
 Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main subversion amd64 1.8.8-1ubuntu3.1 [280 kB]
 Fetched 1,240 kB in 43s (28.3 kB/s)
 Selecting previously unselected package libserf-1-1:amd64.
 (Reading database ... 211229 files and directories currently installed.)
 Preparing to unpack .../libserf-1-1_1.3.3-1ubuntu0.1_amd64.deb ...
 Unpacking libserf-1-1:amd64 (1.3.3-1ubuntu0.1) ...
 Selecting previously unselected package libsvn1:amd64.
 Preparing to unpack .../libsvn1_1.8.8-1ubuntu3.1_amd64.deb ...
 Unpacking libsvn1:amd64 (1.8.8-1ubuntu3.1) ...
 Selecting previously unselected package subversion.
 Preparing to unpack .../subversion_1.8.8-1ubuntu3.1_amd64.deb ...
 Unpacking subversion (1.8.8-1ubuntu3.1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up libserf-1-1:amd64 (1.3.3-1ubuntu0.1) ...
 Setting up libsvn1:amd64 (1.8.8-1ubuntu3.1) ...
 Setting up subversion (1.8.8-1ubuntu3.1) ...
 Processing triggers for libc-bin (2.19-0ubuntu6.5) ...
 [Pharaoh Logging] Adding Package subversion from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************
 

 Single App Installer:
 --------------------------------------------
 SVN: Success
 ------------------------------
 Installer Finished
 ******************************

Un instalar
-------------

El comando utilizado para des instalar el SVN para el ubuntu se muestra a continuación.

.. code-block:: bash

		ptconfigure svn uninstall

Después de introducir el comando anterior, las siguientes operaciones se produce como se muestra en el formato tabular.

.. cssclass:: table-bordered


 +-----------------------+-------------------------------+-----------+----------------------------------------------+
 | Parámetros            | Parámetro Alternativa         | Opciones  | Comentarios                                  |
 +=======================+===============================+===========+==============================================+
 |Uninstall SVN? (Y/N)   | En lugar de SVN, podemos      | Y(Yes)    | Si el usuario desea continuar el proceso de  |
 |                       | utilizar svn también.         |           | desinstalación se puede introducir como Y.   |
 +-----------------------+-------------------------------+-----------+----------------------------------------------+
 |Uninstall SVN? (Y/N)   | En lugar de SVN, podemos      | N(No)     | Si el usuario desea salir del proceso de     |
 |                       | utilizar svn también.         |           | desinstalación que puede introducir como N.| |
 +-----------------------+-------------------------------+-----------+----------------------------------------------+

Si el usuario continúa el proceso de instalación de la ONU, durante la ejecución de desinstalación produce el siguiente proceso:

* Lee las listas de paquetes.
* Construye el árbol de dependencias.
* Lee la información de estado.
* Lista cabo paquetes que se instalan automáticamente.
* Enumera a paquetes que se eliminan.
* Número de archivos actualizados, recién instalados, retirados, sin actualizar.

Por último, la desinstalación de SVN se completó. La siguiente captura de pantalla que muestra sobre el proceso de des instalar subversion en ubuntu.

.. code-block:: bash

 kevell@corp:/# ptconfigure svn uninstall
 Uninstall SVN? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         !Subversion!        *
 *******************************
 [Pharaoh Logging] Removing Package subversion
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following packages were automatically installed and are no longer required:
  libserf-1-1 libsvn1
 Use 'apt-get autoremove' to remove them.
 The following packages will be REMOVED:
  subversion
 0 upgraded, 0 newly installed, 1 to remove and 8 not upgraded.
 After this operation, 1,425 kB disk space will be freed.
 (Reading database ... 211322 files and directories currently installed.)
 Removing subversion (1.8.8-1ubuntu3.1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 [Pharaoh Logging] Removed Package subversion from the Packager Apt
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Uninstaller:
 ------------------------------
 SVN: Success
 ------------------------------
 Installer Finished
 ******************************

asegurar
---------

El comando utilizado para asegurar SVN se muestra a continuación.

.. code-block:: bash

		ptconfigure svn ensure

El proceso de garantizar realiza las siguientes funciones:

* Se asegurará de si el módulo está instalado o no, y no se comprueba la versión.
* Si ya está instalado el módulo se reportará como ya lo está existía.
* Si el módulo no está disponible en la máquina del usuario, a continuación, se procederá de la instalación.

Las siguientes imágenes se aprecia el proceso de asegurar.

.. code-block:: bash

 kevell@corp:/# ptconfigure svn ensure
 [Pharaoh Logging] Ensure module install is not checking versions
 sh: 1: svn: not found
 [Pharaoh Logging] Module SVN reports itself as Not Installed 
 [Pharaoh Logging] Installing as not installed
 *******************************
 *        Pharaoh Tools        *
 *         !Subversion!        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Suggested packages:
  subversion-tools db5.3-util
 The following NEW packages will be installed:
  subversion
 0 upgraded, 1 newly installed, 0 to remove and 8 not upgraded.
 Need to get 0 B/280 kB of archives.
 After this operation, 1,425 kB of additional disk space will be used.
 Selecting previously unselected package subversion.
 (Reading database ... 211282 files and directories currently installed.)
 Preparing to unpack .../subversion_1.8.8-1ubuntu3.1_amd64.deb ...
 Unpacking subversion (1.8.8-1ubuntu3.1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up subversion (1.8.8-1ubuntu3.1) ...
 [Pharaoh Logging] Adding Package subversion from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


Beneficios
--------------

* Los parámetros utilizados en la declaración de la ayuda y de las instalaciones, desinstalación, asegúrese de que no distinguen entre 
  mayúsculas y minúsculas, lo que se añade la ventaja, mientras que en comparación con otros.
* El usuario puede asegurarse sobre la disponibilidad antes de proceder con la instalación.
* No va a sobrescribir los paquetes, por lo que es menos tiempo.

