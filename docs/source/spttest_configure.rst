===========
PTTest 
===========

sinopsis
------------

módulo pttest es para el manejo de configuración conjunto de pruebas y ejecución utilizando un conjunto común de normas a través de una gama de herramientas y tecnologías. Puede ser utilizado para generar conjuntos de pruebas de arranque para sus aplicaciones y automatizar comandos de ejecución de la prueba en cuestión de minutos.
Este módulo tiene como objetivo instalar la última versión de la herramienta pttest.

Ayuda Comando
--------------------

El comando de ayuda guía al usuario para proporcionar lo necesario para realizar la tarea. El comando para hacer uso de la ayuda debajo del terminal se da de la siguiente manera,

.. code-block:: bash

	ptconfigure pttest help


La instantánea de abajo te da una representación pictórica de comando ayuda.

.. code-block:: bash

 kevell@corp:/# ptconfigure pttest help
 ******************************


  This command allows you to update pttest.

  PTTest, cleo, pttest

        - install
        Installs the latest version of pttest
        example: pttest pttest install

 ------------------------------
 End Help
 ******************************

instalación
-------------

La mejor forma de instalar cualquiera de las aplicaciones faraón es a través ptconfigure. Si ya ha instalado ptconfigure entonces usted puede instalar pttest utilizando el siguiente comando,

.. code-block:: bash

	ptconfigure pttest install

La instantánea de abajo te da una representación pictórica de comando ayuda.

.. code-block:: bash

 kevell@corp:/# ptconfigure pttest install
 Install pttest - Update to latest version ? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *          pttest!         *
 *******************************
 What is the program data directory? Found "/opt/pttest" - use this? (Enter nothing for yes, no end slash)

 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'https://github.com/PharaohTools/pttest.git'  /tmp/pttest/pttestCloning into '/tmp/pttest/pttest'...
 remote: Counting objects: 909, done.
 remote: Total 909 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (909/909), 361.15 KiB | 87.00 KiB/s, done.
 Resolving deltas: 100% (412/412), done.
 Checking connectivity... done.
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 pttest: Success
 ------------------------------
 Installer Finished
 ******************************

Opciones
------------

.. cssclass:: table-bordered

 +------------------------------+-------------------------------+--------------+-------------------------------------------------------+
 | Parámetros                   | Parámetro Alternativa         | Opciones     | Comentarios                                           |
 +==============================+===============================+==============+=======================================================+
 |Install pttest - Update to    | PTTest, cleo, pttest          | Y(Yes)       | Si el usuario desea continuar el proceso de           |
 |latest version ? (Y/N)        |                               |              | instalación se puede introducir como Y.               |
 +------------------------------+-------------------------------+--------------+-------------------------------------------------------+
 |Install pttest - Update to    | PTTest, cleo, pttest          | N(No)        | Si el usuario desea abandonar el proceso de           |
 |latest version ? (Y/N)        |                               |              | instalación se puede introducir como N.|              |
 +------------------------------+-------------------------------+--------------+-------------------------------------------------------+

Beneficios
--------------

* Uso fácil de acceso y la instalación
* La codificación es sensible a mayúsculas
* Fuente completo está disponible y no hay costos de licencia.
