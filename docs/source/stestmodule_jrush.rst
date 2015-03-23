=============
Test module
=============

sinopsis
--------------

Testmodule es el jrush más popular pruebas de módulo, a partir de esta revisión sobre la extensión de archivo y hacen uso de ella. Testmodule es un marco pero puede ser utilizado en conjunto con otro artículo de prueba. Como resultado, TestModule proporciona sólo la línea de base pruebas funciones dejando otras bibliotecas para implementar la funcionalidad más específica y sofisticada. Muestra las actuales acciones. Esto es cómodo con Ubuntu y centOS.


comando Ayuda
-----------------------

El comando ayuda guía a los usuarios sobre la finalidad y así como sobre las opciones que están incluidas en el testmodule. Enumera los parámetros alternativos de testmodule. También describe la sintaxis para el funcionamiento del módulo de Jrush. El comando de ayuda para testmodule se muestra a continuación.


.. code-block:: bash

	jrush testmodules help

Después de escribir el comando enumera las opciones de acción. La siguiente imagen visualizarlo obviamente.



.. code-block:: bash

 kevell@corp:/# jrush TestModule help
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

  This command allows you to update TestModule.

  TestModule, testmodule, test-module

        - action-one
        An example action. Currently, we get all titles of articles
        example: jrush test-module action-one

        - action-two
        An example action. Currently, we get all titles of articles
        example: jrush test-module action-two

 ------------------------------
 End Help
 ****************************************



parámetros alternativos
--------------------------------

Alternativamente usando Testmodule el usuario puede utilizar las siguientes opciones.


Test Module, testmodule, test-module.

Opciones
-------------

Hay dos opciones están disponibles. Son los siguientes.

* Action-one
* Action-two

Action-one
-----------------

Muestra los actuales títulos de artículos. El comando utilizado para hacer una acción es como sigue:


.. code-block:: bash

	jrush test-module action-one

Después da el comando muestra los detalles del actual y títulos de los artículos. La imagen representa el mismo.



.. code-block:: bash

 kevell@corp:/# jrush test-module action-one --config-file="/var/www/html/joomla/configuration.php"
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 TestModule Action One:
 -------------------------
 array(6) {
  [0]=>
  string(8) "About Us"
  [1]=>
  string(15) "Article 1 Title"
  [2]=>
  string(18) "Creating Your Site"
  [3]=>
  string(9) "article-1"
  [4]=>
  string(9) "article-2"
  [5]=>
  string(9) "article-3"
 }

 ------------------------------
 TestModule Action One Finished
 ****************************************



Action-two
-----------------

Muestra los actuales títulos de artículos. El comando utilizado para hacer una acción es como sigue:


.. code-block:: bash

	jrush testmodule action-two

Después da el comando muestra los detalles del actual y títulos de los artículos.


beneficios
----------------

* Consultar los módulos de forma correcta. 
* No caso sensible. 
* Menos desperdiciador de tiempo. 
* Más barato para actualizar en sitio simple.       
* Última actualización está disponible 
* apto para trabajar con Ubuntu y centOS.
