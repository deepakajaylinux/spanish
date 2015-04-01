============
NetBeans
============

Sinopsis
-------------

NetBeans es un entorno de desarrollo integrado (IDE) para desarrollar principalmente con Java, pero también con otros idiomas, en particular, PHP, C / C ++ y HTML. También es un marco de plataforma de aplicaciones para aplicaciones de escritorio Java y otros.

El NetBeans IDE está escrito en Java y se puede ejecutar en Windows, OS X, Linux, Solaris y otras plataformas que soportan una JVM compatible. NetBeans IDE es un IDE multiplataforma con una función de soporte para el lenguaje de programación Java.

La plataforma NetBeans permite que las aplicaciones que se desarrollan a partir de un conjunto de componentes de software modulares llamados módulos. Las aplicaciones basadas en la plataforma NetBeans (incluyendo el propio NetBeans IDE) pueden extenderse por los desarrolladores de terceros.

Ayuda Comando
----------------------

Este comando ayuda a determinar el uso del módulo de Netbeans. El usuario se llega a saber acerca de la diferente forma / formato de ejecutar este módulo. Este comando guía al usuario final a conocer el propósito de este comando. A continuación dado son el mando y la pantalla del mismo.

.. code-block:: bash
        
	        ptconfigure Netbeans help


.. code-block:: bash

 kevell@corp:/# ptconfigure netbeans help
 ******************************


  This command allows you to install and uninstall NetBeans - IDE.

  NetBeans, Netbeans, netbeans

        - install
        Installs a version of NetBeans.
        example: ptconfigure netbeans install
	
	- uninstall
        Uninstalls a version of NetBeans.
        example: ptconfigure netbeans uninstall
 ------------------------------
 End Help
 ******************************



instalación
----------------

Este comando ayuda en la instalación de Netbeans en el sistema. El siguiente comando dado se ejecutará el proceso de instalación.

.. code-block:: bash
        
	        ptconfigure netbeans install


.. code-block:: bash


 kevell@corp:/# ptconfigure netbeans install
 Install NetBeans-8.0? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         !!NetBeans!!        *
 *******************************
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module Java reports itself as Installed
 [Pharaoh Logging] Not installing as already installed

 Enter (1) to Install NetBeans in Silent:
 Enter (2) to install NetBeans in UserFriendly:
 1
 Creating /tmp/ptconfigure-temp-script-53829501149.sh
 chmod 755 /tmp/ptconfigure-temp-script-53829501149.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-53829501149.sh Permissions
 Executing /tmp/ptconfigure-temp-script-53829501149.sh
 --2015-04-01 11:42:15--  http://download.netbeans.org/netbeans/8.0/final/bundles/netbeans-8.0-linux.sh
 Resolving download.netbeans.org (download.netbeans.org)... 137.254.120.26
 Connecting to download.netbeans.org (download.netbeans.org)|137.254.120.26|:80... connected.
 HTTP request sent, awaiting response... 302 Moved Temporarily
 Location: http://dlc-cdn.sun.com/netbeans/8.0/final/bundles/netbeans-8.0-linux.sh [following]
 --2015-04-01 11:42:16--  http://dlc-cdn.sun.com/netbeans/8.0/final/bundles/netbeans-8.0-linux.sh
 Resolving dlc-cdn.sun.com (dlc-cdn.sun.com)... 23.205.118.80, 23.205.118.73
 Connecting to dlc-cdn.sun.com (dlc-cdn.sun.com)|23.205.118.80|:80... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: 212403200 (203M) [application/x-sh]
 Saving to: â€˜netbeans-8.0-linux.shâ€™ 

 100%[===========================================================================================>] 21,24,03,200 78.0KB/s   in 78m 40s

 2015-04-01 13:00:58 (43.9 KB/s) - â€˜netbeans-8.0-linux.shâ€™ saved [212403200/212403200]

 Temp File /tmp/ptconfigure-temp-script-53829501149.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 NetBeans: Success
 ------------------------------
 Installer Finished
 ****************************** 


La desinstalación
-----------------

Este comando ayuda a desinstalar Netbeans en el sistema . El siguiente comando dado se ejecutará el proceso de instalación.



.. code-block:: bash

	ptconfigure netbeans uninstall

.. code-block:: bash

 kevell@corp:/# ptconfigure netbeans uninstall

 Uninstall NetBeans-8.0? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         !!NetBeans!!        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-80402838784.sh
 chmod 755 /tmp/ptconfigure-temp-script-80402838784.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-80402838784.sh Permissions
 Executing /tmp/ptconfigure-temp-script-80402838784.sh
 Configuring the installer...
 Searching for JVM on the system...
 Extracting installation data...
 Running the installer wizard...
 Temp File /tmp/ptconfigure-temp-script-80402838784.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Uninstaller:
 ------------------------------
 NetBeans: Success
 ------------------------------
 Installer Finished
 ******************************


Opciones
------------


.. cssclass:: table-bordered

 +------------------------+------------------------------------------------------+-------------+-------------------------------------+
 | Parámetros             | Parámetro Alternativa                                | Opciones    | Comentarios                         |
 +========================+======================================================+=============+=====================================+
 |ptconfigure Netbeans    | Hay tres parámetros alternativos que se pueden       | Y(Yes)      | El sistema se inicia proceso        |
 |Install? (Y/N)          | utilizar en la línea de comandos. Netbeans ,         |             | de instalación                      |
 |                        | NetBeans ,netbeans Por                               |             |                                     |
 |                        | ejemplo: ptconfigure NetBeans install,               |             |                                     |
 |                        | ptconfigure netbeans install                         |             |                                     |
 +------------------------+------------------------------------------------------+-------------+-------------------------------------+
 |ptconfigure Netbeans    | Hay tres parámetros alternativos que se pueden       | N(No)       | El sistema detiene proceso          |
 |Install? (Y/N)          | utilizar en la línea de comandos. Netbeans ,         |             | de instalación                      |
 |                        | NetBeans ,netbeans Por                               |             |                                     |
 |                        | ejemplo: ptconfigure NetBeans install,               |             |                                     |
 |                        | ptconfigure netbeans install|                        |             |                                     |
 +------------------------+------------------------------------------------------+-------------+-------------------------------------+


Beneficios
--------------

* Gestión de la interfaz de usuario (por ejemplo, los menús y barras de herramientas)
* Gestión de Configuración de usuario
* Gestión de Almacenamiento (guardar y cargar cualquier tipo de datos)
* Gestión de Ventana
* Marco Asistente (admite paso a paso diálogos)
* NetBeans Visual Biblioteca
* Herramientas de desarrollo integrado
