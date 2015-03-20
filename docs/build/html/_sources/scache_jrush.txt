=========
Cache
=========


sinopsis
-----------------

Jrush auxiliar para vaciar caché en memoria temporal. Tiene dos tipos de memoria caché. Pero ambos tienen distintas funciones según lo especificado en su nombre. Son sitio claro y claro admin. Es gratificada con Ubuntu y ciento OS. Eliminar archivos, carpetas y aplicaciones y borrar los datos de la memoria temporal, no hará el truco si vas a reciclar el contenido no esté disponible en su computadora.

comando Ayuda
--------------------------

El comando de ayuda encarga de los usuarios con respecto a la determinación y así como sobre las opciones que están incluidas en la memoria caché. Enumera los parámetros alternativos de caché. También describe la sintaxis para el funcionamiento del módulo de Jrush. El comando de ayuda para la memoria caché se muestra a continuación.

.. code-block:: bash

	jrush cache help

Después de escribir el comando enumera las opciones de acción. La siguiente imagen concebirla observable.


.. code-block:: bash

 kevell@corp:/# jrush cache help
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

  This command allows you to clear Cache.

  Cache, cache

        - site-clear
        Deletes a user
        example: jrush cache site-clear

        - admin-clear
        Clear the administrator cache
        example: jrush cache admin-clear

 ------------------------------
 End Help
 ****************************************

 
parámetros alternativos
--------------------------------

Por otro lado utilizar caché el usuario puede conceder las siguientes opciones.


Cache, cache.

Opciones
-------------

Hay dos opciones están disponibles. Son los siguientes.


* Site-clear 
* Admin-clear

Ahora déjenos saber acerca de ambas opciones.


Site-clear
--------------

Sitio-claro es costoff para eliminar el usuario. El siguiente comando se utiliza para limpiar el sitio.


.. code-block:: bash

	jrush cache site-clear 

Después de insumos como sobre comando, la salida viene como una codificación. En la memoria caché de final claro acabado puede ser demostrado. Las capturas de pantalla se presenta el mismo.


.. code-block:: bash

 kevell@corp:/# jrush cache site-clear --config-file="/var/www/html/joomla/configuration.php" 
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 Joomla Cache Clearing Info:

 -------------------------

 Cache: array(2) {
  ["site_cache_clear"]=>
  string(19) "Site Cache Clearing"
  ["site_cache_clear_result"]=>
  array(0) {
  }
 }

 ------------------------------
 Joomla Cache Clearing Finished
 ****************************************

Admin-clear
-------------------

Esta desgastado Borrar caché del administrador. El comando de servicios al usuario para borrar el admin como sigue.


.. code-block:: bash

	jrush cache admin-clear

Las siguientes fotos de pantalla instruyan al usuario sobre la función admin-clear.


.. code-block:: bash

 kevell@corp:/# jrush cache admin-clear --config-file="/var/www/html/joomla/configuration.php" 
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 Joomla Cache Clearing Info:

 -------------------------

 Cache: array(2) {
  ["admin_cache_clear"]=>
  string(20) "Admin Cache Clearing"
  ["admin_cache_clear_result"]=>
  array(0) {
  }
 }

 ------------------------------
 Joomla Cache Clearing Finished
 ****************************************


Beneficios
---------------

* Es complaciente con esfuerzo con Ubuntu y ciento OS. 
* No minúsculas. 
* Lo seminuevo para eliminar el usuario. 
* Ayuda a clara admin.


