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

Después de dar la orden, entonces el sistema va a plantear la cuestión,

Install SFTP server group? Y/N

Si la entrada del usuario como Y entonces

SSh timeout section?

El usuario tiene que introducir el valor

Please enter remote ssh port

El valor predeterminado es 22. El usuario puede introducir cualquier valor

Enter server host IP? 

El usuario tiene que introducir nombre de usuario, contraseña y ruta de la clave.

Add another server?

Si la entrada del usuario como Y él tiene que ingresar el nuevo nombre de servidor

Entonces todo estará conectado.

Si se puede acceder a la entrada del usuario como N anterior nombre del servidor.

La siguiente captura de pantalla te guiará.

.. code-block:: bash

 kevell@corp:/# ptconfigure sftp put

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
