===========
Dapperfy
===========

sinopsis
------------

Dapperfy es una fina pieza de módulo principal defecto que ayuda y apoya a los usuarios en la creación de un conjunto estándar de archivos pilotos automáticos para sus proyectos . Los usuarios pueden configurar los ajustes predeterminados a las aplicaciones . Por ejemplo : usuario admin mysql , anfitrión, pasar.

Veamos cómo utilizar las funciones de lista estándar y apuestos apuestos bajo este módulo a partir de los próximos temas .

Ayuda Comando
--------------------

El comando de ayuda envuelve toda la información necesaria sobre dapperfy como sus principales usos , la lista de parámetros alternativos que se pueden utilizar en la declaración , ¿cuáles son función principal de dapperfy ( Ej: estándar, lista) , y también la sintaxis utilizada para declarar esas funciones interesantes . El siguiente comando se utiliza para declarar opción de ayuda bajo dapperfy ,

.. code-block:: bash


	ptdeploy Dapperfy help

La siguiente captura de pantalla muestra gráficamente sobre el funcionamiento de comando ayuda.


.. code-block:: bash

 kevell@corp:/# ptdeploy Dapperfy help
 ******************************


  This command is part of a default Module Core and provides you with a method by which you can
  create a standard set of Autopilot files for your project from the command line.
  You can configure default application settings, ie: mysql admin user, host, pass


  Dapperfy, dapperfy

        - list
        List all of the autopilot files in your build/config/ptdeploy/autopilots
        example: ptdeploy dapperfy list

        - standard
        Create a standard set of autopilots to manage
        example: ptdeploy dapperfy standard

        The start of the command will be ptdeploy autopilot execute *filename*

        
 --------------
  Drupal Module:

  The Drupal module extends Dapperfy by providing Templates for automated deployment Autopilots that will be configured
  for your particular Drupal site. This module adds the 'drupal' action to dapperfy.

  - drupal
  create drupal tailored automated deployment ptdeploy autopilots
  example: ptdeploy dapperfy drupal --yes --guess

 --------------
  Joomla Module:

  The Joomla module extends Dapperfy by providing Templates for automated deployment Autopilots that will be configured
  for your particular Joomla site. This module adds the 'joomla' action to dapperfy.

  - joomla, joomla30
  create joomla tailored automated deployment ptdeploy autopilots
  example: ptdeploy dapperfy joomla --yes --guess

  - joomla-phlagrant, joomla30-phlagrant
  create joomla tailored automated deployment ptdeploy autopilots for your Phlagrant Virtual Machines
  example: ptdeploy dapperfy joomla-phlagrant --yes --guess
 --------------
  Wordpress Module:

  The Wordpress module extends Dapperfy by providing Templates for automated deployment Autopilots that will be configured
  for your particular Wordpress site. This module adds the 'wordpress' action to dapperfy.

  - wordpress
  create wordpress tailored automated deployment ptdeploy autopilots
  example: ptdeploy dapperfy wordpress --yes --guess
 ------------------------------
 End Help
 ******************************


Cómo utilizar Dapper Standard
---------------------------------------

El comando utilizado para dapperfy estándar se muestra a continuación ,

.. code-block:: bash

	ptdeploy dapperfy standard

Después de introducir el comando dado anteriormente, el siguiente proceso como se describe en la voluntad tabla siguiente se produce en una base paso a paso.


.. cssclass:: table-bordered

 
 +--------------------------+------------------------------------------+-----------+---------------------------------------------------+
 | parámetros		    | parámetros alternativos		       | Opciones  | Comentarios				       |
 +==========================+==========================================+===========+===================================================+
 |Dapperfy This? (Y/N)	    | En lugar de dapperfy , podemos utilizar  | Y(Yes)	   | Si el usuario desea continuar dapperfying         |
 | 			    | Dapperfy también.			       | 	   | proceso que puede introducir como Y.	       |
 +--------------------------+------------------------------------------+-----------+---------------------------------------------------+
 |Dapperfy This? (Y/N)	    | En lugar de dapperfy , podemos utilizar  | N(No)	   | Si el usuario desea salir de la dapperfying       |
 |			    | Dapperfy también.			       |	   | proceso que puede introducir como N.	       |
 +--------------------------+------------------------------------------+-----------+---------------------------------------------------+
 |Utilice entorno existente | 					       | Y(Yes)	   | Si el usuario desea proceder con la               |
 |ajustes? (Y/N)	    |					       | 	   | configuración del entorno existentes que pueden   |
 |			    |					       |	   | de entrada como Y.				       |
 +--------------------------+------------------------------------------+-----------+---------------------------------------------------+
 |Utilice entorno existente |					       | N(No)	   | Si el usuario desea proceder con el nuevo         |
 |ajustes? (Y/N)	    | 					       |           | configuración del entorno que puede               |
 |                          |                                          |           | introducir como N.                                |
 +--------------------------+------------------------------------------+-----------+---------------------------------------------------+
 |¿Quieres añadir	    |					       | Y(Yes)    | Si el usuario desea agregar otro entorno          |
 |otro ambiente ?           | 					       |           | para dapperfying se puede introducir como Y.      |
 +--------------------------+------------------------------------------+-----------+---------------------------------------------------+
 |¿Quieres añadir           | 					       | N(No)	   | Si el usuario no está en la necesidad de añadir   |
 |otro ambiente ?           |					       | 	   | otro ambiente para dapperfying se puede           |
 |			    |					       |	   | introducir como N.|                               |
 +--------------------------+------------------------------------------+-----------+---------------------------------------------------+



Los dos tipos diferentes de capturas de pantalla pueden ser útiles para los usuarios en la definición de una representación gráfica de proceso de dapperfying . La segunda captura de pantalla muestra método de especificar la disposición en el uso de la configuración del entorno existentes.



.. code-block:: bash


 kevell@corp:/# ptdeploy dapperfy standard
 Dapperfy This? (Y/N) 
 Y
 Use existing environment settings? (Y/N) 
 n
 Do you want to add another environment? (Y/N) 
 n
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-enforce-revisions.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-rollback-newest.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-rollback-previous.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-enforce-revisions.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-rollback-newest.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-rollback-previous.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-uninstall-code.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-nodepool-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-phlagrant-host-install-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-phlagrant-host-uninstall-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-phlagrant-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-uninstall-code.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-enforce-revisions.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-rollback-newest.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-rollback-previous.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-enforce-revisions.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-rollback-newest.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-rollback-previous.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-uninstall-code.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-nodepool-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-phlagrant-host-install-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-phlagrant-host-uninstall-host-file-entry.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-phlagrant-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-install-code-no-dbconf.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-uninstall-code-data.php
 //build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-uninstall-code.php
 ******************************


 Success
 In Dapperfy
 ******************************


Cómo utilizar la Lista Dapperfy
---------------------------------

El objetivo principal de la función de la lista es la lista de todos los archivos de piloto automático de los proyectos de los usuarios que están disponibles en un lugar determinado. La sintaxis para utilizar la lista bajo dapperfy se muestra a continuación,

.. code-block:: bash

        ptdeploy dapperfy list

La captura de pantalla muestra a continuación representa el funcionamiento de la opción de lista bajo dapperfy .




Beneficios
-----------

* Es - acomodados tanto en ubuntu y al igual que en ciento OS .
* Los parámetros utilizados en la declaración no distingue entre mayúsculas y minúsculas.
* El usuario puede ver la lista de archivos de pilotos automáticos que están disponibles para sus proyectos.
* Mientras dapperfying , el usuario puede especificar la configuración del entorno que requiere .
* Muchos entornos pueden ser añadidos a dapperfy .
