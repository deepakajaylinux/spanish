==========
Jetty
==========

Sinopsis
-------------
Embarcadero proporciona un servidor Web y el contenedor javax.servlet, además de soporte para SPDY, WebSocket, OSGi, JMX, JNDI, JAAS y mucho otra integración. Estos componentes son de código abierto y disponible para uso comercial y distribution.Jetty se utiliza en una amplia variedad de proyectos y productos, tanto en el desarrollo y la producción. Jetty puede ser fácilmente integrado en los dispositivos, herramientas, marcos de trabajo, servidores de aplicaciones y clusters.

Embarcadero es un servidor HTTP pura basada en Java (web) y el contenedor de servlets de Java. Mientras que los servidores Web se asocian generalmente a entregar los documentos a la gente, Espolón ahora se utiliza a menudo para comunicaciones de máquina a máquina, por lo general dentro de los marcos de software más grandes. Embarcadero se desarrolla como un proyecto de código libre y abierto como parte de la Fundación Eclipse. El servidor web se utiliza en productos tales como Apache ActiveMQ, Alfresco, Apache Geronimo, Apache Maven, Apache Spark, Google App Engine, Eclipse, FUSE, Streaming API de Twitter y Zimbra. Embarcadero también es el servidor en proyectos de código abierto como el Levante, Eucalipto, Red5, Hadoop y I2P. Embarcadero soporta la última API Java Servlet (con soporte JSP), así como los protocolos SPDY y WebSocket.

Ayuda Comando
----------------------

Este comando ayuda a determinar el uso del módulo de muelle. El usuario se llega a saber acerca de la diferente forma / formato de ejecutar este módulo. Este comando guía al usuario final a conocer el propósito de este comando. A continuación dado son el mando y la pantalla del mismo.

.. code-block:: bash
        
	        ptconfigure jetty help

La representación gráfica de la orden anterior se muestra a continuación,

.. code-block:: bash

 kevell@corp:/# ptconfigure Jetty help

 ******************************


  This command allows you to install Jetty, the popular Web Server.

  Jetty, jetty

        - install
        Installs Jetty.  
        example: ptconfigure jetty install

 ------------------------------
 End Help
 ******************************

instalación
----------------

Este comando ayuda en la instalación de amarre en el sistema. El siguiente comando dado se ejecutará el proceso de instalación.

.. code-block:: bash
        
	        ptconfigure jetty install


Opciones
------------

.. cssclass:: table-bordered


 +--------------------------+----------------------------------------+-----------+------------------------------+
 | Parámetros               | Parámetro Alternativa                  | Opciones  | Comentarios                  |
 +==========================+========================================+===========+==============================+
 |ptconfigure jetty Install | Hay dos parámetros alternativos que    | Y(Yes)    | El sistema se inicia proceso |
 |                          | pueden ser utilizados en la línea de   |           | de instalación               |
 |                          | comandos. Jetty, jetty Por ejemplo:    |           |                              |
 |                          | ptconfigure jetty install,             |           |                              |
 |                          | ptconfigure Jetty install              |           |                              |
 +--------------------------+----------------------------------------+-----------+------------------------------+
 |ptconfigure jetty Install | Hay dos parámetros alternativos que    | N(No)     | El sistema detiene proceso   |
 |                          | pueden ser utilizados en la línea de   |           | de instalación               |
 |                          | comandos. Jetty, jetty Por ejemplo:    |           |                              |
 |                          | ptconfigure jetty install,             |           |                              |
 |                          | ptconfigure Jetty install|             |           |                              |
 +--------------------------+----------------------------------------+-----------+------------------------------+


Beneficios
--------------

* Con todas las funciones y basado en estándares
* Flexible y extensible
* Tamaño compacto
* exportable
* asíncrono
* Empresa escalable
* Dual licenciado bajo Apache y Eclipse

