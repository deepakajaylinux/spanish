=======
Behat 
=======

sinopsis
----------

Este módulo tiene como objetivo instalar Behat con la versión más reciente. Esto ayuda en la prueba de un script php. Facilita a los usuarios a identificar los errores en script php. En él se destacan las plantillas habilitadas y discapacitados. El git actúa como un software de soporte para Behat.

Ayuda Comando
----------------------

Las guías de comandos ayuda al usuario obtener conocimiento de los usos, y también las opciones y acciones que se pueden realizar. En él se enumeran las salidas de parámetros alternativos que se pueden utilizar en la declaración. Especifica el comando para instalar la última versión de Behat.

La codificación para hacer uso de la ayuda de mandatos bajo Behat, se da como sigue:

.. code-block:: bash

		cleopatra behat help

La captura de pantalla tal como se indica a continuación que explica gráficamente sobre el uso del comando de ayuda.

.. code-block:: bash

 kevell@corp:/# cleopatra behat help
 ******************************


  This command allows you to install Behat.

  Behat, behat

        - install
        Installs the latest version of behat
        example: cleopatra behat install

 ------------------------------
 End Help
 ******************************

instalación
--------------------

Si el usuario necesita para instalar la última versión de Behat, pueden lograr la instalación, mediante el comando siguiente,

.. code-block:: bash

	cleopatra behat install

Después de introducir el comando anterior, el siguiente proceso están involucrados en la instalación como se muestra en el formato tabular,

.. cssclass:: table-bordered


 +---------------------------+-----------------------------------+---------------+------------------------------------------+
 | Parámetros                | parámetros alternativos           | Necesario     | Comentario                               |
 +===========================+===================================+===============+==========================================+
 |Install Behat? (Y/N)       | En lugar de behat, podemos        | Y(Yes)        | Si el usuario da entrada como sí, se     |
 |                           | utilizar Behat también            |               | va a proceder la instalación.            |
 +---------------------------+-----------------------------------+---------------+------------------------------------------+
 |Install Behat? (Y/N)       | En lugar de behat, podemos        | N(No)         | Si el usuario da entrada como no, que se |
 |                           | utilizar Behat también            |               | cerrará el proceso de instalación|       |
 +---------------------------+-----------------------------------+---------------+------------------------------------------+


Si el usuario continúa la instalación introduciendo como Y, los siguientes pasos son involucrados en la instalación de Behat,


.. cssclass:: table-bordered


 +-------------------------+--------------------------------+------------+--------------------------------------------------+
 | Parámetros              | camino                         | opción     | comentario                                       |
 +=========================+================================+============+==================================================+
 |Program data             | “/opt/behat”                   | Yes        | Si el usuario de proceder con la instalación del |
 |directory (defecto)      |                                |            | directorio de datos de programa predeterminado   |
 |                         |                                |            | que puede introducir como Sí                     |
 +-------------------------+--------------------------------+------------+--------------------------------------------------+
 |Program data directory   | específico del usuario         | No (Fin de | Si el usuario desea continuar con su propio      |
 |                         |                                | Slash)     | directorio de datos del programa, pueden de      |
 |                         |                                |            | entrada como N, y en la mano especificar que     |
 |                         |                                |            | poseen ubicación                                 |
 +-------------------------+--------------------------------+------------+--------------------------------------------------+
 |Program executor         | “/usr/bin”                     | Yes        | Si el usuario de proceder con la instalación del |
 |directory (defecto)      |                                |            | directorio ejecutor programa predeterminado que  |
 |                         |                                |            | puede introducir como sí                         |
 +-------------------------+--------------------------------+------------+--------------------------------------------------+
 |Program executor         | específico del usuario         | No (Fin de | Si el usuario desea continuar con la instalación |      
 |directory                |                                | Slash)     | directorio ejecutor programa propio thir, se     |
 |                         |                                |            | puede introducir como N, y en la mano            |
 |                         |                                |            | especificar que poseen ubicación|                |
 +-------------------------+--------------------------------+------------+--------------------------------------------------+

La captura de pantalla muestra a continuación voluntad le da una representación gráfica de los pasos involucrados en la instalación.

.. code-block:: bash

 kevell@corp:/# cleopatra behat install
 Install Behat ? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *          Behat         *
 *******************************
 What is the program data directory? Found "/opt/behat" - use this? (Enter nothing for yes, no end slash)
 
 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 Creating /tmp/cleopatra-temp-script-69243074239.sh
 chmod 755 /tmp/cleopatra-temp-script-69243074239.sh 2>/dev/null
 Changing /tmp/cleopatra-temp-script-69243074239.sh Permissions
 Executing /tmp/cleopatra-temp-script-69243074239.sh
 --2015-01-27 15:31:39--  https://getcomposer.org/installer
 Resolving getcomposer.org (getcomposer.org)... 87.98.253.108
 Connecting to getcomposer.org (getcomposer.org)|87.98.253.108|:443... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: unspecified [text/plain]
 Saving to: ‘installer’

    [              <=>                                                                                     ] 2,74,634    48.9KB/s   in 5.5s   

 2015-01-27 15:31:47 (48.9 KB/s) - ‘installer’ saved [274634]

 All settings correct for using Composer
 Downloading...

 Composer successfully installed to: /opt/behat/behat/composer.phar


Durante la instalación del Behat, el usuario puede especificar el directorio de datos del programa y el directorio ejecutor del programa.

La imagen anterior explica la sintaxis en cuanto a la especificación del directorio de datos del programa y el directorio de albacea.

versión
---------

Durante la instalación del Behat, la versión más reciente-será instalado en su máquina.

Esto es una ventaja añadida de módulo de Behat bajo Cleopatra en comparación con otros.

Beneficios
--------------

* Se guía a los usuarios a identificar los errores en script php.
* No hay necesidad de buscar la versión más reciente, como la versión actualizada está disponible automáticamente para los usuarios durante la 
  ejecución de la instalación pr oceso.
* El uso de las características de Behat los usuarios pueden enmarcar y especificar el comportamiento del desarrollo impulsado.
* Con la ayuda de comportamiento impulsado el desarrollo, los usuarios pueden asegurar las cualidades de su propio guión.
* Es-acomodada en CentOS y así como en ubuntu.
* Los parámetros utilizados en la declaración no se distingue entre mayúsculas y minúsculas, lo que es una ventaja añadida.
