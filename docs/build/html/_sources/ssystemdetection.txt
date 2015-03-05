==================
SystemDetection
==================

sinopsis
-------------

Este módulo tiene como objetivo la detección de la máquina de los usuarios y en la mano les proporciona la información necesaria para ellos en relación con el sistema del usuario. También proporciona una facilidad para los usuarios configurar sus ajustes de aplicaciones. Los pocos ejemplos de configuración de aplicaciones incluye mysql usuario administrador, anfitrión, pase.

Ayuda Comando
----------------------

El comando de ayuda conduce a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en los módulos de detección del sistema. Las listas de comandos de ayuda fuera de los parámetros alternativos de detección del sistema. También se describe la sintaxis para la detección de la máquina de los usuarios. El comando de ayuda para la detección de sistema se muestra a continuación.

.. code-block:: bash

	ptconfigure systemdetection help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda en virtud de detección del sistema.

.. code-block:: bash

	kevell@corp:/# ptconfigure SystemDetection help
	******************************


	This is a default Module and provides you with a method by which you can configure Application Settings.
	 You can configure default application settings, ie: mysql admin user, host, pass

	 SystemDetection, system-detection, systemdetection

        - detect
        Detects the Operating System
        example: ptconfigure system-detection detect

	------------------------------
	End Help
	******************************


detección
------------

El comando que se utiliza para la detección de sistema es la siguiente.

.. code-block:: bash

		ptconfigure systemdetection detect

Después de introducir el comando anterior, el proceso de detección del sistema comienza. Durante la detección del sistema de la siguiente información con respecto a la máquina correspondiente se informa:

* Sistema Operativo
* Tipo de Linux
* Distro
* Versión
* Arquitectura
* Nombre de host
* Dirección IP 0.
* Dirección IP 1.

Finalmente, después de la detección de la información relativa a las características antes mencionadas se informó claramente. La siguiente captura de pantalla que muestra sobre el proceso de detección del sistema.

.. code-block:: bash

        Kevell@corp:/# ptconfigure system-detection detect
	******************************


	Systems Detection:
	--------------------------------------------

	Operating System: Linux
	Linux Type: Debian
	Distro: Ubuntu
	Version: 14.04
	Architecture: 64
	Host Name: Kevells
	IP Address 0: 127.0.0.1
	IP Address 1: 192.168.1.3

	------------------------------
	Detection Finished
	******************************


parámetros alternativos
-----------------------------

En lugar de systemdetection, los siguientes parámetros pueden ser utilizados:

SystemDetection, system-detection, systemdetection

Beneficios
------------

* Los usuarios pueden configurar los parámetros de la aplicación que utilizan este sistema de detecciones.
* Los parámetros utilizados para la declaración de comando de ayuda, detección de sistemas no son sensibles, que es una ventaja añadida, 
  mientras que en comparación con otros.
* Es-acomodados tanto en OS Cent y así como en Ubuntu.
