====
Apt
====

sinopsis
----------

El principal objetivo de este módulo apto es crear nuevos apartamentos y así está destinada a modificar los apartamentos ya existentes. Este módulo tiene una colección de diversas características para acceder y modificar los apartamentos en función de los requerimientos de los usuarios.

Los temas próximos ocupa de cómo utilizar este módulo y también sobre los diferentes aspectos de este módulo para acceder a apt.

Ayuda Comando
----------------------

El comando de ayuda es un breve manual de usuario que facilita a los usuarios obtener conscientes en cuanto a la utilización de metodologías de manejo de este módulo para realizar diferentes funciones. También se enumeran las salidas de parámetros alternativos que se pueden utilizar en las declaraciones. Se destaca el ejemplo de sintaxis para el uso y acceso a diferentes funciones en virtud de Apt.

El comando utilizado para la declaración de opción de ayuda en virtud de Apt se muestra a continuación,

.. code-block:: bash

	ptconfigure Apt help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda bajo apt.

.. code-block:: bash

 kevell@corp:/# ptconfigure apt help
 ******************************


  This command allows you to modify create or modify apts

  Apt, apt

        - create
        Create a new system apt, overwriting if it exists
        example: ptconfigure apt create --aptname="somename"

        - remove
        Remove a system apt
        example: ptconfigure apt remove --aptname="somename"

        - set-password
        Set the password of a system apt
        example: ptconfigure apt set-password --aptname="somename" --new-password="somepassword"

        - exists
        Check the existence of a apt
        example: ptconfigure apt exists --aptname="somename"

        - show-groups
        Show groups to which a apt belongs
        example: ptconfigure apt show-groups --aptname="somename"

        - add-to-group
        Add apt to a group
        example: ptconfigure apt add-to-group --aptname="somename" --groupname="somegroupname"

        - remove-from-group
        Remove apt from a group
        example: ptconfigure apt remove-from-group --aptname="somename" --groupname="somegroupname"

 ------------------------------
 End Help
 ******************************

Diferentes características de Apt
-------------------------------------------

En este tema se trata con diferentes características de apto en virtud de este módulo, así como las posibles formas de utilizar esas diversas características.

Los diversos aspectos de este módulo bajo apt se enumeran a continuación,

* Crear
* Retire
* Configuración contraseña
* existe
* Show-grupos
* Add-to-grupo
* Quitar-de-grupo

CREAR
---------
Esta función tiene como objetivo la creación de un nuevo sistema de apt, y al igual que sobrescribe en caso de que ya existe. Esta función de apt usando este módulo se puede lograr mediante la siguiente sintaxis,

.. code-block:: bash

	ptconfigure apt create --aptname="somename"

En el lugar de aptname el usuario puede especificar el nombre de la APT que se va a crear. Después de introducir el comando como se especifica anteriormente, el nuevo sistema apt se creará con el nombre especificado.

RETIRE
---------

Esta función tiene como objetivo la eliminación de un apt existente. Esta función de apt usando este módulo se puede lograr mediante la siguiente sintaxis,

.. code-block:: bash

	ptconfigure apt remove --aptname="somename"

En el lugar de aptname el usuario puede especificar el nombre de los apartamentos que se va a eliminar. Después de introducir el comando como se especifica anteriormente, el apartamento especificado se eliminarán.

CONTRASEÑA SET
-----------------------

Esta función facilita el establecimiento de una nueva contraseña a un sistema apto según las necesidades. Esto se puede hacer mediante la aplicación del comando como se indica a continuación,

.. code-block:: bash

	ptconfigure apt set-password --aptname="somename" --new-password="somepassword"

Para llevar a cabo estas funciones, el usuario tiene que especificar los dos campos,

* Nombre Apt
* Nueva contraseña

Después de especificar los dos campos en el formato de comando antes mencionado, se creará la nueva contraseña para el apt especificado.

EXISTE
---------

Esta función tiene por objeto la comprobación de la existencia de un apt. Esto se puede hacer simplemente, mediante el comando de abajo,

.. code-block:: bash

	ptconfigure apt exists --aptname="somename"

Después de aplicar el comando como el anterior, la existencia de un apt mencionados se garantizará con los resultados.

GRUPOS VER
-----------------

Esta función ayuda a los usuarios a conocer a qué grupo pertenece a la APT. Esto se puede conseguir simplemente utilizando el siguiente comando,

.. code-block:: bash

	ptconfigure apt show-groups --aptname="somename"

El usuario tiene que especificar el nombre de los apartamentos en el campo de aptname, con el fin de conocer los detalles de su grupo.

AÑADIR _TO_GROUP
---------------------------

El principal objetivo de esta función es añadir la necesaria apto para el grupo requerido por la simple aplicación de la orden como se indica a continuación,

.. code-block:: bash

	ptconfigure apt add-to-group --aptname="somename" --groupname="somegroupname"

Para implementar esta función, el usuario tiene que especificar los dos campos siguientes de acuerdo a sus necesidades en el formato de la mencionada orden,

* Aptname
* Nombre del grupo

REMOVE_FROM_GROUP
--------------------------------

El objetivo principal de esta función es eliminar el apartamento de un grupo simplemente aplicando el comando como se indica a continuación,

.. code-block:: bash

	ptconfigure apt remove-from-group --aptname="somename" --groupname="somegroupname"

Para implementar esta función, el usuario tiene que especificar los dos campos siguientes de acuerdo a sus necesidades en el formato de la mencionada orden,

* Aptname
* Nombre del grupo

parámetros alternativos
--------------------------------

Los parámetros alternativos para este módulo, cualquiera de los cuales se pueden utilizar en la declaración es,

* Apt
* apt

Beneficios
--------------

* Los parámetros utilizados declarando ayuda y otras características diferentes de apt no distinguen entre mayúsculas y minúsculas.
* Es-acomodado tanto os Cent y así como en Ubuntu.
* El uso de este módulo, el usuario puede crear y, así como modificar el apartamento de acuerdo a sus necesidades.
* La existencia de un apartamento puede garantizarse en este módulo.

