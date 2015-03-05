=================
Selenium Server
=================

sinopsis
-----------

 El selenio es un marco de pruebas de software portátil para aplicaciones web. El selenio proporciona una herramienta de grabación / reproducción para la edición de las pruebas sin tener que aprender un lenguaje de script de prueba (Selenio IDE). También proporciona un lenguaje de dominio específico de prueba (Selenese) [1] para escribir pruebas en varios lenguajes de programación, como Java, C #, Groovy, Perl, PHP, Python y Ruby. Las pruebas pueden ser ejecutadas en contra de la mayoría de los navegadores web modernos. El selenio se despliega en Windows, Linux y 
Macintosh

Veamos cómo este módulo facilita a los usuarios en la instalación de servidor de selenio.

Ayuda Comando
--------------------

El comando help guía a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en el módulo de servidor selenio. En él se enumeran los parámetros alternativos de módulo de servidor selenio. También describe la sintaxis para instalarlo. El comando de ayuda para el módulo de servidor de selenio se muestra a continuación.

.. code-block:: bash

	ptconfigure seleniumserver help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda bajo módulo de servidor selenio.

.. code-block:: bash

 kevell@corp:/# ptconfigure SeleniumServer help
 ******************************


  This command allows you to install Selenium Server.

  SeleniumServer, selenium-server, selenium, selenium-srv, seleniumserver

        - install
        Installs Selenium Server. Note, you'll also need Java installed
        as it is a prerequisite for Selenium
        example: ptconfigure selenium install
        example: ptconfigure selenium install --with-chrome-driver # will set the executor command to use default chrome driver


 ------------------------------
 End Help
 ******************************

instalación
----------------

El comando utilizado para instalar el servidor de selenio es sencillo como introducir el comando que se muestra a continuación.

.. code-block:: bash

		ptconfigure seleniumserver install

La captura de pantalla para el comando anterior se enumeran a continuación,

.. code-block:: bash

 kevell@corp:/# ptconfigure selenium install

 Install Selenium Server? (Y/N)
 y
 *******************************
 *        Pharaoh Tools        *
 *         Selenium Srv        *
 *******************************
 Enter Selenium Version
 (0) 2.39
 (1) 2.40
 (2) 2.41
 (3) 2.42
 (4) 2.43
 (5) 2.44
 5
 PHP Notice:  Undefined index: version in /opt/ptconfigure/ptconfigure/src/Modules/SeleniumServer/Model/SeleniumServerAllLinux.php on line 50
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Command 'git' found
 [Pharaoh Logging] Command 'gitk' found
 [Pharaoh Logging] Command 'git-cola' found
 [Pharaoh Logging] Not installing as already installed
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module Java reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 Creating /tmp/ptconfigure-temp-script-96670533394.sh
 chmod 755 /tmp/ptconfigure-temp-script-96670533394.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-96670533394.sh Permissions
 Executing /tmp/ptconfigure-temp-script-96670533394.sh
 --2015-02-12 15:31:34--  http://selenium-release.storage.googleapis.com//selenium-server-standalone-.0.jar
 Resolving selenium-release.storage.googleapis.com (selenium-release.storage.googleapis.com)... 74.125.236.43, 74.125.236.42, 74.125.236.44, ...
 Connecting to selenium-release.storage.googleapis.com (selenium-release.storage.googleapis.com)|74.125.236.43|:80... connected.
 HTTP request sent, awaiting response... 404 Not Found
 2015-02-12 15:31:35 ERROR 404: Not Found.
 
 mv: cannot stat €˜/tmp/selenium/*€™: No such file or directory
 mv: cannot stat €˜selenium-server-standalone-.0.jar€™: No such file or directory
 Temp File /tmp/ptconfigure-temp-script-96670533394.sh Removed
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************
 

 Single App Installer:
 --------------------------------------------
 SeleniumServer: Success
 ------------------------------
 Installer Finished
 ******************************

Opciones
------------

Después de introducir el comando anterior, las siguientes operaciones se produce como se muestra en el formato tabular.

.. cssclass:: table-bordered

 +------------------------+----------------------------------------------+---------------+----------------------------------------------+
 | Parámetros             | Parámetro Alternativa                        | Opciones      | Comentarios                                  |
 +========================+==============================================+===============+==============================================+
 |Install Selenium        | En lugar de seleniumserver, podemos utilizar | Y(Yes)        | Si el usuario desea continuar el proceso de  |
 |Server? (Y/N)           | SeleniumServer, Selenium, selenium-srv,      |               | instalación se puede introducir como Y.      |
 |                        | selenium-server también.                     |               |                                              |
 +------------------------+----------------------------------------------+---------------+----------------------------------------------+
 |Install Selenium        | En lugar de seleniumserver, podemos utilizar | N(No)         | Si el usuario desea abandonar el proceso de  |
 |Server? (Y/N)           | SeleniumServer, Selenium, selenium-srv,      |               | instalación se puede introducir como N.      |
 |                        | selenium-server también.|                    |               |                                              |
 +------------------------+----------------------------------------------+---------------+----------------------------------------------+


La siguiente captura de pantalla puede dar una representación pictórica sobre el proceso de instalación.

.. code-block:: bash


Beneficios
-------------

* Los parámetros utilizados en la ayuda y la instalación no son sensibles, que es una ventaja añadida, mientras que en comparación con otros.
* Es-acomodados tanto en Ubuntu y así como Cent OS.
* Puede desarrollar pruebas automatizadas en el lenguaje de programación de su elección como C #, Java, Python, PHP, Perl y Ruby, así como 
  aquellos que se ejecutan las pruebas sobre las diferentes combinaciones de navegadores como Chrome, Firefox o IE.
