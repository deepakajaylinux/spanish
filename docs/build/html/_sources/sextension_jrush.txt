=============
Extension
=============

sinopsis
--------------

Extensión debe ser identificado por el sistema operativo puede hacerles frente. Estos nombres tienen normas específicas. La primera parte del nombre a la izquierda de la época se llama el nombre raíz. El nombre de la raíz puede ser el mismo como un nombre de dispositivo. La segunda parte a la derecha de la época es la extensión. Es opcional y es a menudo, pero no necesariamente tres caracteres de largo. Extensión puede agregarse a través de codificación. Consolidó para estafar con Ubuntu y ciento OS.


comando Ayuda
-----------------

El comando ayuda guía a los usuarios sobre la finalidad y así como sobre las opciones que están incluidas en la extensión. Enumera los parámetros alternativos de extensión. También describe la sintaxis para el funcionamiento del módulo de Jrush. El comando de ayuda para la extensión se muestra a continuación.


.. code-block:: bash

	jrush extension help

Después de escribir el comando enumera las opciones de acción. La siguiente imagen visualizarlo obviamente.



.. code-block:: bash

 kevell@corp:/# jrush Extension help
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

  This command allows you to manage Joomla Extensions (Component, Module or Plugin).

  Extension, extension

        - disable
        Deletes a extension
        example: jrush extension disable

        - enable
        Enables a extension
        example: jrush extension enable

        - info
        Display the details of a extension
        example: jrush extension info


 ------------------------------
 End Help
 ****************************************


parámetros alternativos
----------------------------

Como una cuestión de elección con extensión el usuario puede hacer uso de las siguientes opciones.



Extension, extension

Opciones
------------

Hay tres opciones están disponibles. Vamos a ver sobre la opción de extensión.


* Enable
* Disable
* Info

Disable
-----------

Cuando el usuario de entrada como habilitarlo automáticamente elimina la extensión. El siguiente comando utilizado para habilitar.


.. code-block:: bash

	jrush extension Disable

El siguiente tiro de manto puede visualizar su función.



.. code-block:: bash

 kevell@corp:/# jrush Extension disable --config-file="/var/www/html/joomla/configuration.php" 
 Enter a Extension ID. To enter element/extension name use --extension-element or --extension-name parameters
 1
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 Extension:
 -------------------------

 The following extension was modified:

 Extension ID: 1
 Name: com_mailto
 Element: com_mailto
 Enabled: 0
 ------------------------------
 Extension Manage Finished
 ****************************************


Enable
-----------

Permitir usos habilitar la extensión. El siguiente comando ayudan al usuario a habilitar.


.. code-block:: bash

	jrush extension enable

Las siguientes capturas de pantalla guía al usuario para activar su función.



.. code-block:: bash

 kevell@corp:/# jrush Extension enable --config-file="/var/www/html/joomla/configuration.php" 
 Enter a Extension ID. To enter element/extension name use --extension-element or --extension-name parameters
 1
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 Extension:
 -------------------------

 The following extension was modified:
 
 Extension ID: 1
 Name: com_mailto
 Element: com_mailto
 Enabled: 1
 ------------------------------
 Extension Manage Finished
 ****************************************



Info
--------

Info es una ayuda para el usuario para mostrar los detalles de la expansión. Pide id de extensión. Después entra en el valor muestra los detalles de la extensión. El siguiente comando que se utiliza para Mostrar información.


.. code-block:: bash

	jrush extension info

Puede ser visualiza por la captura de pantalla.



.. code-block:: bash

 kevell@corp:/# jrush Extension info --config-file="/var/www/html/joomla/configuration.php" 
 Enter a Extension ID. To enter element/extension name use --extension-element or --extension-name parameters
 1
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 Extension:
 -------------------------

 The following extension was modified:

 Extension ID: 1
 Name: com_mailto
 Element: com_mailto
 Enabled: 0
 ------------------------------
 Extension Manage Finished
 ****************************************

beneficios
----------------

* Extensiones pueden ser consideradas un tipo de metadatos. 
* Múltiples aplicaciones para ser asociado a una extensión determinada. 
* No caso sensible 
* cómodo con Ubuntu y ciento OS. 
* Se utiliza para eliminar la extensión 
* información se utiliza para Mostrar información acerca de extensión.

