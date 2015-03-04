=========
PHPDox
=========

sinopsis
------------

Este módulo facilita a los usuarios en la instalación de la Php Dox con la última versión. phpdox es un generador de documentación para la generación de documentación de la API en formato HTML, por ejemplo, a partir del código fuente de PHP. Veamos cómo este módulo, ayuda en la instalación del Php Dox.

Ayuda Comando
---------------------

El comando help guía a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en el módulo Phpdox. En él se enumeran los parámetros alternativos de módulo Phpdox. También describe la sintaxis para instalar el módulo Phpdox. El comando de ayuda para el módulo Phpdox se muestra a continuación.

.. code-block:: bash
	
		ptconfigure Phpdox help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda bajo Phpdox.

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPDox help

 ******************************

 This command allows you to update PHPDox.

 PHPDox, phpdox

  - install
  Installs the latest version of Docker
 example: ptconfigure phpdox install

 ------------------------------
 End Help
 ******************************

instalación
----------------

El comando utilizado para instalar el phpdox en la máquina de los usuarios se muestra a continuación:

.. code-block:: bash

		ptconfigure phpdox install

Después de introducir el comando anterior, el siguiente proceso se produce como se muestra en el formato tabular.

.. cssclass:: table-bordered

 +-----------------------+------------------------------------------+-------------+-----------------------------------------------+
 | Parámetros            | Parámetro Alternativa                    | Opciones    | Comentarios                                   |
 +=======================+==========================================+=============+===============================================+
 |Install PHPDox? (Y/N)  | En lugar de phpdox, podemos utilizar     | Y(Yes)      | Si el usuario desea continuar el proceso      |
 |                       | PHPDox también.                          |             | de instalación se puede introducir como Y.    |
 +-----------------------+------------------------------------------+-------------+-----------------------------------------------+
 |Install PHPDox? (Y/N)  | En lugar de phpdox, podemos utilizar     | N(No)       | Si el usuario desea abandonar el proceso      |
 |                       | PHPDox también.                          |             | de instalación se puede introducir como N.|   |
 +-----------------------+------------------------------------------+-------------+-----------------------------------------------+

Si el usuario procede de la instalación, el proceso de instalación se parece a la captura de pantalla se indica a continuación:

.. code-block:: bash

 kevell@corp:/# ptconfigure phpdox install

 Install PHPDox? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         PHPDox!        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-27804177792.sh
 chmod 755 /tmp/ptconfigure-temp-script-27804177792.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-27804177792.sh Permissions
 Executing /tmp/ptconfigure-temp-script-27804177792.sh
 --2015-01-28 15:42:36--  http://phpdox.de/releases/phpdox.phar
 Resolving phpdox.de (phpdox.de)... 188.94.27.6
 Connecting to phpdox.de (phpdox.de)|188.94.27.6|:80... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: 801185 (782K) [application/phar]
 Saving to: Ã¢‚¬Ëœphpdox.pharÃ¢‚¬„¢

 100%[=======================================================================================================>] 8,01,185    11.7KB/s   in 2m 9s  

 2015-01-28 15:44:47 (6.08 KB/s) - Ã¢‚¬Ëœphpdox.pharÃ¢‚¬„¢ saved [801185/801185]
 
 PHP Warning:  PHP Startup: Unable to load dynamic library '/usr/lib/php5/20121212/mcrypt.so' - /usr/lib/php5/20121212/mcrypt.so: cannot open 
 shared object file: No such file or directory in Unknown on line 0
 Sorry, but your PHP environment is currently not able to run phpDox due to
 the following issue(s):

 ext/xsl not installed/enabled

 Please adjust your PHP configuration and try again.



 Oups... phpDox encountered a problem and has terminated!

 It most likely means you've found a bug, so please file a report for this
 and paste the following details and the stacktrace (if given) along:

 PHP Version: 5.5.9-1ubuntu4.5 (Linux)
 PHPDox Version: 0.7.0
 ErrorException: E_CORE_WARNING 
 Location: Unknown (Line 0)
 
 PHP Startup: Unable to load dynamic library '/usr/lib/php5/20121212/mcrypt.so' - /usr/lib/php5/20121212/mcrypt.so: cannot open shared object 
 file: No such file or directory

 No stacktrace available
 

 phpDox 0.7.0 - Copyright (C) 2010 - 2015 by Arne Blankerts

 Temp File /tmp/ptconfigure-temp-script-27804177792.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PHPDox: Success
 ------------------------------
 Installer Finished
 ******************************

Beneficios
-----------

* Los parámetros utilizados en la ayuda y la instalación no son sensibles, que es una ventaja añadida, mientras que en comparación con otros.
* Es-acomodados tanto en Ubuntu y así como Cent OS.
* Este módulo se instala el phpdox en versión actualizada.
* Si el módulo ya existe en la máquina del usuario, se mostrará un mensaje, ya que ya existe.
