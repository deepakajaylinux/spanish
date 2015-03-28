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


.. code-block:: bash

 kevell@corp:/# ptconfigure ssh-key-install public-key
 Install Ssh Key Install? (Y/N) 
 y
 Enter Username to install SSH Key to:
 kevell
 [Pharaoh Logging] SSH Directory exists, so not creating.
 [Pharaoh Logging] /home/murali/.ssh/authorized_keys exists, so not creating.
 Enter Public Key:
 ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAACAQCowttwfBq3Y6h+KwdXiGC3orDaTivgZszxT0s6+xUW9iL5F1yXFTy++XAOzIxYBa1uu2EyphXMnJIeYyczlMwpVDPlhQvvRthLRSCQ4u6aBOnQNx2d4RihCokWaobmpv4rN+XD0ZmIMvshkEDc/KKue3kplf80sNpiuehaA1G0L9vnsW2Ndccy9N2983ASwKJB1s082hquw+TOOJOvqbS0G10Ezev3r3y3OwmQKsTA9REqsZsryZVpmtYoKLXwA3tVqSOn8v2+/xqJN7aVi35cDtGTDL7KpYDQpamCQmOz05uDInwiEh6N6BRLvBJlQpe7HuKe9Sd3o3Ns+Unr8IandPF6eTaS/mFcI5o672qXZIY6GSxyZ+YtkJhgogig2J1PKspr3kqLGulKSTssF+fvUgkej2H20Bf0YqrVAeJpqYYiCmlA0pQHDnpWoGpNcAAGDgi6M8Fs7Lb3Pt7l1DLyr78WJGfJUgr9hqocPUZKPLQB/SqS0QWKhdn21nmnLIpEUJZhBLPmxMOOMUUbYjI7jCCT+I0hO2zuRRJMzgkyZEvuj/dOHDSOANsRUMqfkb942A15RyrO6fXpHrttckq+6tRYjXgLI8aZd+ZI5ZSF73IT33lUKoFlXY7vF/6rNPvQtr9DOGTvGP3CTnx7MlBW9c/x61R2NoMRXlNhePjmOQ== mani
 [Pharaoh Logging] Key does not exist in file, so adding.
 PHP Notice:  Undefined property: Model\SshKeyInstallUbuntu::$user in /opt/ptconfigure-enterprise/src/Modules/SshKeyInstall/Model/SshKeyInstallUbuntu.php on line 113
 [Pharaoh Logging] Changing ownership of /home/murali/.ssh/authorized_keys to user .
 [Pharaoh Logging] Restarting ssh service
 ssh stop/waiting
 ssh start/running, process 8043
 ******************************


 SshKeyInstall Modifications:
 --------------------------------------------

 Ssh Key Install: Success

 ------------------------------
 SshKeyInstall Mods Finished
 ******************************




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
