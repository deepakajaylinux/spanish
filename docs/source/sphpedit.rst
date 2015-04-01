=========
PHPEdit  
=========

sinopsis
------------

Módulo PHPEdit es un completo entorno de desarrollo integrado para PHP. Mucho más que una simple modificación de PHP, que ayuda al usuario a realizar sus proyectos de una forma amable y eficiente, con una única herramienta de integración de todas las características que el usuario va a necesitar desde el diseño de sus proyectos, su documentación, para su despliegue. Es apropiado con Ubuntu y CentOS.

comando Ayuda
-----------------------

El comando help guía a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en el módulo PHPEdit. En él se enumeran los parámetros alternativos de módulo PHPEdit. También describe la sintaxis para instalar el módulo PHPEdit. El comando de ayuda para el módulo PHPEdit se muestra a continuación.

.. code-block:: bash

		ptconfigure Phpedit help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda bajo PHPEdit.

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPEdit help

 ******************************


  This command allows you to update PHPEdit.

  PHP-Edit, phpedit, PHPEdit

        - install
        Installs the latest version of PHPEdit
        example: ptconfigure phpedit install

 ------------------------------
 End Help
 ******************************


instalación
----------------

PHPEdit viene con una gran cantidad de extensiones, marcos, archivos de ayuda y herramientas, por lo que se envía en un instalador que se puede personalizar para trajes de la needs.However usuario, porque PHPEdit está en constante evolución, con nuevas características y correcciones de mantenimiento, una actualización automática sistema también está disponible para ayudar a continuar con los últimos lanzamientos de PHPEdit esfuerzo. el comando utilizado para la instalación de este módulo de la siguiente manera,

.. code-block:: bash

		ptconfigure Phpedit install


La captura de pantalla deja claro acerca de este módulo.

.. code-block:: bash


 kevell@corp:/# ptconfigure phpedit install
 Install PHPEdit? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         PHPEdit!        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Suggested packages:
  bluefish-dbg libxml2-utils tidy weblint-perl weblint
 The following NEW packages will be installed:
  bluefish
 0 upgraded, 1 newly installed, 0 to remove and 187 not upgraded.
 Need to get 0 B/243 kB of archives.
 After this operation, 762 kB of additional disk space will be used.
 Selecting previously unselected package bluefish.
 (Reading database ... 196191 files and directories currently installed.)
 Preparing to unpack .../bluefish_2.2.5-1_amd64.deb ...
 Unpacking bluefish (2.2.5-1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Processing triggers for mime-support (3.54ubuntu1.1) ...
 Processing triggers for gnome-menus (3.10.1-0ubuntu2) ...
 Processing triggers for desktop-file-utils (0.22-1ubuntu1) ...
 Processing triggers for bamfdaemon (0.5.1+14.04.20140409-0ubuntu1) ...
 Rebuilding /usr/share/applications/bamf-2.index...
 Setting up bluefish (2.2.5-1) ...
 [Pharaoh Logging] Adding Package bluefish from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ****************************** 


 Single App Installer:
 --------------------------------------------
 PHPEdit: Success
 ------------------------------
 Installer Finished
 ******************************



La desinstalación
-------------------

El comando que se utiliza para la desinstalación del módulo se enumeran a continuación ,

.. code-block:: bash

 kevell@corp:/# ptconfigure phpedit install
 Install PHPEdit? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         PHPEdit!        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Suggested packages:
  bluefish-dbg libxml2-utils tidy weblint-perl weblint
 The following NEW packages will be installed:
  bluefish
 0 upgraded, 1 newly installed, 0 to remove and 187 not upgraded.
 Need to get 0 B/243 kB of archives.
 After this operation, 762 kB of additional disk space will be used.
 Selecting previously unselected package bluefish.
 (Reading database ... 196191 files and directories currently installed.)
 Preparing to unpack .../bluefish_2.2.5-1_amd64.deb ...
 Unpacking bluefish (2.2.5-1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Processing triggers for mime-support (3.54ubuntu1.1) ...
 Processing triggers for gnome-menus (3.10.1-0ubuntu2) ...
 Processing triggers for desktop-file-utils (0.22-1ubuntu1) ...
 Processing triggers for bamfdaemon (0.5.1+14.04.20140409-0ubuntu1) ...
 Rebuilding /usr/share/applications/bamf-2.index...
 Setting up bluefish (2.2.5-1) ...
 [Pharaoh Logging] Adding Package bluefish from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ****************************** 


 Single App Installer:
 --------------------------------------------
 PHPEdit: Success
 ------------------------------
 Installer Finished
 ******************************




opción
-----------

.. cssclass:: table-bordered

 +--------------------------+-------------------------------------------+-------------+---------------------------------------------------+
 | Parámetros               | Parámetro Alternativa                     | Opciones    | Comentarios                                       | 
 +==========================+===========================================+=============+===================================================+
 |Install phpedit? (Y/N)    | En lugar de PHP-Edit, las siguientes      | Y(Yes)      | El usuario desea continuar el proceso de          | 
 |                          | alternativas también se pueden utilizar:  |             | instalación.                                      |
 |                          | phpedit, PHPEdit                          |             |                                                   |
 +--------------------------+-------------------------------------------+-------------+---------------------------------------------------+
 |Install phpedit? (Y/N)    | En lugar de PHP-Edit, las siguientes      | N(No)       | El usuario desea salir del proceso de             |
 |                          | alternativas también se pueden utilizar:  |             | instalación.                                      |
 |                          | phpedit, PHPEdit|                         |             |                                                   |
 +--------------------------+-------------------------------------------+-------------+---------------------------------------------------+


Beneficios
---------------

* Escriba el código de usuario más rápido con todos los asistentes de código disponibles y generadores de código.
* Mejorar la calidad de sus proyectos con el depurador integrado, y el módulo de pruebas unitarias
* Implementar fácilmente con un solo clic los proyectos de usuario, y trabajar de forma transparente con ficheros remotos
* Aumentar la productividad de los usuarios con sus marcos favoritos
* Código de inteligencia es posible.
* Depurador y profiler también disponibles.
* Sensitibilidad caso actúa un papel vital en este módulo
