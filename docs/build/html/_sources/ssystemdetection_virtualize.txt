==================
SystemDetection
==================


Sinopsis
----------------

Este módulo tiene como objetivo detectar la máquina del usuario y en la mano les proporciona la información necesaria para ellos con respecto al sistema de los usuarios. También proporciona un servicio a los usuarios configurar sus ajustes de aplicaciones. Los pocos ejemplos de configuración de aplicaciones incluye mi sql admin, arquitectura, admin usuario, host, versión, tipo de linux, Distro. Es cómodo con Ubuntu y ciento OS.


comando Ayuda
----------------------

El comando help conduce a los usuarios sobre la finalidad y así como sobre las opciones que están incluidas en los módulos de detección del sistema. El comando ayuda enumera los parámetros alternativos de detección de sistemas debajo del módulo ptvirtualize. También describe la sintaxis para la detección de la máquina del usuario. A continuación se muestra el comando de ayuda para la detección de sistemas.


.. code-block:: bash

	ptvirtualize systemdetection help

La sintaxis para el comando de ayuda no mayúsculas y minúsculas que añade una ventaja para este módulo. La siguiente captura de pantalla visualizar al usuario sobre el comando de ayuda en la detección de sistemas.


.. code-block:: bash

 kevell@corp:/# ptvirtualize systemdetection help

 ******************************
 Pharaoh Tools - ptvirtualize
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
----------- 

Detectar utilizado para detectar la configuración del sistema. Utilizando un único comando, el usuario puede obtener toda la información sobre la aplicación del sistema. El comando utilizado para la detección de sistema se expone a continuación.


.. code-block:: bash

	ptvirtualize systemdetection detect

Después de afinar el comando anterior, inicia el proceso de detección de sistemas. Durante la detección de sistemas se divulga la siguiente información con respecto a la máquina correspondiente:


Operating System

Linux Type

Distro

Version

Architecture

Host Name

IP Address 0.

IP Address 1.

Finalmente, después de detectar la información con respecto a lo anterior mencionado características claramente se divulgan. La captura de pantalla siguiente muestra al usuario sobre el proceso de detección de sistemas.


.. code-block:: bash

 kevellscorp:/# ptvirtualize systemdetection detect

 ******************************
 Pharaoh Tools - Virtualize
 ******************************


 Systems Detection:
 --------------------------------------------

 Operating System: Linux
 Linux Type: Debian
 Distro: Ubuntu
 Version: 14.04
 Architecture: 64
 Host Name: kevells
 IP Address 0: 127.0.0.1
 IP Address 1: 192.168.1.19

 ------------------------------
 Detection Finished
 ******************************



parámetros alternativos
----------------------------------

En lugar de detección del sistema, pueden utilizar los siguientes parámetros:


System Detection

system-detection

system detection

beneficios
-------------

* Los usuarios pueden configurar la configuración de la aplicación utilizando las detecciones de este sistema. 
* Los parámetros utilizados para declarar el comando help, detección de sistemas son sensibles al caso no que una ventaja adicional mientras
  que comparado con otros. 
* Es acomodada en ambos OS ciento y así como en Ubuntu. 
* Protección y seguridad es posible. Previniendo daños al sistema y a los recursos, a través de los procesos internos o forasteros maliciosos.


  Autenticación, la propiedad y acceso restringido son partes obvias de este sistema.


* Los administradores de sistemas generalmente determinan interfaz que un usuario inicia con cuando inician sesión primero pulg. 
* generalmente escrito en PHP, aunque algunas están escritas en conjunto para un rendimiento óptimo. * El módulo de detección de sistema  
  proporciona el soporte: 
* identificar un proceso remoto o host con el cual comunicarse. 
* Establecer una conexión entre los dos procesos. 
* Abrir y cerrar la conexión según sea necesario.


