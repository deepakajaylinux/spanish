===========
HAProxy
===========

sinopsis
-------------

HAProxy es una solución de alta disponibilidad libre, de código abierto, proporcionando equilibrio de carga y proxy para TCP y aplicaciones basadas en HTTP mediante la difusión de las solicitudes a través de múltiples servidores. Tiene fama de ser rápido y eficiente (en términos de uso del procesador y la memoria).

Ayuda Comando
----------------------

Este comando ayuda a determinar el uso del módulo HAProxy. El usuario se llega a saber acerca de las diferentes formas / formato para ejecutar este módulo. Este comando le guiará al usuario final para saber cuándo y cómo el comando que desea utilizar. A continuación dado son el mando y la pantalla del mismo.

.. code-block:: bash
        
	        ptconfigure HAproxy help

La representación gráfica de la orden anterior se enumeran a continuación,

.. code-block:: bash


 kevell@corp:/# ptconfigure HAProxy help

 ******************************


  This module provides installs HA Proxy Server

  HAProxy, ha-proxy, haproxy

        - install
        Installs HA Proxy Server
        example: ptconfigure haproxy install

        - configure
        Configure Load Balancing with HA Proxy Server
        example: ptconfigure haproxy configure

 ------------------------------
 End Help
 ******************************


instalación
----------------

Podemos instalar HAProxy usando el gestor de paquetes de la distribución. Cuando el usuario tiene que instalar el módulo HAProxy en máquina. El siguiente comando dado se ejecutará el proceso de instalación.

.. code-block:: bash
        
	        ptconfigure HAproxy install

La representación gráfica de la orden anterior se enumeran a continuación,

.. code-block:: bash

 
 kevell@corp:/# ptconfigure haproxy install
 Install HA Proxy Server? (Y/N)
 y
 *******************************
 *        Pharaoh Tools        *
 *         HA Proxy Server!        *
 *******************************
 [Pharaoh Logging] Package haproxy from the Packager Apt is already installed, so not installing
 HA Proxy Init script config file /etc/default/haproxy added
 [Pharaoh Logging] Restarting haproxy service
 [ALERT] 041/154050 (17460) : parsing [/etc/haproxy/haproxy.cfg:25] : unknown keyword '1' in 'defaults' section
 [ALERT] 041/154050 (17460) : parsing [/etc/haproxy/haproxy.cfg:32] : unknown option 'tcp-check'.
 [ALERT] 041/154050 (17460) : parsing [/etc/haproxy/haproxy.cfg:34] : unknown keyword 'tcp-check' in 'backend' section
 [ALERT] 041/154050 (17460) : parsing [/etc/haproxy/haproxy.cfg:35] : unknown keyword 'tcp-check' in 'backend' section
 [ALERT] 041/154050 (17460) : parsing [/etc/haproxy/haproxy.cfg:36] : unknown keyword 'tcp-check' in 'backend' section
 [ALERT] 041/154050 (17460) : parsing [/etc/haproxy/haproxy.cfg:37] : unknown keyword 'tcp-check' in 'backend' section
 [ALERT] 041/154050 (17460) : parsing [/etc/haproxy/haproxy.cfg:38] : unknown keyword 'tcp-check' in 'backend' section
 [ALERT] 041/154050 (17460) : parsing [/etc/haproxy/haproxy.cfg:39] : unknown keyword 'tcp-check' in 'backend' section
 [ALERT] 041/154050 (17460) : Error(s) found in configuration file : /etc/haproxy/haproxy.cfg
 [ALERT] 041/154050 (17460) : Fatal errors found in configuration.
 * Restarting haproxy haproxy
   ...fail!
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 HAProxy: Success
 ------------------------------
 Installer Finished
 ******************************

Opciones
-----------
.. cssclass:: table-bordered

 +------------------------+------------------------------+-------------+----------------------------------------------+
 | Parámetros             | Parámetro Alternativa        | Opciones    | Comentarios                                  |
 +========================+==============================+=============+==============================================+
 |ptconfigure HAProxy     | HAProxy , ha-proxy, haproxy  | Y(Yes)      | El sistema se inicia proceso de instalación  |
 |Install                 |                              |             |                                              |
 +------------------------+------------------------------+-------------+----------------------------------------------+
 |ptconfigure HAProxy     | HAProxy , ha-proxy, haproxy  | N(No)       | El sistema detiene proceso de instalación    |
 |Install|                |                              |             |                                              |
 +------------------------+------------------------------+-------------+----------------------------------------------+


configuración
--------------------

Este comando ayuda a la hora de configurar el equilibrio de carga con servidor HAProxy. Una vez que se ejecute el comando a continuación se indica el sistema le proporciona el valor predeterminado para cada sección, si hay algún cambio que hacer, el usuario puede proporcionar los datos.

.. code-block:: bash

                ptconfigure HAproxy configure

La captura de pantalla para el comando anterior se enumeran a continuación,

.. code-block:: bash


 kevell@corp:/# ptconfigure haproxy configure

 *******************************
 *        Pharaoh Tools        *
 *         HA Proxy Server!        *
 *******************************
 
 What is the environment name you want to balance load to? 
 
 PHP Notice:  Undefined index:  in /opt/ptconfigure/ptconfigure/src/Modules/HAProxy/Model/HAProxyConfigureUbuntu.php on line 102
 PHP Notice:  Undefined index:  in /opt/ptconfigure/ptconfigure/src/Modules/HAProxy/Model/HAProxyConfigureUbuntu.php on line 102
 PHP Warning:  Invalid argument supplied for foreach() in /opt/ptconfigure/ptconfigure/src/Modules/HAProxy/Model/HAProxyConfigureUbuntu.php on line 75
 Set non-default value for global_log? Default is 127.0.0.1 local0 notice (Y/N) 

 Set non-default value for global_maxconn? Default is 20000 (Y/N) 

 Set non-default value for global_user? Default is haproxy (Y/N) 

 Set non-default value for global_group? Default is haproxy (Y/N) 

 Set non-default value for defaults_log? Default is global (Y/N) 

 Set non-default value for defaults_mode? Default is http (Y/N) 

 Set non-default value for defaults_option_string? Default is option dontlognull
    option redispatch (Y/N) 

 Set non-default value for defaults_retries? Default is 3 (Y/N) 

 Set non-default value for defaults_timeout_connect? Default is 5000 (Y/N) 

 Set non-default value for defaults_timeout_client? Default is 10000 (Y/N) 

 Set non-default value for defaults_timeout_server? Default is 10000 (Y/N) 

 Set non-default value for listen_appname? Default is appname (Y/N) 

 Set non-default value for listen_ip_port? Default is 0.0.0.0:80 (Y/N) 

 Set non-default value for listen_mode? Default is http (Y/N) 

 Set non-default value for listen_balance? Default is roundrobin (Y/N) 

 Set non-default value for listen_option_string? Default is option httpclose
    option forwardfor (Y/N) 

 Set non-default value for listen_server_string? Default is  (Y/N) 

 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 HA Proxy Server: Success
 ------------------------------
 Installer Finished
 ******************************

Beneficios
----------

* Todas las aplicaciones de acceso al clúster a través de una sola dirección IP. La topología de la base de datos de clúster enmascarado detrás   HAProxy.
* Es posible añadir o eliminar nodos de base de datos sin ningún cambio en las aplicaciones.
* Una vez que el número máximo de conexiones de bases de datos (MySQL) alcanzó, HAProxy colas nuevas conexiones adicionales. Esto es una clara 
  forma de peticiones de conexión de base de datos de estrangulamiento y logra protección de sobrecarga.

