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

        - create
        Create a new system gem, overwriting if it exists
        example: ptconfigure gem create --gemname="somename"

        - remove
        Remove a system gem
        example: ptconfigure gem remove --gemname="somename"

        - set-password
        Set the password of a system gem
        example: ptconfigure gem set-password --gemname="somename" --new-password=                                                                                        "somepassword"

        - exists
        Check the existence of a gem
        example: ptconfigure gem exists --gemname="somename"

        - show-groups
        Show groups to which a gem belongs
        example: ptconfigure gem show-groups --gemname="somename"

        - add-to-group
        Add gem to a group
        example: ptconfigure gem add-to-group --gemname="somename" --groupname="so                                                                                        megroupname"

        - remove-from-group
        Remove gem from a group
        example: ptconfigure gem remove-from-group --gemname="somename" --groupnam                                                                                        e="somegroupname"

 ------------------------------
 End Help
 ******************************


Diferentes características de la gema
-------------------------------------------------

Como se muestra en el comando de ayuda anterior, las diversas características de la gema se enumeran a continuación,

* Crear
* Retire
* Establecer contraseña
* Existe
* Show_groups
* Add_to_group
* Remove_from_group


Veamos en detalle acerca de estas características.

crear
--------

Esta función tiene como objetivo la creación de una nueva joya del sistema, y así como sobrescribe en caso de que ya existe. Esta función de joya usando este módulo se puede lograr mediante la siguiente sintaxis,

.. code-block:: bash

	ptconfigure gem create --gemname="somename"

En el lugar de gemname el usuario puede especificar el nombre de la gema que se va a crear. Después de introducir el comando como se especifica anteriormente, la nueva joya se creará con el nombre especificado.

RETIRE
-----------

Esta función tiene como objetivo la eliminación de una joya existente. Esta función de joya usando este módulo se puede lograr mediante la siguiente sintaxis,

.. code-block:: bash

	ptconfigure gem remove --gemname="somename"

En el lugar de gemname el usuario puede especificar el nombre de la joya que se va a eliminar. Después de introducir el comando como se especifica anteriormente, se eliminará la gema especificado.


CONTRASEÑA SET
------------------------

Esta función facilita el establecimiento de una nueva contraseña para una joya sistema según las necesidades. Esto se puede hacer mediante la aplicación del comando como se indica a continuación,

.. code-block:: bash

	ptconfigure gem set-password --gemname="somename" --new-password="somepassword"

Para llevar a cabo estas funciones, el usuario tiene que especificar los dos campos,

* Nombre de la gema
* Nueva contraseña

Después de especificar los dos campos en el formato de comando antes mencionado, se creará la nueva contraseña para la joya especificado.

EXISTE
--------

Esta función tiene por objeto la comprobación de la existencia de una joya. Esto se puede hacer simplemente, mediante el comando de abajo,
.. code-block:: bash

	ptconfigure gem exists --gemname="somename"

Después de aplicar el comando como el anterior, la existencia de una joya mencionada se garantizará con los resultados.

GRUPOS VER
--------------------

Esta función ayuda a los usuarios a conocer a qué grupo pertenece a la gema. Esto se puede conseguir simplemente utilizando el siguiente comando,

.. code-block:: bash

	ptconfigure gem show-groups --gemname="somename"

El usuario tiene que especificar el nombre de la joya en el campo de la gemname, con el fin de conocer los detalles de su grupo.

AÑADIR _TO_GROUP
---------------------------

El principal objetivo de esta función es añadir la gema requerida para el grupo requerido por la simple aplicación de la orden como se indica a continuación,

.. code-block:: bash

	ptconfigure gem add-to-group --gemname="somename" --groupname="somegroupname"

Para implementar esta función, el usuario tiene que especificar los dos campos siguientes de acuerdo a sus necesidades en el formato de la mencionada orden,

* Gemname
* Nombre del grupo

REMOVE_FROM_GROUP
--------------------------------

El principal objetivo de esta función es eliminar la gema de un grupo simplemente aplicando el comando como se indica a continuación,

.. code-block:: bash

	ptconfigure gem remove-from-group --gemname="somename" --groupname="somegroupname"

Para implementar esta función, el usuario tiene que especificar los dos campos siguientes de acuerdo a sus necesidades en el formato de la mencionada orden,

* Gemname
* Nombre del grupo

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
