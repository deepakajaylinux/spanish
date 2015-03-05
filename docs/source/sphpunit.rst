==========
PHPUnit
==========

sinopsis
--------------

Este módulo facilita a los usuarios para instalar PHPUnit de un GC Repo. PHP Unidad Testing Framework es un marco de unidad de pruebas que permite a los desarrolladores de descubrir los errores y, a su vez reducir los costos asociados con el desarrollo de software PHP. El Marco de pruebas Unidad de PHP genera informes, ya sea en XML, XHTML o ASCII. Veamos, ¿cómo funciona este módulo nos ayuda en la instalación de una unidad de PHP.

Ayuda Comando
--------------------

El comando de ayuda conduce a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en el módulo de unidad de PHP. También describe la sintaxis para la instalación de la unidad de PHP. El comando de ayuda para el módulo de unidad de PHP se muestra a continuación.

.. code-block:: bash

		ptconfigure PHPUnit help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda debajo de la unidad de PHP.

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPUnit help
 ******************************

  This command allows you to install PHPUnit from a GC Repo.

  PHPUnit

        - install
        Installs the latest GC Repo version of PHPUnit
        example: ptconfigure phpunit install

 ------------------------------
 End Help
 ******************************

instalación
---------------

El comando que se utiliza para la instalación de la unidad de PHP a la máquina de los usuarios se muestra a continuación.

.. code-block:: bash

		ptconfigure PHPUnit install

Después de introducir el comando anterior, las siguientes operaciones se produce como se muestra en el formato tabular.

.. cssclass:: table-bordered


 +-------------------------+------------------+---------------------------------------------------------------------------------------+
 | Parámetros              | Opciones         | Comentarios                                                                           |
 +=========================+==================+=======================================================================================+
 |Install PHP Unit? (Y/N)  | Y(Yes)           | Si el usuario desea continuar el proceso de instalación se puede introducir como Y.   |
 +-------------------------+------------------+---------------------------------------------------------------------------------------+
 |Install PHP Unit? (Y/N)  | N(No)            | Si el usuario desea abandonar el proceso de instalación se puede introducir como N.|  |
 +-------------------------+------------------+---------------------------------------------------------------------------------------+


Si el usuario continúa el proceso de instalación de las siguientes operaciones se produce como se muestra en el formato tabular.

.. cssclass:: table-bordered

 +-----------------------+------------------------------+-----------+------------------------------------------------------------------+
 | Parámetros            | camino                       | Opciones  | Comentarios                                                      |
 +=======================+==============================+===========+==================================================================+
 |Program data directory | “/opt/phpunit (módulo        | Y(Yes)    | Si el usuario de proceder con la instalación del directorio de   | 
 |(Por defecto)          | correspondiente)”            |           | datos de programa predeterminado que puede introducir como Sí    |
 +-----------------------+------------------------------+-----------+------------------------------------------------------------------+
 |Program data directory | específica de usuario        | N(Fin     | Si el usuario desea continuar con su propio directorio de datos  |
 |                       |                              | barra)    | del programa, pueden de entrada como N, y en la mano especificar |
 |                       |                              |           | que poseen ubicación.                                            |
 +-----------------------+------------------------------+-----------+------------------------------------------------------------------+
 |Program executor       | “/usr/bin”                   | Yes       | Si el usuario de proceder con la instalación del directorio      |
 |directory              |                              |           | ejecutor programa predeterminado que puede introducir como Sí    |
 |(Por defecto)          |                              |           |                                                                  |
 +-----------------------+------------------------------+-----------+------------------------------------------------------------------+
 |Program executor       | específica de usuario        | N(Fin     | Si el usuario desea continuar con su propio directorio ejecutor  | 
 |directory              |                              | barra)    | del programa, pueden de entrada como N, y en la mano especificar |
 |                       |                              |           | que poseen ubicación.|                                           |
 +-----------------------+------------------------------+-----------+------------------------------------------------------------------+


Por último, se ha completado la instalación de la unidad de PHP. La siguiente captura de pantalla muestra visualmente sobre el proceso de instalación.

.. code-block:: bash

 kevell@corp:/# ptconfigure phpunit install
 Install PHP Unit ? (Y/N)
 Y
 *******************************
 *        Pharaoh Tools        *
 *          PHP Unit !         *
 *******************************
 What is the program data directory? Found "/opt/phpunit" - use this? (Enter nothing for yes, no end slash)

 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone -b 3.5 'https://github.com/sebastianbergmann/phpunit.git'  /tmp/phpunit/phpunitCloning into '/tmp/phpunit/phpunit'...

 remote: Counting objects: 50529, done.
 Receiving objects:  71% (35876/50529), 12.02 MiB | 41.00 KiB/s
 Receiving objects:  95% (48003/50529), 16.82 MiB | 38.00 KiB/s
 Receiving objects:  95% (48254/50529), 16.86 MiB | 40.00 KiB/s
 Receiving objects:  96% (48508/50529), 16.95 MiB | 43.00 KiB/s



 remote: Total 50529 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (50529/50529), 17.91 MiB | 36.00 KiB/s, done.
 Resolving deltas: 100% (26834/26834), done.
 Checking connectivity... done.
 git clone -b 1.0 'https://github.com/sebastianbergmann/dbunit.git'  /tmp/phpunit/dbunitCloning into '/tmp/phpunit/dbunit'...
 remote: Counting objects: 4596, done.
 remote: Total 4596 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (4596/4596), 1.04 MiB | 31.00 KiB/s, done.
 Resolving deltas: 100% (3183/3183), done.
 Checking connectivity... done.
 git clone -b 1.2 'https://github.com/sebastianbergmann/php-file-iterator.git'  /tmp/phpunit/php-file-iteratorCloning into '/tmp/phpunit/php-file-iterator'...
 remote: Counting objects: 453, done.
 remote: Total 453 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (453/453), 60.66 KiB | 16.00 KiB/s, done.
 Resolving deltas: 100% (188/188), done.
 Checking connectivity... done.
 git clone -b 1.0 'https://github.com/sebastianbergmann/php-code-coverage.git'  /tmp/phpunit/php-code-coverageCloning into '/tmp/phpunit/php-code-coverage'...
 remote: Counting objects: 7650, done.
 remote: Total 7650 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (7650/7650), 2.77 MiB | 17.00 KiB/s, done.
 Resolving deltas: 100% (3671/3671), done.
 Checking connectivity... done.
 git clone -b 1.0 'https://github.com/sebastianbergmann/php-token-stream.git'  /tmp/phpunit/php-token-streamCloning into '/tmp/phpunit/php-token-stream'...
 remote: Counting objects: 1234, done.
 remote: Total 1234 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (1234/1234), 201.76 KiB | 41.00 KiB/s, done.
 Resolving deltas: 100% (565/565), done.
 Checking connectivity... done.
 git clone -b 1.0 'https://github.com/sebastianbergmann/phpunit-mock-objects.git'  /tmp/phpunit/phpunit-mock-objectsCloning into '/tmp/phpunit/phpunit-mock-objects'...
 remote: Counting objects: 4703, done.
 remote: Total 4703 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (4703/4703), 837.24 KiB | 104.00 KiB/s, done.
 Resolving deltas: 100% (2910/2910), done.
 Checking connectivity... done.
 git clone -b 1.0 'https://github.com/sebastianbergmann/phpunit-selenium.git'  /tmp/phpunit/phpunit-seleniumCloning into '/tmp/phpunit/phpunit-selenium'...
 remote: Counting objects: 8115, done.
 remote: Total 8115 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (8115/8115), 2.07 MiB | 28.00 KiB/s, done.
 Resolving deltas: 100% (4762/4762), done.
 Checking connectivity... done.
 git clone 'https://github.com/phpengine/ptconfigure-phpunit-php-timer'  /tmp/phpunit/php-timerCloning into '/tmp/phpunit/php-timer'...
 remote: Counting objects: 253, done.
 remote: Total 253 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (253/253), 31.55 KiB | 12.00 KiB/s, done.
 Resolving deltas: 100% (126/126), done.
 Checking connectivity... done.
 git clone 'https://github.com/sebastianbergmann/php-text-template.git'  /tmp/phpunit/php-text-templateCloning into '/tmp/phpunit/php-text-template'...
 remote: Counting objects: 209, done.
 remote: Total 209 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (209/209), 33.69 KiB | 16.00 KiB/s, done.
 Resolving deltas: 100% (92/92), done.
 Checking connectivity... done.
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PHPUnit35: Success
 ------------------------------
 Installer Finished
 ******************************

Beneficios
--------------

* Este módulo facilita al usuario en la instalación de la Unidad de PHP desde la versión GC Repo.
* El usuario puede seleccionar su propio camino para el directorio de datos del programa y ejecutor
* Los parámetros utilizados en la declaración de la ayuda y las instalaciones no son sensibles, que se añade la ventaja, mientras que en 
  comparación con otros.
* Es-acomodados tanto en OS ciento y así como en ubuntu.
