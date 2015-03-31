=========
Citadel
=========

sinopsis
----------

Citadel es una plataforma completa y rica en características de groupware de código abierto. El sistema Citadel es extremadamente versátil. Proporciona numerosas extremos delanteros de presentar a los usuarios, tales como una interfaz basada en texto, una interfaz web de estilo AJAX, y muchos clientes PIM populares usando SMTP / POP / IMAP. Todos estos pueden ser utilizados simultáneamente.

También es muy escalable. No sólo puede un soporte de servidor Citadel bien equipado a un gran número de usuarios simultáneos, pero también se puede construir una red distribuida de Ciudadela nodos que comparten habitaciones y su contenido.

Ayuda Comando
----------------------

Este comando ayuda a determinar el uso del módulo de Ciudadela. El usuario se llega a saber acerca de las diferentes formas / formato para ejecutar este módulo. El parámetro alternativa que se utilizan en la declaración está claramente definido en la opción de ayuda. Este comando guía al usuario final saber el comando utilizado para la instalación. A continuación dado son el comando.

.. code-block:: bash
     	
		ptconfigure  Citadel help

La representación gráfica de la pantalla aparece a continuación,

.. code-block:: bash
 

 kevell@corp:/# ptconfigure Citadel help
 ******************************


  This module installs Citadel Server and provides configuration

  Citadel, citadel-server, citadel

        - install
        Installs Citadel Server
        example: ptconfigure citadel install

        - configure
        Configure E-Mail with Citadel Server
        example: ptconfigure citadel configure

 ------------------------------
 End Help
 ******************************

instalación
--------------

Cuando el usuario tiene que instalar el servidor Citadel en la máquina, puede introducir los siguientes comandos para instalar la ciudadela-suite. El sistema ejecutará el proceso de instalación. A continuación dado son el mando y la pantalla del mismo.

.. code-block:: bash
       
	        ptconfigure Citadel  install

.. code-block:: bash




 kevell@corp:/# ptconfigure citadel install 


 Install Citadel Server? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         Citadel Server!        * 
 ******************************* 
 Creating /tmp/ptconfigure-temp-script-77287537627.sh 
 chmod 755 /tmp/ptconfigure-temp-script-77287537627.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-77287537627.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-77287537627.sh 
 Temp File /tmp/ptconfigure-temp-script-77287537627.sh Removed 
 [Pharaoh Logging] Package debconf-utils from the Packager Apt is already installed, so not installing 
 [Pharaoh Logging] Stopping apache2 service 
  * Stopping web server apache2 
  * 
 Creating /tmp/ptconfigure-temp-script-39510208428.sh 
 chmod 755 /tmp/ptconfigure-temp-script-39510208428.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-39510208428.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-39510208428.sh 
 Temp File /tmp/ptconfigure-temp-script-39510208428.sh Removed 
 invoke-rc.d: initscript lighttpd, action "reload" failed. 
 apache2_invoke: Enable configuration javascript-common 
 invoke-rc.d: initscript apache2, action "reload" failed. 
 Reading package lists... 
 Building dependency tree... 
 Reading state information... 
 The following extra packages will be installed: 
  citadel-client citadel-mta citadel-server citadel-webcit javascript-common 
  libcitadel4 libev4 libjs-prototype libjs-scriptaculous libsieve2-1 tinymce 
 Suggested packages: 
  localepurge 
 Recommended packages: 
  db4.6-util 
 The following NEW packages will be installed: 
  citadel-client citadel-mta citadel-server citadel-suite citadel-webcit 
  javascript-common libcitadel4 libev4 libjs-prototype libjs-scriptaculous 
  libsieve2-1 tinymce 
 0 upgraded, 12 newly installed, 0 to remove and 86 not upgraded. 
 Need to get 1,955 kB of archives. 
 After this operation, 8,788 kB of additional disk space will be used. 
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/main javascript-common all 11 [6,066 B] 
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libjs-prototype all 1.7.1-3 [44.2 kB] 
 Get:3 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libjs-scriptaculous all 1.9.0-2 [107 kB] 
 Get:4 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libsieve2-1 amd64 2.2.6-1.2 [73.1 kB] 
 Get:5 http://in.archive.ubuntu.com/ubuntu/ trusty/universe tinymce all 3.4.8+dfsg0-1 [488 kB] 
 Get:6 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libcitadel4 amd64 8.24-1 [60.5 kB] 
 Get:7 http://in.archive.ubuntu.com/ubuntu/ trusty/universe citadel-client amd64 8.24-1 [78.5 kB] 
 Get:8 http://in.archive.ubuntu.com/ubuntu/ trusty/universe libev4 amd64 1:4.15-3 [29.6 kB] 
 Get:9 http://in.archive.ubuntu.com/ubuntu/ trusty/universe citadel-server amd64 8.24-1 [348 kB] 
 Get:10 http://in.archive.ubuntu.com/ubuntu/ trusty/universe citadel-mta amd64 8.24-1 [4,520 B] 
 Get:11 http://in.archive.ubuntu.com/ubuntu/ trusty/universe citadel-webcit amd64 8.24-dfsg-1 [712 kB] 
 Get:12 http://in.archive.ubuntu.com/ubuntu/ trusty/universe citadel-suite all 8.24-dfsg-1 [3,542 B] 
 Preconfiguring packages ... 
 Fetched 1,955 kB in 21s (92.5 kB/s) 
 Selecting previously unselected package javascript-common. 
 (Reading database ... 194611 files and directories currently installed.) 
 Preparing to unpack .../javascript-common_11_all.deb ... 
 Unpacking javascript-common (11) ... 
 Selecting previously unselected package libjs-prototype. 
 Preparing to unpack .../libjs-prototype_1.7.1-3_all.deb ... 
 Unpacking libjs-prototype (1.7.1-3) ... 
 Selecting previously unselected package libjs-scriptaculous. 
 Preparing to unpack .../libjs-scriptaculous_1.9.0-2_all.deb ... 
 Unpacking libjs-scriptaculous (1.9.0-2) ... 
 Selecting previously unselected package libsieve2-1. 
 Preparing to unpack .../libsieve2-1_2.2.6-1.2_amd64.deb ... 
 Unpacking libsieve2-1 (2.2.6-1.2) ... 
 Selecting previously unselected package tinymce. 
 Preparing to unpack .../tinymce_3.4.8+dfsg0-1_all.deb ... 
 Unpacking tinymce (3.4.8+dfsg0-1) ... 
 Selecting previously unselected package libcitadel4. 
 Preparing to unpack .../libcitadel4_8.24-1_amd64.deb ... 
 Unpacking libcitadel4 (8.24-1) ... 
 Selecting previously unselected package citadel-client. 
 Preparing to unpack .../citadel-client_8.24-1_amd64.deb ... 
 Unpacking citadel-client (8.24-1) ... 
 Selecting previously unselected package libev4. 
 Preparing to unpack .../libev4_1%3a4.15-3_amd64.deb ... 
 Unpacking libev4 (1:4.15-3) ... 
 Selecting previously unselected package citadel-server. 
 Preparing to unpack .../citadel-server_8.24-1_amd64.deb ... 
 Unpacking citadel-server (8.24-1) ... 
 Selecting previously unselected package citadel-mta. 
 Preparing to unpack .../citadel-mta_8.24-1_amd64.deb ... 
 Unpacking citadel-mta (8.24-1) ... 
 Selecting previously unselected package citadel-webcit. 
 Preparing to unpack .../citadel-webcit_8.24-dfsg-1_amd64.deb ... 
 Unpacking citadel-webcit (8.24-dfsg-1) ... 
 Selecting previously unselected package citadel-suite. 
 Preparing to unpack .../citadel-suite_8.24-dfsg-1_all.deb ... 
 Unpacking citadel-suite (8.24-dfsg-1) ... 
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ... 
 Processing triggers for ureadahead (0.100.0-16) ... 
 Setting up javascript-common (11) ... 
 * Reloading web server configuration lighttpd 
   ...fail! 
 * Reloading web server apache2 
 * 
 * Apache2 is not running 
 Setting up libjs-prototype (1.7.1-3) ... 
 Setting up libjs-scriptaculous (1.9.0-2) ... 
 Setting up libsieve2-1 (2.2.6-1.2) ... 
 Setting up tinymce (3.4.8+dfsg0-1) ... 
 Setting up libcitadel4 (8.24-1) ... 
 Setting up citadel-client (8.24-1) ... 
 Adding group `citadel' (GID 132) ... 
 Done. 
 Adding system user `citadel' (UID 123) ... 
 Adding new user `citadel' (UID 123) with group `citadel' ... 
 Not creating home directory `/var/lib/citadel'. 
 Setting up libev4 (1:4.15-3) ... 
 Setting up citadel-server (8.24-1) ... 
 Setting up citadel-webcit (8.24-dfsg-1) ... 
 Processing triggers for ureadahead (0.100.0-16) ... 
 Setting up citadel-mta (8.24-1) ... 
 Setting up citadel-suite (8.24-dfsg-1) ... 
 Processing triggers for libc-bin (2.19-0ubuntu6.6) ... 
 [Pharaoh Logging] Adding Package citadel-suite from the Packager Apt executed correctly 
 [Pharaoh Logging] Restarting citadel service 
 sendcommand: started (pid=24114) connecting to Citadel server at /var/run/citadel/citadel-admin.socket 
 200 karthik Citadel server ADMIN CONNECTION ready. 
 DOWN 
 231 Shutting down server.  Goodbye. 
 sendcommand: processing ended. 
 ....................... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 


 Single App Installer: 
 -------------------------------------------- 
 Citadel: Success 
 ------------------------------ 
 Installer Finished 
 ****************************** 



.. cssclass:: table-bordered


 +------------------------+----------------------------------------+---------------+-----------------------------------------+
 | Parámetros             | parámetros alternativos                | Necesario     | Comentario                              |
 +========================+========================================+===============+=========================================+
 |ptconfigure Citadel     | Cualquiera de los tres parámetros      | Y(Yes)        | Una vez que el usuario proporciona esta |
 |Install? (Y/N)          | alternativa se puede utilizar en el    |               | opción, sistema comienza proceso        |
 |                        | comando Citadel, citadel-server,       |               | de instalación                          |
 |                        | citadel Por ejemplo:                   |               |                                         |
 |                        | ptconfigure citadel-server Install     |               |                                         |
 +------------------------+----------------------------------------+---------------+-----------------------------------------+
 |ptconfigure Citadel     | Cualquiera de los tres parámetros      | N(No)         | Una vez que el usuario proporciona esta |
 |Install? (Y/N)          | alternativa se puede utilizar en el    |               | opción, Sistema detiene proceso         |
 |                        | comando Citadel, citadel-server,       |               | de instalación                          |
 |                        | citadel Por ejemplo:                   |               |                                         |
 |                        | ptconfigure citadel-server Install|    |               |                                         |
 +------------------------+----------------------------------------+---------------+-----------------------------------------+

configuración
------------------

Este comando ayuda a la hora de configurar el servidor Citadel. Una vez que se ejecute el comando a continuación se indica el sistema le proporciona el valor predeterminado para cada sección, si hay algún cambio que hacer, el usuario puede proporcionar los datos. El comando que se utiliza para la configuración se muestra a continuación.

.. code-block:: bash
         
	        ptconfigure Citadel configure

Beneficios
-------------

* Correo electrónico, calendario / programación, libretas de direcciones
* Los tablones de anuncios, correo servidor de listas, la mensajería instantánea
* Soporte de dominio múltiple
* Una interfaz web atractivo estilo AJAX intuitiva
