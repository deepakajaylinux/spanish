===========
Varnish
===========

sinopsis
--------------

Este módulo ayuda a instalar el barniz a la máquina de los usuarios. El barniz es un programa que puede acelerar en gran medida de un sitio web al tiempo que reduce la carga en el servidor Web. Según el sitio oficial de barniz, barniz es un "acelerador de aplicaciones Web también conocido como un proxy inverso HTTP caché". Veamos aquí, sobre cómo este módulo realiza la instalación de barniz de apt-get.

Ayuda Comando
---------------------

El comando help guía a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en el módulo de barniz. El comando help enumera los parámetros alternativos de barniz. También se describe la sintaxis para la instalación de barniz. El comando de ayuda en el marco del módulo de barniz se da a continuación:

.. code-block:: bash

		ptconfigure varnish help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla que representa aproximadamente el comando de ayuda bajo módulo de barniz.

.. code-block:: bash

	kevell@corp:/# ptconfigure Varnish help
	******************************


        This command allows you to install Varnish, the popular HTTP Cache

        Varnish, varnish

        - install
        Installs Varnish through apt-get
        example: ptconfigure varnish install

	------------------------------
	End Help
	******************************

instalación
---------------

El comando utilizado para instalar el barniz a la máquina de los usuarios se muestra a continuación.

.. code-block:: bash

		ptconfigure varnish install

Después de introducir el comando anterior, las siguientes operaciones se produce como se muestra en el formato tabular.

.. cssclass:: table-bordered

 +------------------------+------------------------------+-----------+-----------------------------------------------------------+
 | Parámetros             | Parámetro Alternativa        | Opciones  | Comentarios                                               |
 +========================+==============================+===========+===========================================================+
 |Install Varnish? (Y/N)  | Varnish, varnish             | Y(Yes)    | Si el usuario desea continuar el proceso de instalación   |
 |                        |                              |           | se puede introducir como Y.                               |
 +------------------------+------------------------------+-----------+-----------------------------------------------------------+
 |Install Varnish? (Y/N)  | Varnish, varnish             | N(No)     | Si el usuario desea abandonar el proceso de instalación   |
 |                        |                              |           | se puede introducir como N.|                              |
 +------------------------+------------------------------+-----------+-----------------------------------------------------------+


Si el usuario continúa el proceso de instalación, durante la ejecución de la instalación produce el siguiente proceso:

* Lee las listas de paquetes.
* Construye el árbol de dependencias.
* Lee la información de estado.
* Lista de los paquetes instalados.
* Lista de paquetes adicionales instalados.
* Lista de nuevos paquetes instalados.
* Número de archivos actualizados, recién instalados, retirados, sin actualizar.
* Por último, a partir del acelerador HTTP barnizada.
* La siguiente captura de pantalla muestra el proceso mencionado anteriormente:

.. code-block:: bash
   
	Kevell@corp:/# ptconfigure varnish install
	Install Varnish? (Y/N) 
	y
	*******************************
	*        Pharaoh Tools        *
	*          ! Varnish !        *
	*******************************
	Creating /tmp/ptconfigure-temp-script-95745650915.sh
	chmod 755 /tmp/ptconfigure-temp-script-95745650915.sh 2>/dev/null
	Changing /tmp/ptconfigure-temp-script-95745650915.sh Permissions
	Executing /tmp/ptconfigure-temp-script-95745650915.sh
	Reading package lists...
	Building dependency tree...
	Reading state information...
	The following extra packages will be installed:
        libjemalloc1 libvarnishapi1
	Suggested packages:
	varnish-doc
	The following NEW packages will be installed:
	libjemalloc1 libvarnishapi1 varnish
	0 upgraded, 3 newly installed, 0 to remove and 6 not upgraded.
	Need to get 518 kB of archives.
	After this operation, 1,653 kB of additional disk space will be used.
	Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libvarnishapi1 amd64 3.0.5-2 [29.9 kB]
	Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libjemalloc1 amd64 3.5.1-2 [76.8 kB]
	Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty/universe varnish amd64 3.0.5-2 [411 kB]
	Fetched 518 kB in 3s (152 kB/s)
	Selecting previously unselected package libvarnishapi1.
	(Reading database ... 201582 files and directories currently installed.)
	Preparing to unpack .../libvarnishapi1_3.0.5-2_amd64.deb ...
	Unpacking libvarnishapi1 (3.0.5-2) ...
	Selecting previously unselected package libjemalloc1.
	Preparing to unpack .../libjemalloc1_3.5.1-2_amd64.deb ...
	Unpacking libjemalloc1 (3.5.1-2) ...
	Selecting previously unselected package varnish.
	Preparing to unpack .../varnish_3.0.5-2_amd64.deb ...
	Unpacking varnish (3.0.5-2) ...
	Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
	Processing triggers for ureadahead (0.100.0-16) ...
	Setting up libvarnishapi1 (3.0.5-2) ...
	Setting up libjemalloc1 (3.5.1-2) ...
	Setting up varnish (3.0.5-2) ...
	 * Starting HTTP accelerator varnishd
	   ...done.
	Processing triggers for libc-bin (2.19-0ubuntu6.4) ...
	Processing triggers for ureadahead (0.100.0-16) ...
	Temp File /tmp/ptconfigure-temp-script-95745650915.sh Removed
	... All done!
	*******************************
	Thanks for installing , visit www.pharaohtools.com for more
	******************************


	Single App Installer:
	--------------------------------------------
	Varnish: Success
	------------------------------
	Installer Finished
	******************************

Beneficios
-------------

* El barniz es un alto rendimiento moderno, aplicación proxy HTTP inverso caché de código abierto.
* Los parámetros utilizados para la declaración de la ayuda de mandatos, la instalación no son sensibles, que es una ventaja añadida, mientras 
  que en comparación con otros.
* Es-acomodados tanto en OS Cent y así como en Ubuntu.
