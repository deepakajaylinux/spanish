==========
Memcached
==========

sinopsis
---------------

El aspecto principal de este módulo es instalar y actualizar el memcache con la última versión.

Memcached es un sistema de almacenamiento en caché de memoria distribuida de propósito general. A menudo se utiliza para acelerar sitios web dinámicos con bases de datos de almacenamiento en caché de datos y objetos en la memoria RAM para reducir el número de veces que una fuente de datos externa (como una base de datos o API) debe ser leído.

Veamos sobre el proceso de instalar y utilizar este módulo en los próximos temas.

Ayuda Comando
---------------------

El comando help guía a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en el módulo Memcached. En él se enumeran los parámetros alternativos de módulo Memcached. También describe la sintaxis para instalar el módulo de Memcached. El comando de ayuda para el módulo de Memcached es como se muestra.

.. code-block:: bash

		ptconfigure Memcached help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda bajo Memcached.

.. code-block:: bash

 kevell@corp:/# ptconfigure Memcached help

 ******************************


  This command allows you to update Memcached.

  Memcached, memcached

        - install
        Installs the latest version of memcache
        example: ptconfigure memcached install

 ------------------------------
 End Help
 ******************************

instalación
----------------

El comando utilizado para instalar el Memcached en la máquina de los usuarios se muestra a continuación:

.. code-block:: bash

	ptconfigure memcached install

Después de introducir el comando anterior, el siguiente proceso se produce como se muestra en el formato tabular.

.. cssclass:: table-bordered

 +--------------------------+--------------------------------------------+--------------+---------------------------------------------+
 | Parámetros               | Parámetro Alternativa                      | Opciones     | Comentarios                                 |
 +==========================+============================================+==============+=============================================+
 |Install Memcached? (Y/N)  | En lugar de memcached, podemos usar        | Y(Yes)       | Si el usuario desea continuar el proceso    |
 |                          | Memcached también.                         |              | de instalación se puede introducir como Y.  |
 +--------------------------+--------------------------------------------+--------------+---------------------------------------------+
 |Install Memcached? (Y/N)  | En lugar de memcached, podemos usar        | N(No)        | Si el usuario desea abandonar el proceso    |
 |                          | Memcached también.                         |              | de instalación se puede introducir como N.| |
 +--------------------------+--------------------------------------------+--------------+---------------------------------------------+

La siguiente captura de pantalla puede darle una representación pictórica sobre el proceso de instalación.

.. code-block:: bash

Funciones de memcached
-------------------------------

Durante el uso de la memcached, el proceso puede leer y poner en práctica las siguientes funciones que se incluyen en memcached,

* Memcache :: añadir --add un elemento para el servidor
* Memcache :: addServer --add un servidor memcached al pool de conexiones
* Memcache :: close --Close conexión de servidor memcached
* Memcache :: connect --open conexión de servidor memcached
* Valor Memcache :: decremento del artículo --Decrement
* Memcache :: suprimir el punto --delete del servidor
* Memcache :: vaciar --flush todos los elementos existentes en el servidor
* Memcache :: get artículo --retrieve del servidor
* Memcache :: getExtendedStats --get estadísticas de todos los servidores en la piscina
* Memcache :: estado del servidor GetServerStatus --Returns
* Memcache :: getStats --get estadísticas del servidor
* Memcache :: getVersion --Vuelva la versión del servidor
* Valor Memcache :: incremento --Increment el objeto:
* Conexión persistente Memcache :: pconnect --open servidor memcached
* Memcache :: replace valor --replace del elemento existente
* Memcache :: set de datos --Store en el servidor
* Memcache :: setCompressThreshold compresión --enable automática de los valores grandes
* Parámetros Memcache :: setServerParams --Changes servidor y el estado en tiempo de ejecución


Beneficios
------------

* Los parámetros utilizados en la ayuda y la instalación no son sensibles, que es una ventaja añadida, mientras que en comparación con otros.
* Es-acomodados tanto en Ubuntu y así como Cent OS.
* Este módulo se instala el memcached en versión actualizada.
* Si el módulo ya existe en la máquina del usuario, se mostrará un mensaje, ya que ya existe.

