=======
SFTP
=======


sinopsis
-------------

Este módulo ayuda a transferir archivos de un sistema a otro. Puede cargar o descargar los archivos en el sistema. La automatización es posible. Y opciones están disponibles en este módulo. También gestiona caja virtual. Es fácil de usar con Ubuntu y ciento OS.


comando Ayuda
-------------------------

Ayuda comando utilizado para buscar información sobre un comando especificado. Para obtener más información sobre los cambios de funcionalidad de Secure File Transfer Protocol(SFTP) bajo ptvirtualize el usuario puede utilizar este comando de ayuda.


.. code-block:: bash

	ptvirtualize  sftp help


La captura de pantalla siguiente guía.


.. code-block:: bash

 kevell@corp:/# ptvirtualize sftp help

 ******************************
 Pharaoh Tools - ptvirtualize
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


parámetros alternativos
---------------------------------

Hay dos parámetros alternativos están disponibles. Son SFTP y sftp. En lugar de utilizar sftp, el usuario puede utilizar SFTP.



Put
------

La transferencia de archivos puede hacerse desde lo local al servidor remoto. Esta opción le pide los detalles de usuario para servidores. El siguiente comando utilizado para la opción de venta.



.. code-block:: bash

	ptvirtualize  sftp put – yes –source=”/tmp/file” – target=”/home/user/file”

La siguiente captura de pantalla denota el uso de este comando.



.. code-block:: bash

 kevell@corp:ptconfigure sftp put
 
 SFTP on Server group? (Y/N) 
 Y
 Please Enter SSH Timeout in seconds
 90
 Please Enter remote SSH Port
 22
 Use Environments Configured in Project? (Y/N) 
 N
 [Pharaoh Logging] Attempting to load SFTP connections...
 Enter local source file path
 /root/vv
 Enter remote target file path
 /root/gg/vv
 [Pharaoh Logging] Opening SFTP Connections...
 [Pharaoh Logging] All SFTP Puts Completed
 ******************************


SFTP on server group? Y/N

Si el usuario de entrada y luego


SSh timeout section?

El usuario debe introducir el valor

Please enter remote ssh port

Default value is 22. El usuario puede introducir cualquier valor

Enter environments configured in project? (Y/N)

El usuario tiene que entrar y luego empieza a cargar.


Enter local source file path?

El usuario tiene que entrar en la ruta del archive


Entonces todo estará conectado.

Si el usuario de entrada como N, puede ser terminada.



Get
-------

Transferencia de archivos puede hacerse desde la remota al servidor local. Pide al usuario que introduzca el grupo de servidores. El siguiente comando utilizado para tener opción.


.. code-block:: bash

	ptvirtualize  sftp get – yes –source=”/tmp/file” – target=”/home/user/file”

La siguiente captura de pantalla lo explica todo.



.. code-block:: bash

 kevell@corp:/# ptconfigure sftp get
 SFTP on Server group? (Y/N) 
 Y
 Please Enter SSH Timeout in seconds

 Please Enter remote SSH Port

 Use Environments Configured in Project? (Y/N) 

 [Pharaoh Logging] Attempting to load SFTP connections...
 Enter remote source file path

 Enter local target file path

 [Pharaoh Logging] Opening SFTP Connections...
 [Pharaoh Logging] All SFTP Gets Completed
 ******************************


 Shell Result: Success
 SFTP Get

 ------------------------------
 Installer Finished
 ******************************


SFTP on server group? Y/N

Si el usuario de entrada y luego

SSh timeout section?

El usuario debe introducir el valor

Please enter remote ssh port

Default value is 22. El usuario puede introducir cualquier valor

Enter environments configured in project? (Y/N)

El usuario tiene que entrar y luego empieza a cargar.

Enter local target file path?

El usuario tiene que entrar en la ruta del archivo local blanco

Entonces todo estará conectado.

Si el usuario de entrada como N, puede ser terminada. Las siguientes imágenes muestran su función.


.. code-block:: bash

 kevell@corp:/# ptconfigure sftp get
 SFTP on Server group? (Y/N) 
 N
 ******************************


 Shell Result: Failure
 SFTP Get

 ------------------------------
 Installer Finished
 ******************************



Options
-------------

.. cssclass:: table-bordered

 +------------------------+---------------------------+--------------------------------------------------------------+
 | parámetros		  | parámetros alternativos   | comentarios						     |
 +========================+===========================+==============================================================+
 |put			  | SFTP, sftp        	      | Fuente para apuntar -El archivo puede transferirse           |
 +------------------------+---------------------------+--------------------------------------------------------------+
 |get			  | SFTP, sftp                | Ruta de acceso a la fuente : el archivo se puede descargar   |
 |                        |                           | desde el sistema remoto|                                     |
 +------------------------+---------------------------+--------------------------------------------------------------+




Beneficios
-------------

* Multi server de área remota. 
* Especifica el archivo no está disponible error mensaje llegará. 
* Accesibilidad es difícil sin permiso. 
* Automáticamente sobrescribir en caso de ya en caso de archivo existe. 
* No caso sensible. 
* El secreto y la seguridad es posible.

