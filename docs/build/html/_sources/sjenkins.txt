==============
Jenkins
==============

sinopsis
-------------

Jenkins es popular para construir servidor. Jenkins es una herramienta de integración continua de código abierto escrito en Java. Jenkins proporciona servicios de integración continua para el desarrollo de software. Se trata de un sistema en funcionamiento basado en servidor en un contenedor de servlets como Apache Tomcat.

Funcionalidad central de Jenkins y flexibilidad permiten que se ajuste en una variedad de entornos y puede ayudar a simplificar el proceso de desarrollo para todos los grupos de interés involucrados

Ayuda Comando
----------------------

Este comando ayuda a determinar el uso del módulo de Jenkins. El usuario se llega a saber acerca de las diferentes formas / formato para ejecutar este módulo. Este comando guía al usuario final a conocer el propósito de este comando.

.. code-block:: bash
             
		ptconfigure jenkins help

La captura de pantalla para el comando anterior se enumeran a continuación,

.. code-block:: bash
 
 kevell@corp:/# ptconfigure jenkins help
 ******************************


 This command allows you to install Jenkins, the popular Build Server.

 Jenkins, jenkins

 - install
 Installs Jenkins through apt-get
 example: ptconfigure jenkins install

 ------------------------------
 End Help
 ******************************

instalación
----------------

Si el usuario tiene que instalar el módulo Jenkins en la máquina, el siguiente comando dado se ejecutará el proceso de instalación.

.. code-block:: bash
              
	        ptconfigure jenkins install

La captura de pantalla de la orden anterior se enumeran a continuación,

.. code-block:: bash


 kevell@corp:/# ptconfigure jenkins install
 Install Jenkins? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *          ! Jenkins !        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-14615194352.sh
 chmod 755 /tmp/ptconfigure-temp-script-14615194352.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-14615194352.sh Permissions
 Executing /tmp/ptconfigure-temp-script-14615194352.sh
 E: Could not get lock /var/lib/apt/lists/lock - open (11: Resource temporarily unavailable)
 E: Unable to lock directory /var/lib/apt/lists/
 OK
 Temp File /tmp/ptconfigure-temp-script-14615194352.sh Removed
 W: Duplicate sources.list entry http://dl.google.com/linux/chrome/deb/ stable/main amd64 Packages (/var/lib/apt/lists/dl.google.com_linux_chrome_deb_dists_stable_main_binary-amd64_Packages)
 W: Duplicate sources.list entry http://dl.google.com/linux/chrome/deb/ stable/main i386 Packages (/var/lib/apt/lists/dl.google.com_linux_chrome_deb_dists_stable_main_binary-i386_Packages)
 W: You may want to run apt-get update to correct these problems
 W: Duplicate sources.list entry http://dl.google.com/linux/chrome/deb/ stable/main amd64 Packages (/var/lib/apt/lists/dl.google.com_linux_chrome_deb_dists_stable_main_binary-amd64_Packages)
 W: Duplicate sources.list entry http://dl.google.com/linux/chrome/deb/ stable/main i386 Packages (/var/lib/apt/lists/dl.google.com_linux_chrome_deb_dists_stable_main_binary-i386_Packages)
 W: You may want to run apt-get update to correct these problems
 E: Unable to correct problems, you have held broken packages.
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Some packages could not be installed. This may mean that you have
 requested an impossible situation or if you are using the unstable
 distribution that some required packages have not yet been created
 or been moved out of Incoming.
 The following information may help to resolve the situation:
 
 The following packages have unmet dependencies:
 jenkins : Depends: daemon but it is not installable
           Depends: default-jre-headless but it is not installable or
                    java-runtime-headless
 [Pharaoh Logging] Adding Package jenkins from the Packager Apt did not execute correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Jenkins: Success
 ------------------------------
 Installer Finished
 ******************************

Opciones
------------

.. cssclass:: table-bordered


 +----------------------------+-----------------------------------+---------------+--------------------------------------------+
 | Parámetros                 | Parámetro Alternativa             | Opciones      | Comentarios                                |
 +============================+===================================+===============+============================================+
 |ptconfigure Jenkins Install | En lugar de utilizar Jenkins, el  | Y(Yes)        | Una vez que el usuario proporciona la      |
 |                            | usuario puede añadir jenkins      |               | opción, sistema comienza proceso de        |
 |                            |                                   |               | instalación                                |
 +----------------------------+-----------------------------------+---------------+--------------------------------------------+
 |ptconfigure Jenkins Install | En lugar de utilizar Jenkins, el  | N(No)         | Una vez que el usuario proporciona la      |
 |                            | usuario puede añadir jenkins      |               | opción, Sistema detiene proceso de         |
 |                            |                                   |               | instalación|                               |
 +----------------------------+-----------------------------------+---------------+--------------------------------------------+

Beneficios
--------------

* Detección de errores Inmediata
* No paso de integración en el ciclo de vida
* Un sistema de despliegue en cualquier punto dado
* Registro de la evolución del proyecto
