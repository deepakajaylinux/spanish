======
Jrush
======

sinopsis
------------

Este módulo ayuda en la instalación del jrush a su máquina. También facilita la actualización con una versión más reciente. Veamos cómo este Módulos asistencias en la instalación de un jrush.

Ayuda Comando
--------------------

El comando help guía a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en el módulo Jrush. En él se enumeran los parámetros alternativos de módulo Jrush. También describe la sintaxis para instalar el módulo Jrush. El comando de ayuda para el módulo Jrush se muestra a continuación.

.. code-block:: bash

		ptconfigure JRush help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda bajo JRush.

.. code-block:: bash

 kevell@corp:/# ptconfigure JRush help
 ******************************


  This command allows you to install or Update JRush.

  JRush, jrush, Jrush, jRush

        - install
        Installs the latest version of jRush
        example: ptconfigure jRush install

 ------------------------------
 End Help
 ******************************

instalación
----------------

El comando utilizado para instalar el JRush a la máquina de los usuarios se muestra a continuación.

.. code-block:: bash

		ptconfigure JRush install

Opciones
------------

Después de introducir el comando anterior, las siguientes operaciones se produce como se muestra en el formato tabular.

.. cssclass:: table-bordered

 +---------------------------+--------------------------------------+-------------+---------------------------------------------+
 | Parámetros                | Parámetro Alternativa                | Opciones    | Comentarios                                 |
 +===========================+======================================+=============+=============================================+
 |Install JRush - Joomla     | En lugar de JRush podemos utilizar:  | Y(Yes)      | Si el usuario desea continuar el proceso    |
 |Command Line ? (Y/N)       | jrush, Jrush, jRush                  |             | de instalación se puede introducir como Y.  |
 +---------------------------+--------------------------------------+-------------+---------------------------------------------+
 |Install JRush - Joomla     | En lugar de JRush podemos utilizar:  | N(No)       | Si el usuario desea abandonar el proceso    |
 |Command Line ? (Y/N)       | jrush, Jrush, jRush                  |             | de instalación se puede introducir como N|  |
 +---------------------------+--------------------------------------+-------------+---------------------------------------------+


Si el usuario continúa el proceso de instalación de las siguientes operaciones se produce como se muestra en el formato tabular.

.. cssclass:: table-bordered

 +------------------------+--------------------------------+-----------------+----------------------------------------------+
 | Parámetros             | camino                         | Opciones        | Comentarios                                  |
 +========================+================================+=================+==============================================+
 |Program data directory  | “/opt/jrush (módulo            | Yes             | Si el usuario de proceder con la instalación |
 |(Por defecto)           | correspondiente)               |                 | del directorio de datos de programa          |
 |                        |                                |                 | predeterminado que puede introducir como Sí  |
 +------------------------+--------------------------------+-----------------+----------------------------------------------+
 |Program data directory  | específico del usuario         | No (End Slash)  | Si el usuario desea continuar con su propio  |
 |                        |                                |                 | directorio de datos del programa, pueden de  |
 |                        |                                |                 | entrada como N, y en la mano especificar su  |
 |                        |                                |                 | propia ubicación                             |
 +------------------------+--------------------------------+-----------------+----------------------------------------------+
 |Program executor        | “/usr/bin”                     | Yes             | Si el usuario de proceder con la instalación |
 |directory (Por defecto) |                                |                 | del directorio ejecutor programa             |
 |                        |                                |                 | predeterminado que puede introducir como Sí  |
 +------------------------+--------------------------------+-----------------+----------------------------------------------+
 |Program executor        | específico del usuario         | No (End Slash)  | Si el usuario desea continuar con su propio  |
 |directory               |                                |                 | directorio ejecutor del programa, pueden de  |
 |                        |                                |                 | entrada como N, y en la mano especificar que |
 |                        |                                |                 | poseen ubicación.|                           |
 +------------------------+--------------------------------+-----------------+----------------------------------------------+


Durante la instalación, el siguiente proceso:

* Muestra el estado de la recepción de los objetos.
* Muestra el estado de la resolución de los deltas.
* Comprueba la conectividad.
* Se muestra como carpeta de datos de programa pobladas.
* Borra el ejecutor del programa, si ya existía.

Por último, se ha completado la instalación de Jrush. La siguiente captura de pantalla muestra el proceso de instalación del JRush a su máquina:

.. code-block:: bash

 kevell@corp:/# ptconfigure JRush install
 Install JRush - Joomla Command Line ? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         JRush CLI !!        *
 *******************************
 What is the program data directory? Found "/opt/jrush" - use this? (Enter nothing for yes, no end slash)
 
 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'https://github.com/PharaohTools/jrush.git'  /tmp/jrush/jrushCloning into '/tmp/jrush/jrush'...
 remote: Counting objects: 3452, done.
 remote: Total 3452 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (3452/3452), 2.04 MiB | 50.00 KiB/s, done.
 Resolving deltas: 100% (2097/2097), done.
 Checking connectivity... done.
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 JRush: Success
 ------------------------------
 Installer Finished
 ******************************

Beneficios
-------------

* Este módulo facilita al usuario en la instalación de JRush con la última versión.
* El usuario puede seleccionar su propio camino para el directorio de datos del programa y el directorio de albacea.
* Los parámetros utilizados en la declaración de la ayuda y las instalaciones no son sensibles, que se añade la ventaja, mientras que en 
  comparación con otros.
* Es-acomodados tanto en OS ciento y así como en ubuntu.
* El estado requiere se supervisan con claridad durante la instalación.
