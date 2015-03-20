=============
PharaohTools
=============

sinopsis
------------

El módulo de la herramienta de Faraón asiste en la instalación de ptdeploy, pttest, Jrush, generación de informes de ptvirtualize. Esto facilita a los usuarios para asegurar la disponibilidad antes de las instalaciones. Sólo faltan los módulos se puede instalar específicamente.


comando Ayuda
---------------------

El comando ayuda guía a los usuarios sobre cómo hacer uso de este módulo particular bajo ptvirtualize.


También hacerlos conscientes de las opciones que se pueden realizar en este módulo específico.


Lista salidas los parámetros alternativos junto con la sintaxis para la instalación de las herramientas de Faraón.


A continuación, se muestra el comando para el uso de la opción ayuda


.. code-block:: bash

		ptvirtualize pharaoh-tools help


La pantalla como se muestra abajo te da una representación pictórica sobre el uso del comando help.


.. code-block:: bash


instalación
--------------

El módulo de la herramienta de Faraón actúa como una ruta más corta que envuelve la instalación de ptdeploy, pttest, Jrush. Si cualquier un módulo particular no está entre los tres, el módulo específico solo será instalado que es una ventaja añadida. El proceso de asegurar desempeña un papel importante en tomar con respecto a la disponibilidad de módulos de datos.


El comando utilizado para el proceso de instalación debajo de la herramienta de Faraón se expone a continuación,

.. code-block:: bash

	ptvirtualize pharaoh-tools install

Después de introducir el comando anterior, el proceso de instalación comienza ejecución y procede de la siguiente manera como se muestra en la tabla, de



.. cssclass:: table-bordered

 +---------------------------------+----------------------------------+--------------------------------------------------------+
 | parámetros                      | Opciones de entrada disponibles  | comentario             			               |
 +=================================+==================================+========================================================+
 |Install Pharaoh Tools? (Y/N)     | Y(Yes)		              | Si el usuario desea continuar con la instalación       |
 |				   | 			              | proceso, se puede introducir como Y                    |
 +---------------------------------+----------------------------------+--------------------------------------------------------+
 |Install Pharaoh Tools? (Y/N)	   | N(No)		              | Si el usuario desea salir del proceso de instalación,  |
 |				   |			              | que pueden dejar de fumar simplemente usando N|        |
 +---------------------------------+----------------------------------+--------------------------------------------------------+


Mientras se instala el Faraón herramienta los siguientes pasos se realiza:


asegurar
----------

* La herramienta Faraón asegura que los módulos disponibles. 
* Garantizando al mismo tiempo, no mira sobre las versiones.


ptdeploy
------------------

* El módulo ptdeploy se reporta como instalado, en caso de existencia.  
* También comprueba la versión para el módulo de ptdeploy. 
* Si el módulo de ptdeploy no está disponible en la máquina, entonces automáticamente ptdeploy progresarán para instalar.
pttest
------------------

* Después de la terminación de la instalación de ptdeploy, asegurará el módulo pttest.  
* El módulo pttest se reporta como instalado, en caso de existencia.  
* Si el módulo de pttest no está disponible en la máquina, entonces automáticamente pttest progresarán para instalar.


Jrush
--------

* Después de la terminación de la instalación de pttest, asegurará el módulo Jrush. 
* El módulo Jrush se reporta como instalado, en caso de existencia.  
* Si el módulo de Jrush no está disponible en la máquina, entonces automáticamente Jrush progresarán para instalar. 
* Si todos los tres módulos son los ya existentes, entonces se mostrará mensaje excepcional como se indica en la imagen de abajo.


Opciones Adicionales
-------------------------

Durante la instalación de ptdeploy, pttest, Jrush las siguientes opciones se requieren como entrada del usuario. Veamos, las opciones adicionales que pueden ser especificadas por los usuarios si lo desean, se representa en formato tabular como se muestra a continuación.




.. cssclass:: table-bordered

 +----------------------------+--------------------------------------+----------------+--------------------------------------------------+
 | parámetros		      | camino       			     | opción	      | comentario		  		         |
 +============================+======================================+================+==================================================+
 |Program data directory      | "/opt/pttest(corresponding module)"  | Yes	      | Si el usuario de proceder con la instalación     |
 |(Default)		      | 				     |		      | el directorio de datos de programa               |
 |			      |					     |		      | predeterminado que puede introducir como Y       |
 +----------------------------+--------------------------------------+----------------+--------------------------------------------------+
 |Program data directory      | User specific			     | No(End slash)  | Si el usuario proceda a su propio directorio de  |
 |			      |					     |		      | datos del programa , pueden de entrada como N,   |
 |			      |					     |		      | y en la mano especificar que poseen ubicación.   |
 +----------------------------+--------------------------------------+----------------+--------------------------------------------------+
 |Progran executor directory  |                                      |                | Si el usuario de proceder con la instalación     | 
 |(Default)		      |					     |		      | del directorio ejecutor programa por defecto     |
 |			      | 				     |		      | el directorio ejecutor programa predeterminado   |
 +----------------------------+--------------------------------------+----------------+--------------------------------------------------+
 |Program executor directory  | User specific			     | No(End slash)  | Si el usuario desea continuar con su propio      |
 |			      |					     |		      | directorio ejecutor de programas, que pueden     |
 |			      |					     |		      | de entrada como la N, y en la mano especificar   |
 |			      |					     | 		      | poseen ubicación|                                |
 +----------------------------+--------------------------------------+----------------+--------------------------------------------------+


Mientras que lo instale a especificar la ubicación del git clone, muestra el número de objetos, recibir objetos, resolver los deltas, conectividad.


La siguiente captura de pantalla te explica gráficamente el proceso de instalación de la herramienta de Faraón.


.. code-block:: bash


Beneficios
-----------

* Facilita los usuarios para asegurar antes de la instalación. 
* En caso de cualquier módulo particular está desaparecido, el usuario puede proceder a instalar el módulo particular solo. 
* El usuario puede especificar su propio camino o ubicación para su directorio de datos de programa y directorio ejecutor. 
* Si cualquier módulo particular ya existe en la máquina, entonces la herramienta de instalación generará un mensaje de excepción como ya
  está instalado. 
* Evita sobrescribir no deseados de los módulos, por lo tanto, es hora de ahorrar.



