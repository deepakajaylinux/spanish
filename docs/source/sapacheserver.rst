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

 		cleopatra ApacheServer help

La captura de pantalla como se muestra a continuación, representar visualmente el uso del comando de ayuda en virtud de este módulo.

.. code-block:: bash


 kevell@corp:/# cleopatra ApacheServer help
 ******************************


  This command is part of Core and provides you  with a method by which you can install Apache HTTP Server

  ApacheServer, apache-server, apacheserver

        - install
        Installs Apache HTTP Server
        example: cleopatra apacheserver install

 ------------------------------
 End Help
 ******************************

Instalación
-------------

Es más fácil de instalar esta herramienta en particular en virtud de Cleopatra por el simple uso de la orden dada a continuación,

.. code-block:: bash

		cleopatra ApacheServer install

Después de dar el comando anterior, la herramienta le preguntará como

Install Apache Server? (Y/N)

si se le da una entrada como Y, el módulo se instalan correctamente.

La captura de pantalla que figura a continuación explica visualmente sobre los pasos y comandos consiste en la instalación.

.. code-block:: bash

 kevell@corp:/# cleopatra apacheserver install
 Install Apache Server? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         Apache Server!        *
 *******************************
 [Pharaoh Logging] Package apache2 from the Packager Apt is already installed, so not installing
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

