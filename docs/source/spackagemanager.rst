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

 kevell@corp:/# ptconfigure packagemanager help
 ******************************


  This command allows you to use a Package Management wrapper.

  PackageManager, package-manager, packagemanager, package-mgr, pkgmgr

        - pkg-install
        Installs a Package through a Package Manager
        example: ptconfigure package-manager install --package-name="mysql" --package-version="5.0" --packager="apt-get"

        - pkg-ensure
        Installs a Package through a Package Manager
        example: ptconfigure package-manager install --package-name="mysql" --package-version="5.0" --packager="apt-get"

        - pkg-remove
        Removes a Package through a Package Manager
        example: ptconfigure package-manager install --package-name="mysql" --package-version="5.0" --packager="apt-get"

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

Pkg-garantizar
-----------------

Garantizar Pkg un sistema de servicio se está ejecutando. En caso de no correr empezar en otro no intente. A través de este comando el usuario puede identificar si el sistema está funcionando o inactivo. Comandos simples son fáciles de manejar. El siguiente comando utiliza para asegurar a través del gestor de paquetes.

.. code-block:: bash
    
	ptconfigure PackageManager ensure

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
