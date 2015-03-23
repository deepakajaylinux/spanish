===========================
ApacheVHostEditor
===========================

sinopsis
------------------

Apache hosts virtuales se utilizan para ejecutar más de un dominio fuera de una sola dirección IP. Esto es especialmente útil para la gente que necesita para manejar las funciones vhost de apache. Los sitios muestran información diferente a los visitantes, en función con la que los usuarios acceder al sitio. No hay límite para el número de máquinas virtuales que se pueden agregar a un Servidor Privado Virtual (VPS) .Este puede ser adecuado para Ubuntu y CentOS.

comando Ayuda
-----------------------

El comando de ayuda conduce a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en los módulos de apache host virtual editor. Las listas de comandos de ayuda fuera de los parámetros alternativos de editor de host virtual Apache
bajo módulo ptdeploy. También se describe la sintaxis para la instalación de updation del usuario. El comando de ayuda para el editor de host virtual Apache se muestra a continuación.

.. code-block:: bash

	ptdeploy Apache virtualhost editor help

La siguiente captura de pantalla muestra el esfuerzo total de editor VirtualHost de apache.

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
Los siguientes son los parámetros alternativos que pueden ser definidos en las declaraciones:

ApacheVHostEditor, apachevhosteditor, vhosteditor, vhe, vhosted.

añadir
----------

Este comando utiliza para crear un host virtual. Primordial es posible. El siguiente comando se puede adoptar para la creación de un editor de host virtual.

.. code-block:: bash

	sudo ptdeploy vhe add

después de introducir el comando anterior se puede hacer la siguiente, Vhe  document root, Vhe file extension, Vhe apache command, Vhe IP Port, Vhe Vhost Directory, Vhe Template, Vhe Default template name.

El usuario tiene que introducir todos los datos uno por uno de otro modo entran en la propia línea de comandos. La siguiente captura de pantalla, explica al respecto

.. code-block:: bash


 kevell@corp:/# ptdeploy vhe add 
 
 Do you want to add a VHost? (Y/N) 
 y 
 What's the document root? Enter nothing for /home/karunakaran 

 What URL do you want to add as server name? 
 kumar 
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
	ServerName kumar 
	DocumentRoot /home/karunakaran 
	<Directory /home/karunakaran> 
		Options Indexes FollowSymLinks MultiViews 
		AllowOverride All 
		Order allow,deny 
		allow from all 
	</Directory> 
 </VirtualHost> 

 Is this Okay? (Y/N) 
 y 
 What is your VHost directory? Found "/etc/apache2/sites-available" - Enter nothing to use this 

 Do you want to enable this VHost? (hint - ubuntu probably yes, centos probably no) (Y/N) 
 y 
 Enabling site kumar. 
 To activate the new configuration, you need to run: 
  service apache2 reload 
 a2ensite kumar.conf done 
 ****************************** 

 1Apache VHost Editor Finished 
 ******************************

.. code-block:: bash




 kevell@corp:/# ptdeploy vhe add --yes --vhe-docroot=/var/www/the-app --vhe-url=www.murali.com --vhe-file-ext=".conf" --vhe-apache-command="apache2" --vhe-ip-port="127.0.0.1:80" --vhe-vhost-dir="/etc/apache2/sites-available" --vhe-template="*template data*" 

 *template data* 

 Assuming Okay due to yes parameter 
 Enabling site www.murali.com. 
 To activate the new configuration, you need to run: 
  service apache2 reload 
 a2ensite www.murali.com.conf done 
 ****************************** 

 1Apache VHost Editor Finished 
 ****************************** 

.. code-block:: bash


 kevell@corp:/# ptdeploy vhe add --yes --guess --vhe-url=www.kkkkkkkkk.com 

 What is your VHost Template directory? Enter nothing for default templates 

 Please Choose VHost Template: 
 --- Default Virtual Host Templates: --- 
 (0) docroot-no-suffix 
 (1) docroot-src-suffix 
 (2) docroot-web-suffix 
 (3) docroot-www-suffix 
 (4) docroot-docroot-suffix 
 
 0 
 NameVirtualHost 127.0.0.1:80 
 <VirtualHost 127.0.0.1:80> 
 	ServerAdmin webmaster@localhost 
	ServerName www.kkkkkkkkk.com 
	DocumentRoot /home/karunakaran 
	<Directory /home/karunakaran> 
		Options Indexes FollowSymLinks MultiViews 
		AllowOverride All 
		Order allow,deny 
		allow from all 
	</Directory> 
 </VirtualHost> 

 Assuming Okay due to yes parameter 
 Enabling site www.kkkkkkkkk.com. 
 To activate the new configuration, you need to run: 
  service apache2 reload 
 a2ensite www.kkkkkkkkk.com done 
 ****************************** 

 1Apache VHost Editor Finished 
 ******************************






Más- Balancer
---------------------

Este comando utiliza para crear un host virtual. Primordial es posible. Hay dos maneras de entrar en la entrada. En forma simple, el usuario puede dar VHE add. La segunda forma, junto con el nombre de ruta de host comando puede ser mencionado. El siguiente comando se puede adoptar para la creación de un editor de host virtual.

.. code-block:: bash

	sudo ptdeploy vhe add

después de introducir el comando anterior se puede hacer la siguiente, Vhe  document root, Vhe file extension, Vhe apache command, Vhe IP Port,  Vhe Vhost Directory, Vhe Template, Vhe Default template name.

El usuario tiene que introducir todos los datos uno por uno de otra manera entran todo en la propia línea de comandos. La siguiente captura de pantalla, explica al respecto

.. code-block:: bash

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

quitar
-------------

Este comando utiliza para eliminar un host virtual en particular. Hay dos maneras de entrar en la entrada. En forma simple, el usuario puede dar remove VHE (rm). La segunda forma, junto con el nombre de ruta de host comando puede ser mencionado. El siguiente comando se utiliza para eliminar el nombre de host.

.. code-block:: bash

        ptdeploy vhe rm

La siguiente captura de pantalla muestra la función de rm.

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
 (1) ddddddd.conf 
 (2) default-ssl.conf 
 (3) default-ssl.dpkg-remove 
 (4) default.dpkg-remove 
 (5) karuna 
 (6) kumar.conf 
 (7) llllllllllllll.conf 
 (8) mmmmmm.conf 
 (9) ptbuild.conf 
 (10) www.dave.com 
 (11) www.google.com 
 (12) www.kkkkkkkkk.com.conf 
 (13) www.murali.com.conf 
 (14) www.siva.com.conf 
 (15) www.siva1.com 

 14 
 Do you want to disable this VHost? (hint - ubuntu probably yes, centos probably no) (Y/N) 
 y 
 Site www.siva.com disabled. 
 To activate the new configuration, you need to run: 
  service apache2 reload 
 a2dissite www.siva.com.conf done 
 VHost www.siva.com.conf Deleted  if existed 
 ****************************** 

 1Apache VHost Editor Finished 
 ****************************** 

.. code-block:: bash


 kevell@corp:/# ptdeploy vhe rm --yes --

 Deleting vhost
 What is your VHost directory? Found "/etc/apache2/sites-available" - Enter nothing to use this

 Please Choose VHost:
 --- All Virtual Hosts: ---
 (0) 000-default.conf
 (1) ddddddd.conf
 (2) default-ssl.conf
 (3) default-ssl.dpkg-remove
 (4) default.dpkg-remove
 (5) karuna
 (6) kumar.conf
 (7) llllllllllllll.conf
 (8) mmmmmm.conf
 (9) ptbuild.conf
 (10) testrepo.conf
 (11) www.dae.com.conf
 (12) www.dave.com
 (13) www.google.com
 (14) www.kkkkkkkkk.com.conf
 (15) www.murali.com.conf

 14
 Site www.kkkkkkkkk.com already disabled
 a2dissite www.kkkkkkkkk.com.conf done
 VHost www.kkkkkkkkk.com.conf Deleted  if existed
 ******************************

 1Apache VHost Editor Finished
 ******************************


.. code-block:: bash


 kevell@corp:/# ptdeploy vhe rm --yes --guess --vhe-deletion-vhost=www.da.com.conf

 Deleting vhost
 Site www.da.com disabled.
 To activate the new configuration, you need to run:
  service apache2 reload
 a2dissite www.da.com.conf done
 VHost www.da.com.conf Deleted  if existed
 ******************************


 1Apache VHost Editor Finished
 ******************************


.. code-block:: bash

 kevell@corp:/# ptdeploy vhe rm --yes --guess --vhe-deletion-vhost=www.dae.com.conf

 Deleting vhost
 Site www.dae.com disabled.
 To activate the new configuration, you need to run:
  service apache2 reload
 a2dissite www.dae.com.conf done
 VHost www.dae.com.conf Deleted  if existed
 ******************************

 1Apache VHost Editor Finished
 ******************************










lista
--------

Este comando utiliza para enumerar los hosts virtuales actuales. El siguiente comando utiliza para enumerar los hosts virtuales.

.. code-block:: bash

	ptdeploy vhe list

La captura de pantalla muestra la función de lista.

.. code-block:: bash

 kevell@corp:/# ptdeploy vhe list 

 What is your VHost directory? Found "/etc/apache2/sites-available" - Enter nothing to use this 

 You have a sites available dir, so also listing available sites. 
 Current Installed VHosts: 
 --- Enabled Virtual Hosts: --- 
 (0) 000-default.conf 
 (1) ddddddd.conf 
 (2) default-ssl.conf 
 (3) default-ssl.dpkg-remove 
 (4) default.dpkg-remove 
 (5) karuna 
 (6) kumar.conf 
 (7) llllllllllllll.conf 
 (8) mmmmmm.conf 
 (9) ptbuild.conf 
 (10) www.dave.com 
 (11) www.google.com 
 (12) www.kkkkkkkkk.com.conf 
 (13) www.murali.com.conf 
 (14) www.siva.com.conf 
 (15) www.siva1.com 
 --- All Available Virtual Hosts: --- 
 (16) 000-default.conf 
 (17) ddddddd.conf 
 (18) default-ssl.conf 
 (19) default-ssl.dpkg-remove 
 (20) default.dpkg-remove 
 (21) karuna 
 (22) kumar.conf 
 (23) llllllllllllll.conf 
 (24) mmmmmm.conf 
 (25) ptbuild.conf 
 (26) www.dave.com 
 (27) www.google.com 
 (28) www.kkkkkkkkk.com.conf 
 (29) www.murali.com.conf 
 (30) www.siva.com.conf 
 (31) www.siva1.com 
 ****************************** 
 
 1Apache VHost Editor Finished 
 ****************************** 




permitir
-----------

Secure arranque es una función diseñada para evitar que el software malicioso y los medios de comunicación no autorizada de la carga durante el proceso de arranque. Esta opción permitirá activar el bloque de servidor. En host virtual cuando el usado escribe el siguiente comando,

.. code-block:: bash
   
        ptdeploy vhe enable

Esta opción está activada de forma predeterminada. Esta opción permite que el servidor host virtual enable.

Módulo Asiste a desarrollar muchas de las capacidades propicias necesarias para dar servicio a entornos de alto rendimiento a través de la comprensión de las interdependencias entre las personas, procesos y tecnología. La siguiente captura de pantalla explica el mismo.

.. code-block:: bash


 kevell@corp:/# ptdeploy vhe enable 

 Do you want to enable this VHost? (hint - ubuntu probably yes, centos probably no) (Y/N) 
 y 
 Please Choose VHost: 
 --- All Virtual Hosts: --- 
 (0) 000-default.conf 
 (1) ddddddd.conf 
 (2) default-ssl.conf 
 (3) default-ssl.dpkg-remove 
 (4) default.dpkg-remove 
 (5) karuna 
 (6) kumar.conf 
 (7) llllllllllllll.conf 
 (8) mmmmmm.conf 
 (9) ptbuild.conf 
 (10) www.dave.com 
 (11) www.google.com 
 (12) www.kkkkkkkkk.com.conf 
 (13) www.murali.com.conf 
 (14) www.siva.com.conf 
 (15) www.siva1.com 

 7 
 Enabling site llllllllllllll. 
 To activate the new configuration, you need to run: 
  service apache2 reload 
 a2ensite llllllllllllll.conf done 
 ****************************** 

 1Apache VHost Editor Finished 
 ****************************** 




inhabilitar
-------------

Este desactivar utiliza para desactivar el servidor. Conexiones editor de acogida virtual inactivo o inactivos están normalmente desconectados por el servidor después de un cierto período de tiempo. El siguiente comando se utiliza para desactivar el editor de host virtual.

.. code-block:: bash
   
        ptdeploy vhe disable

Después de escribir este comando se puede pedir al usuario para desactivar el servidor. Si el usuario introduce como sí lo desactive el servidor es decir, que no permitirá que ningún cuerpo a trabajar en ese servidor.

La siguiente captura de pantalla visualizarlo evidentemente.

.. code-block:: bash

 kevell@corp:/# ptdeploy vhe disable 

 Do you want to disable this VHost? (hint - ubuntu probably yes, centos probably no) (Y/N) 
 y 
 Please Choose VHost: 
 --- All Virtual Hosts: --- 
 (0) 000-default.conf 
 (1) default-ssl.conf 
 (2) default-ssl.dpkg-remove 
 (3) default.dpkg-remove 
 (4) karuna 
 (5) kumar.conf 
 (6) ptbuild.conf 
 (7) www.dave.com 
 (8) www.google.com 
 (9) www.kkkkkkkkk.com.conf 
 (10) www.murali.com.conf 
 (11) www.siva.com.conf 
 (12) www.siva1.com 

 9 
 Site www.kkkkkkkkk.com disabled. 
 To activate the new configuration, you need to run: 
  service apache2 reload 
 a2dissite www.kkkkkkkkk.com.conf done 
 ****************************** 

 1Apache VHost Editor Finished 
 ****************************** 


Beneficios
---------------

* Multi usuario puede acceder a la vez.
* El usuario puede añadir o eliminar host virtual.
* El editor de host virtual puede activar o desactivar el host virtual de acuerdo con el deseo del usuario.
* Sensitibilidad caso.
* Well-to-do en Ubuntu y CentOS.
