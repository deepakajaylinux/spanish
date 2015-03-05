============
Sudonopass
============

sinopsis
---------------

Sudonopass utiliza para ejecutar un comando en particular con permisos de root. Lo interesante es que cuando el usuario sudo uso de un comando en particular, el sistema solicita al usuario la contraseña del usuario actual. Una vez que el usuario introduzca la contraseña, el comando se ejecuta con privilegios de root. Esto es adecuado para trabajar con Ubuntu y CentOS.

comando Ayuda
-----------------------

Este comando ayuda a guiar al usuario sobre el módulo sudonopass. Esto es adecuado para todo tipo de usuarios de negocios. El comando help muestra una breve lista de los comandos integrados en el módulo sudonopass. La siguiente captura de pantalla que enumera.

.. code-block:: bash

	kevell@corp:/# ptconfigure SudoNoPass help
	******************************


	 This command allows you to add an entry to the system sudo file that will
	 allow your user to have passwordless sudo. This is required for
	 quite a few of the  builds provided by Golden Contact, as
	 will perform test execution, software installs and more, silently.

	 SudoNoPass, sudonopass, sudo-nopass, sudo-passwordless

        - install
        Installs the sudo without password entry
        example: ptconfigure sudo-nopass install

	------------------------------
	End Help
	******************************

instalación
------------------

Utilice este módulo para instalar sudonopass en paquetes del sistema Ubuntu Linux.

.. code-block:: bash

          ptconfigure sudonopass install

Install sudonopass ?(Y/N)

Cuando el usuario se da de entrada, como si automáticamente se instalará configurar el pase de acceso raíz para todos. La siguiente captura de pantalla de lo explicará.

.. code-block:: bash

	kevell@corp:/# ptconfigure sudo-nopass install
	Install Sudo w/o Pass for User? (Y/N) 
	y
	*******************************
	*        Pharaoh Tools        *
	*         Sudo NoPass!        *
	*******************************
	Enter User To Install As:
	Kevells
	The following will be written to /etc/sudoers
	Please check if it looks wrong
	You may not be able to use Sudo if it is incorrect!!!
	Kevells ALL=NOPASSWD: ALL
	Is this okay? (Y/N) 
	y
	... All done!
	*******************************
	Thanks for installing , visit www.pharaohtools.com for more
	******************************
	
	
	Single App Installer:
	--------------------------------------------
	SudoNoPass: Success
	------------------------------
	Installer Finished
	******************************

Opciones
------------

.. cssclass:: table-bordered

 +--------------------------+----------------------------------------+-------------------------+--------------------------------------------+
 | Parámetros               | Parámetro Alternativa                  | Dirctory (por defecto)  | Comentarios                                |
 +==========================+========================================+=========================+============================================+
 |Install Sudo w/o Pass     | SudoNoPass, sudonopass, sudo-nopass,   | Y(Yes)                  | Si el usuario desea continuar el proceso   |
 |for User? (Y/N)           | sudo-passwordless                      |                         | de instalación se puede introducir como Y. |
 +--------------------------+----------------------------------------+-------------------------+--------------------------------------------+
 |Install Sudo w/o Pass     | SudoNoPass, sudonopass, sudo-nopass,   | N(No)                   | Si el usuario desea abandonar el proceso   |
 |for User? (Y/N)           | sudo-passwordless                      |                         | de instalación se puede introducir como N| |
 +--------------------------+----------------------------------------+-------------------------+--------------------------------------------+


Beneficios
------------

* Sudonopass se asegura de que los privilegios de root están allí para un comando específico (o por un tiempo específico) y no para la sesión 
  completa que puede resultar en el mal uso accidental de los privilegios de root.
* El usuario puede utilizar sudonopass incluso conceder privilegios limitados a un usuario. Esto es útil cuando el usuario no desea que un 
  usuario tenga el control de todos los poderes de superusuario mientras haciendo un sudonopass.
* La mejor ventaja es que sudonopass requiere propia contraseña de inicio de sesión del usuario en lugar de la contraseña de root. Esto ayuda 
  a mantener la contraseña de root privado y no hay necesidad de cambiarlo, aun cuando un usuario (sudoer) deja.
* Este archivo proporciona información sobre los comandos que se ejecutan usando sudo y su tiempo de ejecución. Esto ayuda al administrador para  realizar un seguimiento de los usuarios, incluso de confianza
