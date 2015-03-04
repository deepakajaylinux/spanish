============
Parallax
============

sinopsis
----------

El paralaje promueve las funciones multitarea en la máquina de los usuarios. Los parámetros que definen la instalación y ayuda no son sensibles, mientras que en comparación con otros. Es más fácil para definir la función multitarea ya sea en el momento de la instalación o en el momento de ejecutar el proceso de instalación.

Ayuda Comando
--------------------

El comando de ayuda guía al usuario en el trabajo con este paralaje. También especifica el comando que se utiliza para la instalación de la paralaje y también la sintaxis para dos tipos de declarar instalación. El comando de ayuda también enumera los parámetros alternativos que se pueden utilizar. El comando utilizado para la opción de ayuda bajo el paralaje es la siguiente.

.. code-block:: bash

	ptconfigure parallax help

La visualización de los resultados después de la entrada de comando de ayuda se representa en la siguiente imagen.

.. code-block:: bash


	kevell@corp:/# ptconfigure Parallax help
	******************************



	This Module lets you execute commands in parallel

        Parallax, parallax

        - cli
        Go through all questions to execute parallel programs
        example: ptconfigure parallax cli
        example: ptconfigure parallax cli --yes --command-1="pwd" --command-2="ls"

        - child
        Unlikely you'll use this, its used by cli to spawn child processes
        example: parallax cli child

	------------------------------
	End Help
	******************************


instalación
--------------

Es más fácil ir con paralaje para la instalación como instalación se puede definir de dos maneras diferentes según las necesidades de los usuarios. Estas dos formas se definen como a continuación:

* Al mencionar los tipos de múltiples tareas que se requieren al definir el mandato de instalación.
* O, al mencionar los tipos de tareas durante la ejecución (tiempo de ejecución) de la instalación.

El comando que se utiliza para especificar las múltiples tareas en el momento del comando de instalación declarar se muestra a continuación:

.. code-block:: bash

	ptconfigure parallax cli --yes --command-1="pwd" --command-2="who"

Después de mencionar este comando, el paralaje ejecuta tanto de las funciones especificadas anteriormente al mando-1 y comando-2. Las dos tareas se realizan en paralelo y se visualizan resultado. La captura de pantalla adjunta a continuación es un ejemplo muy bueno para el tipo de declaración se ha definido anteriormente.

.. code-block:: bash

	kevell@corp:/# ptconfigure parallax cli --yes --command-1="pwd" --command-2="who"
	Completed task: pwd
	Completed task: who
	******************************


	COMMAND: pwd
	COMPLETE: 1
	EXIT_STATUS: 0
	OUTPUT: /home/kevells


	COMMAND: who
	COMPLETE: 1
	EXIT_STATUS: 0
	OUTPUT: kevells   :0           2015-01-08 12:15 (:0)
	kevells   pts/2        2015-01-08 14:11 (:0)
	kevells   pts/1        2015-01-08 16:36 (:0)
	kevells   pts/10       2015-01-08 16:36 (:0)



	-----------------

	In Cli


	******************************

El comando utilizado para declarar las tareas múltiples en tiempo de ejecución se muestra a continuación:

.. code-block:: bash

	ptconfigure parallax cli

Después de introducir el comando anterior se produce el siguiente proceso:

.. cssclass:: table-bordered

 +--------------------------+--------------------------------------------------+-------------+---------------------------------------------+
 | Parámetros               | Parámetro Alternativa                            | Opciones    | Comentarios                                 |
 +==========================+==================================================+=============+=============================================+
 |Run Commands in           | A pesar de parallax, las siguientes alternativas | Y(Yes)      | Si el usuario desea continuar el proceso de |
 |Parallel? (Y/N)           | también se pueden utilizar., Parallax            |             | instalación se puede introducir como Y.     |
 +--------------------------+--------------------------------------------------+-------------+---------------------------------------------+
 |Run Commands in           | A pesar de parallax, las siguientes alternativas | N(No)       | Si el usuario desea abandonar el proceso de |
 |Parallel? (Y/N)           | también se pueden utilizar., Parallax            |             | instalación se puede introducir como N.|    |
 +--------------------------+--------------------------------------------------+-------------+---------------------------------------------+


Si el usuario desea continuar la instalación, el usuario puede especificar las múltiples tareas según sus necesidades. Tras la finalización de la especificación de las múltiples tareas, si los usuarios desean dejar que pueden detener con sólo introducir ninguna.

Por último, los resultados de las tareas realizadas, junto con su estado se definen al final. Las siguientes capturas de pantalla que puede una representación gráfica sobre el proceso antes mencionado.

.. code-block:: bash

   
	kevell@corp:/# ptconfigure parallax cli 
	
	Run Commands in Parallel? (Y/N) 
	y
	Enter Command to include next. Enter none to end.
	pwd
	Enter Command to include next. Enter none to end.
	who
	Enter Command to include next. Enter none to end.

	Completed task: pwd
	Completed task: who
	******************************


	COMMAND: pwd
	COMPLETE: 1
	EXIT_STATUS: 0
	OUTPUT: /home/kevells


	COMMAND: who
	COMPLETE: 1
	EXIT_STATUS: 0
	OUTPUT: kevells   :0           2015-01-08 12:15 (:0)
	kevells   pts/2        2015-01-08 14:11 (:0)
	kevells   pts/1        2015-01-08 16:36 (:0)
	kevells   pts/10       2015-01-08 16:36 (:0)



	-----------------

	In Cli


	******************************


Beneficios
-------------

* El usuario puede definir las tareas en paralelo, ya sea en tiempo de ejecución o en un modo predefinido según sus necesidades.
* Por último, tras la finalización de las multi-tareas de los resultados y el estado de las tareas completadas se informan con claridad.
* La sintaxis utilizada para declarar no distingue entre mayúsculas y minúsculas al comparar a los demás lo que es una ventaja añadida.
* Es-acomodados tanto en CentOS y así como mayúsculas y minúsculas.
