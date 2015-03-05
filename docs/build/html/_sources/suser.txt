====
User
====

Sinopsis
-------------

Un usuario es cualquier persona que usa una computadora. La computadora tiene un nombre para cada cuenta que crea, y es este nombre por el cual una persona adquiere el acceso a usar la computadora. Algunos servicios del sistema también se ejecutan utilizando cuentas de usuario restringidas o privilegiados.

Administración de usuarios se realiza con el propósito de la seguridad limitando el acceso de ciertas maneras específicas. El superusuario (root) tiene acceso completo al sistema operativo y su configuración; que está diseñado sólo para uso administrativo. Los usuarios sin privilegios pueden utilizar los programas del SU y sudo para una escalada de privilegios controlada.

Una parte fundamental de la administración del sistema es la configuración y administración de usuarios y grupos. Parte de esta tarea consiste en la vigilancia de la log en las capacidades de todas las entidades del sistema.

Vamos a explorar estos conceptos en un Ubuntu 12.04 VPS, pero se puede seguir a lo largo de toda distribución hasta al fecha Linux.

Ayuda Comando
---------------------

Este comando ayuda a determinar el uso del módulo de usuario. El usuario se llega a saber acerca de la diferente forma / formato de ejecutar este módulo. Este comando guía al usuario final a conocer el propósito de este comando. A continuación dado son el mando y la pantalla del mismo.

.. code-block:: bash

	ptconfigure user help

La captura de pantalla para el comando anterior se enumeran a continuación,

.. code-block:: bash

 kevell@corp:/# ptconfigure user help
 ******************************
 This command allows you to modify create or modify users
 User, user

       - create
       Create a new system user, overwriting if it exists
       example: ptconfigure user create --username="somename"

       - remove
       Remove a system user
       example: ptconfigure user remove --username="somename"

       - set-password
       Set the password of a system user
       example: ptconfigure user set-password --username="somename" --new-password="somepassword"

       - exists
       Check the existence of a user
       example: ptconfigure user exists --username="somename"

       - show-groups
       Show groups to which a user belongs
       example: ptconfigure user show-groups --username="somename"

       - add-to-group
       Add user to a group
       example: ptconfigure user add-to-group --username="somename" --groupname="somegroupname"

       - remove-from-group
       Remove user from a group
       example: ptconfigure user remove-from-group --username="somename" --groupname="somegroupname"

 ------------------------------
 End Help
 ******************************


crear
---------

Cuando el usuario necesita para crear una nueva cuenta de usuario del sistema, el comando a continuación se indica se ejecutará el proceso.

.. code-block:: bash

	ptconfigure user create --username="somename"

quitar
-------------

Cuando el usuario necesita eliminar una cuenta de usuario del sistema, el comando a continuación se indica se ejecutará el proceso.

.. code-block:: bash

	ptconfigure user remove --username="somename"

Set-contraseña
------------------

Cuando el usuario necesita para establecer la contraseña de un usuario del sistema, el comando a continuación se indica se ejecutará el proceso.

.. code-block:: bash

	ptconfigure user set-password --username="somename" --new-password="somepassword"

existe
--------

Cuando el usuario necesita para comprobar la existencia de un usuario, el comando a continuación se indica se ejecutará el proceso.

.. code-block:: bash

	ptconfigure user exists --username="somename"

Mostrar grupos
------------------

Cuando el usuario necesita para mostrar grupos a los que pertenece un usuario, el comando a continuación se indica se ejecutará el proceso.

.. code-block:: bash

	ptconfigure user show-groups --username="somename"

Add-a grupo
---------------

Cuando el usuario necesita añadir usuario a un grupo, el siguiente comando dado se ejecutará el proceso.

.. code-block:: bash

	ptconfigure user add-to-group --username="somename" --groupname="somegroupname"

Remove-de-grupo
--------------------------

Cuando el usuario necesita para eliminar el usuario de un grupo, el siguiente comando dado se ejecutará el proceso.

.. code-block:: bash

	ptconfigure user remove-from-group --username="somename" --groupname="somegroupname"

Parámetro Alternativa
-----------------------------

Hay dos parámetros alternativos que pueden ser utilizados en la línea de comandos.

User, user

ejemplo: ptconfigure User help /ptconfigure user help

Beneficios
---------------

La autenticación de usuarios en Linux es un área relativamente flexible de gestión del sistema. Hay muchas maneras de lograr el mismo objetivo con herramientas muy simples.
