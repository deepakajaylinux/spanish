===========
Cleopatra
===========

sinopsis
----------- 

Esta instalación de ascensor módulo en versión actualizada. La automatización es posible. Ubicación de directorio de datos y directorio albacea se puede especificar durante la instalación de este módulo. En él se especifica la configuración de su entorno. Es fácil de usar con Ubuntu y CentOS.

comando Ayuda
----------------------

  Este comando ayuda a guiar al usuario acerca de Cleopatra. Adecuado para todo tipo de usuario. Representa los parámetros alternativos y comandos para la instalación. El siguiente comando ayuda y la captura de pantalla y ayudarán al usuario en relación con el uso.

.. code-block:: bash

		cleopatra Cleopatra help

.. code-block:: bash
 
	kevell@corp:/# cleopatra Cleopatra help
	******************************


	This command allows you to update Cleopatra.

	Cleopatra, cleo, cleopatra

        - install
        Installs the latest version of cleopatra
        example: cleopatra cleopatra install

	------------------------------
	End Help
	******************************


instalación
-------------

Es un proceso más simple para instalar módulo Cleopatra simplemente usando la orden dada a continuación,

.. code-block:: bash

  cleopatra Cleopatra install

Después de dar la orden de la Cleopatra se instalará con nuevas actualizaciones.

Después de la entrada del usuario ha pasado comprobará si cualquier archivo falta y, en parte, se instalará automáticamente.

La siguiente captura de pantalla que enumera.

.. code-block:: bash

 kevell@corp:/# cleopatra cleopatra install

 Install Cleopatra - Update to latest version ? (Y/N)
 y
 *******************************
 *        Pharaoh Tools        *
 *          Cleopatra!         *
 *******************************
 What is the program data directory? Found "/opt/cleopatra" - use this? (Enter nothing for yes, no end slash)
 
 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'https://github.com/PharaohTools/cleopatra.git'  /tmp/cleopatra/cleopatraCloning into '/tmp/cleopatra/cleopatra'...
 remote: Counting objects: 19656, done.
 remote: Total 19656 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (19656/19656), 6.15 MiB | 66.00 KiB/s, done.
 Resolving deltas: 100% (11790/11790), done.
 Checking connectivity... done.
 Program Data Folder /opt/cleopatra Deleted if existed
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Cleopatra: Success
 ------------------------------
 Installer Finished
 ******************************

.. cssclass:: table-bordered


 +------------------------+-----------------------------------------+--------------+---------------------------------------+
 | Parámetros             | parámetros alternativos                 | Necesario    | Comentario                            |
 +========================+=========================================+==============+=======================================+
 |Install cleopatra       | En lugar de cleopatra podemos utilizar  | Y(Yes)       | Se instalará cleopatra cleopatra bajo |
 |cleopatra Update to     | Cleopatra, cleo también                 |              |                                       |
 |latest version? (Y/N)   |                                         |              |                                       |
 +------------------------+-----------------------------------------+--------------+---------------------------------------+
 |Install cleopatra       | En lugar de cleopatra podemos utilizar  | N(No)        | Saldrá desde la instalación           |
 |cleopatra Update to     | Cleopatra, cleo también                 |              |                                       |
 |latest version? (Y/N)|  |                                         |              |                                       |
 +------------------------+-----------------------------------------+--------------+---------------------------------------+


Beneficios
--------------

* Cleopatra se utiliza para instalar el archivo de configuración. Durante la instalación si hay algún archivo se Sobrescribir el contenido.
* La nueva versión puede actualizar automáticamente.
* Updation se puede hacer en este módulo sin búsqueda en la web.

