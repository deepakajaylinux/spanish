==============
Nginx Control
==============

sinopsis
-------------

Nginx (pronunciado "motor -x" ) es una fuente abierta de servidor proxy inverso para HTTP , HTTPS , SMTP , POP3 e IMAP , así como un equilibrador de carga , caché HTTP y un servidor web (servidor de origen ) . El proyecto nginx empezó con un fuerte enfoque en la alta concurrencia , alto rendimiento y bajo uso de memoria . Es licenciado bajo la licencia BSD de 2 clausulas y se ejecuta en Linux , las variantes BSD, Mac OS X , Solaris , AIX , HP- UX , así como en otros sabores nix .

Nginx utiliza un enfoque orientado a eventos asíncronos a las solicitudes de control , en lugar del modelo de Apache HTTP Server que por defecto un enfoque roscada o orientado al proceso , donde se requiere que el MPM de eventos para el procesamiento asincrónico . Modular la arquitectura orientada a eventos de Nginx puede proporcionar un rendimiento más predecible bajo altas cargas .

Ayuda Comando
----------------------

Este comando ayuda a determinar el uso del módulo de Nginx . El usuario se llega a saber acerca de las diferentes formas / formato para ejecutar este módulo. Este comando guía al usuario final a conocer el propósito de este comando. A continuación dado son el mando y la pantalla del mismo . 

.. code-block:: bash
	
	ptdeploy nginxcontrol help
       
 kevell@corp:/# ptdeploy NginxControl help
 ******************************


  This command is part of Default Modules and handles Nginx Server Control Functions.

  NginxControl, nginxcontrol, nginxctl

          - start
          Start the Nginx server
          example: ptdeploy nginxcontrol start

          - stop
          Stop the Nginx server
          example: ptdeploy nginxcontrol stop

          - restart
          Restart the Nginx server
          example: ptdeploy nginxcontrol restart

          - reload
          Reloads the Nginx server configuration without restarting
          example: ptdeploy nginxcontrol reload

 ------------------------------
 End Help
 ******************************


comienzo
----------------

Cuando el usuario necesita para iniciar el servidor Nginx , el comando a continuación se indica se ejecutará el proceso.

.. code-block:: bash
	
		ptdeploy nginxcontrol start                           

Antes de la ejecución , el sistema pide la confirmación para continuar , si desea continuar enter ' Y', si no entran en 'N'.

Deténgase
----------------

Cuando el usuario necesita para detener el servidor Nginx , el comando a continuación se indica se ejecutará el proceso.

.. code-block:: bash
	
	ptdeploy nginxcontrol stop	

Antes de la ejecución , el sistema pide la confirmación para continuar , si desea continuar enter ' Y', si no entran en 'N'.

reanudar
----------------

Cuando el usuario necesita para reiniciar el servidor Nginx ( cuando haya cambios ocurridos en el archivo de configuración se utiliza esta opción ), el comando a continuación se indica se ejecutará el proceso.

.. code-block:: bash
 	
	ptdeploy nginxcontrol restart                          

Antes de la ejecución , el sistema pide la confirmación para continuar , si desea continuar enter ' Y', si no entran en 'N'.

recargar
----------------

Cuando el usuario necesita para Actualizar el servidor Nginx sin reiniciar , el comando a continuación se indica se ejecutará el proceso.

.. code-block:: bash
	
	ptdeploy nginxcontrol reload

Antes de la ejecución , el sistema pide la confirmación para continuar , si desea continuar enter ' Y', si no entran en 'N'.


Parámetro Alternativa
--------------------------------------

Cualquiera de los tres parámetros alternativa se puede utilizar en ngnixcontrol de comandos , NgnixControl y nginxcil

por ejemplo : ngnixcontrol ptdeploy ayuda / ptdeploy ngnixControl ayuda



Beneficios
--------------
   
* Habilidad para manejar más de 10,000 conexiones simultáneas con una huella de memoria baja 
* Manejo de archivos estáticos , archivos de índice , y el auto-indicador
* Proxy inverso con el almacenamiento en caché 
* Equilibrio de carga con controles de salud dentro de la banda
* La tolerancia a fallos
* TLS / SSL con SNI y OCSP grapado apoyo , a través de OpenSSL .
* FastCGI , SCGI , apoyo uWSGI con el almacenamiento en caché
* Servidores virtuales nombre- e IP basados ​​en las direcciones
* Compatible con IPv6
* Soporte para el protocolo SPDY
* WebSockets y HTTP / 1.1 Upgrade ( 101 Protocolos de conmutación ) 
* FLV y MP4 de streaming
* Autenticación de acceso a la página Web
* compresión gzip y descompresión
* reescritura de URL
* De registro personalizado con en la marcha de compresión gzip 
* La tasa de respuesta y la limitación de peticiones concurrentes
* del ancho de banda
* Server Side Includes 
* IP address-based geolocation 
* User tracking 
* WebDAV 
* XSLT data processing 
* Embedded Perl scripting
