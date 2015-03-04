=====
PECL
=====

sinopsis
----------------

PECL significa para "Emisor lógica positiva Acoplado". Pecl son salidas lógicas diferenciales comúnmente utilizados en los circuitos de distribución de reloj de alta velocidad. Este comando proporciona al usuario crear, eliminar, setpassward, existe. Las actividades de grupo también posible a través de este comando. Esta función de control principal se basa en el sistema. Es adecuado con Ubuntu y CentOS.

comando Ayuda
----------------------

Pecl hace que el desarrollo conjunto de una brisa: trabaja con existir, modificar, crear, para apoyar el conjunto passward para pecl sistema. Con pecl, modificar un paquete llega a ser tan fácil que será el diseño predeterminado de usuario cada vez que el usuario está escribiendo una cantidad significativa de código.

.. code-block:: bash

		ptconfigure pecl help

La siguiente captura de pantalla y explica su función.

.. code-block:: bash

 kevell@corp:/# ptconfigure PECL help

 ******************************


  This command allows you to modify create or modify pecls

  PECL, pecl

        - create
        Create a new system pecl, overwriting if it exists
        example: ptconfigure pecl create --peclname="somename"

        - remove
        Remove a system pecl
        example: ptconfigure pecl remove --peclname="somename"

        - set-password
        Set the password of a system pecl
        example: ptconfigure pecl set-password --peclname="somename" --new-password="somepassword"

        - exists
        Check the existence of a pecl
        example: ptconfigure pecl exists --peclname="somename"

        - show-groups
        Show groups to which a pecl belongs
        example: ptconfigure pecl show-groups --peclname="somename"

        - add-to-group
        Add pecl to a group
        example: ptconfigure pecl add-to-group --peclname="somename" --groupname="somegroupname"

        - remove-from-group
        Remove pecl from a group
        example: ptconfigure pecl remove-from-group --peclname="somename" --groupname="somegroupname"

 ------------------------------
 End Help
 ******************************

crear
------------

Este comando permite al usuario crear un nuevo pecl sistema. Overwriting es posible en caso de la existencia. Nuevo nombre pecl puede ser mencionado en un solo comando en sí.

El comando utilizado para crear es el siguiente

.. code-block:: bash

		ptconfigure pecl create 

Después de la entrada como el comando anterior, comienza a crear pecl. En caso de archivo existente aparece la indicación de mensaje. El comando y su función se explica con las capturas de pantalla.

.. code-block:: bash

        - create
        Create a new system pecl, overwriting if it exists
        example: ptconfigure pecl create --peclname="somename"

quitar
------------

Este comando permite al usuario eliminar una pecl. Nombre pecl extraíble puede ser mencionado en una sola línea de comandos.
El comando utilizado para crear es el siguiente

.. code-block:: bash

		ptconfigure pecl remove 

Después de la entrada como el comando anterior, comienza a retirar pecl. En el caso de archivos ya eliminados de la pecl aparece la indicación de mensaje. El comando y su función se explica con las capturas de pantalla.

.. code-block:: bash

        - remove
        Remove a system pecl
        example: ptconfigure pecl remove --peclname="somename"

Establecer contraseña
--------------------------

Setpassward se utiliza para ejecutar un comando en particular con permisos de root en pecl. Lo interesante es que cuando el usuario usa passward de un comando en particular, el sistema solicita al usuario la contraseña del usuario actual. El comando utilizado para crear es el siguiente

.. code-block:: bash

	ptconfigure pecl  set-password

Nombre Pecl y nueva passward también mencionan en la misma línea de comandos. Esto hace que otro beneficio para este módulo. La siguiente captura de pantalla de visualización de sus funciones.

.. code-block:: bash

        - set-password
        Set the password of a system pecl
        example: ptconfigure pecl set-password --peclname="somename" --new-password="somepassword"

existe
-----------

Este comando sirve para comprobar la existencia de un pecl. Comando simple que hace que este trabajo de comando correctamente. En primer lugar se comprueba nombre pecl en el sistema, entonces indica si está vigente o no. El siguiente comando usa para hacer esta función

.. code-block:: bash

		ptconfigure pecl Exists

La siguiente captura de pantalla de visualización de sus funciones.

.. code-block:: bash

        - exists
        Check the existence of a pecl
        example: ptconfigure pecl exists --peclname="somename"

Show-Grupo
------------------

Este comando sirve para comprobar el grupo de trabajo de un pecl. Comando simple que hace que este trabajo de comando correctamente. En primer lugar, comprueba el nombre del grupo y luego pecl nombre en el sistema entonces indica el nombre del grupo al que pertenece un pecl. El siguiente comando usa para hacer esta función.

.. code-block:: bash

        - show-groups
        Show groups to which a pecl belongs
        example: ptconfigure pecl show-groups --peclname="somename"

Add-To-Grupos
------------------------

Esto facilita al usuario añadir un pecl a un grupo. Mientras que la adición de lo posible pide nombre pecl y nombre del grupo. El usuario puede entrar en el acuerdo a su deseo.

.. code-block:: bash
   
		ptconfigure pecl add-to-group

Después de introducir el comando que añadir un pecl en grupo.

.. code-block:: bash

        - add-to-group
        Add pecl to a group
        example: ptconfigure pecl add-to-group --peclname="somename" --groupname="somegroupname"

Remove-de-grupo
----------------------------

Este comando permite al usuario eliminar una pecl del grupo. Nombre pecl extraíble puede ser mencionado en una sola línea de comandos.
El comando utilizado para crear es el siguiente

.. code-block:: bash

		ptconfigure pecl remove-from-group 

Después de la entrada como el comando anterior, comienza a retirar pecl de grupo. En el caso de archivos ya eliminados de la pecl aparece la indicación de mensaje. El comando y su función se explica con las capturas de pantalla.

.. code-block:: bash

        - remove-from-group
        Remove pecl from a group
        example: ptconfigure pecl remove-from-group --peclname="somename" --groupname="somegroupname"


Beneficios
----------------

* Sensitibilidad caso.
* Well-to-do en Ubuntu y CentOS.
* Menor consumo de energía.
* Crear un nuevo pecl sistema
* Retirar un pecl
* Añadir a grupo es posible
* Retire el grupo es posible
* Mostrar grupo es posible
