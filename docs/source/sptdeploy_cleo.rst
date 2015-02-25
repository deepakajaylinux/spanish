============
PTDeploy
============

Sinopsis
-------------
El ptdeploy envuelve las aplicaciones de los usuarios con la implementación automatizada, construir y lanzar funciones, aplicación web de control de versiones y la infraestructura de código en PHP.

Con el fin de construir para el bienestar de la implementación, se necesitan muchos archivos a copiar de FTP u otras soluciones ad hoc . Y también gran cantidad de herramientas de automatización Empresa faltaban . Para superar estas carencias ptdeploy bajo la herramienta faraón eran acumule. PHP tiene ptdeploy tan rubí fiils la brecha en ptdeploy .

Esta herramienta es para aplicaciones de provisiones y construye a sus cajas. El usuario puede configurar aún patrón de despliegue de aplicaciones simples o complejas a su sistema con uno o dos archivos PHP o, de forma rápida patrones de despliegue amigables de configuración en la nube.

Ptdeploy es modular, orientado a objetos y extensible. Así que si el usuario requiere ningún módulo extra que pueden crear y añadir los nuevos módulos en función de sus necesidades.

Este ptdeploy actúa como un contenedor en el que todos los pasos de despliegue de usuario se cubren en un solo archivo. Esto permite el uso de un solo comando para arrancar una instancia de sus aplicaciones.

Ayuda Comando
----------------------

Este comando ayuda a determinar el uso de ptdeploy módulo. El usuario se llega a saber acerca de la diferente forma / formato de ejecutar este módulo. Este comando guía al usuario final a conocer el propósito de este comando. A continuación dado son el mando y la pantalla del mismo.

.. code-block:: bash
        
        ptconfigure ptdeploy help

La captura de pantalla para el comando anterior se enumeran a continuación ,

.. code-block:: bash

 kevell@corp:/# ptconfigure Ptdeploy help
 ******************************


  This command allows you to update Ptdeploy.

  Ptdeploy, dapper, ptdeploy

        - install
        Installs the latest version of ptdeploy
        example: ptconfigure ptdeploy install

        - ensure
        Installs the latest version of ptdeploy, only if a version is not installed
        example: ptconfigure ptdeploy ensure

 ------------------------------
 End Help
 ******************************

instalación
----------------

Este comando ayuda a instalar la última versión de ptdeploy. El siguiente comando dado se ejecutará el proceso de instalación.

.. code-block:: bash
        
         ptconfigure ptdeploy install

La captura de pantalla para el comando anterior se enumeran a continuación ,

.. code-block:: bash

 kevell@corp:/# ptconfigure ptdeploy install
 Install ptdeploy ? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *          ptdeploy         *
 *******************************
 What is the program data directory? Found "/opt/ptdeploy" - use this? (Enter nothing for yes, no end slash)
 
 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'https://github.com/PharaohTools/ptdeploy.git'  /tmp/ptdeploy/ptdeployCloning into '/tmp/ptdeploy/ptdeploy'...
 remote: Counting objects: 6989, done.
 remote: Total 6989 (delta 0), reused 0 (delta 0), pack-reused 6989
 Receiving objects: 100% (6989/6989), 2.61 MiB | 176.00 KiB/s, done.
 Resolving deltas: 100% (4335/4335), done.
 Checking connectivity... done.
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 ptdeploy: Success
 ------------------------------
 Installer Finished
 ******************************


asegurar
----------------

Este comando ayuda a instalar la última versión de ptdeploy, solamente si una versión no está instalado. El siguiente comando dado se ejecutará el proceso de instalación.

.. code-block:: bash

                ptconfigure ptdeploy ensure

La captura de pantalla para el comando anterior se enumeran a continuación ,

.. code-block:: bash

 kevell@corp:/# ptconfigure ptdeploy ensure
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module ptdeploy reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 ******************************


 Single App Installer:
 --------------------------------------------
 ptdeploy: Success
 ------------------------------
 Installer Finished
 ******************************


Opciones
-------------

.. cssclass:: table-bordered

 +---------------------------+------------------------------------------+------------+----------------------------------------------+
 | parámetros                | Parámetro Alternativa                    | Opciones   | Comentarios                                  |
 +===========================+==========================================+============+==============================================+
 |ptconfigure ptdeploy       | Hay tres parámetros alternativos que     | Y(Yes)     | El sistema se inicia proceso de instalación  |
 |install                    | pueden ser utilizados en la línea de     |            |                                              |
 |                           | comandos. Ptdeploy, dapper, ptdeploy     |            |                                              |
 |                           | ejemplo: ptconfigure ptdeploy install /  |            |                                              | 
 |                           |          ptconfigure dapper install      |            |                                              |
 +---------------------------+------------------------------------------+------------+----------------------------------------------+
 |ptconfigure ptdeploy       | Hay tres parámetros alternativos que     | N(No)      | El sistema detiene proceso de instalación    |
 |install                    | pueden ser utilizados en la línea de     |            |                                              |
 |                           | comandos. Ptdeploy, dapper, ptdeploy     |            |                                              |
 |                           | ejemplo: ptconfigure ptdeploy install /  |            |                                              |
 |                           |          ptconfigure dapper install|     |            |                                              |
 +---------------------------+------------------------------------------+------------+----------------------------------------------+

Beneficios
--------------

* Edición de los archivos de host, los archivos de la máquina virtual, archivos de configuración, actualizaciones de bases de datos y más 
  pueden ser automatizadas usando esto.
* Mediante el uso de la capacidad de gestión de servidor remoto, los usuarios pueden automatizar despliegues en toda la infraestructura de 
  cualquier tamaño.
