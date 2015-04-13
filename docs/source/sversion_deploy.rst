=========
Version
=========

sinopsis
----------------

En este módulo se utiliza para instalar la versión actualizada con arreglo a ptdeploy . El control de versiones más comúnmente ejecutar como aplicaciones independientes , pero el control de revisión también está incrustado en diversos tipos de sistema operativo como Ubuntu y CentOS . La mayoría versión permite múltiples desarrolladores para editar el mismo archivo al mismo tiempo. El primer desarrollador de "check in " cambios en el repositorio central siempre tiene éxito . El sistema puede proporcionar instalaciones para fusionar más cambios en el repositorio central, y preservar los cambios desde el primer desarrollador cuando otros desarrolladores comprobar in.It soporta Ubuntu y CentOS .

comando Ayuda
-----------------------

El comando de ayuda conduce a los usuarios con respecto a la versión de la ptdeploy . Las opciones que se incluyen en los módulos de versión . El comando help enumera los parámetros alternativos de versión bajo módulo ptdeploy . También se describe la sintaxis de la versión . El comando de ayuda para la versión se muestra a continuación .

.. code-block:: bash

	ptdeploy  version help

La siguiente captura de pantalla muestra el esfuerzo total de ptdeploy .


.. code-block:: bash


 kevell@corp:/# ptdeploy Version help
 ******************************


  This command is part of Default Modules and handles Application Versioning, allowing for rollbacks and the like.

  Version, version, vrs

          - specific
          Will change back the *current* symlink to whichever available version you pick
          example: ptdeploy version specific --limit=4 --container=/var/www/applications/the-app --version=2

          - latest
          Will change back the *current* symlink to the latest created version
          example: ptdeploy version latest
          example: ptdeploy version latest --limit=3 --container=/var/www/applications/the-app

          - rollback
          Will change back the *current* symlink to the latest created version but one
          example: ptdeploy version rollback
          example: ptdeploy version rollback --limit=3 --container=/var/www/applications/the-app


      You can also apply a limit to the number of Versions to keep by using the --limit parameter
          example: ptdeploy version latest --limit=3

 ------------------------------
 End Help
 ******************************


parámetro Alternativa
--------------------------------

Hay dos alternativas disponibles en la versión . Ellos son

Version, version, vrs



Specific
-----------

La opción específica permite al usuario cambiar de nuevo el directorio de la versión actual para hacer la versión específica . El comando de la opción específica se muestra a continuación,

.. code-block:: bash

        ptdeploy version specific

or

.. code-block:: bash

        ptdeploy version specific --limit=4 --container=/opt/versiontest/ --version=2

.. code-block:: bash


 kevell@corp:/# ptdeploy version specific

 Do you want to change the version that *current* points to? (Y/N) 
 y
 What is the Project Container Directory? (The one with versions in) Enter none for /opt/versiontest
 /opt/versiontest/
 Please Choose Version to make current (Showing newest first, Enter none for newest):
 --- All Versions: ---
 (0) karuna 

 0
 How many Versions to limit to? Enter 0 to ignore version limits
 2
 Removed Version Symlink
 Created Version Symlink
 ********************************
 Seems Fine...Versioning Finished
 ********************************
 
.. code-block:: bash

 kevell@corp:/# ptdeploy version specific --limit=4 --container=/opt/versiontest/ --version=2

 Do you want to change the version that *current* points to? (Y/N) 
 y
 Removed Version Symlink
 Created Version Symlink
 ********************************
 Seems Fine...Versioning Finished
 ******************************** 

Latest
----------

La última opción permite al usuario cambiar de nuevo el enlace disponible para versión más reciente. El comando para el último proceso de ejecución se muestra a continuación,

.. code-block:: bash 

        ptdeploy version latest

or

.. code-block:: bash

        ptdeploy version latest --limit=3 --container=/var/www/applications/the-app

.. code-block:: bash


 kevell@corp:/# ptdeploy version latest

 Do you want to change the version that *current* points to? (Y/N) 
 y
 What is the Project Container Directory? (The one with versions in) Enter none for /opt/versiontest
 /opt/versiontest/
 How many Versions to limit to? Enter 0 to ignore version limits
 5
 Removed Version Symlink
 Created Version Symlink
 ********************************
 Seems Fine...Versioning Finished
 ******************************** 

.. code-block:: bash

 kevell@corp:/# ptdeploy version latest --limit=3 --container=/opt/versiontest/

 Do you want to change the version that *current* points to? (Y/N) 
 y
 Removed Version Symlink
 Created Version Symlink
 ********************************
 Seems Fine...Versioning Finished
 ********************************

Rollback
----------

La opción de deshacer permite a los usuarios realizar cambios en la versión existente. El proceso de ejecución de reversión se muestra a continuación,

.. code-block:: bash

        ptdeploy version rollback

or

.. code-block:: bash

        ptdeploy version rollback --limit=3 --container=/opt/versiontest/

.. code-block:: bash


 kevell@corp:/# ptdeploy version rollback

 Do you want to change the version that *current* points to? (Y/N) 
 y
 What is the Project Container Directory? (The one with versions in) Enter none for /opt/versiontest
 /opt/versiontest/
 How many Versions to limit to? Enter 0 to ignore version limits
 4
 Removed Version Symlink
 ********************************
 Seems Fine...Versioning Finished
 ******************************** 

.. code-block:: bash

 kevell@corp:/# ptdeploy version rollback --limit=3 --container=/opt/versiontest/

 Do you want to change the version that *current* points to? (Y/N) 
 y
 Removed Version Symlink
 ********************************
 Seems Fine...Versioning Finished
 ********************************



opción
------------

.. cssclass:: table-bordered

 +--------------------------+-----------------+---------------------------------------------+--------------------------------------+
 | parámetros		    | opción 	      | Parámetro Alternativa		            | Comentarios	 	           |
 +==========================+=================+=============================================+======================================+
 |Install version?(Y/N)	    | Yes	      | En lugar de utilizar la versión             | instalado con éxito		   |
 |			    |		      | el usuario puede utilizar Version,          | bajo módulo ptdeploy      	   |
 |                          |                 | version, vrs                                |                                      |
 +--------------------------+-----------------+---------------------------------------------+--------------------------------------+
 |Install version?(Y/N)	    | No	      | En lugar de utilizar la versión             | Salir de la pantalla		   |
 |			    |		      |	el usuario puede utilizar Version,          | 				           |
 |                          |                 | version, vrs|                               |                                      |
 +--------------------------+-----------------+---------------------------------------------+--------------------------------------+


Beneficios
---------------

* La nueva versión se puede actualizar.
* Es adecuado con Ubuntu y CentOS .
* Sensitibilidad caso
* La automatización es posible
* Fácil de escribir los comandos

