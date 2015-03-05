===============
SshKeyInstall
===============

sinopsis
----------------

Clave ssh Instalar utiliza para instalar clave ssh para un nuevo usuario. Una autenticación es más segura que la autenticación de contraseña. Esto es particularmente importante si el sistema es visible en Internet. Con la autenticación de clave pública, la entidad de autenticación tiene una clave pública y una clave privada. Cada clave es un gran número con propiedades matemáticas especiales. Es adecuado con Ubuntu y CentOS.

comando Ayuda
-------------------------

Guía el comando de ayuda a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en el SSHKEY instalar el módulo. En él se enumeran los parámetros alternativos de módulo Sshkeyinstall. También describe la sintaxis para instalar el módulo Sshkeyinstall. El comando de ayuda para el módulo Sshkeyinstall se muestra a continuación.

.. code-block:: bash
 
		ptconfigure Sshkeyinstall help


La sintaxis para declarar el comando de ayuda no es caso sensible que una ventaja añadida es. La siguiente captura de pantalla a visualizar al usuario sobre el comando de ayuda bajo Sshkeyinstall.

.. code-block:: bash

 kevell@corp:/# ptconfigure SshKeyInstall help

 ******************************


  This command allows you to install an SSH Public key for a user

  SshKeyInstall, sshkeyinstall, ssh-key-install

        - public-key
        Add an SSH Public Key to an account
        example: ptconfigure ssh-key-install public-key
        example: ptconfigure ssh-key-install public-key --yes --public-key-data="zzzzz"
        example: ptconfigure ssh-key-install public-key --yes --public-key-file="id_rsa.pub" --user-name=dave

 ------------------------------
 End Help
 ******************************


instalación
------------------

Instalación incluye la instalación de Sshkeyinstall requerida para hacer la instalación en una versión actualizada. Es un proceso de manifiesto para instalar módulo Sshkeyinstall bajo ptconfigure Sshkeyinstall sólo por el uso de la orden dada a continuación,

.. code-block:: bash

 		ptconfigure  Sshkeyinstall  public-key

Después de vitalizar el comando se catequizar entrada.

Cuando la entrada de usuario como si automáticamente se instalará Sshkeyinstall con la comprobación del sistema. Si no salir de la instalación. La siguiente captura de pantalla demonstSshkeyinstallte Sshkeyinstall ella.

Opciones
--------------

.. cssclass:: table-bordered

 +------------------------+---------------------------------------------+--------------+-------------------------------------------------+
 | Parámetros             | Parámetro Alternativa                       | Opciones     | Comentarios                                     |
 +========================+=============================================+==============+=================================================+
 |Install Sshkeyinstall?  | En lugar de utilizar SshKeyInstall podemos  | Y(Yes)       | Si el usuario desea continuar el proceso de     |
 |(Y/N)                   | utilizar Sshkeyinstall, ssh-key-install     |              | instalación se puede introducir como Y.         |
 +------------------------+---------------------------------------------+--------------+-------------------------------------------------+
 |Install Sshkeyinstall?  | En lugar de utilizar SshKeyInstall podemos  | N(No)        | Si el usuario desea abandonar el proceso de     |
 |(Y/N)                   | utilizar Sshkeyinstall, ssh-key-install     |              | instalación se puede introducir como N.|        |
 +------------------------+---------------------------------------------+--------------+-------------------------------------------------+


Beneficios
----------------

* Sshkeyinstall es acomodado en Ubuntu y CentOS
* Sshkeyinstall puede atraco sensibilidad no caso
* Sshkeyinstall es flexible
* Sshkeyinstall utilizado instalar sshkey
* Sshkeyinstall apoya la seguridad
