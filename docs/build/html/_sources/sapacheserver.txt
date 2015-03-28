==============
ApacheServer
==============

Sinopsis
-----------
Esta módulos pretende instalar el servidor Apache. Sin ningún tipo de solicitud, se instalará automáticamente la versión actual del servidor apache mientras instalación.

comando Ayuda
--------------------

El comando de ayuda describe sobre el propósito y los comandos disponibles bajo estos módulos. También explica el comando para instalar el módulo en particular.

.. code-block:: bash

 		ptconfigure ApacheServer help

La captura de pantalla como se muestra a continuación, representar visualmente el uso del comando de ayuda en virtud de este módulo.

.. code-block:: bash


 kevell@corp:/# ptconfigure ApacheServer help
 ******************************


  This command is part of Core and provides you  with a method by which you can install Apache HTTP Server

  ApacheServer, apache-server, apacheserver

        - install
        Installs Apache HTTP Server
        example: ptconfigure apacheserver install

 ------------------------------
 End Help
 ******************************

Instalación
-------------

Es más fácil de instalar esta herramienta en particular en virtud de ptconfigure por el simple uso de la orden dada a continuación,

.. code-block:: bash

		ptconfigure ApacheServer install

Después de dar el comando anterior, la herramienta le preguntará como

Install Apache Server? (Y/N)

si se le da una entrada como Y, el módulo se instalan correctamente.

La captura de pantalla que figura a continuación explica visualmente sobre los pasos y comandos consiste en la instalación.

.. code-block:: bash


 kevell@corp:/# ptconfigure ApacheServer install
 Install Apache Server? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Apache Server!        *
 *******************************
 AH00558: apache2: Could not reliably determine the server's fully qualified domain name, using 127.0.1.1. Set the 'ServerName' directive globally to suppress this message
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following packages were automatically installed and are no longer required:
   php5-cli php5-readline
 Use 'apt-get autoremove' to remove them.
 Suggested packages:
  apache2-doc apache2-suexec-pristine apache2-suexec-custom apache2-utils
 The following NEW packages will be installed:
  apache2
 0 upgraded, 1 newly installed, 0 to remove and 39 not upgraded.
 Need to get 0 B/87.4 kB of archives.
 After this operation, 473 kB of additional disk space will be used.
 Selecting previously unselected package apache2.
 (Reading database ... 193457 files and directories currently installed.)
 Preparing to unpack .../apache2_2.4.7-1ubuntu4.4_amd64.deb ...
 Unpacking apache2 (2.4.7-1ubuntu4.4) ...
 Processing triggers for ureadahead (0.100.0-16) ...
 ureadahead will be reprofiled on next reboot
 Processing triggers for ufw (0.34~rc-0ubuntu2) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up apache2 (2.4.7-1ubuntu4.4) ...
 Enabling module mpm_event.
 Enabling module authz_core.
 Enabling module authz_host.
 Enabling module authn_core.
 Enabling module auth_basic.
 Enabling module access_compat.
 Enabling module authn_file.
 Enabling module authz_user.
 Enabling module alias.
 Enabling module dir.
 Enabling module autoindex.
 Enabling module env.
 Enabling module mime.
 Enabling module negotiation.
 Enabling module setenvif.
 Enabling module filter.
 Enabling module deflate.
 Enabling module status.
 Enabling conf charset.
 Enabling conf localized-error-pages.
 Enabling conf other-vhosts-access-log.
 Enabling conf security.
 Enabling conf serve-cgi-bin.
 Enabling site 000-default.
 * Starting web server apache2
 * 
 Processing triggers for ureadahead (0.100.0-16) ...
 Processing triggers for ufw (0.34~rc-0ubuntu2) ...
 [Pharaoh Logging] Adding Package apache2 from the Packager Apt executed correctly
 [Pharaoh Logging] Restarting apache2 service
 AH00558: apache2: Could not reliably determine the server's fully qualified domain name, using 127.0.1.1. Set the 'ServerName' directive globally to suppress this message
 * Restarting web server apache2
   ...done.
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 ApacheServer: Success
 ------------------------------
 Installer Finished
 ******************************



Opciones
------------

.. cssclass:: table-bordered

 +-----------------------------+------------------------------------+----------------+-------------------------------------------+
 | Parámetros                  | parámetros alternativos            | Necesario      | Comentario                                |
 +=============================+====================================+================+===========================================+
 |Install Apache Server? (Y/N) | en lugar de ApacheServer, podemos  | Y(Yes)         | Si el usuario da entrada como sí, se va   |
 |                             | utilizar apache-server,            |                | a proceder la instalación                 |
 |                             | apacheserver también.              |                |                                           |
 +-----------------------------+------------------------------------+----------------+-------------------------------------------+
 |Install Apache Server? (Y/N) | en lugar de ApacheServer, podemos  | N(No)          | Si el usuario da entrada como no, que     |
 |                             | utilizar apache-server,            |                | se cerrará el proceso de instalación      |
 |                             | apacheserver también.|             |                |                                           |
 +-----------------------------+------------------------------------+----------------+-------------------------------------------+


versión
---------

Mientras que la herramienta está procesando lo hará agarra automáticamente la versión actualizada más reciente y lo hace para estar listo para la instalación.

Beneficios
-----------

* Esta módulos de ayuda a los usuarios a instalar el servidor apache. Simplifica el trabajo de los usuarios durante la instalación del servidor   como su  comprobar automáticamente la versión actual del servidor apache.
* Es-acomodada en CentOS y así como en Ubuntu.
* Los parámetros utilizados en la declaración no se distingue entre mayúsculas y minúsculas, lo que es una ventaja añadida.

