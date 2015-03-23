=====================
LighttpdControl
=====================

sinopsis
---------------

Lighttpd es un servidor web seguro, rápido, compatible, y muy flexible que ha sido optimizada para entornos de alto rendimiento. Lighttpd que la eficiencia de un ptdeploy redefiniendo rápidamente; ya que está diseñado y optimizado para entornos de alto rendimiento. Con una pequeña huella de memoria en comparación con otros servidores web, la gestión eficaz de la cpu-carga, y conjunto de características avanzadas lighttpd es la solución perfecta para cada servidor que está sufriendo problemas de carga. Esto es adecuado para trabajar con Ubuntu y CentOS.

comando Ayuda
----------------------

Ayuda se utiliza para acceder a la información sobre lighttpd. Para una consulta rápida con los comandos de ayuda en cualquiera de las versiones de ptdeploy también puede utilizar el comando de ayuda. El comando de ayuda es un comando interno y está disponible en el módulo ptdeploy.

.. code-block:: bash
   
               ptdeploy lighttpdcontrol help

La siguiente captura de pantalla y ayuda al usuario a la servidumbre con ptdeploy.

.. code-block:: bash

 kevell@corp:/# ptdeploy LighttpdControl help
 ******************************


  This command is part of Default Modules and handles Lighttpd Server Control Functions.

  LighttpdControl, lighttpdcontrol, lighttpdctl

          - start
          Start the Lighttpd server
          example: ptdeploy lighttpdcontrol start
          example: ptdeploy lighttpdcontrol start --yes

          - stop
          Stop the Lighttpd server
          example: ptdeploy lighttpdcontrol stop
          example: ptdeploy lighttpdcontrol stop --yes

          - restart
          Restart the Lighttpd server
          example: ptdeploy lighttpdcontrol restart
          example: ptdeploy lighttpdcontrol restart --yes

          - reload
          Reloads the Lighttpd server configuration without restarting
          example: ptdeploy lighttpdcontrol reload
          example: ptdeploy lighttpdcontrol reload --yes

 ------------------------------
 End Help
 ******************************

Parámetro Alternativa
--------------------------------

Preferiblemente usando Lighttpd el usuario puede esfuerzo las siguientes opciones.

LighttpdControl, lighttpdcontrol, lighttpdctl.

comienzo
-------------

Opción utilizada para iniciar el servidor lighttpd Iniciar. Lighttpdcontrol es una sesión interactiva que se ejecuta con la opción módulo ptdeploy. Dependiendo de cómo se ejecuta el servidor, el comando de arranque podría ser almacenado en un guión, en el registro de Linux.

El servidor se puede iniciar el uso de un simple comando con la opción de conectarse de nuevo con el control de servidor para obtener opciones adicionales.

.. code-block:: bash
   
               ptdeploy lighttpdcontrol start

después de escribir el comando, que permite al usuario iniciar el funcionamiento del servidor lighttpd.


.. code-block:: bash

 kevell@corp:/# ptdeploy lighttpdcontrol start 

 Do you want to Start Lighttpd? (Y/N) 
 y 
 Starting Lighttpd... 
 * Starting web server lighttpd 
   ...done. 
 ****************************** 

 1Lighttpd Controller Finished 
 ****************************** 

.. code-block:: bash


 kevell@corp:/# ptdeploy lighttpdcontrol start --yes 

 Starting Lighttpd... 
 * Starting web server lighttpd 
   ...done. 
 ****************************** 

 1Lighttpd Controller Finished 
 ****************************** 




Deténgase
-------------

Esta opción de parada se utiliza para detener el servicio lighttpd. Específicamente Ubuntu Linux, el comando de parada llama al lighttpd para detener un trabajo que se ejecuta en el sistema. Es equivalente a la parada del servicio de mandatos. A continuación se muestra una descripción completa del comando de parada.

.. code-block:: bash
   
               ptdeploy lighttpdcontrol stop

Después de la entrada como el comando anterior, el servicio se detiene la función.


.. code-block:: bash

 kevell@corp:/# ptdeploy lighttpdcontrol stop 

 Do you want to Stop Lighttpd? (Y/N) 
 y 
 Stopping Lighttpd... 
 * Stopping web server lighttpd 
   ...done. 
 ****************************** 

 1Lighttpd Controller Finished 
 ****************************** 


.. code-block:: bash

 
 kevell@corp:/# ptdeploy lighttpdcontrol stop --yes 

 Stopping Lighttpd... 
 * Stopping web server lighttpd 
   ...done. 
 ****************************** 

 1Lighttpd Controller Finished 
 ****************************** 


reanudar
------------

El término se refiere a un reinicio del sistema operativo de cerrar todos los programas antes de un arranque en caliente del servidor lighttpd. Reiniciar veces es necesario para recuperarse de un error, o para reiniciar los controladores o dispositivos de hardware. Un programa de almacenamiento informático normalmente realizar un reinicio con el siguiente comando simple.

.. code-block:: bash
   
               ptdeploy lighttpdcontrol restart

Después de la entrada como el comando anterior, el servicio, reinicie el servicio lighttpd.


.. code-block:: bash

 kevell@corp:/# ptdeploy lighttpdcontrol restart 

 Do you want to Restart Lighttpd? (Y/N) 
 y 
 Restarting Lighttpd... 
 * Stopping web server lighttpd 
   ...done. 
 * Starting web server lighttpd 
   ...done. 
 ****************************** 

 1Lighttpd Controller Finished 
 ****************************** 


.. code-block:: bash


 kevell@corp:/# ptdeploy lighttpdcontrol restart --yes 

 Restarting Lighttpd... 
 * Stopping web server lighttpd 
   ...done. 
 * Starting web server lighttpd 
   ...done. 
 ****************************** 

 1Lighttpd Controller Finished 
 ****************************** 



recargar
------------

Recargar significa que las cosas están cambiando. El lighttpd está experimentando una revisión y una limpieza. Facilita la reutilización de lighttpd y servicios. Sin matar el proceso se puede recargar lighttpd. El siguiente comando assis el usuario para recargar. Junto con el comando si el uso del usuario sí .. opciones sin hacer ninguna pregunta de forma automática puede funcionar.

.. code-block:: bash
   
               ptdeploy lighttpdcontrol reload

.. code-block:: bash

 kevell@corp:/# ptdeploy lighttpdcontrol reload 
 
 Do you want to Reload Lighttpd? (Y/N) 
 y 
 Reloading Lighttpd... 
 * Reloading web server configuration lighttpd 
   ...done. 
 ****************************** 

 1Lighttpd Controller Finished 
 ****************************** 

.. code-block:: bash



 kevell@corp:/# ptdeploy lighttpdcontrol reload --yes 

 Reloading Lighttpd... 
 * Reloading web server configuration lighttpd 
   ...done. 
 ****************************** 

 1Lighttpd Controller Finished 
 ****************************** 




Beneficios
--------------

* Hosting virtual flexible.
* Compatible con todo tipo de módulos.
* Ligero (menos de 1 MB).
* No mayúsculas y minúsculas.
* El usuario puede funcionar según su deseo.
* La terminación es posible.
* La automatización es posible.
