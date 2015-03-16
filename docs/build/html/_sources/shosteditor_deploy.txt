======================
Host Editor
======================

sinopsis
------------------

Este módulo es compatible para manejar Apache Virtual Editor anfitrión en ptdeploy . Puede funcionar de dos maneras. Están agregar y quitar . Vhost Editor es una herramienta PHP escrito para hacer la adición de hosts virtuales para apache una brisa. Vhost Editor permitirá al usuario agregar , editar o eliminar la información de host virtual en servidor web del usuario . Es conveniente trabajar con Ubuntu y CentOS . Vamos a ver cómo la Vhost Editor apache puede funcionar bajo ptdeploy .

comando Ayuda
-----------------------

Este comando ayuda guía al usuario para crear un servidor virtual. Esto también muestra que añadir una máquina virtual , eliminar un host virtual, habilitar un host virtual , y deshabilitar un host virtual .

El comando de ayuda para Apachevhosteditor se muestra a continuación .

.. code-block:: bash

	ptdeploy Apachevhosteditor help

Después de entradas el comando anterior, comienza a funcionar para agregar un editor de host virtual. Es la catequesis de las funciones en las capturas de pantalla .


.. code-block:: bash

 kevell@corp:/# ptdeploy ApacheVHostEditor help
 ******************************


  This command is part of Default Modules and handles Apache VHosts Functions.

  ApacheVHostEditor, apachevhosteditor, vhosteditor, vhe, vhosted

          - add
          create a Virtual Host
          example: sudo ptdeploy vhe add
          example: sudo ptdeploy vhe add --yes --vhe-docroot=/var/www/the-app --vhe-url=www.dave.com --vhe-file-ext="" --vhe-apache-command="apache2" --vhe-ip-port="127.0.0.1:80" --vhe-vhost-dir="/etc/apache2/sites-available" --vhe-template="*template data*"
          example: sudo ptdeploy vhe add --yes --guess --vhe-url=www.dave.com
              # will attempt to guess the following but you can override any
              # --vhe-docroot=*current working dir*
              # --vhe-file-ext="ubuntu none, others .conf"
              # --vhe-apache-command="apache2 or httpd depends on system"
              # --vhe-ip-port="127.0.0.1:80"
              # --vhe-vhost-dir="/etc/apache2/sites-available or /etc/httpd/vhosts.d"
              # --vhe-template="*template data*"
              # --vhe-default-template-name="docroot-src-suffix" // from default templates

          - add-balancer
          create a Virtual Host
          example: sudo ptdeploy vhe add
          example: sudo ptdeploy vhe add --yes --vhe-docroot=/var/www/the-app --vhe-url=www.dave.com --vhe-file-ext="" --vhe-apache-command="apache2" --vhe-ip-port="127.0.0.1:80" --vhe-vhost-dir="/etc/apache2/sites-available" --vhe-template="*template data*"
          example: sudo ptdeploy vhe add --yes --guess --vhe-url=www.dave.com
              # will attempt to guess the following but you can override any
              # --vhe-docroot=*current working dir*
              # --vhe-file-ext="ubuntu none, others .conf"
              # --vhe-apache-command="apache2 or httpd depends on system"
              # --vhe-ip-port="127.0.0.1:80"
              # --vhe-vhost-dir="/etc/apache2/sites-available or /etc/httpd/vhosts.d"
              # --vhe-template="*template data*"
              # --vhe-default-template-name="docroot-src-suffix" // from default templates

          - rm
          example: ptdeploy vhe rm
          example: ptdeploy vhe rm --yes --
          example: ptdeploy vhe rm --yes --guess --vhe-deletion-vhost=www.site.com
          example: ptdeploy vhe rm --yes --guess --vhe-deletion-vhost=www.site.com

          - list
          List current Virtual Hosts
          example: ptdeploy vhe list

          - enable
          enable a Server Block
          example: ptdeploy vhe enable

          - disable
          disable a Server Block
          example: ptdeploy vhe disable

 ------------------------------
 End Help
 ******************************



parámetros alternativos
-----------------------------------

Los siguientes son los parámetros alternativos que pueden ser definidos en las declaraciones :

ApacheVHostEditor, apachevhosteditor, vhosteditor, vhe, vhosted.


añadir
--------

Esto facilita al usuario crear un host virtual . Si bien la adición de host virtual que pueda pide VHE - docroot , VHE -file- ext , VHE - apache- comando , puerto - VHE ip , VHE - host- dir, VHE -plantillas , VHE - default- template -name. El usuario puede entrar en el acuerdo a su deseo.

.. code-block:: bash

	sudo ptdeploy vhe add

Después de la entrada como el comando anterior , el usuario puede llenar el siguiente proceso.

.. cssclass:: table-bordered

 +----------------------------------+--------------+------------------------------+-------------------------------------------------------+
 | parámetros			    | directorio   | opción			  | Comentarios						  |
 +==================================+==============+==============================+=======================================================+
 |ptdeploy vhe add (Default)        | Yes	   |Se puede pedir al usuario  	  | Host virtual añadida en la raíz del documento 	  |
 |				    |		   |para Document root		  | especificad bajo deploy                               |
 +----------------------------------+--------------+------------------------------+-------------------------------------------------------+
 |¿Cuál es el nombre del servidor   |-		   |Se puede pedir al usuario 	  | Nombre del servidor secundario bajo ptdeploy          |
 |				    |	  	   |para server name		  | 							  |
 +----------------------------------+--------------+------------------------------+-------------------------------------------------------+
 |What IP:Port (default)	    |127.0.0.1:80  |Se puede pedir al usuario     | Cuando la entrada de usuario como introducir el valor |
 |				    |		   |para IP port		  | por defecto para el puerto IP                         |
 +----------------------------------+--------------+------------------------------+-------------------------------------------------------+
 |¿Qué extensión de archivo debe    |None	   |Se puede pedir al usuario 	  | El usuario da entrada como extensión de archivo       |
 |ser usado? (Default)		    |		   |extension			  |							  |
 +----------------------------------+--------------+------------------------------+-------------------------------------------------------+
 |ptdeploy vhe add		    |No		   |Se puede pedir al usuario	  | Puede termina el proceso                              |
 |				    |		   |input.|			  |							  |
 +----------------------------------+--------------+------------------------------+-------------------------------------------------------+


Por último, el sistema puede pide directorio templates host virtual. Hay 5 opciones están disponibles en las plantillas. Ellos son los siguientes.

0 for doc root-no-suffix

1 for doc –src-suffix   used for document screen suffix

2 for doc –web-suffix used for document web suffix

3 for doc –www-suffix used for world wide web suffix

4 for docroot-suffix used for document root suffix

El usuario desee seleccionar los valores de acuerdo con sus necesidades. A continuación, el sistema puede pedir el nombre de host virtual , la dirección y el usuario root IP etc es correcto o incorrecto. Si el usuario dice que sí, entonces se muestra el directorio vhost y habilitar este host virtual ?

El usuario contesta sí que pueden permitir al host virtual de lo contrario pueden salir.

.. code-block:: bash

 kevell@corp:/# ptdeploy vhe add
 Do you want to add a VHost? (Y/N) 
 Y
 What's the document root? Enter nothing for /
 root
 What URL do you want to add as server name?
 www.vh.com
 What IP:Port should be set? Enter nothing for 127.0.0.1:80

 What File Extension should be used? Enter nothing for None (probably .conf on this system)

 What is your VHost Template directory? Enter nothing for default templates

 Please Choose VHost Template: 
 --- Default Virtual Host Templates: ---
 (0) docroot-no-suffix
 (1) docroot-src-suffix
 (2) docroot-web-suffix
 (3) docroot-www-suffix
 (4) docroot-docroot-suffix

 0
 Please check VHost: NameVirtualHost 127.0.0.1:80
 <VirtualHost 127.0.0.1:80>
	ServerAdmin webmaster@localhost
	ServerName www.vh.com
	DocumentRoot root
	<Directory root>
		Options Indexes FollowSymLinks MultiViews
		AllowOverride All
		Order allow,deny
		allow from all
	</Directory>
 </VirtualHost>

 Is this Okay? (Y/N) 

 ******************************


 Apache VHost Editor Finished
 ******************************



quitar
--------------

El comando de terminal para borrar host virtual ( s ) es rm . El formato general de este comando es rm . rm elimina un host virtual si especifica una ruta correcta para él y si no lo hace, entonces se muestra un mensaje de error y pasa a la siguiente anfitrión . A veces, puede que no tenga los permisos de escritura para un host virtual , en ese caso se le pide confirmación. Escriba yes si desea eliminarlo.

Si el nombre eliminado era el último eslabón de una máquina virtual y no hay procesos tienen la abierta host virtual , la máquina virtual se elimina y el espacio que estaba usando se pone a disposición para su reutilización.

Si el nombre era el último eslabón de una máquina virtual, pero cualquier proceso todavía tienen la abierta host virtual , la máquina virtual se mantendrá en existencia hasta el último descriptor host virtual en referencia a que se cierre.

Si el nombre se refiere a un enlace simbólico, se elimina el vínculo. El siguiente comando utiliza para eliminar el host virtual.

.. code-block:: bash
   
	sudo ptdeploy vhe rm –yes –guess –vhe-deletion-vhost=www.kevell.com

La siguiente captura de pantalla puede explicar sus funciones.

.. code-block:: bash

 - rm
          example: ptdeploy vhe rm
          example: ptdeploy vhe rm --yes --
          example: ptdeploy vhe rm --yes --guess --vhe-deletion-vhost=www.site.com
          example: ptdeploy vhe rm --yes --guess --vhe-deletion-vhost=www.site.com


.. code-block:: bash

 kevell@corp:/# ptdeploy vhe rm
 Do you want to delete VHost/s? (Y/N) 
 y
 Deleting vhost
 What is your VHost directory? Found "/etc/apache2/sites-available" - Enter nothing to use this

 Please Choose VHost:
 --- All Virtual Hosts: ---
 (0) 000-default.conf
 (1) default-ssl.conf

 0
 Do you want to disable this VHost? (hint - ubuntu probably yes, centos probably no) (Y/N) 
 yes
 Site 000-default disabled.
 To activate the new configuration, you need to run:
  service apache2 reload
 a2dissite 000-default.conf done
 VHost 000-default.conf Deleted  if existed
 ******************************


 1Apache VHost Editor Finished
 ******************************



lista
--------

Información sobre el anfitrión virtual ( el directorio actual por defecto). Ordenar las entradas por orden alfabético. Los argumentos obligatorios tiene opciones largas , así como opciones cortas . Una lista invoca con una URL que especifica tanto el nombre de la lista y también la opinión subyacente que proporcionará y organizar los datos. El siguiente comando usa para listar el host virtual.

.. code-block:: bash
   
	ptdeploy vhe list

Tenga en cuenta que si una lista se puede utilizar con una variedad de puntos de vista , o podría ser adaptado para producir una página elaborada a partir de una vista diseñado específicamente para organizar los datos para ello. Listas almacenados bajo el campo de las listas de un documento de diseño . Puede ser visualizado por las capturas de pantalla .

.. code-block:: bash

 - list
          List current Virtual Hosts
          example: ptdeploy vhe list


.. code-block:: bash

 kevell@corp:/# ptdeploy vhe list
 What is your VHost directory? Found "/etc/apache2/sites-available" - Enter nothing to use this

 You have a sites available dir, so also listing available sites.
 Current Installed VHosts:
 --- Enabled Virtual Hosts: ---
 (0) 000-default.conf
 (1) default-ssl.conf
 --- All Available Virtual Hosts: ---
 (2) 000-default.conf
 (3) default-ssl.conf
 ******************************


 1Apache VHost Editor Finished
 ******************************




permitir
---------

Secure arranque es una función diseñada para evitar que el software malicioso y los medios de comunicación no autorizada de la carga durante el proceso de arranque. Esta opción permitirá activar el bloque de servidor. En host virtual cuando el usado escribe el siguiente comando ,

.. code-block:: bash
   
	ptdeploy vhe enable

Esta opción está activada de forma predeterminada. Esta opción permite que el servidor host virtual enable.

Módulo Asiste a desarrollar muchas de las capacidades propicias necesarias para dar servicio a entornos de alto rendimiento a través de la comprensión de las interdependencias entre las personas, procesos y tecnología. La siguiente captura de pantalla explica el mismo .

.. code-block:: bash

 - enable
          enable a Server Block
          example: ptdeploy vhe enable


.. code-block:: bash

 kevell@corp:/# ptdeploy vhe enable
 Do you want to enable this VHost? (hint - ubuntu probably yes, centos probably no) (Y/N) 
 y
 Please Choose VHost:
 --- All Virtual Hosts: ---
 (0) default-ssl.conf
 
 0
 ERROR: Site default-ssl.conf does not exist!
 a2ensite default-ssl.conf.conf done
 ******************************


 1Apache VHost Editor Finished
 ******************************





inhabilitar
-------------

Este desactivar utiliza para desactivar el servidor. Conexiones editor de acogida virtual inactivo o inactivos están normalmente desconectados por el servidor después de un cierto período de tiempo. El siguiente comando se utiliza para desactivar el editor de host virtual.

.. code-block:: bash
   
	ptdeploy vhe disable

Después de escribir este comando se puede pedir al usuario para desactivar el servidor . Si el usuario introduce como sí lo desactive el servidor es decir, que no permitirá que ningún cuerpo a trabajar en ese servidor.

La siguiente captura de pantalla visualizarlo evidentemente .

.. code-block:: bash


 - disable
          disable a Server Block
          example: ptdeploy vhe disable


.. code-block:: bash

 kevell@corp:/# ptdeploy vhe disable
 Do you want to disable this VHost? (hint - ubuntu probably yes, centos probably no) (Y/N) 
 y
 Please Choose VHost:
 --- All Virtual Hosts: ---
 (0) default-ssl.conf

 0
 Site default-ssl already disabled
 a2dissite default-ssl.conf done
 ******************************


 1Apache VHost Editor Finished
 ******************************




Beneficios
---------------

* Multi usuario puede acceder a la vez.
* El usuario puede añadir o eliminar host virtual.
* El editor de host virtual puede activar o desactivar el host virtual de acuerdo con el deseo del usuario .
* Sensitibilidad caso.
