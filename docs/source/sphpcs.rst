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

        - uninstall 
        Uninstalls the latest version of PHPCS 
        example: ptconfigure phpcs uninstall 

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



Después de estos procesos tal como se muestra en el formato tabular , los resultados se informaron claramente junto con el estado . La siguiente captura de pantalla que explica gráficamente sobre el proceso involucrado en la instalación y desinstalación de PHPCS .

.. code-block:: bash


 kevell@corp:/# ptconfigure PHPCS install 
 Install PHP Code Sniffer? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         PHP CSniffer        * 
 ******************************* 
 Creating /tmp/ptconfigure-temp-script-74085209498.sh 
 chmod 755 /tmp/ptconfigure-temp-script-74085209498.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-74085209498.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-74085209498.sh 
 Reading package lists... 
 Building dependency tree... 
 Reading state information... 
 php-pear is already the newest version. 
 0 upgraded, 0 newly installed, 0 to remove and 3 not upgraded. 
 downloading PHP_CodeSniffer-2.3.0.tgz ... 
 Starting to download PHP_CodeSniffer-2.3.0.tgz (464,453 bytes) 
 .............................................................................................done: 464,453 bytes 
 install ok: channel://pear.php.net/PHP_CodeSniffer-2.3.0 
 Temp File /tmp/ptconfigure-temp-script-74085209498.sh Removed 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 


 Single App Installer: 
 -------------------------------------------- 
 PHPCS: Success 
 ------------------------------ 
 Installer Finished 
 ****************************** 


.. code-block:: bash


 kevell@corp:/# ptconfigure PHPCS uninstall 
 Uninstall PHP Code Sniffer? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         PHP CSniffer        * 
 ******************************* 
 Creating /tmp/ptconfigure-temp-script-50071430908.sh 
 chmod 755 /tmp/ptconfigure-temp-script-50071430908.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-50071430908.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-50071430908.sh 
 uninstall ok: channel://pear.php.net/PHP_CodeSniffer-2.3.0 
 Temp File /tmp/ptconfigure-temp-script-50071430908.sh Removed 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 


 Single App Uninstaller: 
 ------------------------------ 
 PHPCS: Success 
 ------------------------------ 
 Installer Finished 
 ******************************  



Beneficios
------------

* Este módulo facilita al usuario en la instalación de PHP CS con la versión actualizada.
* El usuario puede seleccionar su propio camino para el directorio de datos del programa y ejecutor
* Los parámetros utilizados en la declaración de la ayuda y las instalaciones no son sensibles, que se añade la ventaja, mientras que en 
  comparación con otros.
