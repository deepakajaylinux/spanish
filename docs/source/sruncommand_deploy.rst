=============
Run Command
=============

sinopsis
------------

Los módulos de comando run permite a los usuarios ejecutar un comando del sistema operativo. Esto es principalmente se utiliza en piloto automático. Con este comando de ejecución el usuario puede especificar el comando, nombre del usuario y también para ejecutar el ya sea en el fondo o front-end. Vamos a ver los usos de la orden de marcha.

comando Ayuda
---------------------

El comando de ayuda describe los usos de la orden de marcha, su gran funcionalidad, sus parámetros alternativos, los comandos utilizados para ejecutar un comando y también acerca de la sintaxis para especificar el comando, nombre del usuario y también para ejecutar el ya sea en el fondo o front-end. A continuación se muestra la sintaxis utilizada para declarar el comando help.


.. code-block:: bash

	ptdeploy RunCommand help

La captura de pantalla siguiente muestra gráficamente sobre el funcionamiento del comando help.



.. code-block:: bash

 kevell@corp:/# ptdeploy runcommand help 

 ****************************** 

  This allows you to execute an Operating System command. This would primarily be used in an Autopilot. 

  RunCommand, runcommand, run-command 

        - execute 
        Execute a Command 
        example: ptdeploy run-command install --yes --command="ls -lah /tmp" --run-as-user="ubuntu" --background 

 ------------------------------ 
 End Help 
 ****************************** 


Cómo usar el comando Ejecutar
--------------------------------


La sintaxis utilizada para especificar el funcionamiento comando en se muestra a continuación.


.. code-block:: bash


	ptdeploy run-command install --yes --command="ls -lah /tmp" --run-as-user="ubuntu" --background 


.. cssclass:: table-bordered

 +------------------------------+-----------------------------------------------+-----------------------------------------------+
 | parámetro			| función					| uso	                                        |
 +==============================+===============================================+===============================================+
 |command="ls -lah /tmp"	| Permite al usuario especificar el      	| Mediante el uso de esto, el usuario puede	|
 |				| comando y su propósito.               	| especificar su propio comando de acuerdo a	|
 |                              |                                               | sus requerimientos.                           |
 +------------------------------+-----------------------------------------------+-----------------------------------------------+
 |run-as-user="ubuntu"		| Al usar este el usuario puede especificar     | Mediante el uso de esto, el usuario puede 	|
 |				| el nombre del usuario				| especificar su usuario requerido de           |
 |                              |                                               | acuerdo a sus requerimientos.                 |
 +------------------------------+-----------------------------------------------+-----------------------------------------------+
 |" --background		| Permite al usuario especificar dónde ejecutar | Mediante el uso de esto, el usuario puede  	|
 |				| el comando en particular , ya sea             | especificar su plataforma de uso de    	|
 |				| en el fondo o en el front-end .		| acuerdo a sus requerimientos.|		|
 +------------------------------+-----------------------------------------------+-----------------------------------------------+




La sintaxis y la mesa como se describió anteriormente puede ayuda al usuario cómo utilizar el comando ejecutar.

.. code-block:: bash

 kevell@corp:/# ptdeploy run-command install --yes --command="ls -lah /tmp" --run-as-user="ubuntu" --background 

 ******************************* 
 *   Golden Contact Computing  * 
 *         Run Command        * 
 ******************************* 
 Use NoHup?: (Y/N) 
 y 
 cd /home/karunakaran 
 su  ubuntu 
 nohup ls -lah /tmp & 
 exit 
 Creating /tmp/ptconfigure-temp-script-56005480696.sh 
 chmod 755 /tmp/ptconfigure-temp-script-56005480696.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-56005480696.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-56005480696.sh 
 No passwd entry for user 'ubuntu' 
 nohup: redirecting stderr to stdout 
 total 92K 
 drwxrwxrwt 10 root        root        4.0K Mar 20 17:06 . 
 drwxr-xr-x 29 root        root        4.0K Mar 20 16:18 .. 
 -rw-------  1 karunakaran karunakaran 4.1K Mar 20 11:27 .bamficonKEKGVX 
 -rw-------  1 karunakaran karunakaran 4.1K Mar 20 11:27 .bamficonMKENVX 
 -rw-------  1 karunakaran karunakaran 4.1K Mar 20 10:07 .bamficonN2NXVX 
 -rw-------  1 karunakaran karunakaran 4.1K Mar 20 11:27 .bamficonSM8KVX 
 -rwxr-xr-x  1 root        root          58 Mar 20 17:06 ptconfigure-temp-script-56005480696.sh 
 -rw-------  1 karunakaran karunakaran    0 Mar 20 09:50 config-err-UrGst6 
 -rw-------  1 root        root        1000 Mar 20 09:49 .configtest.KiQIacNN 
 -rw-r--r--  1 root        root          33 Mar 20 09:50 cxtracker.start.log 
 drwxr-xr-x  2 root        root        4.0K Mar 20 09:50 hsperfdata_root 
 drwxrwxrwt  2 root        root        4.0K Mar 20 09:50 .ICE-unix 
 -rw-r--r--  1 root        root           3 Mar 20 15:40 kk.txt 
 drwx------  2 karunakaran karunakaran 4.0K Mar 20 16:58 luh3hawd.tmp 
 srwxrwxrwx  1 mongodb     nogroup        0 Mar 20 09:49 mongodb-27017.sock 
 drwx------  2 karunakaran karunakaran 4.0K Mar 20 10:07 .org.chromium.Chromium.VRBmwX 
 srwxrwxr-x  1 karunakaran karunakaran    0 Mar 20 10:06 OSL_PIPE_1000_SingleOfficeIPC_8a32f718ac801a6e525d3030e0878e45 
 -rw-r--r--  1 root        root           0 Mar 20 15:42 papyrusfile 
 drwx------  2 karunakaran karunakaran 4.0K Mar 20 14:33 plugtmp 
 drwxr-xr-x  2 root        root        4.0K Mar 20 14:42 ServerBlocktemp 
 -rw-rw-r--  1 karunakaran karunakaran    0 Mar 20 09:50 unity_support_test.0 
 drwxr-xr-x  2 root        root        4.0K Mar 20 13:02 vhosttemp 
 -r--r--r--  1 root        root          11 Mar 20 09:49 .X0-lock 
 drwxrwxrwt  2 root        root        4.0K Mar 20 09:49 .X11-unix 
 Temp File /tmp/ptconfigure-temp-script-56005480696.sh Removed 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.gcsoftshop.co.uk for more 
 ****************************** 

 Single App Installer: 
 -------------------------------------------- 

 RunCommand: Success 

 ------------------------------ 
 Installer Finished 
 ****************************** 



beneficios
------------

* Los parámetros utilizados para declarar el comando help, instalación no son mayúsculas y minúsculas que es una ventaja añadida mientras que 
  comparado con otros. 
* Es acomodada en ambos OS ciento y así como en Ubuntu. 
* Los usuarios pueden especificar el comando, nombre del usuario y también para ejecutar el ya sea en el fondo o front-end. 
* El comando help guía a los usuarios en la forma de ejecutar el commando ejecutar un también su propósito.

