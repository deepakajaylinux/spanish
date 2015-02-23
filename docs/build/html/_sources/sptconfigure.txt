=============
PTConfigure
=============

sinopsis
----------- 

Esta instalación de ascensor módulo en versión actualizada. La automatización es posible. Ubicación de directorio de datos y directorio albacea se puede especificar durante la instalación de este módulo. En él se especifica la configuración de su entorno. Es fácil de usar con Ubuntu y CentOS.

comando Ayuda
----------------------

  Este comando ayuda a guiar al usuario acerca de ptconfigure. Adecuado para todo tipo de usuario. Representa los parámetros alternativos y comandos para la instalación. El siguiente comando ayuda y la captura de pantalla y ayudarán al usuario en relación con el uso.

.. code-block:: bash

		ptconfigure ptconfigure help

.. code-block:: bash
 
	kevell@corp:/# ptconfigure ptconfigure help
	******************************


	This command allows you to update ptconfigure.

	ptconfigure, cleo, ptconfigure

        - install
        Installs the latest version of ptconfigure
        example: ptconfigure ptconfigure install

	------------------------------
	End Help
	******************************


instalación
-------------

Es un proceso más simple para instalar módulo ptconfigure simplemente usando la orden dada a continuación,

.. code-block:: bash

  ptconfigure ptconfigure install

Después de dar la orden de la ptconfigure se instalará con nuevas actualizaciones.

Después de la entrada del usuario ha pasado comprobará si cualquier archivo falta y, en parte, se instalará automáticamente.

La siguiente captura de pantalla que enumera.

.. code-block:: bash

 kevell@corp:/# ptconfigure ptconfigure install

 Install ptconfigure - Update to latest version ? (Y/N)
 y
 *******************************
 *        Pharaoh Tools        *
 *          ptconfigure!         *
 *******************************
 What is the program data directory? Found "/opt/ptconfigure" - use this? (Enter nothing for yes, no end slash)
 
 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'https://github.com/PharaohTools/ptconfigure.git'  /tmp/ptconfigure/ptconfigureCloning into '/tmp/ptconfigure/ptconfigure'...
 remote: Counting objects: 19656, done.
 remote: Total 19656 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (19656/19656), 6.15 MiB | 66.00 KiB/s, done.
 Resolving deltas: 100% (11790/11790), done.
 Checking connectivity... done.
 Program Data Folder /opt/ptconfigure Deleted if existed
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 ptconfigure: Success
 ------------------------------
 Installer Finished
 ******************************

.. cssclass:: table-bordered


 +------------------------+------------------------------------------+--------------+-------------------------------------------+
 | Parámetros             | parámetros alternativos                  | Necesario    | Comentario                                |
 +========================+==========================================+==============+===========================================+
 |Install ptconfigure     | En lugar de ptconfigure podemos utilizar | Y(Yes)       | Se instalará ptconfigure ptconfigure bajo |
 |ptconfigure Update to   | ptconfigure, cleo también                |              |                                           |
 |latest version? (Y/N)   |                                          |              |                                           |
 +------------------------+------------------------------------------+--------------+-------------------------------------------+
 |Install ptconfigure     | En lugar de ptconfigure podemos utilizar | N(No)        | Saldrá desde la instalación               |
 |ptconfigure Update to   | ptconfigure, cleo también                |              |                                           |
 |latest version? (Y/N)|  |                                          |              |                                           |
 +------------------------+------------------------------------------+--------------+-------------------------------------------+


Beneficios
--------------

* ptconfigure se utiliza para instalar el archivo de configuración. Durante la instalación si hay algún archivo se Sobrescribir el contenido.
* La nueva versión puede actualizar automáticamente.
* Updation se puede hacer en este módulo sin búsqueda en la web.

