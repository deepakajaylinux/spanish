==========
Process
==========

sinopsis
------------

Este módulo ayuda a los usuarios en el manejo de unas funciones de proceso requeridos, y también para matar un proceso. El usuario puede especificar el proceso en particular sobre la base de sus requisitos. El usuario puede especificar el nombre del proceso, el archivo o directorio, ya sea desde el ámbito local o en un equipo remoto. Veamos, el uso y las metodologías que participan en ella.

Ayuda Comando
---------------------

El comando de ayuda sirve a los usuarios respecto a cómo manejar y trabajar con procesos de acuerdo a sus necesidades. También enumera los parámetros alternativos de proceso. Se describe la sintaxis para matar un proceso, y también acerca de cómo especificar matar a un proceso sobre la base de sus necesidades. El comando de ayuda para el módulo de proceso se muestra a continuación.

.. code-block:: bash

		ptconfigure process help

La siguiente captura de pantalla como se muestra a continuación, muestra cómo matar un proceso, y cómo definir matar a un proceso.

.. code-block:: bash 

 kevell@corp:/# ptconfigure process help
 ******************************


  This command handles process functions, kill a process for now

  Process, process

        - kill
        Will ask you for process name, aa file or directory from local to remote
        example: ptconfigure process kill
        example: ptconfigure process kill --yes --name="selenium" --use-psax # default, will look for string in result of
        example: ptconfigure process kill --yes --name="selenium" --use-pkill # will allow pkill to find  by string to kill
        example: ptconfigure process kill --yes
                                        --guess
                                        --id="1234 # will kill a process by id
                                        --level # will guess a 9

 ------------------------------
 End Help
 ******************************



¿Cómo definir y utilizar el proceso
--------------------------------------------

Para matar a un proceso de la siguiente sintaxis se puede utilizar.

.. code-block:: bash

		ptconfigure process kill
or
.. code-block:: bash

		ptconfigure process kill --yes --name="selenium" --use-psax # default

La sintaxis que se muestra arriba voluntad busca la cadena en consecuencia de.

.. code-block:: bash

		ptconfigure process kill --yes --name="selenium" --use-pkill #

La sintaxis que se muestra arriba se utiliza para especificar o buscar una cadena que se va a morir.

.. code-block:: bash

		ptconfigure process kill --yes
				--guess
				id="1234 # 

El comando como se muestra arriba voluntad mata a un proceso como por el id indicado.

.. code-block:: bash

		ptconfigure process kill --yes
			--level #

El comando que arriba se utiliza para matar un proceso como por el nivel especificado.

.. code-block:: bash

	ptconfigure process kill --yes --guess --name="skype"

El comando que arriba se utiliza para matar un proceso especificando su nombre. La siguiente captura de pantalla muestra el trabajo de matar a un proceso.

Matar a un proceso utilizando un PID
----------------------------------------------

Si el PID # 3486 se asigna al proceso lighttpd. Para matar el servidor lighttpd, necesita pasar un PID de la siguiente manera:

.. code-block:: bash

 # kill 3486

or
.. code-block:: bash
 
 $ sudo kill 3486

Esto terminar un proceso con un PID de 3486.

¿Cómo puedo verificar que el proceso se ha ido / mató?
-----------------------------------------------------------------

Utilice el comando pidof ps o:

.. code-block:: bash
 
 $ ps aux | grep lighttpd
 $ pidof lighttpd

¿Cómo puedo matar a dos o más PID?
--------------------------------------------

La sintaxis es la siguiente para matar a dos o más los PID como lo requiere se puede utilizar en un solo comando:

.. code-block:: bash

 kill  pid1 pid2 pid3
 kill -15  pid1 pid2 pid3
 kill -9  pid1 pid2 pid3
 kill  -9 3546 5557 4242

Saluda a matar a todos los comandos
----------------------------------------------

Se trata de un único comando Linux. para matar procesos por nombre. Así que no hay necesidad de encontrar los PID utilizando el 'proceso pidof "o" ps aux | grep proceso' comando. No utilice killall comandos en sistemas operativos Unix. Se trata de un comando específico Linux.

La sintaxis es

.. code-block:: bash

 killall Process-Name-Here

Para matar el servidor lighttpd, escriba:

.. code-block:: bash
 
 # killall -15 lighttpd

or
.. code-block:: bash

 # killall -9 lighttpd

Para matar el proceso navegador web Firefox, escriba:

.. code-block:: bash

 # killall -9 firefox-bin

Como he dicho antes, el comando en todo sistema UNIX matan Qué otra cosa. Mata a todos los procesos y proceso no sólo una parte. No utilice matar a todos en el sistema UNIX.

Beneficios
------------

* El usuario puede matar a un proceso con diferentes parámetros de acuerdo a sus requerimientos. Por ejemplo: a través de la identificación, nivel del proceso se puede especificar para matar.
