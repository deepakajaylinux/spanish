========
Chgrp       
========

sinopsis
-----------

Los archivos y directorios pertenecen tanto a un propietario y un grupo. Un grupo normalmente consiste en una colección de usuarios, todos ellos pertenecientes al mismo grupo. El primer conjunto de tres es la lectura, escritura y ejecución para el propietario del archivo.

Un grupo también puede constar de un usuario, normalmente el usuario que crea el archivo. Cada usuario del sistema, incluido el usuario root, se le asigna su propio grupo de que él o ella es el único miembro, garantizando el acceso sólo por ese usuario. El segundo grupo de tres es la lectura, escritura y ejecución permisos para cualquier persona que pertenece al grupo de usuarios para el archivo.

El usuario root, el administrador del sistema, es dueño de la mayor parte de los archivos del sistema que también pertenecen al grupo de las raíces, de las cuales sólo el usuario root es miembro. La mayoría de los archivos de administración, como los archivos de configuración en el directorio / etc, son propiedad del usuario root y pertenecen al grupo de raíz. Sólo el usuario root tiene permiso para modificarlos, mientras que los usuarios normales pueden leer y, en el caso de los programas, también ejecutarlos

Ayuda Comando
----------------------

Este comando ayuda a determinar el uso del módulo de grupo Cambio. El usuario se llega a saber acerca de la diferente forma / formato de ejecutar este módulo. Este comando guía al usuario final a conocer el propósito de este comando. A continuación dado son el mando y la pantalla del mismo.

.. code-block:: bash
        
	        cleopatra Chgrp help

La representación gráfica de la pantalla se da a continuación,

.. code-block:: bash

 kevell@corp:/#  cleopatra Chgrp help
 ******************************


  This command handles file group ownership changing functions.

  Chgrp, chgrp

        - path
        Will change the file group ownership of a path
        example: cleopatra chgrp path --yes --guess --recursive --path=/a/file/path --group=golden


 ------------------------------
 End Help
 ******************************

Camino
----------

Cuando el usuario tiene que cambiar la propiedad del grupo de archivo de una ruta, el siguiente comando dado se ejecutará el proceso.

.. code-block:: bash
        
	        cleopatra chgrp path –yes –guess –recursive –path=/”File path” –group=”group name”

Parámetro Alternativa
--------------------------------

Hay dos parámetros alternativos que pueden ser utilizados en la línea de comandos.

chgrp, Chgrp

Por ejemplo: cleopatra Chgrp path/ cleopatra chgrp path

Beneficios
--------------

* Aunque otros usuarios pueden ser capaces de acceder a un archivo, sólo el propietario puede cambiar sus permisos. Si usted desea dar a otro 
  usuario para controlar más de uno de los permisos de su archivo, puede cambiar el propietario del archivo de uno mismo al otro usuario.
* También puede cambiar el grupo de un archivo y directorios, utilizando el comando chgrp. chgrp toma como primer argumento el nombre del 
  nuevo grupo por unos archivos o directorios.
