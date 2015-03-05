==================
RubySystem
==================

sinopsis
------------

Ruby es un sistema, reflexivo, lenguaje de scripting de alto nivel dinámico. Sistema Ruby no es sólo para el desarrollo de aplicaciones Web que trabaja con el Rubí RVM. También se puede utilizar como un potente como un lenguaje de script y una muy buena alternativa a las secuencias de comandos shell habitual, utiliza comúnmente para alcanzar las necesidades de secuencias de comandos en los sistemas de adminstration.Set incorporadas en módulos y unas pocas bibliotecas externas, el sistema de Ruby puede hacer adminstration sistemas más efficient.Ruby sistema es una herramienta muy útil y potente que es imprescindible tener en toolbox.It de cada administrador del sistema es cómodo con Ubuntu y CentOS.

comando Ayuda
--------------------

Este comando puede funcionar sobre los objetivos y los comandos disponibles bajo módulo del sistema de Ruby. También explica el comando para instalar el sistema de Ruby. Antes de la instalación, el usuario puede leer este comando de ayuda explica su función.

.. code-block:: bash
        
		ptconfigure RubySystem help

La siguiente imagen también ayuda a entender este módulo con claridad.

.. code-block:: bash

 kevell@corp:/# ptconfigure RubySystem help
 ******************************


  This command allows you to install Ruby RVM, the system wide version.

  RubySystem, rubysystem, ruby-system, rubysys

        - install
        Installs Ruby a System Wide version of Ruby for you
        example: ptconfigure ruby-rvm install

  Ruby is installed the recommended per-user way. To use ruby after the install
  first run "source ~/.rvm/scripts/rvm" to get access to the Ruby install for
  your user, then "rvm install 1.9.3" (to install, specify version as needed)
  then "rvm use 1.9.3" (to select your default version for the session)

 ------------------------------
 End Help
 ******************************

instalación
-------------------

Es un proceso evidente para instalar módulo del sistema de Ruby bajo ptconfigure sólo por el uso de la orden dada a continuación,

.. code-block:: bash
        
                ptconfigure rubysystem install

Después de clave en el comando, puede pregunta

Install Ruby, system wide?(Y/N)

En caso de que la entrada del usuario como Y, se puede instalar Rubysystem del paquete. Si no, se puede salir de la pantalla. Las siguientes capturas de pantalla pueden explicarlo.

.. code-block:: bash


 kevell@corp:/# ptconfigure RubySystem install
 
 Install Ruby, System Wide? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         Ruby System!        *
 *******************************

 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following packages were automatically installed and are no longer required:
  linux-headers-3.13.0-32 linux-headers-3.13.0-32-generic
  linux-image-3.13.0-32-generic linux-image-extra-3.13.0-32-generic
 Use 'apt-get autoremove' to remove them.
 Suggested packages:
  ruby1.9.1-examples ri1.9.1 graphviz ruby1.9.1-dev
 The following NEW packages will be installed:
  ruby1.9.1
 0 upgraded, 1 newly installed, 0 to remove and 12 not upgraded.
 1 not fully installed or removed.
 Need to get 37.5 kB of archives.
 After this operation, 240 kB of additional disk space will be used.
 Get:1 http://us.archive.ubuntu.com/ubuntu/ precise/main ruby1.9.1 amd64 1.9.3.0-1ubuntu1 [37.5 kB]
 Fetched 37.5 kB in 7s (5232 B/s)
 Selecting previously unselected package ruby1.9.1.
 (Reading database ... 282890 files and directories currently installed.)
 Preparing to unpack .../ruby1.9.1_1.9.3.0-1ubuntu1_amd64.deb ...
 Unpacking ruby1.9.1 (1.9.3.0-1ubuntu1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up zend-server-php-5.3 (6.1.0+b1177) ...
 Module php5 already enabled
 Module rewrite already enabled
 Site zendserver_gui already enabled
 X-Powered-By: PHP/5.3.26 ZendServer/6.1.0
 Content-type: text/html

 Setting up ruby1.9.1 (1.9.3.0-1ubuntu1) ...
 update-alternatives: using /usr/bin/gem1.9.1 to provide /usr/bin/gem (gem) in auto mode
 [Pharaoh Logging] Adding Package ruby1.9.1 from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 RubySystem: Success
 ------------------------------
 Installer Finished
 ******************************

Opciones
--------------

.. cssclass:: table-bordered

 +-------------------------+---------------------------------------------+-------------+-------------------------------------------------+
 | Parámetros              | Parámetro Alternativa                       | Opciones    | Comentarios                                     |
 +=========================+=============================================+=============+=================================================+
 |Install Ruby, System     | Podemos utilizar RubySystem, rubysystem,    | Y(Yes)      | Si el usuario desea continuar el proceso de     |
 |Wide? (Y/N)              | ruby-system, rubysys.                       |             | instalación se puede introducir como Y.         |
 +-------------------------+---------------------------------------------+-------------+-------------------------------------------------+
 |Install Ruby, System     | Podemos utilizar RubySystem, rubysystem,    | N(No)       | Si el usuario desea abandonar el proceso de     | 
 |Wide? (Y/N)              | ruby-system, rubysys.                       |             | instalación se puede introducir como N.|        |
 +-------------------------+---------------------------------------------+-------------+-------------------------------------------------+


Beneficios
-------------

* Sistema de Ruby es una, reflexivo, lenguaje de scripting de alto nivel dinámico para la programación orientada a objetos rápida y fácil.
* En el sistema de Ruby, es una herramienta cómoda y agradable. Incluyendo las herramientas que se utilizan en el proceso de despliegue.
* El sistema de Ruby ya es un extremo que tenga conocimiento profesional con experiencia tanto en el desarrollo web y las habilidades 
  generales de ingeniería de software.
* La principal ventaja del lenguaje de programación Ruby y el Sistema de Ruby se considera que es la velocidad de desarrollo.

