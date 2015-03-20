==========
JFeature
==========

sinopsis
---------------

JFeatures es uno de los paquetes de software más populares del mundo solíamos construir, organizar, gestionar y publicar contenidos para sitios web, blogs, Intranets. Cuando el usuario presione el archivo zip a otro archivo se agregará todas las características. Debido a su arquitectura escalable es también una gran base para crear aplicaciones web. Se utiliza para administrar el componente de la migración de la etapa. Es una comodidad con Ubuntu y CentOS.


comando Ayuda
----------------------

El comando ayuda guía a los usuarios sobre la finalidad y así como sobre las opciones que se incluyen en el módulo JFeatures. Enumera los parámetros alternativos del módulo JFeatures. También describe la sintaxis para instalar el módulo JFeatures. El comando de ayuda para el módulo JFeatures se muestra a continuación.


.. code-block:: bash

	ptconfigure JFeatures help

La sintaxis para declarar el comando help es sensible al caso no que es una ventaja añadida. La siguiente captura de pantalla visualizar al usuario sobre el comando de ayuda en JFeatures.



.. code-block:: bash

 kevell@corp:/# jrush JFeature help
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

  This command manages the JFeature Component for Stage Migration.

  JFeature, jfeature

        - folder-defaults
          Reset the feature file storage folders being used to the default
          example jrush jfeature folder-defaults --config-file="/var/www/website/configuration.php"

        - feature-install
          Install the metadata for a database migration, fileset, or both from the GC Features component
          example jrush jfeature feature-install --feature-file="/var/www/website/XXX_XXX.zip" --config-file="/var/www/website/configuration.php"

        - feature-pull
          perform a pull on an installed feature so it is integrated into the site, db and file changes executed.
          example jrush jfeature feature-pull --pull-unique-time="XXX_XXX" --config-file="/var/www/website/configuration.php"
          example jrush jfeature feature-pull --pull-id="XX" --config-file="/var/www/website/configuration.php"

        - feature-push
          perform a push on an installed feature so it is saved locally.
          example jrush jfeature feature-push --profile-unique="XXX" --config-file="/var/www/website/configuration.php" --push-type="local"

        - group-install
          Install the metadata for a database migration, fileset, or both from the GC Features component
          example jrush jfeature group-install --group-file="/var/www/website/XXXX.group" --config-file="/var/www/website/configuration.php"

        - group-install-all
          Install the metadata for a database migration, fileset, or both from the GC Features component. Will scan the configured metadata
          Directory for group files, and install or update all found groups.
          example jrush jfeature group-install-all --config-file="/var/www/website/configuration.php"

        - group-push
          perform a push of a group profile into a locally saved file.
          example jrush jfeature group-push --group-unique="XXXXXXXXXXXXXXXX" --config-file="/var/www/website/configuration.php"

        - group-pull
          perform a pull on all installed features in the specified group so they are integrated into the site, db and
          file changes executed.
          example jrush jfeature group-pull --group-id="XX" --config-file="/var/www/website/configuration.php"
          example jrush jfeature group-pull --group-name="my group" --config-file="/var/www/website/configuration.php"
          example jrush jfeature group-pull --group-unique="XX1234" --config-file="/var/www/website/configuration.php"

 ------------------------------
 End Help
 ****************************************



parámetros alternativos
-----------------------------------

Los siguientes son los parámetros alternativos que pueden definirse en declaraciones:


JFeature, jfeature


Folder-default
----------------------

Este proceso que se utiliza para establecer el valor predeterminado de la carpeta de archivo de almacenamiento. Un ajuste preestablecido o valor que se utilizará si ninguna opción se realiza en carpeta. Interacción del usuario debería ser obligatoria. Configuración predeterminada para las opciones seleccionadas más comúnmente sirve para este propósito.


El comando de ayuda para el proceso de carpeta predeterminada se muestra a continuación.


.. code-block:: bash

	 Jrush JFeature folder-defaults

La captura de pantalla siguiente muestra su función.



.. code-block:: bash

 	folder-defaults
        Reset the feature file storage folders being used to the default
        example jrush jfeature folder-defaults --config-file="/var/www/website/configuration.php"


Feature-install
----------------------

Este proceso utilizado para instalar los metadatos para una migración de base de datos. Aquí pide característica nombre del archivo y nombre de archivo configurado. El usuario tiene que introducir todos los datos anteriores uno por uno. De lo contrario el usuario puede introducir como todo en una misma línea. Se utiliza el siguiente comando para instalar jfeature.


.. code-block:: bash

	 Jrush JFeature feature-install


La captura de pantalla muestra sus funciones.


.. code-block:: bash

       feature-install
       Install the metadata for a database migration, fileset, or both from the GC Features component
       example jrush jfeature feature-install --feature-file="/var/www/website/XXX_XXX.zip" --config-file="/var/www/website/configuration.php"


Feature-Pull
-------------------

Disponen de tracción utilizado para realizar un tirón en una característica instalada. Debido a la integración de cambios en el archivo pueden ser ejecutados.El siguiente comando puede utilizarse para tirar de archivo de configuración.


.. code-block:: bash

	 Jrush JFeature feature-pull


Después de introducir el comando anterior dijo, pide tiempo y dirección Ip. Basado en esta atracción puede ser ejecutado. La captura de pantalla siguiente explica su función.


.. code-block:: bash

	feature-pull
        perform a pull on an installed feature so it is integrated into the site, db and file changes executed.
        example jrush jfeature feature-pull --pull-unique-time="XXX_XXX" --config-file="/var/www/website/configuration.php"
        example jrush jfeature feature-pull --pull-id="XX" --config-file="/var/www/website/configuration.php"

Feature-Push
--------------------

Cuentan con empuje solía alcanza un empujón sobre una característica instalada. Cuando se empuja completa puede guardarse localmente. El comando utilizado para empujar la característica.


.. code-block:: bash

	 Jrush JFeature feature-push


Después de entrada el comando anterior dijo, pide perfil único y tipo de archivo y empuje la configuración. El usuario debe introducir uno o todo en la misma línea. Esto puede explicarse como sigue a través de las instantáneas,



.. code-block:: bash

 	feature-push
        perform a push on an installed feature so it is saved locally.
        example jrush jfeature feature-push --profile-unique="XXX" --config-file="/var/www/website/configuration.php" --push-type="local"

Group-install
-------------------

Este proceso utilizado para instalar los metadatos para una migración de base de datos. Aquí pide a nombre de archivo de grupo de función y nombre de archivo configurado. El usuario tiene que introducir todos los datos anteriores uno por uno. De lo contrario el usuario puede introducir como todo en una misma línea.


.. code-block:: bash

	 Jrush JFeature group-install

La captura de pantalla muestra sus funciones.



.. code-block:: bash

	group-install
        Install the metadata for a database migration, fileset, or both from the GC Features component
        example jrush jfeature group-install --group-file="/var/www/website/XXXX.group" --config-file="/var/www/website/configuration.php"


Group-install-all
-----------------------------

Establezca este proceso utilizado para instalar los metadatos de archivo de migración de base de datos. Componente de las características de la configuración de grupo. Instalación y actualización es posible. El siguiente comando para instalar todo el grupo.

.. code-block:: bash

	 Jrush JFeature group-install-all


Entrando en el comando anterior dijo que pide el archivo de configuración. El usuario puede introducir el nombre del archivo de configuración. La siguiente pantalla disparó a guías del usuario para instalar a grupo todos.



.. code-block:: bash

	group-install-all
        Install the metadata for a database migration, fileset, or both from the GC Features component. Will scan the configured metadata
        Directory for group files, and install or update all found groups.
        example jrush jfeature group-install-all --config-file="/var/www/website/configuration.php"



Group-push
------------------ 

Este proceso puede realizar un empuje de un perfil de grupo en el archivo local. Aquí se pueden mencionar el grupo único y nombre del archivo de configuración. El siguiente comando utilizado para empujar el perfil del grupo en localmente guardó el archivo.



.. code-block:: bash

	 Jrush JFeature group-push

La siguiente pantalla disparó a guías del usuario para instalar empuje del grupo.


.. code-block:: bash

	 group-push
         perform a push of a group profile into a locally saved file.
         example jrush jfeature group-push --group-unique="XXXXXXXXXXXXXXXX" --config-file="/var/www/website/configuration.php"


beneficios
-----------------

* Apoyo para todo tipo de usuarios 
* fáciles actualizaciones 
* mejor, búsqueda inteligente de búsqueda 
* potente extensibilidad 
* hacer más con menos tiempo pasar para la codificación y hacer más con menos comandos jfeature * bueno hacerlo con Ubuntu y ciento OS 
* sensibilidad a mayúsuclas y no




