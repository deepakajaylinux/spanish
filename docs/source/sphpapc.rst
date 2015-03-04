=======
PHPAPC
=======

sinopsis
-------------

Este módulo tiene como objetivo instalar el PHP APC a la máquina de los usuarios de todas las maneras posibles.

APC es uno de los mecanismo de caché más popular para código de operación de almacenamiento en caché de PHP. Una vez activado, se inicia el almacenamiento en caché códigos PHP automáticamente. También funciona muy bien con W3 Total Cache plugin para almacenar objetos y MySQL cachés.

Los temas que serán las próximas guías su totalidad en todos los aspectos que intervienen en la instalación del PHP APC.

Ayuda Comando
---------------------

El comando help guía a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en el módulo PHP APC. En él se enumeran los parámetros alternativos de módulo PHP APC. También describe la sintaxis para instalar el módulo PHP APC. El comando de ayuda para el módulo PHP APC se muestra a continuación.

.. code-block:: bash
	
		ptconfigure PHPAPC help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda bajo PHP APC.

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPAPC help

 ******************************


  This command allows you to install some common and helpful PHP APC.

  PHPAPC, php-apc, phpapc, phpapc

        - install
        Install PHP APC.
        example: ptconfigure phpapc install

 ------------------------------
 End Help
 ******************************

instalación
----------------

El comando utilizado para instalar el PHP APC en la máquina de los usuarios se muestra a continuación:

.. code-block:: bash
	
		ptconfigure phpapc install

Después de introducir el comando anterior, el siguiente proceso se produce como se muestra en el formato tabular.

.. cssclass:: table-bordered
 
 +--------------------------+----------------------------------------------+-------------+----------------------------------------------+
 | Parámetros               | Parámetro Alternativa                        | Opciones    | Comentarios                                  |
 +==========================+==============================================+=============+==============================================+
 |Install PHP APC? (Y/N)    | En lugar de phpapc, podemos utilizar         | Y(Yes)      | Si el usuario desea continuar el proceso de  |
 |                          | PHPAPC, php-apc                              |             | instalación se puede introducir como Y.      |
 +--------------------------+----------------------------------------------+-------------+----------------------------------------------+
 |Install PHP APC? (Y/N)    | En lugar de phpapc, podemos utilizar         | N(No)       | Si el usuario desea abandonar el proceso de  |
 |                          | PHPAPC, php-apc                              |             | instalación se puede introducir como N.|     |
 +--------------------------+----------------------------------------------+-------------+----------------------------------------------+


Si el usuario procede de la instalación, durante el proceso de instalación se describe en las listas siguientes:

* Lee las listas de paquetes.
* Construye el árbol de dependencias.
* Lee la información de estado.
* Lista outs los paquetes que se instalan automáticamente.
* Lista outs el paquete adicional que está instalando.
* Lista outs los paquetes sugeridos.
* Lista outs los nuevos paquetes que está instalando.
* Los detalles sobre el número de archivos actualizados, recién instalados, retirados y no actualizados.

Finalmente, el proceso de instalación se completó. La siguiente captura de pantalla representar visualmente el proceso de instalación del PHP APC.

.. code-block:: bash

 kevell@corp:/# ptconfigure phpapc install

 Install PHP APC? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         PHP APC!        *
 *******************************
 E: Could not get lock /var/cache/apt/archives/lock - open (11: Resource temporarily unavailable)
 E: Unable to lock directory /var/cache/apt/archives/
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following packages were automatically installed and are no longer required:
  gyp libc-ares-dev libc-ares2 libjs-node-uuid libv8-3.14-dev
  linux-headers-3.13.0-32 linux-headers-3.13.0-32-generic
  linux-image-3.13.0-32-generic linux-image-extra-3.13.0-32-generic
  node-abbrev node-ansi node-archy node-async node-block-stream
  node-combined-stream node-cookie-jar node-delayed-stream node-forever-agent
  node-form-data node-fstream node-fstream-ignore node-github-url-from-git
  node-glob node-graceful-fs node-gyp node-inherits node-ini
  node-json-stringify-safe node-lockfile node-lru-cache node-mime
  node-minimatch node-mkdirp node-mute-stream node-node-uuid node-nopt
  node-normalize-package-data node-npmlog node-once node-osenv node-qs
  node-read node-read-package-json node-request node-retry node-rimraf
  node-semver node-sha node-sigmund node-slide node-tar node-tunnel-agent
  node-which nodejs nodejs-dev ttf-dejavu-core
 Use 'apt-get autoremove' to remove them.
 The following extra packages will be installed:
  php5-apcu
 The following packages will be REMOVED:
  php5-xcache
 The following NEW packages will be installed:
  php-apc php5-apcu
 0 upgraded, 2 newly installed, 1 to remove and 78 not upgraded.
 9 not fully installed or removed.
 [Pharaoh Logging] Adding Package php-apc from the Packager Apt did not execute correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PHPAPC: Success
 ------------------------------
 Installer Finished
 ******************************

Funciones de APC
---------------------

Esta sub temas se ocupa de las funciones más usadas bajo APC. Mientras trabajaba con Php APC el usuario puede hacer referencia a estas funciones de APC.

* Apc_add -cache una nueva variable en el almacén de datos
* Apc_bin_dump -Obtener una copia binaria de los archivos dados y variables de usuario
* Apc_bin_dumpfile -Salida una copia binaria de los archivos almacenados en caché y las variables de usuario en un archivo
* Apc_bin_load -load un volcado binario en la caché de archivos APC / usuario
* Apc_bin_loadfile -Carga un volcado binario de un archivo en la memoria caché de archivos APC / usuario
* Apc_cache_info -Retrieves información almacenada en caché del almacén de datos de APC
* Apc_cas -Actualizaciones un valor antiguo con un nuevo valor
* Apc_clear_cache -Clears la caché de APC
* Apc_compile_file -tiendas un archivo en la memoria caché de código de bytes, por encima de todos los filtros.
* Apc_dec -Disminución un número almacenado
* apc_define_constants: define un conjunto de constantes para la recuperación y la masa definición
* Apc_delete_file: elimina los archivos de la caché de código de operación
* Apc_delete: se toma una variable almacenada en el caché
* Apc_exists para comprobar que las clave existe APC
* Apc_fetch -Fetch una variable almacenada en la caché
* Apc_inc -Aumentar un número almacenado
* apc_load_constants -Loads un conjunto de constantes de la caché
* La información de asignación de memoria compartida de apc_sma_info -Retrieves APC
* Apc_store -cache una variable en el almacén de datos

Beneficios
-------------

* Los parámetros utilizados en la ayuda y la instalación no son sensibles, que es una ventaja añadida, mientras que en comparación con otros.
* Es-acomodados tanto en Ubuntu y así como Cent OS.
* Este módulo se instala el apc php en la versión actualizada.
* Si el módulo ya existe en la máquina del usuario, se mostrará un mensaje, ya que ya existe.
* APC viene con archivo llamado apc.php, que proporciona una sencilla interfaz basada en web.
