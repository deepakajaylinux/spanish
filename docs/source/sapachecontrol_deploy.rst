================
Apache Control
================

sinopsis
-------------

Este módulo es uno de los módulos por defecto que tiene como objetivo en el manejo de las funciones de control del servidor apache. Se permite y facilita las funciones de control necesarias que han de realizarse en el servidor Apache. Veamos, el trabajo y el propósito de las funciones de control y cómo estos módulos involucrados en el manejo de las funciones de control del servidor apache.

Ayuda Comando
---------------------

El comando ayuda actúa como una guía de usuario breve que lleva a los usuarios cómo manejan y utilizan este módulo en particular.
La sintaxis de comando de ayuda bajo el control de Apache se muestra a continuación:

.. code-block:: bash

		ptdeploy ApacheControl help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. El comando de ayuda también enumera los parámetros alternativos que se pueden utilizar en la declaración. La siguiente captura de pantalla a visualizar sobre el comando de ayuda bajo control Apache.

.. code-block:: bash

 kevell@corp:/# ptdeploy ApacheControl help
 ******************************


  This command is part of Default Modules and handles Apache Server Control Functions.

  ApacheControl, apachecontrol, apachectl

          - start
          Start the Apache server
          example: ptdeploy apachecontrol start
          example: ptdeploy apachecontrol start --yes --guess
          example: ptdeploy apachecontrol start --yes --apache-command="apache2"

          - stop
          Stop the Apache server
          example: ptdeploy apachecontrol stop
          example: ptdeploy apachecontrol stop --yes --guess
          example: ptdeploy apachecontrol stop --yes --apache-command="apache2"

          - restart
          Restart the Apache server
          example: ptdeploy apachecontrol restart
          example: ptdeploy apachecontrol restart --yes --guess
          example: ptdeploy apachecontrol restart --yes --apache-command="apache2"

          - reload
          Reloads the Apache server configuration without restarting
          example: ptdeploy apachecontrol reload
          example: ptdeploy apachecontrol reload --yes --guess
          example: ptdeploy apachecontrol reload --yes --apache-command="apache2"

 ------------------------------
 End Help
 ******************************

Las cuatro funciones básicas de control incluidos en el servidor Apache son:

* Inicio
* Deténgase
* Reanudar
* Recargar

Hay tres formas posibles en la definición de una función de control. Por ejemplo, si tomamos función de inicio, se puede definir de tres formas diferentes según los requisitos del usuario, como se muestra a continuación.

.. code-block:: bash
		
		ptdeploy ApacheControl start

or
.. code-block:: bash

		ptdeploy ApacheControl start --yes --guess

or
.. code-block:: bash

		ptdeploy ApacheControl start --yes --apache-command="apache2"

Veamos el uso de tres sintaxis diferente al declarar en los próximos temas.

parámetros alternativos
-------------------------------

Los siguientes son los parámetros alternativos que pueden ser definidos en las declaraciones:

ApacheControl, apachecontrol, apachectl

función de arranque
------------------------

Si el usuario desea iniciar la función de control de apache, la puede usar las siguientes sintaxis como se muestra:

.. code-block:: bash

	ptdeploy ApacheControl start

(Este es el primer tipo de sintaxis en la definición de funciones de control para un apche servidor)

Después de introducir el comando que el anterior, se realizan los siguientes pasos:

Paso 1: Do you want to start Apache? (Y/N).

El usuario tiene que especificar Y o N.

Paso 2: What is the apache service name?

(0) apache2

(1) httpd

El usuario debe especificar si 0 o 1 como por la exigencia.

Después de conseguir la entrada del nombre de servicio de apache, lo hará inicia el proceso.

La siguiente captura de pantalla muestra el proceso de inicio pictóricamente.

.. code-block:: bash

 kevell@corp:/# ptdeploy apachecontrol start
 Do you want to Start Apache? (Y/N)
 y
 What is the apache service name?
 (0) apache2
 (1) httpd
 0
 Starting Apache...
 * Starting web server apache2
 *
 ******************************


 1Apache Controller Finished
 ******************************

Función Stop
------------------

Si el usuario desea detener la función de control de apache, la puede usar las siguientes sintaxis como se muestra:

.. code-block:: bash

	ptdeploy apachecontrol stop --yes --guess

(Este es el segundo tipo de sintaxis en la definición de unas funciones de control de servidor apache)

La opción conjetura se puede utilizar para realizar un valores predeterminados de las funciones definidas en particular.

Para ubuntu la apche2 es el valor predeterminado.

Para httpd Cent OS es el valor predeterminado.

La siguiente captura de pantalla que muestra sobre la función de parada y el propósito de las opciones guess ilustrado.

.. code-block:: bash

 kevell@corp:/# ptdeploy apachecontrol stop --yes --guess
 Stopping Apache...
 * Stopping web server apache2
 *
 ******************************


 1Apache Controller Finished
 ******************************

Reinicie una función
-----------------------

Si el usuario desea reiniciar la función de control de apache, la puede usar las siguientes sintaxis como se muestra:

.. code-block:: bash
	
		ptdeploy apachecontrol restart --yes --apache-command="apache2"
	
(Este es el tercer tipo de sintaxis en la definición de unas funciones de control para apche servidor)

El usuario puede utilizar este tercer tipo de sintaxis para especificar el valor de la orden de Apache requeridos. La captura de pantalla como se muestra a continuación muestra este tercer tipo de sintaxis y proceso de reiniciar una función pictóricamente.

.. code-block:: bash

 kevell@corp:/# ptdeploy apachecontrol restart --yes --apache-command="apache2"
 Restarting Apache...
 AH00558: apache2: Could not reliably determine the server's fully qualified domain name, using 127.0.1.1. Set the 'ServerName' directive globa lly to suppress this message
 * Restarting web server apache2
 â€‚
  ....done.
 ******************************


 1Apache Controller Finished
 ******************************

Recarga de una función
----------------------------

Si el usuario desea volver a cargar la función de control de apache, la puede usar las siguientes sintaxis como se muestra:

.. code-block:: bash

	ptdeploy apachecontrol reload

or

.. code-block:: bash

	ptdeploy apachecontrol --yes --guess

or

.. code-block:: bash

	ptdeploy apachecontrol --yes --apache-command="apache2"


La función de recarga realiza la recarga del servidor apache sin necesidad de reiniciar.

Beneficios
-----------

* Es así que ver tanto en ciento-OS y ubuntu.
* Los parámetros utilizados para las declaraciones no distinguen entre mayúsculas y minúsculas, lo que es una ventaja añadida, mientras que en 
  comparación con otros.
* Hay tres sintaxis diferente utilizado para la declaración, el usuario puede elegir uno de ellos según las necesidades.
* La sintaxis tres diferentes son aplicables para las cuatro funciones de control de arranque, parada, reiniciar, volver a cargar.
