========
Logging
========

sinopsis
-----------
Este módulo de registro se utiliza con el propósito de registrar un mensaje a la consola, y se utiliza opcionalmente para registro de errores php. Veamos cómo instalar y utilizar el registro para la declaración de mensaje y en registro de errores php.

Ayuda Comando
--------------------

El comando ayuda actúa como un breve manual de usuario que lleva al usuario acerca de su uso y metodologías. Se especifica los parámetros alternativos que se pueden utilizar en la declaración, y un ejemplo de sintaxis para definir un registro. El comando utilizado para declarar la opción de ayuda se da a continuación:

.. code-block:: bash

		ptdeploy Logging help

La siguiente captura de pantalla muestra gráficamente sobre el funcionamiento de comando ayuda.

.. code-block:: bash

 kevell@corp:/# ptdeploy Logging help
 ******************************


  Use this to log a message to the Console, and optionally the php error log.

  Logging, logging

        - log
        Logs a message the console or
        example: ptconfigure logging log --php-log --log-message="Here is something logging to the console and error log"

 ------------------------------
 End Help
 ******************************

instalación
---------------

El comando utilizado para instalar el registro bajo ptdeploy se da a continuación:

.. code-block:: bash

		ptdeploy logging log

Después de la introducción, el comando anterior, el proceso de instalación se representa en la siguiente columna tabular.

.. cssclass:: table-bordered


 +-------------------------+-------------------------------------+-------------+------------------------------------------------+
 | Parámetros              | Parámetro Alternativa               | Opciones    | Comentarios                                    |
 +=========================+=====================================+=============+================================================+
 |Install Logging? (Y/N)   | En lugar de Logging, podemos        | Y(Yes)      | Si el usuario desea continuar el proceso de    |
 |                         | utilizar logging también.           |             | instalación se puede introducir como Y.        |
 +-------------------------+-------------------------------------+-------------+------------------------------------------------+
 |Install Logging? (Y/N)   | En lugar de Logging, podemos        | N(No)       | Si el usuario desea abandonar el proceso de    |
 |                         | utilizar logging también.           |             | instalación se puede introducir como N.|       |
 +-------------------------+-------------------------------------+-------------+------------------------------------------------+

Si el usuario continúa el proceso de instalación, el proceso de solicitud de los usuarios para especificar el mensaje de registro pidiendo

.. code-block:: bash

	"Enter Log Message"
	
	"Good Morning"

Una vez que la entrada del usuario el mensaje, el mensaje de registro dan irán apareciendo en la pantalla como se muestra:
"Good Morning"

Por último, la instalación se completó. La siguiente captura de pantalla muestra el proceso de instalación ilustrado.

.. code-block:: bash

 kevell@corp:/#  ptdeploy logging log
 Install Logging? (Y/N) 
 Y
 *******************************
 *   Golden Contact Computing  *
 *           Logging!          *
 *******************************
 Enter Log Message
 Good Morning
 [Pharaoh Logging] Good Morning
 ... All done!
 *******************************
 Thanks for installing , visit www.gcsoftshop.co.uk for more
 ******************************


 Single App Installer:
 --------------------------------------------


 No Data.

 ------------------------------
 Installer Finished

¿Cómo definir php registro de errores
------------------------------------------------

La sintaxis para declarar el registro de registro de errores php se muestra a continuación:

.. code-block:: bash

	ptconfigure logging log --php- log --log-message="Here is something logging to the console and error log"

en lugar de

.. code-block:: bash

 	log-message="Here is something logging to the console and error log"

el usuario puede añadir cualquier texto a la parte del mensaje de registro en función de sus necesidades.

Beneficios
--------------

* El usuario puede añadir su mensaje de registro frecuentemente utilizado para el registro de errores php.
* Durante la instalación del registro que el usuario puede introducir y garantizar la visualización de mensaje de registro.
* Es-acomodados tanto en ubuntu y al igual que en ciento OS.
* Los parámetros utilizados en la declaración no distingue entre mayúsculas y minúsculas.

