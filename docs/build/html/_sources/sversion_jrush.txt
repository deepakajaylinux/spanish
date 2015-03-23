==============
Version
==============


sinopsis
-------------

Este artículo es sobre el término "versión" como se utiliza en diversos contextos. Control de versiones de software es el proceso de asignación de números de versión única o nombres de versión única a Estados únicos de los programas informáticos. Dentro de una categoría número determinada versión (mayor, menor), estos números se asignan generalmente en orden creciente y corresponden a los nuevos desarrollos en el software. Nivel de grano fino, control de revisión a menudo se utiliza para hacer el seguimiento de forma incremental diferentes versiones de la información electrónica, o no esta información es un software de computadora.


comando Ayuda
----------------------

Este comando permite para determinar el uso del módulo de versión. El usuario llegará a conocer el diferente formas/formato para ejecutar este módulo. Este comando guía al usuario final para conocer el propósito de este comando. A continuación dado son el comando y la captura de pantalla del mismo.


.. code-block:: bash
        
	jrush  version help

La representación pictórica del comando de ayuda se enumera a continuación,


.. code-block:: bash

 kevell@corp:/# jrush  version help
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

  This command Joomls Version information.

  Version, version

        - available
        Returns available Joomla Versions
        example: jrush version available

        - current
        Returns the current Joomla Version
        example: jrush version current

 ------------------------------
 End Help
 ****************************************


Available
----------------

Cuando el usuario necesita saber acerca de la versión de joomla disponibles, la continuación dado comando se ejecutará el proceso de instalación.


.. code-block:: bash
        
	jrush version available ..config file=”bootstrap file path”


La representación pictórica de la captura de pantalla se enumera a continuación,

.. code-block:: bash

 kevell@corp:/# jrush version available --config-file="/var/www/html/joomla/configuration.php" 
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 Joomla Version Info:

 -------------------------

 Version: array(1) {
  ["availableVersions"]=>
  array(2) {
    [0]=>
    string(5) "1.5.0"
    [1]=>
    string(6) "1.5.26"
  }
 }

 ------------------------------
 Joomla Version Info Finished
 ****************************************

Current
----------------

Cuando el usuario necesita saber acerca de la actual versión de joomla, la continuación dado comando se ejecutará el proceso de instalación.

.. code-block:: bash
        
	jrush version current ..config file=”bootstrap file path”

La representación pictórica del comando anterior se enumera a continuación,

.. code-block:: bash

 kevell@corp:/# jrush version current --config-file="/var/www/html/joomla/configuration.php" 
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 Joomla Version Info:

 -------------------------

 Version: array(3) {
  ["shortVersion"]=>
  string(5) "3.3.3"
  ["longVersion"]=>
  string(53) "Joomla! 3.3.3 Stable [ Ember ] 25-July-2014 13:00 GMT"
  ["detailed"]=>
  object(ArrayObject)#47 (1) {
    ["storage":"ArrayObject":private]=>
    object(JVersion)#7 (11) {
      ["PRODUCT"]=>
      string(7) "Joomla!"
      ["RELEASE"]=>
      string(3) "3.3"
      ["DEV_LEVEL"]=>
      string(1) "3"
      ["DEV_STATUS"]=>
      string(6) "Stable"
      ["BUILD"]=>
      string(0) ""
      ["CODENAME"]=>
      string(5) "Ember"
      ["RELDATE"]=>
      string(12) "25-July-2014"
      ["RELTIME"]=>
      string(5) "13:00"
      ["RELTZ"]=>
      string(3) "GMT"
      ["COPYRIGHT"]=>
      string(72) "Copyright (C) 2005 - 2014 Open Source Matters, Inc. All rights reserved."
      ["URL"]=>
      string(107) "<a href="http://www.joomla.org">Joomla!</a> is Free Software released under the GNU General Public License."
    }
  }
 }

 ------------------------------
 Joomla Version Info Finished
 ****************************************


parámetros alternativos
----------------------------

Ninguno de los dos parámetros alternativos pueden utilizarse en comando-

jarticle, JArticle

eg:  jrush version current ..config file=”bootstrap file path”/ jrush Version current ..config file=”bootstrap file path”

beneficios
--------------

* Ayuda a obtener la información sobre una versión de manera fácil 
* ayuda al usuario a conocer acerca de la disponibilidad de la versión de joomla 
* ayuda al usuario a conocer acerca de la actual versión de joomla

