=================
PackageManager
=================

sinopsis
----------------

Este comando utiliza para envolver la gestión de paquetes. Se trata de tener tres opciones. Están PKG-instalar, pkg-asegurar, pkg-remove. Esto permite al usuario instalar en cualquier sistema. Se gestionar las funciones del Administrador de paquetes. Es adecuado para trabajar con Ubuntu y CentOS.

comando Ayuda
-----------------------

Este comando ayuda guía al usuario a instalar, asegurar, eliminar de gestión de paquetes. Esto permite la instalación, asegurarse, retire. El comando de ayuda para el paquete Administrador se muestra a continuación.

.. code-block:: bash

		ptconfigure packagemanager help

Después de entradas el comando anterior, comienza a funcionar para envolver. Es la catequesis de las funciones en las capturas de pantalla.

.. code-block:: bash



 kevell@corp:/# ptconfigure PackageManager help 

 ****************************** 


  This command allows you to use a Package Management wrapper. 

  PackageManager, package-manager, packagemanager, package-mgr, pkgmgr 

        - pkg-install 
        Installs a Package through a Package Manager 
        example: ptconfigure package-manager pkg-install --package-name="mysql" --packager-name="apt" 

        - pkg-ensure 
        Installs a Package through a Package Manager 
        example: ptconfigure package-manager pkg-ensure --package-name="mysql" --packager-name="apt" 
 
        - pkg-remove 
        Removes a Package through a Package Manager 
        example: ptconfigure package-manager pkg-remove --package-name="mysql" --packager-name="apt" 

  A package manager wrapper that will allow you to install packages on any system 

 ------------------------------ 
 End Help 
 ****************************** 



parámetros alternativos
--------------------------------

Los siguientes son los parámetros alternativos que pueden ser definidos en las declaraciones:
PackageManager, package-manager, packagemanager, pkgmgr, package-mgr.

Paquete a instalar
-------------------

Instalación incluye la instalación de PackageManager requerida para hacer la instalación en una versión actualizada. Es un proceso de manifiesto para instalar módulo PackageManager bajo ptconfigure. PackageManager sólo por el uso de la orden dada a continuación,

.. Code-block:: bash

	ptconfigure PackageManager Install

Después de vitalizar el comando se catequizar entrada.

Cuando la entrada de usuario como si automáticamente se instalará PackageManager con la comprobación del sistema. Si no salir de la instalación. La siguiente captura de pantalla de demostrar PackageManager y sus funciones.

.. code-block:: bash


 kevell@corp:/# ptconfigure package-manager pkg-install --package-name="ssh" --packager-name="apt" 

 Reading package lists... 
 Building dependency tree... 
 Reading state information... 
 The following NEW packages will be installed: 
   ssh 
 0 upgraded, 1 newly installed, 0 to remove and 87 not upgraded. 
 Need to get 0 B/1,106 B of archives. 
 After this operation, 29.7 kB of additional disk space will be used. 
 Selecting previously unselected package ssh. 
 (Reading database ... 198126 files and directories currently installed.) 
 Preparing to unpack .../ssh_1%3a6.6p1-2ubuntu2_all.deb ... 
 Unpacking ssh (1:6.6p1-2ubuntu2) ... 
 Setting up ssh (1:6.6p1-2ubuntu2) ... 
 [Pharaoh Logging] Adding Package ssh from the Packager Apt executed correctly 
 ****************************** 


 Apt Modifications: 
 -------------------------------------------- 

 Package Manager: Success 

 ------------------------------ 
 Apt Mods Finished 
 ****************************** 



Pkg-garantizar
-----------------

Garantizar Pkg un sistema de servicio se está ejecutando. En caso de no correr empezar en otro no intente. A través de este comando el usuario puede identificar si el sistema está funcionando o inactivo. Comandos simples son fáciles de manejar. El siguiente comando utiliza para asegurar a través del gestor de paquetes.

.. code-block:: bash
    
	ptconfigure PackageManager ensure


 kevell@corp:/# ptconfigure package-manager pkg-ensure --package-name="mysql" --packager-name="apt" 


 [Pharaoh Logging] Package mysql from the Packager apt is already installed, so not installing 
 ****************************** 


 Apt Modifications: 
 -------------------------------------------- 

 Package Manager: Success 

 ------------------------------ 
 Apt Mods Finished 
 ****************************** 

.. code-block:: bash


 kevell@corp:/# ptconfigure package-manager pkg-ensure --package-name="ssh" --packager-name="apt" 

 Reading package lists... 
 Building dependency tree... 
 Reading state information... 
 The following NEW packages will be installed: 
  ssh 
 0 upgraded, 1 newly installed, 0 to remove and 87 not upgraded. 
 Need to get 0 B/1,106 B of archives. 
 After this operation, 29.7 kB of additional disk space will be used. 
 Selecting previously unselected package ssh. 
 (Reading database ... 198126 files and directories currently installed.) 
 Preparing to unpack .../ssh_1%3a6.6p1-2ubuntu2_all.deb ... 
 Unpacking ssh (1:6.6p1-2ubuntu2) ... 
 Setting up ssh (1:6.6p1-2ubuntu2) ... 
 [Pharaoh Logging] Adding Package ssh from the Packager Apt executed correctly 
 ****************************** 


 Apt Modifications: 
 -------------------------------------------- 

 Package Manager: Success 

 ------------------------------ 
 Apt Mods Finished 
 ****************************** 



Pkg-remove
-----------------

Pkg comando utilizado para eliminar un paquete de administrador de paquetes quitar. El gestor de paquetes comprueba en primer lugar el paquete para eliminarlas de su gestor de paquetes. Luego se pide confirmación. A continuación, utilice la opción Eliminar.

.. code-block:: bash

 		ptconfigure PackageManager remove

Beneficios
-------------

* Sensitibilidad caso.
* Well-to-do en Ubuntu y CentOS.
* Retire el paquete es posible
* Envolver el gestor de paquetes
* Los comandos son fáciles de usar
