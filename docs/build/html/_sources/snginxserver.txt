=============
NginxServer
=============

Synopsis
---------

Nginx, pronounced "Engine X", is a high-performance Web server. The Nginx Web Server is a light weight and versatile server that can be configured for all the different tasks that many modern websites demand. Ngnix server acts as a facilitator to the users in configuring applications settings. Few examples for applications settings includes mysql admin user, host, pass. Nginx is making headlines as the new Web server of choice for many webmasters. The top reason for its popularity is its speed. Nginx is faster than Apache in non-testing environments because its architecture is event driven while Apache's is process driven. The ptconfigure modules acts as a way through for installing this Nginx Server.

Help Command
------------

The help command leads the users regarding the purpose and as well as about the options that are included in the Ngnix server module. The help command lists out the alternative parameters of Ngnix server. It also describes the syntax for installing Ngnix server. The help command for Ngnix server is given below.

.. code-block:: bash

	ptconfigure nginx-server help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda bajo Nginx Server.

.. code-block:: bash


	kevell@corp:/# ptconfigure NginxServer help
	******************************


	This command is part of Core and provides you  with a method by which you can configure Application Settings.
	You can configure default application settings, ie: mysql admin user, host, pass

	NginxServer, nginx-server, nginxserver

        - install
        Installs Nginx HTTP Server
        example: ptconfigure nginx-server install

	------------------------------
	End Help
	******************************

instalación
------------

Instalación del servidor Nginx es más simple utilizando el siguiente comando como se muestra:

.. code-block:: bash

	ptconfigure nginx-server install

Después de introducir el comando anterior las siguientes operaciones como se muestra en el formato tabular ocurre.

.. cssclass:: table-bordered

 +---------------------+-------------------------------------------+-------------+-------------------------------------------+
 | Parámetros          | Parámetro Alternativa                     | Opciones    | Comentarios                               |
 +=====================+===========================================+=============+===========================================+
 |ptconfigure          | En lugar de Nginx Server, las siguientes  | Y(Yes)      | Si el usuario desea continuar el proceso  |
 |nginx-server         | alternativas también se pueden utilizar:  |             | de instalación se puede introducir        |
 |install? (Y/N)       | NginxServer, nginx-server, nginxserver.   |             | como Y.                                   |
 +---------------------+-------------------------------------------+-------------+-------------------------------------------+
 |ptconfigure          | En lugar de Nginx Server, las siguientes  | N(No)       | Si el usuario desea abandonar el proceso  |
 |nginx-server         | alternativas también se pueden utilizar:  |             | de instalación se puede introducir        |
 |install? (Y/N)       | NginxServer, nginx-server, nginxserver.|  |             | como N.                                   |
 +---------------------+-------------------------------------------+-------------+-------------------------------------------+

Si el usuario continúa el proceso de instalación, se instalará el servidor HTTP Nginx. Si ya está el paquete existe de Nginx en la máquina de los usuarios, a continuación, aparecerá un mensaje para indicar al usuario como Nginx es ya existe en esa máquina. Finalmente se generan informes con resultados claros y el estado. La siguiente captura de pantalla explica el proceso mencionado anteriormente pictóricamente.

.. code-block:: bash
	

	Kevell@corp:/# ptconfigure nginx-server install
	
	Install Nginx Server? (Y/N) 
	y	
	*******************************
	*        Pharaoh Tools        *
	*         Nginx Server!       *
	*******************************
	Reading package lists...
	Building dependency tree...
	Reading state information...
	The following extra packages will be installed:
	nginx-common nginx-core
	Suggested packages:
	fcgiwrap nginx-doc
	The following NEW packages will be installed:
	nginx nginx-common nginx-core
	0 upgraded, 3 newly installed, 0 to remove and 278 not upgraded.
	Need to get 347 kB of archives.
	After this operation, 1,295 kB of additional disk space will be used.
	Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main nginx-common all 1.4.6-1ubuntu3.1 [17.9 kB]
	Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main nginx-core amd64 1.4.6-1ubuntu3.1 [324 kB]
	Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main nginx all 1.4.6-1ubuntu3.1 [5,218 B]
	Fetched 347 kB in 3s (104 kB/s)
	Selecting previously unselected package nginx-common.
	(Reading database ... 168194 files and directories currently installed.)
	Preparing to unpack .../nginx-common_1.4.6-1ubuntu3.1_all.deb ...
	Unpacking nginx-common (1.4.6-1ubuntu3.1) ...
	Selecting previously unselected package nginx-core.
	Preparing to unpack .../nginx-core_1.4.6-1ubuntu3.1_amd64.deb ...
	Unpacking nginx-core (1.4.6-1ubuntu3.1) ...
	Selecting previously unselected package nginx.
	Preparing to unpack .../nginx_1.4.6-1ubuntu3.1_all.deb ...
	Unpacking nginx (1.4.6-1ubuntu3.1) ...
	Processing triggers for ureadahead (0.100.0-16) ...
	ureadahead will be reprofiled on next reboot
	Processing triggers for ufw (0.34~rc-0ubuntu2) ...
	Processing triggers for man-db (2.6.7.1-1) ...
	Setting up nginx-common (1.4.6-1ubuntu3.1) ...
	Processing triggers for ureadahead (0.100.0-16) ...
	Processing triggers for ufw (0.34~rc-0ubuntu2) ...
	Setting up nginx-core (1.4.6-1ubuntu3.1) ...
	Setting up nginx (1.4.6-1ubuntu3.1) ...
	[Pharaoh Logging] Adding Package nginx from the Packager Apt executed correctly
	... All done!
	*******************************
	Thanks for installing , visit www.pharaohtools.com for more
	******************************


	Single App Installer:
	--------------------------------------------
	NginxServer: Success
	------------------------------
	Installer Finished
	******************************

Beneficios
----------

* Al utilizar el usuario esta Nginx Server puede configurar sus ajustes de la aplicación.
* Los parámetros utilizados en ayuda de instalación y operaciones no son sensibles, que es una ventaja añadida, mientras que en comparación 
  con otros.
* Nginx es rápido, ya que no necesita para crear un nuevo proceso para cada nueva solicitud.
* Nginx utiliza muy poca memoria, especialmente para páginas Web estáticas.
* Nginx se puede utilizar con una amplia gama de sistemas.
* Nginx es altamente escalable, y el rendimiento no depende de hardware.
* Nginx es fácil de instalar y configurar.
* Al igual que Apache, Nginx tiene todas las características que usted esperaría de un servidor web líder:
* Fichero estático de servir.
* Soporte SSL / TLS.
* Hosts virtuales.
* Invertir proxy.
* El equilibrio de carga.
* Compresión.
* Los controles de acceso.
* Reescritura de URL.
* Registro personalizado.
* Del lado del servidor incluye.
* WebDAV.
* Streaming FLV.
* FastCGI.

