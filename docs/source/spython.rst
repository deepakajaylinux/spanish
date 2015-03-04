==============
Python 
==============


sinopsis
-----------

Python es un propósito general, el lenguaje de programación de alto nivel utilizado. Este módulo tiene como objetivo instalar la última versión del paquete python y sus dependencias.

Ayuda Comando
--------------------

El comando de ayuda guía al usuario para proporcionar lo necesario para realizar la tarea. El comando para hacer uso de la ayuda debajo del terminal se da de la siguiente manera,

.. code-block:: bash

	ptconfigure python help

La instantánea de abajo te da una representación pictórica de comando de ayuda y aparece dos parámetros como Python y Python. (Los parámetros son mayúsculas y minúsculas)

.. code-block:: bash

	  kevell@corp:/# ptconfigure Python help
	  ******************************


	  This command allows you to install the latest available Python in the Ubuntu
	  repositories.

	  Python, python

          - install
           Installs the latest version of Python
           example: ptconfigure python install

	  ------------------------------
	  End Help
	  ******************************

instalación
-------------

El comando que se utiliza para la instalación de módulo de python se da a continuación,

.. code-block:: bash

	ptconfigure python install

La captura de pantalla para el comando anterior se enumeran a continuación,

.. code-block:: bash

 kevell@corp:/# ptconfigure python install

 Install Python? (Y/N)
 y
 *******************************
 *        Pharaoh Tools        *
 *         !Python!!        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
  python is already the newest version.
 0 upgraded, 0 newly installed, 0 to remove and 13 not upgraded.
 [Pharaoh Logging] Package python from the Packager Apt is already installed, so not installing.
 dpkg: warning: parsing file '/var/lib/dpkg/available' near line 47618 package 'ptconfigure':
  missing maintainer
 dpkg: warning: parsing file '/var/lib/dpkg/available' near line 47618 package 'ptconfigure':
 missing architecture
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
  docutils-common docutils-doc python-pygments python-roman
 Suggested packages:
  texlive-latex-recommended texlive-latex-base texlive-lang-french
  ttf-linux-libertine ttf-bitstream-vera
 The following NEW packages will be installed:
  docutils-common docutils-doc python-docutils python-pygments python-roman
 0 upgraded, 5 newly installed, 0 to remove and 13 not upgraded.
 Need to get 2,190 kB of archives.
 After this operation, 8,623 kB of additional disk space will be used.
 Get:1 http://us.archive.ubuntu.com/ubuntu/ precise/main docutils-common all 0.8.1-4ubuntu1 [153 kB]
 Get:2 http://us.archive.ubuntu.com/ubuntu/ precise/main docutils-doc all 0.8.1-4ubuntu1 [1,289 kB]
 Get:3 http://us.archive.ubuntu.com/ubuntu/ precise/main python-roman all 0.8.1-4ubuntu1 [12.6 kB]
 Get:4 http://us.archive.ubuntu.com/ubuntu/ precise/main python-docutils all 0.8.1-4ubuntu1 [382 kB]
 Get:5 http://us.archive.ubuntu.com/ubuntu/ precise/main python-pygments all 1.4+dfsg-2 [353 kB]
 Fetched 2,190 kB in 7s (277 kB/s)
 Selecting previously unselected package docutils-common.
 (Reading database ... 254879 files and directories currently installed.)
 Preparing to unpack .../docutils-common_0.8.1-4ubuntu1_all.deb ...
 Unpacking docutils-common (0.8.1-4ubuntu1) ...
 Selecting previously unselected package docutils-doc.
 Preparing to unpack .../docutils-doc_0.8.1-4ubuntu1_all.deb ...
 Unpacking docutils-doc (0.8.1-4ubuntu1) ...
 Selecting previously unselected package python-roman.
 Preparing to unpack .../python-roman_0.8.1-4ubuntu1_all.deb ...
 Unpacking python-roman (0.8.1-4ubuntu1) ...
 Selecting previously unselected package python-docutils.
 Preparing to unpack .../python-docutils_0.8.1-4ubuntu1_all.deb ...
 Unpacking python-docutils (0.8.1-4ubuntu1) ...
 Selecting previously unselected package python-pygments.
 Preparing to unpack .../python-pygments_1.4+dfsg-2_all.deb ...
 Unpacking python-pygments (1.4+dfsg-2) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Processing triggers for sgml-base (1.26+nmu4ubuntu1) ...
 Processing triggers for doc-base (0.10.5) ...
 Processing 1 added doc-base file...
 Setting up docutils-common (0.8.1-4ubuntu1) ...
 update-catalog: Suppressing action on super catalog. Invoking trigger instead.
 Setting up docutils-doc (0.8.1-4ubuntu1) ...
 Setting up python-roman (0.8.1-4ubuntu1) ...
 Setting up python-pygments (1.4+dfsg-2) ...
 Processing triggers for sgml-base (1.26+nmu4ubuntu1) ...
 Setting up python-docutils (0.8.1-4ubuntu1) ...
 update-alternatives: using /usr/share/docutils/scripts/python2/rst-buildhtml to provide /usr/bin/rst-buildhtml (rst-buildhtml) in auto mode
 update-alternatives: using /usr/share/docutils/scripts/python2/rst2html to provide /usr/bin/rst2html (rst2html) in auto mode
 update-alternatives: using /usr/share/docutils/scripts/python2/rst2latex to provide /usr/bin/rst2latex (rst2latex) in auto mode
 update-alternatives: using /usr/share/docutils/scripts/python2/rst2man to provide /usr/bin/rst2man (rst2man) in auto mode
 update-alternatives: using /usr/share/docutils/scripts/python2/rst2odt to provide /usr/bin/rst2odt (rst2odt) in auto mode
 update-alternatives: using /usr/share/docutils/scripts/python2/rst2odt_prepstyles to provide /usr/bin/rst2odt_prepstyles (rst2odt_prepstyles) in auto mode
 update-alternatives: using /usr/share/docutils/scripts/python2/rst2pseudoxml to provide /usr/bin/rst2pseudoxml (rst2pseudoxml) in auto mode
 update-alternatives: using /usr/share/docutils/scripts/python2/rst2s5 to provide /usr/bin/rst2s5 (rst2s5) in auto mode
 update-alternatives: using /usr/share/docutils/scripts/python2/rst2xetex to provide /usr/bin/rst2xetex (rst2xetex) in auto mode
 update-alternatives: using /usr/share/docutils/scripts/python2/rst2xml to provide /usr/bin/rst2xml (rst2xml) in auto mode
 update-alternatives: using /usr/share/docutils/scripts/python2/rstpep2html to provide /usr/bin/rstpep2html (rstpep2html) in auto mode
 [Pharaoh Logging] Adding Package python-docutils from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Python: Success
 ------------------------------
 Installer Finished
 ******************************

Opciones
-----------

.. cssclass:: table-bordered

 +------------------------+----------------------------------+------------+----------------------------------------------------+
 | Parámetros             | Parámetro Alternativa            | Opciones   | Comentarios                                        |
 +========================+==================================+============+====================================================+
 |Install Python? (Y/N)   | Python, python                   | Y(Yes)     | Si el usuario desea continuar el proceso de        |
 |                        |                                  |            | instalación se puede introducir como Y.            |
 +------------------------+----------------------------------+------------+----------------------------------------------------+
 |Install Python? (Y/N)   | Python, python                   | N(No)      | Si el usuario desea abandonar el proceso de        |
 |                        |                                  |            | instalación se puede introducir como N.|           |
 +------------------------+----------------------------------+------------+----------------------------------------------------+


Beneficios
--------------

* Pérdida de tiempo
* Uso La facilidad de acceso y la instalación
* La codificación es sensible a mayúsculas
* Fuente completo está disponible y no hay costos de licencia.
