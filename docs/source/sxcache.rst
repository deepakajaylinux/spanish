==========
Xcache
==========

sinopsis
---------

XCache es un cacher código de operación libre de código abierto, está diseñado para mejorar el rendimiento de la ejecución de scripts PHP en servidores. Optimiza el rendimiento eliminando el tiempo de compilación de código PHP en caché la versión compilada del código en la memoria y de esta manera la versión compilada de cargas el script PHP directamente desde la memoria.

comando Ayuda
----------------

Este comando ayuda a determinar el uso de xcache. Enumera los parámetros alternativos de xcache. También describe la sintaxis para el funcionamiento del módulo xcache. El comando ayuda para xcache se muestra a continuación.

.. code-block:: bash

	ptconfigure xcache help

La representación pictórica del comando anterior se enumera a continuación,

.. code-block:: bash

 kevell@corp:/# ptconfigure xcache help
 ******************************


  This command allows you to update Xcache.

  Xcache, xcache

        - install
        Installs the latest version of xcache
        example: ptconfigure xcache install

 ------------------------------
 End Help
 ******************************


instalación
-------------


El comando utilizado para instalar el módulo xcache en el terminal se enumera a continuación,

.. code-block:: bash

        ptconfigure xcache install

El comando anterior pretende instalar la última versión de xcache y sus dependencias.

La representación pictórica del comando anterior se enumera a continuación,

.. code-block:: bash

 kevell@corp:/# ptconfigure xcache install
 Install Xcache? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Xcache!        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-56147605410.sh
 chmod 755 /tmp/ptconfigure-temp-script-56147605410.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-56147605410.sh Permissions
 Executing /tmp/ptconfigure-temp-script-56147605410.sh
 --2015-03-20 17:05:11--  http://kr.archive.ubuntu.com/ubuntu/pool/universe/x/xcache/php5-xcache_3.1.0-2_amd64.deb
 Resolving kr.archive.ubuntu.com (kr.archive.ubuntu.com)... 103.22.220.133
 Connecting to kr.archive.ubuntu.com (kr.archive.ubuntu.com)|103.22.220.133|:80... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: 108582 (106K) [application/x-debian-package]
 Saving to: ‘php5-xcache_3.1.0-2_amd64.deb.1’

 100%[=======================================================================================================>] 1,08,582    36.1KB/s   in 2.9s   

 2015-03-20 17:05:15 (36.1 KB/s) - ‘php5-xcache_3.1.0-2_amd64.deb.1’ saved [108582/108582]

 php5_invoke xcache: already enabled for apache2 SAPI
 php5_invoke xcache: already enabled for cli SAPI
 AH00558: apache2: Could not reliably determine the server's fully qualified domain name, using 127.0.1.1. Set the 'ServerName' directive globally to suppress this message
 (Reading database ... 195553 files and directories currently installed.)
 Preparing to unpack php5-xcache_3.1.0-2_amd64.deb ...
 Unpacking php5-xcache (3.1.0-2) over (3.1.0-2) ...
 Setting up php5-xcache (3.1.0-2) ...
 * Restarting web server apache2
   ...done.
 Temp File /tmp/ptconfigure-temp-script-56147605410.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Xcache: Success
 ------------------------------
 Installer Finished
 ******************************



parámetros alternativos
-------------------------

Hay dos parámetros alternativos que pueden utilizarse en la línea de comandos.


Xcache, xcache


beneficios
-----------

* Operación estable 
* rápida adaptación a las nuevas versiones PHP 
* instalación Simple









