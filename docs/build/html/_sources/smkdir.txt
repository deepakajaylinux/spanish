========
Mkdir
========

sinopsis
------------

Este módulo ayuda a crear un directorio. El usuario puede especificar el camino mientras que declara la creación del directorio o en tiempo de ejecución de la creación de un directorio. Se puede realizar ya sea en la máquina remota o local. Veamos cómo este módulo ayuda en la creación de un directorio.

Ayuda Comando
---------------------

El comando de ayuda conduce a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en el Mk Dir. El comando help enumera los parámetros alternativos de MK Dir. . También se describe la sintaxis para crear un directorio de dos maneras diferentes, ya sea al momento de la declaración o en tiempo de ejecución. . El comando de ayuda para MK dir se muestra a continuación.

.. code-block:: bash

	ptconfigure mkdir help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda bajo MK dir.

.. code-block:: bash

	kevell@corp:/# ptconfigure Mkdir help
	******************************


        This command handles file copying functions.

         Mkdir, mkdir

        - path
        Will ask you for details for servers, then copy a file or directory from local to remote
        example: ptconfigure mkdir path
        example: ptconfigure mkdir path --yes --path="/path/to/new/directory"

	------------------------------
	End Help
	******************************

parámetros alternativos
------------------------------

Durante el uso de los comandos de ayuda y la creación de un directorio, en lugar de mkdir Mkdir también se puede utilizar.

Creación de un Mc Dir
---------------------------

Creación de un Dir Mc se puede hacer de dos maneras diferentes:

.. rubric:: Ya sea en tiempo de ejecución

.. code-block:: bash

	Example: ptconfigure mkdir path

.. rubric:: O bien, en el momento de la declaración

.. code-block:: bash

	Example: ptconfigure mkdir path --yes --path="/path/to/new/directory"

La siguiente captura de pantalla muestra la segunda forma de crear un directorio.

.. code-block:: bash

	kevell@corp:/# ptconfigure mkdir path --yes --path="/kevellsdoc"
	
	[Pharaoh Logging] [Mkdir] Executing mkdir /kevellsdoc
	******************************


	Mkdir Result: Success
	------------------------------
	Mkdir Finished
	******************************

Beneficios
------------

* Los parámetros utilizados en la ayuda y la creación de unas operaciones de directorio no son sensibles, que es una ventaja añadida, mientras 
  que en comparación con otros.
* Creación de un directorio se puede definir de dos maneras diferentes como el tiempo de declaración o en tiempo de ejecución.
* Se puede realizar tanto en el equipo local o remoto.
* Es-acomodados tanto en Ubuntu y así como Cent OS.

