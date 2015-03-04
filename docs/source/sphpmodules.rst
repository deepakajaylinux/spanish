===========
PHPModules
===========

sinopsis
-------------

Esto apunta a la instalación de los módulos y envolviendo algunos de los módulos de PHP comunes y útiles, de apoyo. Algunos ejemplos son: php5-gd el libs imagen, php5-imagick la libs imagen, php5-rizo el archivo remoto manejo libs, php5-mysql las librerías para el manejo de conexiones mysql. Veamos cómo utilizar este módulo, el proceso de instalación en los próximos temas.

Ayuda Comando
----------------------

El comando help guía a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en el módulo de PHP. En él se enumeran los parámetros alternativos de módulo PHP. También describe la sintaxis para instalar el módulo de PHP. El comando de ayuda para el módulo de PHP se muestra a continuación.

.. code-block:: bash
	
		ptconfigure PHPModules help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda bajo módulo PHP.

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPModules help

 ******************************


  This command allows you to install some common and helpful PHP Modules.

  PHPModules, php-mods, phpmods, php-modules, phpmodules

        - install
        Installs some common PHP Modules. These include php5-gd the image libs,
        php5-imagick the image libs, php5-curl the remote file handling libs,
        php5-mysql the libs for handling mysql connections.
        example: ptconfigure phpmods install

 ------------------------------
 End Help
 ******************************

Instalación
--------------

El comando que se utiliza para la instalación de los módulos de php en la máquina de los usuarios se muestra a continuación:

.. code-block:: bash

		ptconfigure phpmods install

Después de introducir el comando anterior, el siguiente proceso se produce como se muestra en el formato tabular.

.. cssclass:: table-bordered

 +---------------------------+--------------------------------------------+--------------+----------------------------------------------+
 | Parámetros                | Parámetro Alternativa                      | Opciones     | Comentarios                                  |
 +===========================+============================================+==============+==============================================+
 |Install PHP Modules? (Y/N) | En lugar de phpmods, podemos utilizar      | Y(Yes)       | Si el usuario desea continuar el proceso de  |
 |                           | PHPModules, php-mods, php-modules,         |              | instalación se puede introducir como Y.      |
 |                           | phpmodules también.                        |              |                                              |
 +---------------------------+--------------------------------------------+--------------+----------------------------------------------+
 |Install PHP Modules? (Y/N) | En lugar de phpmods, podemos utilizar      | N(No)        | Si el usuario desea abandonar el proceso de  | 
 |                           | PHPModules, php-mods, php-modules,         |              | instalación se puede introducir como N.      |
 |                           | phpmodules también.|                       |              |                                              |
 +---------------------------+--------------------------------------------+--------------+----------------------------------------------+


Si el usuario procede de la instalación, durante el proceso de instalación se describe en las listas siguientes:

* Construye el árbol de dependencias.
* Lee la información de estado.
* Lista outs los paquetes que se instalan automáticamente.
* Lista outs los nuevos paquetes que está instalando.
* Detalles sobre el número de archivos actualizados, recién instalados, retirados y no actualizados.

La siguiente captura de pantalla representa gráficamente el proceso anteriormente descrito de la instalación.

.. code-block:: bash


 kevell@corp:/# ptconfigure phpmods install
 
 Install PHP Modules? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         PHP Mods!        *
 *******************************
 E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
 [Pharaoh Logging] Adding Package php-apc from the Packager Apt did not execute correctly
 E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
 [Pharaoh Logging] Adding Package php5-gd from the Packager Apt did not execute correctly
 E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
 [Pharaoh Logging] Adding Package php5-imagick from the Packager Apt did not execute correctly
 E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
 [Pharaoh Logging] Adding Package php5-curl from the Packager Apt did not execute correctly
 E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
 [Pharaoh Logging] Adding Package php5-mysql from the Packager Apt did not execute correctly
 E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
 [Pharaoh Logging] Adding Package php5-memcache from the Packager Apt did not execute correctly
 E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
 [Pharaoh Logging] Adding Package php5-memcached from the Packager Apt did not execute correctly
 E: dpkg was interrupted, you must manually run 'sudo dpkg --configure -a' to correct the problem. 
 [Pharaoh Logging] Adding Package php5-mongo from the Packager Apt did not execute correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PHPModules: Success
 ------------------------------
 Installer Finished
 ******************************



Beneficios
--------------

* Los parámetros utilizados en la ayuda y la instalación no son sensibles, que es una ventaja añadida, mientras que en comparación con otros.
* Es-acomodados tanto en Ubuntu y así como Cent OS.
* Todos los módulos de la instalación de php utilizado con frecuencia se envolvió en un único proceso.
