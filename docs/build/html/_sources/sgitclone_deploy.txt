==========
GitClone
==========

sinopsis
------------

El objetivo final de este módulo es para manejar el registro de salida funciones. Se puede realizar la comprobación de las funciones en la carpeta del proyecto de la usuario.

La naturaleza de trabajo de este módulo consiste en clonar un repositorio en un directorio recién creado, crea ramas de rastreo remoto para cada rama en el repositorio clonado y crea, comprueba a cabo una rama inicial que se bifurcaba de rama actualmente activo del repositorio clonado.

Veamos cómo este módulo facilita a los usuarios en el manejo de la comprobación de las funciones, y también acerca de cómo utilizar este módulo de los próximos temas.


Ayuda Comando
-------------------

El comando de ayuda es un breve manual de usuario. Se destaca la función principal de este módulo, se enumeran las salidas de los parámetros alternativos que se pueden utilizar en la declaración, y también explica acerca de las opciones de sintaxis y posibles de utilizar la comprobación de las funciones previstas en una opción única mediante el uso de comando de ayuda, como se muestra a continuación,

.. code-block:: bash

		ptdeploy GitClone help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda bajo git clone.

.. code-block:: bash

 kevell@corp:/# ptdeploy GitClone help
 ******************************


  This command is part of Default Modules and handles Checkout Functions.

  clone, co

          - perform a checkout into configured projects folder. If you don't want to specify target dir but do want
          to specify a branch, then enter the text "none" as that parameter.
          example: ptdeploy git co https://github.com/phpengine/yourmum {optional target dir} {optional branch}
          example: ptdeploy git co https://github.com/phpengine/yourmum none {optional branch}

 ------------------------------
 End Help
 ******************************

Cómo utilizar las funciones de pago y envío
-------------------------------------------

La sintaxis para utilizar el cheque las funciones previstas en git clone es la siguiente.

.. code-block:: bash

	ptdeploy git co https: // github.com/ phpengine/yourmum

Después de entrar en la orden dada anteriormente, la ejecución de la función de pago comienza como se describe en la siguiente tabla,

.. cssclass:: table-bordered

 +-------------------------+--------------------------------------+------------+-------------------------------------------------------+
 | Parámetros              | Parámetro Alternativa                | Opciones   | Comentarios                                           |
 +=========================+======================================+============+=======================================================+
 |Perform a clone/download | En lugar de co, podemos utilizar     | Y(Yes)     | Si el usuario necesita para llevar a cabo un clon /   |
 |of files? (Y/N)          | checkout, Checkout también.          |            | descarga de los archivos se puede introducir como Y.  |
 +-------------------------+--------------------------------------+------------+-------------------------------------------------------+
 |Perform a clone/download | En lugar de co, podemos utilizar     | N(No)      | Si el usuario no se necesita realizar un clon /       |
 |of files? (Y/N)          | checkout, Checkout también.          |            | descarga de archivos que pueden como N.|              |
 +-------------------------+--------------------------------------+------------+-------------------------------------------------------+


La siguiente captura de pantalla muestra gráficamente sobre el proceso y el trabajo de comprobar a cabo funciones.

.. code-block:: bash

Beneficios
-----------

* Es-acomodados tanto en ubuntu y al igual que en ciento OS.
* Los parámetros utilizados en la declaración no distingue entre mayúsculas y minúsculas.
* El usuario puede realizar y supervisar las funciones de comprobación en virtud git clone.
* Mientras se realiza la comprobación de las funciones, el usuario puede especificar el directorio de destino, es necesario especificar la rama.
