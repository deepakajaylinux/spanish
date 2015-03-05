============
SshKeygen
============

sinopsis
----------

Es una ayuda para generar el valor de la clave. Este módulo es tener dos tipos de clave. Son DSA, RSA. dsa valor clave de bits es 1024 y el valor del bit de claves RSA es más de 768. A continuación, sólo puede funcionar. Es muy útil en la tarea con Ubuntu y CentOS.

Ayuda Comando
---------------------

Este comando ayuda explica acerca de la instalación de un módulo en particular. El comando de ayuda es fácil de manejar por el usuario final. El siguiente comando guió al usuario acerca de la instalación.

.. code-block:: bash
		
		ptconfigure Sshkeygen help

Después de dar el comando, el comando listará las opciones de ayuda. Las siguientes capturas de pantalla darán efecto visual para el uso de este módulo.

.. code-block:: bash

 kevell@corp:/# ptconfigure SshKeygen help
 ******************************


  This command allows you to install an SSH Key Pair.

  SshKeygen, ssh-keygen, sshkeygen

        - install
        Installs a new SSH Key
        example: ptconfigure ssh-keygen install
        example: ptconfigure ssh-keygen install --yes --bits=4096 --type=rsa --path="/home/dave/.ssh/id_rsa" --comment="Daves"

        - uninstall
        Removes an SSH Key
        example: ptconfigure ssh-keygen uninstall

 ------------------------------
 End Help
 ******************************


instalación
-------------

La instalación no es un proceso difícil de instalar este módulo bajo ptconfigure por la mera utilización de la orden dada a continuación,

.. code-block:: bash

		ptconfigure sshkeygen install

Después de introducir los insumos claves SSH gen se ha instalado correctamente. Las siguientes capturas de pantalla darán efecto visual para el uso de este módulo.

.. code-block:: bash

 kevell@corp:/# ptconfigure ssh-keygen install
 Install SSH Key Generation? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         sshkeygen!        *
 *******************************
 Enter number of bits for SSH Key (multiple of 1024):
 1024
 Choose Key type (rsa/dsa)
 (0) rsa 
 (1) dsa 
 1
 Enter path to store private key (public key will be same with .pub):
 /root/SSH/abcd
 Plain text comment appended to public key. None is fine
 kevell
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 SshKeygen: Success
 ------------------------------
 Installer Finished
 ******************************

Opciones
---------

.. cssclass:: table-bordered

 +------------------------+-----------------------------+-----------+----------------------------------------------------------+
 | Parámetros             | Directorio (por defecto)    | Opciones  | Comentarios                                              |
 +========================+=============================+===========+==========================================================+
 |Install Key Generation  | Yes                         |           | Se instalará la generación de claves bajo ptconfigure    |
 +------------------------+-----------------------------+-----------+----------------------------------------------------------+
 |Install Key Generation  | No                          |           | El proceso se cierra.                                    |
 +------------------------+-----------------------------+-----------+----------------------------------------------------------+
 |Choose key type         | rsa                         | 0         | Se instalará la generación de claves bajo tipo de clave  |
 |                        |                             |           | seleccionado                                             |
 +------------------------+-----------------------------+-----------+----------------------------------------------------------+
 |Choose key type         | dsa                         | 1         | Se instalará la generación de claves bajo tipo de clave  |
 |                        |                             |           | seleccionado                                             |
 +------------------------+-----------------------------+-----------+----------------------------------------------------------+
 |path                    | /root/ssh/filename          |           | Se va a crear el archivo con la clave pública y privada| |
 +------------------------+-----------------------------+-----------+----------------------------------------------------------+



Beneficios
--------------

Podemos trabajar de un lugar remoto. El usuario tiene que indicar al sistema para la ruta. Generación automática es posible. Podemos añadir el archivo cuando lo necesite. Podemos compartir las llaves sin contraseña. No entre mayúsculas y minúsculas.
