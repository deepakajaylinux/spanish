===============
InstallPackage
===============

sinopsis
------------------

Instalar paquete son salidas lógicas diferenciales comúnmente utilizados en los circuitos de distribución de reloj de alta velocidad. Este comando proporciona al usuario instalar el paquete, construir servidor, cliente dev, servidor de prueba, servidor dev, la producción. Esta función principal mandamiento es lista preconfigurada de software. Es adecuado con Ubuntu y CentOS.

comando Ayuda
-----------------------

El comando de ayuda conduce a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en los módulos InstallPackage. El comando help enumera los parámetros alternativos de InstallPackage bajo módulo ptconfigure. También describe la sintaxis para la instalación. El comando de ayuda para el módulo InstallPackage se muestra a continuación.

.. code-block:: bash

		ptconfigure installpackage help


La siguiente captura de pantalla muestra el esfuerzo total del módulo InstallPackage.

.. code-block:: bash

 kevell@corp:/# ptconfigure InstallPackage help

 ******************************


  This command is part of Core and provides you  with a method by which you can perform some default CLI Installs of
  different types of box.

  InstallPackage, installpackage, installpack, install-pack, install, inpack, install-package

    - dev-client
      install a dev client machine for you to work on, a bunch of IDE's, DB's and a complete set of the
      tools you need to start work immediately.
      example: ptconfigure install autopilot dev-client

    - dev-server
      Install the preconfigured list of software for a developers server.
      example: ptconfigure install autopilot dev-server

    - test-server
      Install the preconfigured list of software for a testing server.
      example: ptconfigure install autopilot test-server

    - build-server
      Install the preconfigured list of software for a build server.
      example: ptconfigure install autopilot test-server

    - production
      Install the preconfigured list of software for a production server.
      example: ptconfigure install autopilot test-server

 ------------------------------
 End Help
 ******************************

instalación
---------------

Instalación incluye la instalación de InstallPackage requerida para hacer la instalación en una versión actualizada. Es un proceso de manifiesto para instalar módulo InstallPackage bajo ptconfigure. InstallPackage sólo por el uso de la orden dada a continuación,

.. code-block:: bash

	ptconfigure installpackage Install

Después de vitalizar el comando se catequizar entrada.

Cuando la entrada de usuario como si automáticamente se instalará InstallPackage con la comprobación del sistema. Si no salir de la instalación. La siguiente captura de pantalla de demostrar InstallPackage y sus funciones.

.. code-block:: bash

parámetros alternativos
-------------------------------

Los siguientes son los parámetros alternativos que pueden ser definidos en las declaraciones:

InstallPackage, installpackage, installpack, install, inpack, installpackage.

Dev-cliente
---------------

Este comando se utiliza para trabajar en un montón de Entorno de Desarrollo Integrado de la base de datos de y un juego completo de las herramientas que el usuario necesita para empezar a trabajar de inmediato. El siguiente comando se utiliza para la máquina cliente prog.

.. code-block:: bash

		ptconfigure install autopilot dev-client

Después de entrada como por encima de dicho comando se inicia proceso de instalación.

La siguiente instantánea muestra sus funciones.

.. code-block:: bash

Dev-servidor
----------------

Este comando se utiliza para instalar preconfigura lista de software para el servidor de un desarrollador. Piloto automático actúa como un papel vital en este proceso. Para calcular estas funciones correctamente ptconfigure recomienda dev-servidor utilizando este comando.

.. code-block:: bash

		ptconfigure install autopilot dev-server

La captura de pantalla guía al usuario acerca de su función.

.. code-block:: bash

Test-servidor
-----------------

Aquí piloto automático actúa un papel importante en el servidor de prueba. Se utiliza para instalar la lista preconfigurada de software para el servidor de prueba. Software también dispone de pruebas. El siguiente comando utilizado para instalar el servidor de prueba.

.. code-block:: bash

		ptconfigure install autopilot test-server

La captura de pantalla guía al usuario acerca de su función.

.. code-block:: bash

construir servidor
---------------------

Este comando se utiliza para instalar preconfigura lista de software para un servidor de compilación. Piloto automático actúa como un papel vital en este proceso. Para calcular estas funciones correctamente ptconfigure recomienda construir-servidor utilizando este comando.

.. code-block:: bash

	ptconfigure install autopilot build-server

La captura de pantalla guía al usuario acerca de su función.

.. code-block:: bash

producción
-----------------

Este comando se utiliza para instalar preconfigura lista de software para un servidor de producción. Piloto automático actúa como un papel vital en este proceso. Para calcular estas funciones correctamente ptconfigure recomienda servidor de producción mediante el uso de este comando.

.. code-block:: bash

		ptconfigure install autopilot build-server

La captura de pantalla guía al usuario acerca de su función.

.. code-block:: bash

Beneficios
-------------

* Sensitibilidad caso.
* Well-to-do en Ubuntu y CentOS.
* Instalación dev-servidor, dev-cliente, la producción, construir-servidor, prueba de servidor es una ventaja añadida para este módulo.
* Piloto automático actúa como un papel vital.
