============
Pear
============

Sinopsis
-------------

PEAR es la abreviatura de "Extensión PHP y Repositorio de aplicaciones" y se pronuncia igual que la fruta. El propósito de PEAR es proporcionar:

* Una biblioteca estructurada de código abierto para los usuarios de PHP
* Un sistema de distribución de código y mantenimiento de paquetes
* Un estilo estándar para el código escrito en PHP, especifica aquí
* El PHP Extension Community Library (PECL)

La misión de PEAR es proporcionar componentes reutilizables, la innovación principal en PHP, proporcionar las mejores prácticas para el desarrollo de PHP y educar a los desarrolladores.

El código de PEAR se divide en "paquetes". Cada paquete es un proyecto independiente con su propio equipo de desarrollo, el número de versión, ciclo de lanzamiento, la documentación y una relación definida con otros paquetes (incluyendo dependencias). Los paquetes se distribuyen como ficheros tar comprimidos con gzip con un archivo de descripción en el interior, y se instalan en el sistema local utilizando el instalador de PEAR.

Ayuda Comando
----------------------

Este comando ayuda a determinar el uso del módulo PEAR. El usuario se llega a saber acerca de la diferente forma / formato de ejecutar este módulo. Este comando guía al usuario final a conocer el propósito de este comando. A continuación dado son el mando y la pantalla del mismo.

.. code-block:: bash
        
	        ptconfigure pear help

La representación gráfica de la orden anterior se enumeran a continuación,

.. code-block:: bash


 kevell@corp:/# ptconfigure pear help
 ******************************


  This command allows you to modify create or modify pears

  Pear, pear

        - create
        Create a new system pear, overwriting if it exists
        example: ptconfigure pear create --pearname="somename"

        - remove
        Remove a system pear
        example: ptconfigure pear remove --pearname="somename"

        - set-password
        Set the password of a system pear
        example: ptconfigure pear set-password --pearname="somename" --new-password="somepassword"

        - exists
        Check the existence of a pear
        example: ptconfigure pear exists --pearname="somename"

        - show-groups
        Show groups to which a pear belongs
        example: ptconfigure pear show-groups --pearname="somename"

        - add-to-group
        Add pear to a group
        example: ptconfigure pear add-to-group --pearname="somename" --groupname="somegroupname"

        - remove-from-group
        Remove pear from a group
        example: ptconfigure pear remove-from-group --pearname="somename" --groupname="somegroupname"

 ------------------------------
 End Help
 ******************************

crear
------------

Cuando el usuario necesita para crear un nuevo sistema de pera o necesita para sobrescribir el existente, el comando a continuación se indica se ejecutará el proceso.

.. code-block:: bash
	
        ptconfigure pear create --pearname="somename"

quitar
------------

Cuando el usuario necesita para eliminar una pera sistema, el comando a continuación se indica se ejecutará el proceso.

.. code-block:: bash

	ptconfigure pear remove --pearname="somename"

Establecer contraseña
---------------------------

Cuando el usuario necesita establecer una contraseña de una pera sistema, el comando a continuación se indica se ejecutará el proceso.

.. code-block:: bash
	
	 ptconfigure pear set-password --pearname="somename" --new-password="somepassword"
existe
---------------------

Cuando el usuario necesita conocer la existencia de la pera, el siguiente comando dado se ejecutará el proceso.

.. code-block:: bash
	
	ptconfigure pear exists --pearname="somename"

Mostrar grupos
---------------------

Cuando el usuario necesita conocer el grupo al que pertenece una pera, el siguiente comando dado se ejecutará el proceso.

.. code-block:: bash
	
	ptconfigure pear show-groups --pearname="somename"

Añadir al grupo
---------------------

Cuando el usuario necesita asignar pera a un grupo particular, el siguiente comando dado se ejecutará el proceso.

.. code-block:: bash
	
	ptconfigure pear add-to-group --pearname="somename" --groupname="somegroupname"

Eliminar de grupo
----------------------------

Cuando el usuario necesita para eliminar la pera de un grupo, el siguiente comando dado se ejecutará el proceso.

.. code-block:: bash
	
	ptconfigure pear remove-from-group --pearname="somename" --groupname="somegroupname"

Parámetro Alternativa
--------------------------------

Hay dos parámetros alternativos que pueden ser utilizados en la línea de comandos.

Pear, pear

.. code-block:: bash

 Por ejemplo: ptconfigure pear create --pearname="somename"/ ptconfigure Pear create --pearname="somename"

Beneficios
--------------

Pear.php.net proporciona tanto un ser humano-friendly (HTML) y máquina mascotas (currently REST) interfaz para los paquetes disponibles en pear.php.net. Toda la comunicación se produce a través del protocolo HTTP. Otras funciones del sitio pear.php.net ofrece son:

* Gestión de cuentas de usuario (independiente del servidor SVN)
* Gestión de paquetes
* Gestión de la liberación
* Well-to-do en Ubuntu y CentOS
* Sensitibilidad caso
