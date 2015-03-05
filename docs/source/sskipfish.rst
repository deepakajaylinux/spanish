=============
Skipfish
=============

sinopsis
------------

módulo Skipfish utiliza para instalar Skipfish. Skipfish es una herramienta de reconocimiento de seguridad de aplicaciones web activa. Se prepara un mapa del sitio interactivo para el sitio específico mediante la realización de un rastreo recursivo y sondas basados en diccionario. El mapa resultante se anota a continuación, con la salida de un número de controles de seguridad activa. El informe final generado por la herramienta está destinada a servir de base para las evaluaciones profesionales de seguridad de aplicaciones web. Este módulo fortalecer con Ubuntu y CentOS.

comando Ayuda
----------------------

El comando help guía a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en el módulo Skipfish. En él se enumeran los parámetros alternativos de módulo Skipfish. También describe la sintaxis para instalar el módulo Skipfish. El comando de ayuda para el módulo Skipfish se muestra a continuación.

.. code-block:: bash	

		ptconfigure Skipfish help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda bajo Skipfish.

.. code-block:: bash

 kevell@corp:/# ptconfigure Skipfish help

 ******************************


  This command allows you to install Skipfish.
  Skipfish, skipfish

        - install
        Installs Skipfish. 
        example: ptconfigure skipfish install

 ------------------------------
 End Help
 ******************************



instalación
-----------------

Este comando autoriza a instalar Skipfish con mapa interactivo del sitio. Cuando el usuario desea instalar Skipfish el comando siguiente guía al usuario para instalar.

.. code-block:: bash

                ptconfigure skipfish install

después de escribir este comando el sistema pide que los usuarios desean. El otro proceso explica la instalación a través de la pantalla.

.. code-block:: bash


 kevell@corp:/# ptconfigure Skipfish install
 Install  Skipfish? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *          Skipfish !        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
  skipfish
 0 upgraded, 1 newly installed, 0 to remove and 15 not upgraded.
 Need to get 233 kB of archives.
 After this operation, 574 kB of additional disk space will be used.
 Get:1 http://us.archive.ubuntu.com/ubuntu/ trusty/universe skipfish amd64 2.10b-1 [233 kB]
 Fetched 233 kB in 29s (7,910 B/s)
 Selecting previously unselected package skipfish.
 (Reading database ... 199429 files and directories currently installed.)
 Preparing to unpack .../skipfish_2.10b-1_amd64.deb ...
 Unpacking skipfish (2.10b-1) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up skipfish (2.10b-1) ...
 [Pharaoh Logging] Adding Package skipfish from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Skipfish: Success
 ------------------------------
 Installer Finished

 ******************************

Opciones
-----------

.. cssclass:: table-bordered

 +---------------------------+---------------------------------+--------------+------------------------------------------------+
 | Parámetros                | Parámetro Alternativa           | Opciones     | Comentarios                                    |
 +===========================+=================================+==============+================================================+
 |Install Skipfish ? (Y/N)   | En lugar de Skipfish podemos    | Y(Yes)       | Si el usuario desea continuar el proceso de    |
 |                           | utilizar skipfish.              |              | instalación se puede introducir como Y.        |
 +---------------------------+---------------------------------+--------------+------------------------------------------------+
 |Install Skipfish ? (Y/N)   | En lugar de Skipfish podemos    | N(No)        | Si el usuario desea abandonar el proceso de    |
 |                           | utilizar skipfish               |              | instalación se puede introducir como N.|       |
 +---------------------------+---------------------------------+--------------+------------------------------------------------+



Beneficios
--------------

* Skipfish es altamente adaptable y fiable.
* Bien diseñados los controles de seguridad.
* Manejo agraciada de sitios multi-marco
* Instalación automática versión actualizada
* Alta velocidad de acceso.
* Sensitibilidad caso.
* Así que hacer en Ubuntu y CentOS.
