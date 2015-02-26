=============
NetworkTools
=============

sinopsis
----------

Las herramientas de red son utilidades de software diseñadas para analizar y configurar varios aspectos de la red informática. Las herramientas de red más comunes que se encuentran en la mayor parte del sistema operativo incluye Traceroute, Netstat y Ping. Cada herramientas de red tienen sus propias funciones.

Por ejemplo:

Ping se utiliza para comprobar la conectividad

Netstat se utiliza para mostrar la conexión entrante y saliente de la red

Ayuda Comando
-------------------

Este comando ayuda a determinar el uso del módulo de herramientas de red. El usuario se llega a saber acerca de las diferentes formas / formato para ejecutar este módulo. Este comando le guiará al usuario final para saber cuándo y cómo el comando que desea utilizar. A continuación dado son el mando y la pantalla del mismo.

.. code-block:: bash

		ptconfigure networktools help

La representación gráfica de la orden anterior se enumeran a continuación,

.. code-block:: bash

 kevell@corp:/# ptconfigure NetworkTools help
 ******************************


  This command allows you to install a set of common Network Tools. These include
  traceroute, netstat, lsof, telnet and ps.

  NetworkTools, networktools, network-tools

        - install
        Installs the latest version of Network Tools
        example: ptconfigure networktools install

 ------------------------------
 End Help
 ******************************

instalación
---------------

Cuando el usuario necesita para instalar cualquier herramienta de red en la máquina. El siguiente comando dado se ejecutará el proceso de instalación.

.. code-block:: bash


 	ptconfigure networktool install



.. cssclass:: table-bordered

 +---------------------+-------------------------------------------+-------------+---------------------------------------------+
 | Parámetros          | Parámetro Alternativa                     | Opciones    | Comentarios                                 |
 +=====================+===========================================+=============+=============================================+
 |Install Network      | En lugar de NetworkTools, podemos         | Y(Yes)      | Si el usuario desea continuar el proceso de |
 |Tools? (Y/N)         | utilizar networktools, network-tools      |             | instalación se puede introducir como Y.     |
 |                     | también.                                  |             |                                             |
 +---------------------+-------------------------------------------+-------------+---------------------------------------------+
 |Install Network      | En lugar de NetworkTools, podemos         | N(No)       | Si el usuario desea abandonar el proceso de |
 |Tools? (Y/N)         | utilizar networktools, network-tools      |             | instalación se puede introducir como N.     |
 |                     | también.|                                 |             |                                             |
 +---------------------+-------------------------------------------+-------------+---------------------------------------------+


Si la instalación procede de usuario, durante el proceso de instalación de los siguientes pasos están involucrados,

* Construye el árbol de dependencias.
* Lee la información de estado.
* Lista outs los nuevos paquetes que está instalando.
* Detalles sobre el número de archivos actualizados, recién instalados, retirados y no actualizados.

La siguiente captura de pantalla representa gráficamente el proceso anteriormente descrito de la instalación.

.. code-block:: bash

 kevell@corp:/# ptconfigure NetworkTools install
 Install Network Tools? (Y/N)
 Y
 *******************************
 *        Pharaoh Tools        *
 *         !Network Tools!!        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
  traceroute
 0 upgraded, 1 newly installed, 0 to remove and 301 not upgraded.
 Need to get 45.0 kB of archives.
 After this operation, 176 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/universe traceroute amd64 1:2.0.20-0ubuntu0.1 [45.0 kB]
 Fetched 45.0 kB in 4s (10.0 kB/s)
 Selecting previously unselected package traceroute.
 (Reading database ... 182980 files and directories currently installed.)
 Preparing to unpack .../traceroute_1%3a2.0.20-0ubuntu0.1_amd64.deb ...
 Unpacking traceroute (1:2.0.20-0ubuntu0.1) ...
 Processing triggers for man-db (2.6.7.1-1) ...
 Setting up traceroute (1:2.0.20-0ubuntu0.1) ...
 update-alternatives: using /usr/bin/traceroute.db to provide /usr/bin/traceroute (traceroute) in auto mode
 update-alternatives: using /usr/bin/lft.db to provide /usr/bin/lft (lft) in auto mode
 update-alternatives: using /usr/bin/traceproto.db to provide /usr/bin/traceproto (traceproto) in auto mode
 update-alternatives: using /usr/sbin/tcptraceroute.db to provide /usr/sbin/tcptraceroute (tcptraceroute) in auto mode
 [Pharaoh Logging] Adding Package traceroute from the Packager Apt executed correctly
 [Pharaoh Logging] Package netstat from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package lsof from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package telnet from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package ps from the Packager Apt is already installed, so not installing
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 NetworkTools: Success
 ------------------------------
 Installer Finished
 ******************************

Beneficios
--------------

Este módulo ayuda en la instalación del conjunto de herramientas de red comunes. Esto beneficia a los usuarios para instalar varias herramientas que pueden ser útiles al trabajo en red con otros ordenadores, tanto dentro de la red ya través de internet. Esto ayuda a los usuarios que 
 trabajan con máquinas remotas.
