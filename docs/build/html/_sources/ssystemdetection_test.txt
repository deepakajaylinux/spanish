===================
SystemDetection
===================


sinopsis
-----------

Este módulo tiene como objetivo detectar la máquina del usuario y en la mano les proporciona la información necesaria para ellos con respecto al sistema de los usuarios. También proporciona un servicio a los usuarios configurar sus ajustes de aplicaciones. Los pocos ejemplos de configuración de aplicaciones incluye mysql admin, arquitectura, admin usuario, host, versión, tipo de linux, Distro. Es cómodo con Ubuntu y ciento OS.


comando Ayuda
---------------

El comando help conduce a los usuarios sobre la finalidad y así como sobre las opciones que están incluidas en los módulos de detección del sistema. El comando ayuda enumera los parámetros alternativos de detección de sistemas debajo del módulo pttest. También describe la sintaxis para la detección de la máquina del usuario. A continuación se muestra el comando de ayuda para la detección de sistemas.



.. code-block:: bash

	pttest systemdetection help

La sintaxis para el comando help es sensible al caso no que añade una ventaja para este módulo. La siguiente captura de pantalla visualizar sobre el comando de ayuda en la detección de sistemas.


.. code-block:: bash

 kevell@corp:/# pttest systemdetection help
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


Detect
----------

Cuando el usuario necesita detectar la configuración del sistema, el siguiente dado comando obtendrá toda la información sobre la aplicación del sistema.


.. code-block:: bash
	
	pttest systemdetection detect

Sistema termina con el abastecimiento de la continuación dado detalles:


* Operating System
* Linux Type
* Distro
* Version
* Architecture
* Host Name
* IP Address 0.

La siguiente captura de pantalla te muestra sobre el proceso de detección de sistemas.

.. code-block:: bash

 kevell@corp:/# pttest system-detection detect
 ******************************


 Systems Detection:
 --------------------------------------------

 Operating System: Linux
 Linux Type: Debian
 Distro: Ubuntu
 Version: 14.04
 Architecture: 64
 Host Name: kevells
 IP Address 0: 172.16.201.1
 IP Address 1: 172.16.39.1
 IP Address 2: 192.168.1.16

 ------------------------------
 Detection Finished
 ******************************


parámetros alternativos
----------------------------------

En lugar de detección del sistema, pueden utilizar los siguientes parámetros:


* SystemDetection
* system-detection
* systemdetection


Beneficios
-------------

* Los usuarios pueden configurar la configuración de la aplicación mediante la detección de este sistema. 
* Los parámetros utilizados para declarar el comando help, detección de sistemas no son mayúsculas y minúsculas que es una ventaja añadida 
  mientras que comparado con otros. 
* Es acomodada en ambos OS ciento y así como en Ubuntu. 
* Protección y seguridad es posible. Previniendo daños al sistema y a los recursos, a través de los procesos internos o forasteros maliciosos.
  Authntication, la propiedad y acceso restringido son partes obvias de este sistema. 
* Los administradores de sistemas generalmente determinan interfaz que un usuario inicia con cuando inician sesión primero pulg. 
* generalmente escrito en PHP, aunque algunas están escritas en conjunto para un rendimiento óptimo.



  


