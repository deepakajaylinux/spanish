=============
ApacheConf
=============

Sinopsis
-----------
Este módulo ayuda en el manejo y la instalación de la configuración de Apache. En él se especifica la configuración de su entorno. Es-acomodada en ubuntu y así como en CentOS.

comando Ayuda
--------------------

El comando de ayuda describe sobre el propósito y los comandos disponibles bajo estos módulos. También explica el comando para instalar el módulo en particular.

En él se enumeran los parámetros alternativos que se pueden utilizar para la declaración. El comando utilizado para la declaración de ayuda se muestra a continuación:

.. code-block:: bash

	ptconfigure apacheconf help

La captura de pantalla como se muestra a continuación, representar visualmente el uso del comando de ayuda en virtud de este módulo.

.. code-block:: bash
	
 kevell@corp:/# ptconfigure apacheconf help
 ******************************


  This module lets you install a configuration for Apache HTTP Server. The only commands available are this help
  and install.

  ApacheConf, apache-configure, apache-configuration, apache-conf, apacheconf

        - install
        Installs a configuration for Apache
        example: ptconfigure apacheconf install

 ------------------------------
 End Help
 ******************************

instalación
--------------

Es más fácil de instalar esta herramienta en particular en virtud de ptconfigure por el simple uso de la orden dada a continuación,

.. code-block:: bash
 
	  ptconfigure apacheconf install

Después de dar el comando anterior, la herramienta le preguntará como

.. code-block:: bash

  Install Apache conf? (Y/N)

si se le da una entrada como Y, el módulo se instalan correctamente.

También lanzará algunos comandos para especificar los valores no predeterminados para LockFile, PidFile, tiempo de espera, KeepAlive, MaxKeepAliveRequest, KeepAliveTimeout. Si el usuario da entrada como Y (Sí) se fijará automáticamente el valor predeterminado. Si el usuario da entrada como N (No), entonces se indagará acerca de los valores de usuario.

La captura de pantalla que figura a continuación explica visualmente sobre los pasos y comandos consiste en la instalación.

.. code-block:: bash


 kevell@corp:/# ptconfigure ApacheConf install
 Install Apache Conf? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Apache Conf!        *
 *******************************
 Set non-default value for LockFile? Default is ${APACHE_LOCK_DIR}/accept.lock (Y/N) 
 y
 What value for LockFile?
 ${APACHE_LOCK_DIR}/accept.lock
 Set non-default value for PidFile? Default is ${APACHE_PID_FILE} (Y/N) 
 y
 What value for PidFile?
 ${APACHE_PID_FILE}
 Set non-default value for Timeout? Default is 300 (Y/N) 
 y
 What value for Timeout?
 300
 Set non-default value for KeepAlive? Default is On (Y/N) 
 y
 What value for KeepAlive?
 On
 Set non-default value for MaxKeepAliveRequests? Default is 100 (Y/N) 
 y
 What value for MaxKeepAliveRequests?
 100
 Set non-default value for KeepAliveTimeout? Default is 5 (Y/N) 
 y
 What value for KeepAliveTimeout?
 5
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************
 

Opciones
------------

.. cssclass:: table-bordered


 +-----------------------------+----------------------------------------+--------------+-------------------------------------------+
 | Parámetros		       | parámetros alternativos		| Necesario    | Comentario				   |
 +=============================+========================================+==============+===========================================+
 |Install Apache conf? (Y/N)   | En lugar de apachemodules, podemos     | Y(Yes)       | Si el usuario da entrada como sí, va a    | 
 |                             | utilizar ApacheModules, apachemods,    |              | instalar el módulo. el módulo.            |
 |                             | apache-modules también                 |              |                                           |
 +-----------------------------+----------------------------------------+--------------+-------------------------------------------+
 |Install Apache conf? (Y/N)   | En lugar de apachemodules, podemos     | N(No)        | Si el usuario da entrada como No,         |
 |                             | utilizar ApacheModules, apachemods,    |              | obtendrá salida.                          |
 |                             | apache-modules también|                |              |                                           |
 +-----------------------------+----------------------------------------+--------------+-------------------------------------------+


Beneficios
-------------

* El módulo de ayuda al usuario final en la instalación y gestión de la configuración de Apache.
* Durante la instalación de la herramienta de Apache, el usuario final puede diseñar y gestionar la configuración según sus necesidades usando 
  este módulo.
* Si se funda la configuración ya existe sobrescribirá la existente.
* Es-acomodada en CentOS y así como en Ubuntu.
* Los parámetros utilizados en la declaración no se distingue entre mayúsculas y minúsculas, lo que es una ventaja añadida.
