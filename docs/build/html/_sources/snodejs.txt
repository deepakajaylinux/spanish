=========
Node-JS
=========

sinopsis
-------------

Este módulo ayuda a los usuarios a instalar Nodo JS que es un lado del servidor JS Idioma. Node.js es un código abierto, entorno de ejecución multiplataforma para el lado del servidor y aplicaciones de red. Aplicaciones Node.js están escritos en JavaScript, y se puede ejecutar en el tiempo de ejecución Node.js en OS X, Microsoft Windows, Linux y FreeBSD. Aquí, vamos a ver cómo este módulo facilita en la instalación y uso del Nodo-JS.

Ayuda Comando
---------------------

El comando de ayuda conduce a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en el módulo Node-JS. Las listas de comandos de ayuda fuera de los parámetros alternativos de módulo Node-JS. También describe la sintaxis para instalar el módulo Node-JS. El comando de ayuda para el módulo Node-JS se muestra a continuación.

.. code-block:: bash

		ptconfigure NodeJS help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda bajo Nodo JS.

.. code-block:: bash
		


 kevell@corp:/# ptconfigure NodeJS help
 ******************************


  This command allows you to install Node JS, The Server Side JS Language

  NodeJS, node-js, nodejs

        - install
        Installs NodeJS through apt-get.
        example: ptconfigure node-js install

 ------------------------------
 End Help
 ******************************

instalación
----------------

Instalación del Nodo-JS para su máquina, se puede hacer simplemente usando el comando siguiente como se muestra:

.. code-block:: bash

		ptconfigure node-js install

Después de introducir el comando anterior, las siguientes operaciones se produce como se muestra en el formato tabular.

.. cssclass:: table-bordered

 +------------------------+------------------------------------+----------------+---------------------------------------------+
 | Parámetros             | Parámetro Alternativa              | Opciones       | Comentarios                                 |
 +========================+====================================+================+=============================================+
 |Install Node JS? (Y/N)  | En lugar de Nodo JS, NodeJS,       | Y(Yes)         | Si el usuario desea continuar el proceso    |
 |                        | nodo-js, también se pueden         |                | de instalación se puede introducir como Y.  |
 |                        | utilizar nodejs.                   |                |                                             |
 +------------------------+------------------------------------+----------------+---------------------------------------------+
 |Install Node JS? (Y/N)  | En lugar de Nodo JS, NodeJS,       | N(No)          | Si el usuario desea continuar el proceso    |
 |                        | nodo-js, también se pueden         |                | de instalación se puede introducir como N.  |
 |                        | utilizar nodejs.|                  |                |                                             |
 +------------------------+------------------------------------+----------------+---------------------------------------------+

Si el usuario continúa el proceso de instalación, durante la ejecución de la instalación produce el siguiente proceso:

* Lee las listas de paquetes.
* Construye el árbol de dependencias.
* Lee la información de estado.
* Lista de los paquetes que se instalan automáticamente.
* Lista de nuevos paquetes instalados.
* Muestra el número de archivos que se actualizan, recién instalados, removidos, no actualizados.

Por último, se informa claramente de los informes y de estado. Y también, añadiendo paquete nodejs del Packager Apt ejecutados correctamente. La siguiente captura de pantalla muestra todo el proceso de instalación como se describe.

Si el nodo-js módulo ya existe en la máquina de los usuarios, se mostrará un mensaje como el paquete de nodo-js del empaquetador Apt ya está instalado. La captura de pantalla de la siguiente es un buen ejemplo de ese tipo de mensajes.

.. code-block:: bash

 kevell@corp:/# ptconfigure node-js install
 Install Node JS? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Node JS!        *
 *******************************
	Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  ax25-node libax25 openbsd-inetd
 The following NEW packages will be installed:
  ax25-node libax25 node openbsd-inetd
 0 upgraded, 4 newly installed, 0 to remove and 17 not upgraded.
 Need to get 110 kB of archives.
 After this operation, 465 kB of additional disk space will be used.
 Get:1 http://archive.ubuntu.com/ubuntu/ trusty/universe libax25 amd64 0.0.12-rc2+cvs20120204-2ubuntu2 [22.7 kB]
 Get:2 http://archive.ubuntu.com/ubuntu/ trusty/main openbsd-inetd amd64 0.20091229-2ubuntu3 [30.8 kB]
 Get:3 http://archive.ubuntu.com/ubuntu/ trusty/universe ax25-node amd64 0.3.2-7.4 [54.8 kB]
 Get:4 http://archive.ubuntu.com/ubuntu/ trusty/universe node all 0.3.2-7.4 [1,284 B]
 Fetched 110 kB in 2s (39.1 kB/s)
 Selecting previously unselected package libax25.
 (Reading database ... 237551 files and directories currently installed.)
 Preparing to unpack .../libax25_0.0.12-rc2+cvs20120204-2ubuntu2_amd64.deb ...
 Unpacking libax25 (0.0.12-rc2+cvs20120204-2ubuntu2) ...
 Selecting previously unselected package openbsd-inetd.
 Preparing to unpack .../openbsd-inetd_0.20091229-2ubuntu3_amd64.deb ...
 Unpacking openbsd-inetd (0.20091229-2ubuntu3) ...
 Selecting previously unselected package ax25-node.
 Preparing to unpack .../ax25-node_0.3.2-7.4_amd64.deb ...
 Unpacking ax25-node (0.3.2-7.4) ...
 Selecting previously unselected package node.
 Preparing to unpack .../node_0.3.2-7.4_all.deb ...
 Unpacking node (0.3.2-7.4) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Processing triggers for ureadahead (0.100.0-16) ...
 Setting up libax25 (0.0.12-rc2+cvs20120204-2ubuntu2) ...
 Setting up openbsd-inetd (0.20091229-2ubuntu3) ...
 * Stopping internet superserver inetd
   ...done.
 * Not starting internet superserver: no services enabled
 Processing triggers for ureadahead (0.100.0-16) ...
 Setting up ax25-node (0.3.2-7.4) ...
 Setting up node (0.3.2-7.4) ...
 Processing triggers for libc-bin (2.19-0ubuntu6.4) ...
 [Pharaoh Logging] Adding Package node from the Packager Apt executed correctly
            
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libv8-3.14.5
 The following NEW packages will be installed:
  libv8-3.14.5 nodejs
 0 upgraded, 2 newly installed, 0 to remove and 17 not upgraded.
 Need to get 1,873 kB of archives.
 After this operation, 7,429 kB of additional disk space will be used.
 Get:1 http://archive.ubuntu.com/ubuntu/ trusty/universe libv8-3.14.5 amd64 3.14.5.8-5ubuntu2 [1,189 kB]
 Get:2 http://archive.ubuntu.com/ubuntu/ trusty/universe nodejs amd64 0.10.25~dfsg2-2ubuntu1 [684 kB]
 Fetched 1,873 kB in 14s (126 kB/s)
 Selecting previously unselected package libv8-3.14.5.
 (Reading database ... 237621 files and directories currently installed.)
 Preparing to unpack .../libv8-3.14.5_3.14.5.8-5ubuntu2_amd64.deb ...
 Unpacking libv8-3.14.5 (3.14.5.8-5ubuntu2) ...
 Selecting previously unselected package nodejs.
 Preparing to unpack .../nodejs_0.10.25~dfsg2-2ubuntu1_amd64.deb ...
 Unpacking nodejs (0.10.25~dfsg2-2ubuntu1) ...
 Processing triggers for doc-base (0.10.5) ...
 Processing 1 added doc-base file...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up libv8-3.14.5 (3.14.5.8-5ubuntu2) ...
 Setting up nodejs (0.10.25~dfsg2-2ubuntu1) ...
 update-alternatives: using /usr/bin/nodejs to provide /usr/bin/js (js) in auto mode
 Processing triggers for libc-bin (2.19-0ubuntu6.4) ...
 [Pharaoh Logging] Adding Package nodejs from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 NodeJS: Success
 ------------------------------
 Installer Finished

 ------------------------------

Beneficios
------------

* Los parámetros utilizados para la declaración de la ayuda de mandatos, la instalación no son sensibles, que es una ventaja añadida, mientras 
  que en comparación con otros.
* Es-acomodados tanto en OS Cent y así como en Ubuntu.
* Si el paquete nodo-js ya existe en la máquina del usuario, lo hará no sobrescribe, en lugar de que se mostrará un mensaje como ya  existir.
* Node.js utiliza el motor de Google V8 JavaScript para ejecutar código, y un gran porcentaje de los módulos básicos están escritas en 
  JavaScript.
* Node.js contiene una biblioteca incorporada para permitir que las aplicaciones para actuar como un servidor Web sin necesidad de software 
  como Apache HTTP Server o IIS.
