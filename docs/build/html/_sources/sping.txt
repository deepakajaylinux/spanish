==========
Ping
==========

sinopsis
-----------

Como verbo, PING significa "para llamar la atención de" o "para comprobar la presencia de" la otra parte en línea. PING módulo (Packet Internet Groper) utiliza para probar la conectividad del sistema. PING utiliza para enviar los datos de red a, y recibir datos de la red de, otro equipo de una red. PING utiliza con frecuencia para probar, si otro sistema es accesible a través de una red, y si es así, ¿cuánto tiempo se necesita para que los datos que se intercambian.

comando Ayuda
-------------------

Este comando ayuda a determinar el uso del módulo de PING. Este comando figura ayuda a las opciones para utilizar junto con el comando PING. Este comando guiará al usuario final para saber el uso de diferentes opciones y la sintaxis de esas opciones. A continuación dado son el mando y la pantalla del mismo.

.. code-block:: bash

	ptconfigure ping help

.. code-block:: bash

 kevell@corp:/# ptconfigure ping help

 ******************************


  This command allows you to test the status of ports

  Ping, ping

        - once
        ping a target once
        example: ptconfigure ping once --yes --guess
            --target=www.google.com # url/ip to ping test
            --interval=5 # no seconds to wait between requests, will guess 2

        - ten
        ping a target ten times
        example: ptconfigure ping ten --yes --guess
            --target=www.google.com # url/ip to ping test
            --interval=5 # no seconds to wait between requests, will guess 2

        - until-responding
        ping a target for a set amount of time until it responds
        example: ptconfigure ping once --yes --guess
            --target=www.google.com # url/ip to ping test
            --interval=5 # no seconds to wait between requests, will guess 2
            --max-wait=100 # no seconds in total to keep trying, will guess 60

 ------------------------------
 End Help
 ******************************

Opciones
-----------

Módulo PING tiene tres opciones diferentes, que recuperan datos como por la opción utilizada en los comandos. Por debajo de la mesa, explica la misma

.. cssclass:: table-bordered

 +--------------+----------------------------------------------+-----------------------------------------------------------------+
 | Options      | Befehle                                      | Funktionen                                                      |
 +==============+==============================================+=================================================================+
 |Once          | ptconfigure ping once – yes –guess –         | Nos ping a un destino una vez. Una vez que la opción            |
 |              | target=google.com – interval=5               | será recuperar los datos una sola vez                           |
 +--------------+----------------------------------------------+-----------------------------------------------------------------+
 |Ten           | ptconfigure ping ten – yes –guess –          | Diez datos de extracción de opciones para diez veces, con       |
 |              | target=google.com – interval=5               | intervalo de tiempo como de 5 segundos [espera a segundos antes |
 |              |                                              | de enviar el siguiente paquete                                  |
 +--------------+----------------------------------------------+-----------------------------------------------------------------+
 |Until-        | ptconfigure ping once – yes –guess           | Nos ping al destino de una cantidad fija de tiempo hasta que se |
 |responding    | --target=google.com -- interval=5            | responde , que tiene tiempo de intervalo como 5 segundos y un   |
 |              | -- max-wait=100                              | máximo de 100 segundos para tratar de la meta|                  |
 +--------------+----------------------------------------------+-----------------------------------------------------------------+


Nota:

* Intervalo - Número de segundos a esperar entre cada solicitud
* Max-espera - El número de segundos en total para seguir intentando
* Tiempo de intervalo y Max-espera frecuencia de tiempo puede ser decidida por el usuario como por la exigencia

Una vez Opción
-------------------

.. code-block:: bash

 kevell@corp:/# ptconfigure ping once --yes --guess --target=www.google.com

 [Pharaoh Logging] Ping Latency is 34 ms
 ******************************


 Ping Modifications:
 --------------------------------------------
 
 Ping: Success

 ------------------------------
 Ping Mods Finished
 ******************************

Diez Opción
---------------

.. code-block:: bash

 kevell@corp:/# ptconfigure ping ten --yes --guess --target=www.google.com 

 [Pharaoh Logging] Ping Latency is 36 ms
 [Pharaoh Logging] Ping Latency is 34 ms
 [Pharaoh Logging] Ping Latency is 34 ms
 [Pharaoh Logging] Ping Latency is 34 ms
 [Pharaoh Logging] Ping Latency is 36 ms
 ******************************


 Ping Modifications:
 --------------------------------------------

 Ping: Success

 ------------------------------
 Ping Mods Finished
 ******************************

hasta responder
---------------------

.. code-block:: bash

 kevell@corp:/# ptconfigure ping once -- yes --guess --target=google.com -- interval=5 -- max-wait=100

 [Pharaoh Logging] Ping Latency is 37 ms
 ******************************


 Ping Modifications:
 --------------------------------------------

 Ping: Success

 ------------------------------
 Ping Mods Finished
 ******************************

parámetros alternativos
-----------------------

Los parámetros alternativos para este módulo son:

Ping

ping

Beneficios
------------

PING ayuda al usuario a verificar una existencia determinada dirección IP y puede aceptar la solicitud. Comando PING es la mejor manera de probar la conectividad entre dos nodos. Ya se trate de la red de área local (LAN) o red de área amplia (WAN).
