==============
NagiosServer
==============

Sinopsis
-------------

Nagios es una aplicación de software de monitorización del sistema informático de código abierto, monitoreo de red y monitoreo de la infraestructura. Nagios ofrece monitoreo y servicios de alerta para los servidores, switches, aplicaciones y servicios. Se alerta a los usuarios cuando las cosas van mal y los alerta por segunda vez cuando el problema se ha resuelto.

Nagios, creado originalmente bajo el nombre Netsaint, fue escrito y en la actualidad se mantiene por Ethan Galstad junto con un grupo de desarrolladores que están manteniendo activamente tanto el oficial y plugins no oficiales. Nagios fue originalmente diseñado para ejecutarse en Linux, pero también funciona bien en otras variantes de Unix. Es software libre licenciado bajo los términos de la Licencia Pública General GNU versión 2 publicada por la Free Software Foundation.

Ayuda Comando
----------------------

Este comando ayuda a determinar el uso del módulo de Nagios. El usuario se llega a saber acerca de la diferente forma / formato de ejecutar este módulo. Este comando guía al usuario final a conocer el propósito de este comando. A continuación dado son el mando y la pantalla del mismo.

.. code-block:: bash
        
	        ptconfigure nagios help

La captura de pantalla pictórica del comando anterior se enumeran a continuación,

.. code-block:: bash

 kevell@corp:/# ptconfigure nagiosserver help

 ******************************


  This command is part of Core and provides you with a method by which you can install Nagios.

  NagiosServer, nagios-server, nagiosserver, nagios

        - install
        Installs Nagios Network Monitoring Server
        example: ptconfigure nagios-server install

 ------------------------------
 End Help
 ******************************

instalación
----------------

Este comando ayuda en la instalación del Nagios en el sistema. El siguiente comando dado se ejecutará el proceso de instalación.

.. code-block:: bash
        
	        ptconfigure nagios install

La representación gráfica de la orden anterior se enumeran a continuación,

.. code-block:: bash

 kevell@corp:/# ptconfigure nagios-server install

 Install Nagios Server? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Nagios Server!        *
 *******************************

 * Starting nagios3 monitoring daemon nagios3                                                                                  [ OK ] 
 enabling Apache2 config...
 apache2_invoke: Enable module cgi
 * Restarting web server apache2                                                                                                  AH00558:  
 apache2: Could not reliably determine the server's fully qualified domain name, using 127.0.1.1. Set the 'ServerName' directive globally to 
 suppress this message
                                                                                                                               [ OK ]
 apache2_invoke: Enable configuration nagios3
 * Reloading web server apache2                                                                                                        * 
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  libjs-jquery nagios-images nagios3-cgi nagios3-common nagios3-core
 Suggested packages:
  javascript-common
 The following NEW packages will be installed:
  libjs-jquery nagios-images nagios3 nagios3-cgi nagios3-common nagios3-core
 0 upgraded, 6 newly installed, 0 to remove and 250 not upgraded.
 Need to get 3,748 kB of archives.
 After this operation, 12.3 MB of additional disk space will be used.
 Get:1 http://archive.ubuntu.com/ubuntu/ trusty/main libjs-jquery all 1.7.2+dfsg-2ubuntu1 [78.8 kB]
 Get:2 http://archive.ubuntu.com/ubuntu/ trusty/main nagios-images all 0.8 [2,589 kB]
 Get:3 http://archive.ubuntu.com/ubuntu/ trusty/main nagios3-common all 3.5.1-1ubuntu1 [53.7 kB]
 Get:4 http://archive.ubuntu.com/ubuntu/ trusty/main nagios3-cgi amd64 3.5.1-1ubuntu1 [794 kB]
 Get:5 http://archive.ubuntu.com/ubuntu/ trusty/main nagios3-core amd64 3.5.1-1ubuntu1 [231 kB]
 Get:6 http://archive.ubuntu.com/ubuntu/ trusty/main nagios3 amd64 3.5.1-1ubuntu1 [1,528 B]
 Preconfiguring packages ...
 Fetched 3,748 kB in 1min 11s (52.1 kB/s)
 Selecting previously unselected package libjs-jquery.
 (Reading database ... 231932 files and directories currently installed.)
 Preparing to unpack .../libjs-jquery_1.7.2+dfsg-2ubuntu1_all.deb ...
 Unpacking libjs-jquery (1.7.2+dfsg-2ubuntu1) ...
 Selecting previously unselected package nagios-images.
 Preparing to unpack .../nagios-images_0.8_all.deb ...
 Unpacking nagios-images (0.8) ...
 Selecting previously unselected package nagios3-common.
 Preparing to unpack .../nagios3-common_3.5.1-1ubuntu1_all.deb ...
 Unpacking nagios3-common (3.5.1-1ubuntu1) ...
 Selecting previously unselected package nagios3-cgi.
 Preparing to unpack .../nagios3-cgi_3.5.1-1ubuntu1_amd64.deb ...
 Unpacking nagios3-cgi (3.5.1-1ubuntu1) ...
 Selecting previously unselected package nagios3-core.
 Preparing to unpack .../nagios3-core_3.5.1-1ubuntu1_amd64.deb ...
 Unpacking nagios3-core (3.5.1-1ubuntu1) ...
 Selecting previously unselected package nagios3.
 Preparing to unpack .../nagios3_3.5.1-1ubuntu1_amd64.deb ...
 Unpacking nagios3 (3.5.1-1ubuntu1) ...
 Processing triggers for ureadahead (0.100.0-16) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up libjs-jquery (1.7.2+dfsg-2ubuntu1) ...
 Setting up nagios-images (0.8) ...
 Setting up nagios3-common (3.5.1-1ubuntu1) ...
 Setting up nagios3-cgi (3.5.1-1ubuntu1) ...
 Setting up nagios3-core (3.5.1-1ubuntu1) ...
 Setting up nagios3 (3.5.1-1ubuntu1) ...
 [Pharaoh Logging] Adding Package nagios3 from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 NagiosServer: Success
 ------------------------------
 Installer Finished
 ******************************



Opciones
-----------
.. cssclass:: table-bordered

 +----------------------+-------------------------------------------------------+--------------+------------------------------------------+
 | Parámetros           | Parámetro Alternativa                                 | Opciones     | Comentarios                              |
 +======================+=======================================================+==============+==========================================+
 |Install Nagios        | Hay cuatro parámetros alternativos que pueden ser     | Y(Yes)       | Si el usuario desea continuar el proceso |
 |Server? (Y/N)         | utilizados en la línea de comandos.NagiosServer,      |              | de instalación se puede introducir       |
 |                      | nagios-server, nagiosserver, nagios Por               |              | como Y.                                  |
 |                      | ejemplo: ptconfigure nagios install/                  |              |                                          |
 |                      | ptconfigure nagiosserver install                      |              |                                          |
 +----------------------+-------------------------------------------------------+--------------+------------------------------------------+
 |Install Nagios        | Hay cuatro parámetros alternativos que pueden ser     | N(No)        | Si el usuario desea abandonar el proceso |
 |Server? (Y/N)         | utilizados en la línea de comandos.NagiosServer,      |              | de instalación se puede introducir como  |
 |                      | nagios-server, nagiosserver, nagios Por            	|              | N.                                       |
 |                      | ejemplo: ptconfigure nagios install/                  |              |                                          |
 |                      | ptconfigure nagiosserver install|                     |              |                                          |
 +----------------------+-------------------------------------------------------+--------------+------------------------------------------+


Beneficios
--------------

* Seguimiento de los servicios de red (SMTP, POP3, HTTP, NNTP, ICMP, SNMP, FTP, SSH)
* Seguimiento de los recursos de acogida (carga del procesador, uso de disco, los registros del sistema) en la mayoría de los sistemas 
  operativos de red, incluyendo Microsoft Ventanas con plugin de la NSClient ++ o Comprobar MK.
* Monitoreo de cualquier otra cosa, como sondas (temperatura, alarmas, etc.) Que tienen la capacidad de enviar los datos recogidos a través de 
  una red de  plugins escritos específicamente
* Vigilancia a través de ejecutar scripts de forma remota a través de Nagios Ejecutor Plugin remoto
* Remoto monitoreo apoyado a través de SSH o SSL cifrada túneles.
* Un diseño simple plugin que permite a los usuarios desarrollar fácilmente sus propias comprobaciones de servicio en función de las necesidades, mediante el uso de sus herramientas de elección  (shell scripts, C ++, Perl, Ruby, Python, PHP, C #, etc.)
* plugins gráficas de datos disponible
* comprobaciones de servicio paralelizado
* La capacidad de definir jerarquías de acogida de red utilizando hosts "padre", lo que permite la detección de y la distinción entre hosts 
  que están abajo o fuera de cobertura
* Contacto notificaciones cuando se producen problemas de servicio o de acogida y se resuelven (a través de correo electrónico, buscapersonas, 
  SMS, o cualquier método definido por el usuario a través de plugin de sistema)
* La capacidad de definir controladores de eventos para ejecutar los servicios o realizar eventos para la resolución de problemas de manera 
  proactiva
* Registro automático de rotación de archivos
* Apoyo a la implementación de los ejércitos de monitoreo redundantes
* Una interfaz web opcional para ver el estado actual de la red, notificaciones, historial de problemas, archivos, etc. log
* Almacenamiento de datos a través de archivos de texto en lugar de la base de datos
