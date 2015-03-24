======================
Host Editor
======================

sinopsis
------------------

Este módulo soporta para manejar Apache Virtual Host Editor bajo ptdeploy. Puede funcionar de dos maneras. Ellos son añadir y quitar. Vhost Editor es una herramienta de PHP para hacer agregar hosts virtuales en apache una brisa. Vhost Editor le permitirá al usuario añadir, editar o eliminar la información Virtual Host de servidor Web del usuario. Es conveniente trabajar con Ubuntu y ciento OS.  Vamos a ver cómo los apaches Vhost Editor pueden funcionar bajo ptdeploy.

comando Ayuda
-----------------------

Este comando ayuda guía al usuario para crear un hosteditor. A continuación se muestra el comando de ayuda para Hosteditor.

.. code-block:: bash

	ptdeploy Hosteditor help

Después de entradas el comando anterior, comienza funcionamiento para agregar un editor de host virtual. Lo catequesis las funciones en las capturas de pantalla.

.. code-block:: bash

 kevell@corp:/# ptdeploy HostEditor help 

 ****************************** 

  This command is part of Default Modules and handles Host File Management Functions. 

  HostEditor, hosteditor, he, hostEditor 

          - add 
          add a Host File entry 
          example: ptdeploy hosteditor add 
          example: ptdeploy hosteditor add --yes 
              --host-ip=127.0.0.1  # guess will assume 127.0.0.1 
              --host-name=dave.com 

          - rm 
          remove a Host File entry 
          example: ptdeploy hosteditor rm 
          example: ptdeploy hosteditor rm --yes 
              --host-ip=127.0.0.1 # guess will ignore this, and remove any entry matching the host name 
              --host-name=dave.com 

 ------------------------------ 
 End Help 
 ****************************** 



parámetros alternativos
-----------------------------------

Los siguientes son los parámetros alternativos que pueden definirse en declaraciones:

HostEditor, hosteditor, he, hostEditor 


Add
-------

Esto facilita el usuario para crear un host editor. El usuario puede escribir según su deseo.

.. code-block:: bash

		sudo ptdeploy hosteditor add

Después de entrada como el comando anterior, el usuario puede llenar el siguiente proceso.

.. code-block:: bash

 kevell@corp:/# ptdeploy hosteditor add 

 Do you want to add a hosts file entry? (Y/N) 
 y 
 Do you want a non-default IP? Enter for 127.0.0.1 
 127.0.0.1 
 What URI do you want to affect to the hostfile? 
 karuna 
 Please check host file: 127.0.0.1	localhost 
 127.0.1.1	karuna 
 127.0.1.1       www.kevell.com 
 
 127.0.1.1	www.ptbuild.tld 
 # The following lines are desirable for IPv6 capable hosts 
 ::1     ip6-localhost ip6-loopback 
 fe00::0 ip6-localnet 
 ff00::0 ip6-mcastprefix 
 ff02::1 ip6-allnodes 
 ff02::2 ip6-allrouters 
              --host-ip=127.0.0.1  # guess will assume 127.0.0.1              --host-name=dave.com127.0.0.1          dave.com 
 127.0.0.1          dave.com 
 192.168.1.4          
 127.0.0.1          deepak 
 clear          
 127.0.0.1          www.kevell.com 
 127.0.0.1          
 127.0.0.1          karuna 


 Is this Okay?  (Y/N) 
 y 
 ****************************** 

 1Host Editor Finished 
 ****************************** 

.. code-block::  bash

 kevell@corp:/# ptdeploy hosteditor add --yes 

 Do you want a non-default IP? Enter for 127.0.0.1 
 127.0.0.1 
 What URI do you want to affect to the hostfile? 
 kumar 
 ****************************** 

 1Host Editor Finished 
 ****************************** 




quitar
--------------

El comando en el terminal para eliminar hosteditor es rm. El formato general de este comando es rm. RM quita un host si se especifica una ruta de acceso correcta para él y si no, entonces se muestra un mensaje de error y pasar al siguiente anfitrión.


El siguiente comando utilizado para borrar el host virtual.

.. code-block:: bash
   
		sudo ptdeploy hosteditor rm

La siguiente captura de pantalla puede explicar sus funciones.

.. code-block:: bash

 kevell@corp:/# ptdeploy hosteditor rm 

 Do you want to remove a hosts file entry? (Y/N) 
 y 
 Do you want a non-default IP? Enter for 127.0.0.1 
 127.0.0.1 
 What URI do you want to affect to the hostfile? 
 karuna 
 Please check host file: 127.0.0.1	localhost 
 127.0.1.1	karuna 
 127.0.1.1       www.kevell.com 

 127.0.1.1	www.ptbuild.tld 
 # The following lines are desirable for IPv6 capable hosts 
 ::1     ip6-localhost ip6-loopback 
 fe00::0 ip6-localnet 
 ff00::0 ip6-mcastprefix 
 ff02::1 ip6-allnodes 
 ff02::2 ip6-allrouters 
              --host-ip=127.0.0.1  # guess will assume 127.0.0.1              --host-name=dave.com127.0.0.1          dave.com 
 127.0.0.1          dave.com 
 192.168.1.4          
 127.0.0.1          deepak 
 clear          
 127.0.0.1          www.kevell.com 
 127.0.0.1          
 127.0.0.1          nithin 
 127.0.0.1          kumar 
 


 Is this Okay?  (Y/N) 
 y 
 ****************************** 

 1Host Editor Finished 
 ****************************** 

.. code-block:: bash


 kevell@corp:/# ptdeploy hosteditor rm --yes 

 Do you want a non-default IP? Enter for 127.0.0.1 
 127.0.0.1 
 What URI do you want to affect to the hostfile? 
 nithin 
 ****************************** 
 
 1Host Editor Finished 
 ****************************** 


beneficios
---------------

* Multi usuario puede acceder a la vez. 
* El usuario puede agregar o quitar host. 
* No minúsculas.

