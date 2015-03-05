===========
VNC
===========

sinopsis
-------------

Este módulo ofrece asistencia para la instalación vnc4server través get apt. Se permite la conectividad para la máquina virtual. Facilita asegurar antes de la instalación.

Ayuda Comando
---------------------

El comando de ayuda proporciona una toma de conciencia con respecto al módulo de VNC. También describe acerca de las opciones que se pueden realizar en virtud de este módulo de VNC.

El comando de ayuda para este módulo VNC se da a continuación,

.. code-block:: bash

	ptconfigure vnc help

La captura de pantalla que figura a continuación muestra una representación gráfica sobre el uso del comando de ayuda bajo módulo de VNC.

.. code-block:: bash

 Kevell@corp:/# ptconfigure vnc help
 ******************************


        This command allows you to install VNC, the popular Virtual Machine Solution.

	 VNC, vnc

        - install
        Installs VNC through apt-get
        example: ptconfigure vnc install

	------------------------------
	End Help
	******************************

instalación
------------------

.. code-block:: bash
	
		ptconfigure vnc install

Después de introducir el comando como se indica más arriba, las siguientes operaciones se lleva a lugares.

.. cssclass:: table-bordered

 +-----------------------+-----------------------------+---------------+-------------------------------------------------+
 | Parámetros            | Parámetro Alternativa       | Opciones      | Comentarios                                     |
 +=======================+=============================+===============+=================================================+
 |Install VNC? (Y/N)     | VNC, vnc                    | Y(Yes)        | Si el usuario desea continuar el proceso de     |
 |                       |                             |               | instalación se puede introducir como Y.         |
 +-----------------------+-----------------------------+---------------+-------------------------------------------------+
 |Install VNC? (Y/N)     | VNC, vnc                    | N(No)         | Si el usuario desea abandonar el proceso de     |
 |                       |                             |               | instalación se puede introducir como N.|        |
 +-----------------------+-----------------------------+---------------+-------------------------------------------------+


Durante la instalación del servidor VNC realiza las siguientes operaciones como se indica a continuación:

* Lee la lista de paquetes, información de estado,
* Construye el árbol de dependencias.
* Instala los xbase-clientes como paquetes adicionales, vnc-java como paquetes sugeridos.
* Instala vnc4server xbase-clientes como nuevos paquetes.
* También muestra el número de archivos actualizados, recién instalado, quitar, no actualizado.

La captura de pantalla se indican a continuación, se explican los usuarios gráficamente en relación con el proceso de instalación.

.. code-block:: bash

 kevell@corp:/# ptconfigure vnc install
 Install VNC? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *          ! VNC !        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  xbase-clients
 Suggested packages:
  vnc-java
 The following NEW packages will be installed:
  vnc4server xbase-clients
 0 upgraded, 2 newly installed, 0 to remove and 8 not upgraded.
 Need to get 1,579 kB of archives.
 After this operation, 5,418 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty/universe xbase-clients all 1:7.7+1ubuntu8 [2,752 B]
 Get:2 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/universe vnc4server amd64 4.1.1+xorg4.3.0-37ubuntu5.0.1 [1,577 kB]
 Fetched 1,579 kB in 33s (46.6 kB/s)
 Selecting previously unselected package xbase-clients.
 (Reading database ... 211210 files and directories currently installed.)
 Preparing to unpack .../xbase-clients_1%3a7.7+1ubuntu8_all.deb ...
 Unpacking xbase-clients (1:7.7+1ubuntu8) ...
 Selecting previously unselected package vnc4server.
 Preparing to unpack .../vnc4server_4.1.1+xorg4.3.0-37ubuntu5.0.1_amd64.deb ...
 Unpacking vnc4server (4.1.1+xorg4.3.0-37ubuntu5.0.1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up xbase-clients (1:7.7+1ubuntu8) ...
 Setting up vnc4server (4.1.1+xorg4.3.0-37ubuntu5.0.1) ...
 update-alternatives: using /usr/bin/vnc4server to provide /usr/bin/vncserver (vncserver) in auto mode
 update-alternatives: using /usr/bin/Xvnc4 to provide /usr/bin/Xvnc (Xvnc) in auto mode
 update-alternatives: using /usr/bin/x0vnc4server to provide /usr/bin/x0vncserver (x0vncserver) in auto mode
 update-alternatives: using /usr/bin/vnc4passwd to provide /usr/bin/vncpasswd (vncpasswd) in auto mode
 update-alternatives: using /usr/bin/vnc4config to provide /usr/bin/vncconfig (vncconfig) in auto mode
 [Pharaoh Logging] Adding Package vnc4server from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 VNC: Success
 ------------------------------
 Installer Finished
 ******************************



Si el servidor VNC ya existe en la máquina de los usuarios, lo hará lanza un mensaje de excepción como el servidor VNC ya está instalado. La siguiente pantalla da una representación pictórica respecto el mensaje de excepción.

.. code-block:: bash

 kevell@corp:/# ptconfigure vnc install
 Install VNC? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *          ! VNC !        *
 *******************************
 [Pharaoh Logging] Package vnc4server from the Packager Apt is already installed, so not installing
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 VNC: Success
 ------------------------------
 Installer Finished
 ******************************



Beneficios
---------------

* Permite el proceso de garantizar antes de la instalación.
* Facilita la instalación a través de get apt.
* Permite la conectividad de las máquinas virtuales.
* En caso de servidor VNC es ya existe, se lanza el mensaje excepcional durante el proceso de garantizar.
