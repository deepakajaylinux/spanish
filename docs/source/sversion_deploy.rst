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

Version, version, VERSION

instalación
----------------

La instalación incluye la instalación de la versión requerida para hacer la instalación en una versión actualizada . Es un proceso de manifiesto para instalar módulo versión bajo ptdeploy . versión con sólo usar la orden dada a continuación ,

.. code-block:: bash

	ptdeploy version Install

Después de vitalizar el comando se catequizar entrada.

Cuando la entrada de usuario como si automáticamente se instalará la versión con la comprobación del sistema. Si no salir de la instalación . La siguiente captura de pantalla de demostrar versión y sus funciones.

opción
------------

.. cssclass:: table-bordered

 +--------------------------+-----------------+---------------------------------------------+--------------------------------------+
 | parámetros		    | opción 	      | Parámetro Alternativa		            | Comentarios	 	           |
 +==========================+=================+=============================================+======================================+
 |Install version?(Y/N)	    | Yes	      | En lugar de utilizar la versión             | instalado con éxito		   |
 |			    |		      | el usuario puede utilizar Version, VERSION  | bajo módulo ptdeploy      	   |
 +--------------------------+-----------------+---------------------------------------------+--------------------------------------+
 |Install version?(Y/N)	    | No	      | En lugar de utilizar la versión             | Salir de la pantalla		   |
 |			    |		      |	el usuario puede utilizar Version, VERSION| | 				           |
 +--------------------------+-----------------+---------------------------------------------+--------------------------------------+


Beneficios
---------------

* La nueva versión se puede actualizar.
* Es adecuado con Ubuntu y CentOS .
* Sensitibilidad caso
* La automatización es posible
* Fácil de escribir los comandos

