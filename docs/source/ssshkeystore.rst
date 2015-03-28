============
SshKeyStore 
============

Sinopsis
------------

SSH, o Secure Shell, es un protocolo de cifrado utilizado para administrar y comunicarse con los servidores. Cuando se trabaja con un servidor Linux, es probable que, usted pasa la mayor parte de su tiempo en una sesión de terminal conectado a su servidor a través de SSH.
Claves SSH son una manera de identificar los equipos de confianza, sin la participación de las contraseñas. Claves SSH proporcionan una manera segura de conectarse a un servidor basado en Unix Linux y.

Servidor OpenSSH soporta varios esquemas de autenticación. Los dos más populares son los siguientes:

Autenticación de contraseñas basado

Clave pública de autenticación basado. Es un método de seguridad alternativa al uso de contraseñas. Este método se recomienda en un VPS, nube, dedicado o incluso de servidor basado en casa.

En el método basado en clave pública puede iniciar sesión en hosts remotos y el servidor, y transferir archivos a ellos, sin usar las contraseñas de la cuenta. Este módulo le permite encontrar las credenciales para una clave en una máquina.

Ayuda Comando
---------------------

Este comando ayuda a determinar el uso del módulo sshkeystore. El usuario se llega a saber acerca de la diferente forma / formato de ejecutar este módulo. Este comando guía al usuario final a conocer el propósito de este comando. A continuación dado son el mando y la pantalla del mismo.

.. code-block:: bash

	ptconfigure sshkeystore help

La captura de pantalla para el comando anterior se enumeran a continuación,

.. code-block:: bash

 kevell@corp:/# ptconfigure SshKeyStore help
 ******************************

 This command allows you to find credentials for a key on a machine

 SshKeyStore, sshkeystore, ssh-key-store

       - find
       Add an SSH Public Key to an account
       example: ptconfigure ssh-key-store find --key=daveylad
       example: ptconfigure ssh-key-store find --key=daveylad --prefer=user

 ------------------------------
 End Help
 ******************************


encontrar
----------

Cuando el usuario necesita para agregar una clave pública SSH a una cuenta, el siguiente comando dado se ejecutará el proceso.

.. code-block:: bash

	ptconfigure ssh-key-store find --key=daveylad

.. code-block:: bash

 kevell@corp:/# ptconfigure ssh-key-store find --key=id_rsa
 [Pharaoh Logging] Trying keystore keys
 Enter User home directory:
 /
 [Pharaoh Logging] User key not found at //.ssh/id_rsa
 Enter User home directory:
 /
 [Pharaoh Logging] Other User key not found at //.ssh/id_rsa
 [Pharaoh Logging] Root key found at /root/.ssh/id_rsa
 ******************************


 SshHarden Modifications:
 --------------------------------------------

 Ssh Key Store: Success
 /root/.ssh/id_rsa

 ------------------------------
 SshHarden Mods Finished
 ******************************




Parámetro Alternativa
-----------------------------

Hay tres parámetros alternativos que pueden ser utilizados en la línea de comandos.

SshKeyStore, sshkeystore, ssh-key-store

ejemplo: ptconfigure sshkeystore help /ptconfigure ssh-key-store help


Beneficios
-----------

* La clave privada SSH (la parte que se puede proteger frase de contraseña), nunca se expone en la red. La frase de contraseña sólo se utiliza 
  para descifrar la clave de la máquina local. Esto significa que bruta basada en la red forzando no será posible en contra de la frase de 
  contraseña.
* La clave privada se mantiene dentro de un directorio restringido. El cliente SSH no reconocerá las claves privadas que no se guardan en 
  directorios restringidos. La clave en sí también debe haber restringido los permisos (de lectura y escritura sólo está disponible para el 
  propietario). Esto significa que los demás usuarios del sistema no pueden fisgonear.
* Cualquier atacante con la esperanza de romper el SSH frase de contraseña de clave privada ya debe tener acceso al sistema. Esto significa que 
  ya tendrán acceso a su cuenta de usuario o la cuenta de root. Si se encuentra en esta posición, la frase de contraseña puede evitar que el 
  atacante de la tala de inmediato en los demás servidores. Esperamos que esto le dará tiempo para crear y poner en práctica un nuevo par de 
  claves SSH y eliminar el acceso de la clave comprometida.
