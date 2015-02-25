=========
Logging
=========

sinopsis
------------------

Este módulo registra una información al panel de control y opcionalmente registro php.

El proceso de utilizar este módulo para recoger datos a través de sensores, analizar los datos y guardar e imprimir los resultados de la reunión y el análisis. Registro implica también la controlpanel del sistema instala y analiza los datos. Sensitibilidad caso es una corona para este módulo. Esto se adapta para trabajar con Ubuntu y CentOS.

comando Ayuda
-----------------------

Este comando puede funcionar sobre los objetivos y los comandos disponibles en el registro bajo módulo ptconfigure. También explica el comando para instalar módulo de registro. Antes de la instalación, el usuario puede leer este comando de ayuda explica su función.

.. code-block:: bash
        
	        ptconfigure logging help

Las siguientes imágenes pueden visualizar el comando de ayuda

.. code-block:: bash


 kevell@corp:/# ptconfigure Logging help

 ******************************


  Use this to log a message to the Console, and optionally also the php error log.

  Logging, logging

        - log
        Logs a message to the console and optionally the php log
        example: ptconfigure logging log --log-message="Here is something logging to the console and error log"
        example: ptconfigure logging log --php-log --log-message="Here is something logging to the console and error log"

 ------------------------------
 End Help
 ******************************

instalación
-----------------

Estos procedimientos de instalación son para acceder php control. Esta sección incluye información sobre la compatibilidad y requisitos, instrucciones básicas sobre cómo instalar y configurar ptconfigure a información más detallada. Este comando puede funcionar sobre los objetivos y los comandos disponibles bajo módulo de registro ptconfigure. También explica el comando para instalar módulo de registro. Antes de la instalación, el usuario puede leer este comando de ayuda explica su función.

.. code-block:: bash
        
                ptconfigure logging  log

Las siguientes imágenes pueden visualizar el comando de ayuda

.. code-block:: bash

 kevell@corp:/# ptconfigure logging log 

 Install Logging? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *           Logging!          *
 *******************************
 Enter Log Message
 Good Morning
 [Pharaoh Logging] Good Morning
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Logging: Success
 ------------------------------
 Installer Finished
 ******************************

opción
------------

.. cssclass:: table-bordered


 +---------------------------+------------------------------------+--------------+------------------------------------------+
 | Parámetros                | Parámetro Alternativa              | Opciones     | Comentarios                              |
 +===========================+====================================+==============+==========================================+
 |ptconfigure logging        | Podemos utilizar el Logging,       | Y(Yes)       | El sistema detiene el proceso de         |          
 |Install                    | logging                            |              | registro bajo ptconfigure                |
 +---------------------------+------------------------------------+--------------+------------------------------------------+
 |ptconfigure logging        | Podemos utilizar el Logging,       | N(No)        | Proceso de registro del sistema se       |
 |Install                    | logging                            |              | detiene bajo ptconfigure|                |
 +---------------------------+------------------------------------+--------------+------------------------------------------+

Beneficios
-------------

* En tiempo real Visualización de Datos
* Sensitibilidad caso
* Funcionalidad definida por el usuario
* Terabytes de almacenamiento de datos
* Conectividad de red
* Bueno, para hacer en Ubuntu y CentOS
