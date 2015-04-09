====
Gem
====

sinopsis
-----------

Este módulo envuelve todas las necesidades de los usuarios para trabajar con GEM. Cubre varias características, y en la mano promueve diversas funciones a realizar.

RubyGems es un gestor de paquetes para el lenguaje de programación Ruby que proporciona un formato estándar para la distribución de programas y bibliotecas de Ruby (en un formato autónomo llamado una "joya"), una herramienta diseñada para gestionar fácilmente la instalación de las joyas, y un servidor para la distribución de ellos.

Veamos las diversas características y cómo utilizar este módulo de los próximos temas.

Ayuda Comando
----------------------

El comando de ayuda instruye a los usuarios acerca de la finalidad y diversas características, y la sintaxis para aplicar esas diversas características. También se enumeran las salidas de parámetros alternativos que se pueden utilizar en las declaraciones. El formato de la sintaxis para la aplicación de opción de ayuda en virtud de este módulo, se da a continuación,

.. code-block:: bash

	ptconfigure gem help

La siguiente captura de pantalla y visualizar la salida y de trabajo de la opción de ayuda en virtud de este módulo.

.. code-block:: bash

 kevell@corp:/# ptconfigure gem help
 ******************************


  This command allows you to modify create or modify gems

  Gem, gem

        - install
        Install
        example: ptconfigure gem pkg-install --package-name="somename"

        - remove
        Remove
        example: ptconfigure gem pkg-remove --package-name="somename"

        - ensure
        Ensure
        example: ptconfigure gem pkg-ensure --package-name="somename"

        - update
        Update
        example: ptconfigure gem update


 ------------------------------
 End Help
 ******************************



Diferentes características de la gema
-------------------------------------------------

Como se muestra en el comando de ayuda anterior, las diversas características de la gema se enumeran a continuación,

* Install
* Remove
* Ensure
* Update


Veamos en detalle acerca de estas características.


Install
------------

Esta función le permite instalar el paquete que necesita el usuario . La siguiente captura de pantalla y visualizar la salida ,


.. code-block:: bash

 kevell@corp:/# ptconfigure gem pkg-install --package-name=cucumber
 Successfully installed cucumber-2.0.0
 1 gem installed
 Installing ri documentation for cucumber-2.0.0...
 Installing RDoc documentation for cucumber-2.0.0...
 ******************************


 Gem Modifications:
 --------------------------------------------

 Gem: Success

 ------------------------------
 Gem Mods Finished
 ******************************


Remove
-----------

Esta función tiene como objetivo la eliminación de una joya existente. Esta función de joya usando este módulo se puede lograr mediante la siguiente sintaxis,

.. code-block:: bash

	ptconfigure gem remove --gemname="somename"

En el lugar de gemname el usuario puede especificar el nombre de la joya que se va a eliminar. Después de introducir el comando como se especifica anteriormente, se eliminará la gema especificado.

.. code-block:: bash

 kevell@corp:/# ptconfigure gem pkg-remove --package-name=cucumber
 Removing cucumber
 Successfully uninstalled cucumber-2.0.0
 ******************************


 Gem Modifications:
 --------------------------------------------

 Gem: Failure

 ------------------------------
 Gem Mods Finished
 ****************************** 



Ensure
-------------

Esta función asegura que el paquete se ha instalado correctamente en la máquina.

.. code-block:: bash

	ptconfigure gem pkg-ensure --package="ssh"

.. code-block:: bash


 kevell@corp:/# ptconfigure gem pkg-ensure
 Enter Package:
 cucumber
 true
 [Pharaoh Logging] Package cucumber from the Packager Gem is Installed
 ******************************


 Gem Modifications:
 --------------------------------------------

 Gem: Success

 ------------------------------
 Gem Mods Finished
 ******************************


.. code-block:: bash

 kevell@corp:/# ptconfigure gem pkg-ensure
 Enter Package:
 cucumber
 false
 [Pharaoh Logging] Package cucumber from the Packager Gem is not Installed
 ******************************


 Gem Modifications:
 --------------------------------------------

 Gem: Success

 ------------------------------
 Gem Mods Finished
 ******************************




parámetros alternativos
-----------------------------

Los parámetros alternativos para este módulo, cualquiera de los cuales se pueden utilizar en la declaración es,

* Gem
* gem

Beneficios
--------------

* Los parámetros utilizados declarando ayuda y otras características diferentes de la gema no distinguen entre mayúsculas y minúsculas.
* Es-acomodado tanto os Cent y así como en Ubuntu.
* El uso de este módulo, el usuario puede crear y, así como modificar la gema de acuerdo a sus necesidades.
* La existencia de una joya puede garantizarse en este módulo.
