==========
PHPCS
==========

sinopsis
-----------

Este módulo ayuda a la instalación de php cs de GC Repo. Durante la instalación, este módulo obtiene la última versión. El usuario puede especificar la ubicación para el directorio de datos del programa y el directorio de albacea. Finalmente resultados se presentan con claridad.

Ayuda Comando
--------------------

El comando de ayuda conduce a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en el módulo cs php. También describe la sintaxis para la instalación de php cs. El comando de ayuda para php cs es la siguiente.

.. code-block:: bash

	ptconfigure PHPCS help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda bajo PHPCS.

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPCS help
 ******************************


 This command allows you to install PHPCS from a GC Repo.

 PHPCS
 - install
 Installs the latest version of PHPCS
 example: ptconfigure phpcs install

 ------------------------------
 End Help
 ******************************

instalación
-------------

Instalación del PHP CS es más simple utilizando el siguiente comando como se muestra:

.. code-block:: bash
	
	ptconfigure PHPCS install

Después de introducir el comando anterior las siguientes operaciones como se muestra en el formato tabular ocurre.

.. cssclass:: table-bordered

 +--------------------------------+-----------+-------------------------------------------------------------------+
 | Parámetros                     | Opciones  | Comentarios                                                       |
 +================================+===========+===================================================================+
 |Install PHP Code Sniffer? (Y/N) | Y(Yes)    | Si el usuario desea continuar el proceso de instalación se        |
 |                                |           | puede introducir como Y.                                          |
 +--------------------------------+-----------+-------------------------------------------------------------------+
 |Install PHP Code Sniffer? (Y/N) | N(No)     | Si el usuario desea abandonar el proceso de instalación se puede  |
 |                                |           | introducir como N.|                                               |
 +--------------------------------+-----------+-------------------------------------------------------------------+


Si el usuario continúa el proceso de instalación de las siguientes operaciones se produce como se muestra en el formato tabular.

.. cssclass:: table-bordered


 +---------------------------+-------------------------------+---------------+----------------------------------------------------------+
 | Parámetros                | camino                        | Opciones      | Comentarios                                              |
 +===========================+===============================+===============+==========================================================+
 |Program data directory     | “/opt/pttest (módulo          | Y(Yes)        | Si el usuario proceder instalación con el directorio de  |
 |(Por defecto)              | correspondiente)”             |               | datos de programa predeterminado que puede introducir    |
 |                           |                               |               | como Sí                                                  |
 +---------------------------+-------------------------------+---------------+----------------------------------------------------------+
 |Program data directory     | específica de usuario         | N(Fin barra)  | Si el usuario desea continuar con su propio directorio   |
 |                           |                               |               | de datos del programa, pueden de entrada como N, y en la |
 |                           |                               |               | mano especificar que poseen ubicación.                   |
 +---------------------------+-------------------------------+---------------+----------------------------------------------------------+
 |Program executor directory | “/usr/bin”                    | Yes           | Si el usuario de proceder con la instalación del         |
 |(Por defecto)              |                               |               | directorio ejecutor programa predeterminado que puede    |
 |                           |                               |               | introducir como Sí                                       |
 +---------------------------+-------------------------------+---------------+----------------------------------------------------------+
 |Program executor directory | específica de usuario         | N(Fin barra)  | Si el usuario desea continuar con su propio directorio   |
 |                           |                               |               | ejecutor del programa, pueden de entrada como N, y en la |
 |                           |                               |               | mano especificar que poseen ubicación.|                  |
 +---------------------------+-------------------------------+---------------+----------------------------------------------------------+


Después de estos procesos tal como se muestra en el formato tabular, los resultados se informaron claramente junto con el estado. La siguiente captura de pantalla que explica gráficamente sobre el proceso para la instalación de PHPCS.

.. code-block:: bash

 Kevell@corp:/# ptconfigure PHPCS install
 Install PHP Code Sniffer ? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         PHP CSniffer        *
 *******************************
 What is the program data directory? Found "/opt/phpcs" - use this? (Enter nothing for yes, no end slash)
 
 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'https://github.com/phpengine/ptconfigure-phpcs.git'  /tmp/phpcs/phpcsCloning into '/tmp/phpcs/phpcs'...
 remote: Counting objects: 862, done.
 remote: Total 862 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (862/862), 491.23 KiB | 64.00 KiB/s, done.
 Resolving deltas: 100% (378/378), done.
 Checking connectivity... done.
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PHPCS: Success
 ------------------------------
 Installer Finished
 ****************************

Beneficios
------------

* Este módulo facilita al usuario en la instalación de PHP CS con la versión actualizada.
* El usuario puede seleccionar su propio camino para el directorio de datos del programa y ejecutor
* Los parámetros utilizados en la declaración de la ayuda y las instalaciones no son sensibles, que se añade la ventaja, mientras que en 
  comparación con otros.
