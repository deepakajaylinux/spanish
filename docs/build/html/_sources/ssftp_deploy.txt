======
SFTP
======



Sinopsis
--------------

          Este módulo ayuda a transferir archivos de un sistema a otro. Puede cargar o descargar los archivos en el sistema. La automatización es posible. Y opciones están disponibles en este módulo. Especifica la configuración de su entorno. Es fácil de usar con Ubuntu y ciento OS.



comando Ayuda
-----------------------

Ayuda comando utilizado para buscar información sobre un comando especificado. Para obtener más información sobre los cambios de funcionalidad de SFTP podemos usar este comando de ayuda.


.. code-block:: bash
   
	ptdeploy SFTP help


La captura de pantalla siguiente guía.


.. code-block:: bash

 kevell@corp:/# ptdeploy sftp help
 ******************************


  This command handles SFTP Transfer Functions.

  SFTP, sftp

        - put
        Will ask you for details for servers, then copy a file or directory from local to remote
        example: ptconfigure sftp put
        example: ptconfigure sftp put --yes --environment-name=staging --source="/tmp/file" --target="/home/user/file"
        example: ptconfigure sftp put --yes --source="/tmp/file" --target="/home/user/file" # will ask for server details

        - get
        Will ask you for details for servers, then copy a file or directory from remote to local
        example: ptconfigure sftp get
        example: ptconfigure sftp get --yes --environment-name=staging --source="/tmp/file" --target="/home/user/file"
        example: ptconfigure sftp get --yes --source="/tmp/file" --target="/home/user/file" # will ask for server details

 ------------------------------
 End Help
 ******************************



Instalación
-----------------

Como empresa y como individuos, SFTP se ha dedicado a cumplir retos tecnológicos de cada socio, cumpliendo con sus requerimientos de ingeniería y satisfacer sus objetivos de negocio. Es un proceso obvio instalar módulos SFTP bajo ptdeploy sólo mediante el comando siguiente,


.. code-block:: bash
  
	ptdeploy SFTP  install 


Después de dar el comando entonces el sistema plantea la cuestión que,

Install SFTP server group? Y/N

Si el usuario de entrada y luego


SSh timeout section?

El usuario debe introducir el valor

Please enter remote ssh port

Default value is 22. El usuario puede introducir cualquier valor

Enter server host IP? 

El usuario tiene que introducir nombre de usuario, contraseña y ruta clave.

Add another server?

Si la entrada del usuario y tiene que introducir el nuevo nombre del servidor

Entonces todo estará conectado.

Si el usuario de entrada como N anterior encontrará el nombre del servidor.



.. code-block:: bash

 kevell@corp:/# ptdeploy sftp put 

 SFTP on Server group? (Y/N) 
 y 
 Please Enter SSH Timeout in seconds 
 20 
 Please Enter remote SSH Port 
 22 
 *********************************** 
 *   Due to a software limitation, * 
 *    The user that you use here   * 
 *  will have their command prompt * 
 *    changed to PHARAOHPROMPT     * 
 *  ... I'm working on that one... * 
 *  Exit program to stop (CTRL+C)  * 
 *********************************** 
 Enter Server Info: 
 Please Enter SSH Server Target Host Name/IP 
 192.168.1.14 
 Please Enter SSH User 
 karthik 
 Please Enter Server Password or Key Path 
 123456 
 Add Another Server? (Y/N) 
 n 
 [Pharaoh Logging] Attempting to load SFTP connections... 
 [Pharaoh Logging] Connection to Server 192.168.1.14 successful. 
 Enter local source file path 
 /home/karunakaran/Desktop/server.odt 
 Enter remote target file path 
 /home/karthik/Desktop/server.odt 
 [Pharaoh Logging] Opening SFTP Connections... 
 [Pharaoh Logging] [192.168.1.14] Executing SFTP Put... 
 [Pharaoh Logging] 1 
 [Pharaoh Logging] [192.168.1.14] SFTP Put Completed... 
 [Pharaoh Logging] All SFTP Puts Completed 
 ****************************** 

 SFTP Put: Success 

 ------------------------------ 
 Installer Finished 
 ****************************** 

.. code-block:: bash


 kevell@corp:/# ptdeploy sftp put --yes --environment-name=karthik --source="/tmp/kk.txt" --target="/tmp/kk.txt" 

 Please Enter SSH Timeout in seconds 
 20 
 Please Enter remote SSH Port 
 22 
 [Pharaoh Logging] Attempting to load SFTP connections... 
 [Pharaoh Logging] Connection to Server 192.168.1.14 successful. 
 [Pharaoh Logging] Opening SFTP Connections... 
 [Pharaoh Logging] [192.168.1.14] Executing SFTP Put... 
 [Pharaoh Logging] 1 
 [Pharaoh Logging] [192.168.1.14] SFTP Put Completed... 
 [Pharaoh Logging] All SFTP Puts Completed 
 ****************************** 

 SFTP Put: Success 

 ------------------------------ 
 Installer Finished 
 ****************************** 

.. code-block:: bash


 kevell@corp:/# ptdeploy sftp put --yes --source="/home/karunakaran/Desktop/readme.txt" --target="/home/karthik/Desktop/readme.txt" 

 Please Enter SSH Timeout in seconds 
 20 
 Please Enter remote SSH Port 
 22 
 *********************************** 
 *   Due to a software limitation, * 
 *    The user that you use here   * 
 *  will have their command prompt * 
 *    changed to PHARAOHPROMPT     * 
 *  ... I'm working on that one... * 
 *  Exit program to stop (CTRL+C)  * 
 *********************************** 
 Enter Server Info: 
 Please Enter SSH Server Target Host Name/IP 
 192.168.1.14 
 Please Enter SSH User 
 karthik 
 Please Enter Server Password or Key Path 
 123456 
 Add Another Server? (Y/N) 
 n 
 [Pharaoh Logging] Attempting to load SFTP connections... 
 [Pharaoh Logging] Connection to Server 192.168.1.14 successful. 
 [Pharaoh Logging] Opening SFTP Connections... 
 [Pharaoh Logging] [192.168.1.14] Executing SFTP Put... 
 [Pharaoh Logging] 1 
 [Pharaoh Logging] [192.168.1.14] SFTP Put Completed... 
 [Pharaoh Logging] All SFTP Puts Completed 
 ****************************** 

 SFTP Put: Success 

 ------------------------------ 
 Installer Finished 
 ****************************** 


.. code-block:: bash


 kevell@corp:/# ptdeploy sftp get 

 SFTP on Server group? (Y/N) 
 y 
 Please Enter SSH Timeout in seconds 
 200 
 Please Enter remote SSH Port 
 22 
 *********************************** 
 *   Due to a software limitation, * 
 *    The user that you use here   * 
 *  will have their command prompt * 
 *    changed to PHARAOHPROMPT     * 
 *  ... I'm working on that one... * 
 *  Exit program to stop (CTRL+C)  * 
 *********************************** 
 Enter Server Info: 
 Please Enter SSH Server Target Host Name/IP 
 192.168.1.14 
 Please Enter SSH User 
 karthik 
 Please Enter Server Password or Key Path 
 123456 
 Add Another Server? (Y/N) 
 n 
 [Pharaoh Logging] Attempting to load SFTP connections... 
 [Pharaoh Logging] Connection to Server 192.168.1.14 successful. 
 Enter remote source file path 
 /tmp/testing 
 Enter local target file path 
 /opt/testr 
 [Pharaoh Logging] Opening SFTP Connections... 
 [Pharaoh Logging] [192.168.1.14] Executing SFTP Get... 
 [Pharaoh Logging] 1 
 [Pharaoh Logging] [192.168.1.14] SFTP Get Completed... 
 [Pharaoh Logging] All SFTP Gets Completed 
 ****************************** 

 Shell Result: Success 
 SFTP Get 
 
 ------------------------------ 
 Installer Finished 
 ****************************** 

.. code-block:: bash

 kevell@corp:/# ptdeploy sftp get --yes --environment-name=karthik --source="/tmp/testing" --target="/opt/testr" 

 Please Enter SSH Timeout in seconds 
 200 
 Please Enter remote SSH Port 
 22 
 [Pharaoh Logging] Attempting to load SFTP connections... 
 [Pharaoh Logging] Connection to Server 192.168.1.14 successful. 
 [Pharaoh Logging] Opening SFTP Connections... 
 [Pharaoh Logging] [192.168.1.14] Executing SFTP Get... 
 [Pharaoh Logging] 1 
 [Pharaoh Logging] [192.168.1.14] SFTP Get Completed... 
 [Pharaoh Logging] All SFTP Gets Completed 
 ****************************** 

 Shell Result: Success 
 SFTP Get 
 
 ------------------------------ 
 Installer Finished 
 ****************************** 
 

.. code-block:: bash

 kevell@corp:/# ptdeploy sftp get --yes --source="/tmp/testing" --target="/opt/testr" 

 Please Enter SSH Timeout in seconds 
 200 
 Please Enter remote SSH Port 
 22 
 *********************************** 
 *   Due to a software limitation, * 
 *    The user that you use here   * 
 *  will have their command prompt * 
 *    changed to PHARAOHPROMPT     * 
 *  ... I'm working on that one... * 
 *  Exit program to stop (CTRL+C)  * 
 *********************************** 
 Enter Server Info: 
 Please Enter SSH Server Target Host Name/IP 
 192.168.1.14 
 Please Enter SSH User 
 karthik 
 Please Enter Server Password or Key Path 
 123456 
 Add Another Server? (Y/N) 
 n 
 [Pharaoh Logging] Attempting to load SFTP connections... 
 [Pharaoh Logging] Connection to Server 192.168.1.14 successful. 
 [Pharaoh Logging] Opening SFTP Connections... 
 [Pharaoh Logging] [192.168.1.14] Executing SFTP Get... 
 [Pharaoh Logging] 1 
 [Pharaoh Logging] [192.168.1.14] SFTP Get Completed... 
 [Pharaoh Logging] All SFTP Gets Completed 
 ****************************** 

 Shell Result: Success 
 SFTP Get 

 ------------------------------ 
 Installer Finished 
 ****************************** 



Opciones
------------


.. cssclass:: table-bordered

 +-------------+-------------------------+----------------------+---------------------------------------------------------+
 | parámetros  | parámetros alternativos | opciones             | comentarios                                             |
 +=============+=========================+======================+=========================================================+
 |put	       | SFTP, sftp              | Fuente para apuntar  | El archivo puede transferirse                           |
 +-------------+-------------------------+----------------------+---------------------------------------------------------+
 |get	       | SFTP, sftp              | camino a la fuente   | El archivo se puede descargar desde el sistema remoto|  |
 +-------------+-------------------------+----------------------+---------------------------------------------------------+




Beneficios
----------

* Multi server de área remota. 
* Especifica el archivo no está disponible error mensaje llegará. 
* Accesibilidad es difícil sin permiso. 
* Automáticamente sobrescribir en caso de ya en caso de archivo existe. 
* No caso sensible. 
* El secreto y la seguridad es posible.

 Resolución de los clientes más difíciles problemas de tecnología y permitiendo su éxito es la misión SFTP y pasión.




