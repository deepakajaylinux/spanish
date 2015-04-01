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

        - install
        Install
        example: ptconfigure pear pkg-install --package-name="somename"

        - remove
        Remove
        example: ptconfigure pear pkg-remove --package-name="somename"

        - ensure
        Ensure
        example: ptconfigure pear pkg-ensure --package-name="somename"
        
 ------------------------------
 End Help

Install
----------

Cuando el usuario necesita instalar una pera , el comando a continuación se indica se ejecutará el proceso.


.. code-block:: bash

	ptconfigure pear pkg-install --package-name="somename"

.. code-block:: bash

 kevell@corp:/# ptconfigure pear pkg-install --package-name="file"
 downloading File-1.4.1.tgz ...
 Starting to download File-1.4.1.tgz (8,164 bytes)
 .....done: 8,164 bytes
 install ok: channel://pear.php.net/File-1.4.1
 ******************************


 Pear Modifications:
 --------------------------------------------

 Pear: Success

 ------------------------------
 Pear Mods Finished
 ******************************



Remove
------------

Cuando el usuario necesita para eliminar una pera sistema , el comando a continuación se indica se ejecutará el proceso.


.. code-block:: bash

	ptconfigure pear pkg-remove --package-name="somename"

.. code-block:: bash

 kevell@corp:/# ptconfigure pear pkg-remove --package-name="file"
 pear/File (version >= 1.4.0) is required by installed package "pear/File_CSV"
 pear/File (version >= 1.4.0) is required by installed package "pear/File_Util"
 pear/File cannot be uninstalled, other installed packages depend on this package
 [Pharaoh Logging] Removing Package file from the Packager Pear did not execute correctly
 ******************************


 Pear Modifications:
 --------------------------------------------

 Pear: Failure

 ------------------------------
 Pear Mods Finished
 ******************************



Ensure
---------

Cuando el usuario necesita para garantizar una pera, el siguiente comando dado se ejecutará el proceso. 

.. code-block:: bash

	ptconfigure pear pkg-ensure --package-name="somename"

.. code-block:: bash

 kevell@corp:/# ptconfigure pear pkg-ensure --package-name="file"
 downloading File-1.4.1.tgz ...
 Starting to download File-1.4.1.tgz (8,164 bytes)
 .....done: 8,164 bytes
 install ok: channel://pear.php.net/File-1.4.1
 ******************************


 Pear Modifications:
 --------------------------------------------

 Pear: Success

 ------------------------------
 Pear Mods Finished
 ******************************





Parámetro Alternativa
--------------------------------

Hay dos parámetros alternativos que pueden ser utilizados en la línea de comandos.

Pear, pear


Beneficios
--------------

Pear.php.net proporciona tanto un ser humano-friendly (HTML) y máquina mascotas (currently REST) interfaz para los paquetes disponibles en pear.php.net. Toda la comunicación se produce a través del protocolo HTTP. Otras funciones del sitio pear.php.net ofrece son:

* Gestión de cuentas de usuario (independiente del servidor SVN)
* Gestión de paquetes
* Gestión de la liberación
* Well-to-do en Ubuntu y CentOS
* Sensitibilidad caso
