=========
PhpSSH
=========

sinopsis
-----------

  PhpSSH ahora se ha convertido en aún más fácil para su creación y funcionamiento. Por lo que es mucho más fácil de ptconfigure actualización automática a través PhpSSH. Tomando shell remoto, para llevar a cabo diferentes tareas es una norma, si el usuario tiene varios equipos de servidor en una infraestructura.

comando Ayuda
--------------------

En este comando ayuda, el usuario estará discutiendo una de estas herramientas, que fue diseñado para eliminar las fallas en los programas de shell remotos anteriores. tema ptconfigure de interés por este comando no es otro que el de Venta Segura, más conocido como phpSSH. El comando de la ayuda de la siguiente manera

.. code-block:: bash

                ptconfigure PHPSSH help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda bajo PHP SSH.

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPSSH help
 ******************************


  This command allows you to install the PHP SSH default Module

  PHPSSH, php-ssh, phpssh

        - install
        Installs the PECL PHP SSH Extension.
        example: ptconfigure phpssh install

 ------------------------------
 End Help
 ******************************

instalación
---------------------

Este es un proceso importante para instalar módulo Phpssh bajo ptconfigure simplemente usando el comando dado a continuación,

.. code-block:: bash
         
                ptconfigure phpssh install

Después de introducir el comando anterior, los siguientes pasos son involucrados durante el proceso de instalación como se describe en la tabla,

.. cssclass:: table-bordered

 +-----------------------+---------------------------------------+-------------+---------------------------------------------------+
 | Parámetros            | Parámetro Alternativa                 | Opciones    | Comentarios                                       |
 +=======================+=======================================+=============+===================================================+
 |Install PHP SSH? (Y/N) | En vez de usar PHP SSH Podemos        | Y(Yes)      | Si el usuario desea continuar el proceso de       |
 |                       | utilizar phpssh, php-ssh              |             | se puede introducir como Y.                       |
 +-----------------------+---------------------------------------+-------------+---------------------------------------------------+
 |Install PHP SSH? (Y/N) | En vez de usar PHP SSH Podemos        | N(No)       | Si el usuario desea abandonar el proceso de       |
 |                       | utilizar phpssh, php-ssh              |             | instalación se puede introducir como N.|          |
 +-----------------------+---------------------------------------+-------------+---------------------------------------------------+


Si el usuario procede de la instalación, durante el proceso de instalación se describe en las listas siguientes:

* Construye el árbol de dependencias.
* Lee la información de estado.
* Lista outs los paquetes adicionales que están instalando.
* Lista outs los nuevos paquetes que está instalando.
* Detalles sobre el número de archivos actualizados, recién instalados, retirados y no actualizados.

La siguiente captura de pantalla representa gráficamente el proceso anteriormente descrito de la instalación.

.. code-block:: bash


 kevell@corp:/# ptconfigure phpssh install
 Install PHP SSH? (Y/N)
 Y
 *******************************
 *        Pharaoh Tools        *
 *         PHP SSH!        *
 *******************************
 
 Creating config file /etc/php5/mods-available/ssh2.ini with new version
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libssh2-1
 The following NEW packages will be installed:
  libssh2-1 libssh2-php
 0 upgraded, 2 newly installed, 0 to remove and 301 not upgraded.
 Need to get 91.0 kB of archives.
 After this operation, 389 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libssh2-1 amd64 1.4.3-2 [66.3 kB]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libssh2-php amd64 0.12-1build1 [24.7 kB]
 Fetched 91.0 kB in 4s (19.8 kB/s)
 Selecting previously unselected package libssh2-1:amd64.
 (Reading database ... 183000 files and directories currently installed.)
 Preparing to unpack .../libssh2-1_1.4.3-2_amd64.deb ...
 Unpacking libssh2-1:amd64 (1.4.3-2) ...
 Selecting previously unselected package libssh2-php.
 Preparing to unpack .../libssh2-php_0.12-1build1_amd64.deb ...
 Unpacking libssh2-php (0.12-1build1) ...
 Setting up libssh2-1:amd64 (1.4.3-2) ...
 Setting up libssh2-php (0.12-1build1) ...
 Processing triggers for libc-bin (2.19-0ubuntu6) ...
 [Pharaoh Logging] Adding Package libssh2-php from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PHPSSH: Success
 ------------------------------
 Installer Finished
 ******************************		     

Beneficios
-----------------

* La primera y la más importante es la privacidad de la comunicación. Esto significa que la conexión, que proporciona un shell de login 
  remoto, debe estar encriptada para prevenir el espionaje.
* Debe haber un mecanismo para comprobar si los datos a enviar por cualquiera de las partes no se altera, ni manipula. En resumen, comprobación   de integridad es necesaria.
* Identidad de el servidor y el cliente debe ser proporcionada a la otra, para establecer una autenticación correcta.
* Mecanismos de cifrado y autenticación proporcionadas por PhpSSH mejora la seguridad en mayor medida.
