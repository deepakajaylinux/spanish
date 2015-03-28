=======
SFTP
=======

sinopsis
------------

  Este módulo ayudar en la transferencia de archivos de un sistema a otro. Se puede cargar o descargar los archivos en el sistema. La automatización es posible. PUT y GET opciones están disponibles en este módulo. En él se especifica la configuración de su entorno. Es fácil de usar con Ubuntu y CentOS.

comando Ayuda
--------------------

Comando que se utiliza para encontrar información sobre un comando especificado Ayuda. Para obtener más información acerca de los cambios a la funcionalidad de SFTP podemos utilizar este comando ayuda.

.. code-block:: bash

 		ptconfigure sftp help

La siguiente captura de pantalla te guiará.

.. code-block:: bash


 kevell@corp:/# ptconfigure sftp help
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

instalación
-------------

Como empresa y como individuos, SFTP se ha dedicado a responder a los retos tecnológicos de cada socio, el cumplimiento de sus requisitos de ingeniería, y la satisfacción de sus objetivos de negocio. Es un proceso obvio para instalar el módulo SFTP bajo ptconfigure sólo por el uso de la orden dada a continuación,

.. code-block:: bash

		ptconfigure SFTP put


.. code-block:: bash

 kevell@corp:/# ptconfigure sftp put

 SFTP on Server group? (Y/N) 
 y
 Please Enter SSH Timeout in seconds
 100
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
 192.168.1.4
 Please Enter SSH User
 murali
 Please Enter Server Password or Key Path
 123456
 Add Another Server? (Y/N) 
 n
 [Pharaoh Logging] Attempting to load SFTP connections...
 [Pharaoh Logging] Connection to Server 192.168.1.4 failed.
 Enter local source file path
 /home/kevells/Desktop/graphs
 Enter remote target file path
 /home/murali/Desktop/graphs
 [Pharaoh Logging] Opening SFTP Connections...
 [192.168.1.4]Connection failure. Will not execute commands on this box..
 [Pharaoh Logging] All SFTP Puts Completed
 ******************************



 SFTP Put: Success

 ------------------------------
 Installer Finished
 ******************************

.. code-block:: bash



 kevell@corp:/# ptconfigure sftp get

 SFTP on Server group? (Y/N) 
 y
 Please Enter SSH Timeout in seconds
 100
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
 192.168.1.4
 Please Enter SSH User
 murali
 Please Enter Server Password or Key Path
 123456
 Add Another Server? (Y/N) 
 n
 [Pharaoh Logging] Attempting to load SFTP connections...
 [Pharaoh Logging] Connection to Server 192.168.1.4 failed.
 Enter remote source file path
 /home/murali/Desktop/graphs
 Enter local target file path
 /hoem/kevells/Desktop/graphs1
 [Pharaoh Logging] Opening SFTP Connections...
 [Pharaoh Logging] [192.168.1.4] Executing SFTP Get...
 [Pharaoh Logging] No SFTP Object
 [Pharaoh Logging] 
 [Pharaoh Logging] [192.168.1.4] SFTP Get Completed...
 [Pharaoh Logging] All SFTP Gets Completed
 ******************************


 Shell Result: Success
 SFTP Get

 ------------------------------
 Installer Finished
 ******************************




Opciones
-----------

.. cssclass:: table-bordered

 +--------------------+----------------------------+-------------------------------------------------------------------------+
 | Parámetros         | Parámetro Alternativa      | Comentarios                                                             |
 +====================+============================+=========================================================================+
 |put                 | SFTP, sftp                 | Source to target_El archivo puede transferirse del origen al destino.   |
 +--------------------+----------------------------+-------------------------------------------------------------------------+
 |get                 | SFTP, sftp                 | Path to source_El archivo se puede recoger del sistema remoto.|         |
 +--------------------+----------------------------+-------------------------------------------------------------------------+


Beneficios
-------------

* Servidor Multi de área remota.
* El archivo especificado no es mensaje de error disponibles vendrá.
* Accessability es difícil sin permiso.
* Sobrescribe automáticamente en caso de que ya en el caso de archivo existir.
* No mayúsculas y minúsculas.
* El secreto y la seguridad es posible.

Resolución de problemas de la tecnología a los clientes más exigentes y permitiendo su éxito es la misión SFTP y pasión.
