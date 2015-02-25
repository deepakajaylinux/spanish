===========
Firewall
===========

sinopsis
----------

Un firewall es un sistema de seguridad de la red que controla el tráfico de red entrante y saliente en base a un conjunto de reglas aplicadas. Existen Firewalls tanto como una solución de software y como un dispositivo de hardware.

comando Ayuda
---------------------

Este comando ayuda ayudar al usuario acerca de Ptconfigure. Guía al usuario permiso.

El usuario puede hacer la modificación según el deseo. Ayuda imagen guiará al usuario. Vamos a visualizar la misma.

.. code-block:: bash

  ptconfigure Firewall help

La captura de pantalla para el comando anterior se enumeran a continuación,

.. code-block:: bash

 kevell@corp:/# ptconfigure Firewall help
 ******************************
 This command allows you to modify create or modify firewalls

  Firewall, firewall

        - enable
        Enable system firewall
        example: ptconfigure firewall enable

        - disable
        Disable system firewall
        example: ptconfigure firewall disable

        - allow
        Allow a Firewall rule
        example: ptconfigure firewall allow --firewall-rule="ssh/tcp"

        - deny
        Deny a Firewall rule. Allow connection attempts to be ignored and time out.
        example: ptconfigure firewall deny --firewall-rule="ssh/tcp"

        - reject
        Reject a Firewall rule. Terminate connections attempts with an error to the connector.
        example: ptconfigure firewall reject --firewall-rule="ssh/tcp"

        - limit
        Limit a Firewall rule. ufw will deny connections if an IP address has attempted
        to initiate 6 or more connections in the last 30 seconds.
        example: ptconfigure firewall limit --firewall-rule="ssh/tcp"

        - delete
        Delete a Firewall rule.
        example: ptconfigure firewall delete --firewall-rule="ssh/tcp"

        - insert
        Insert a Firewall rule.
        example: ptconfigure firewall insert --firewall-rule="ssh/tcp"

        - reset
        Reset a Firewall rule.
        example: ptconfigure firewall reset --firewall-rule="ssh/tcp"

        - default
        Set default policy, should be allow, deny, or reject
        example: ptconfigure firewall default --policy="deny"

 ------------------------------
 End Help
 ******************************

Opciones
-------------

Reglas Firewalls se pueden personalizar según sus necesidades, requisitos y niveles de amenaza de seguridad. El usuario puede crear o desactivar reglas de firewall basado en condiciones tales como:

.. cssclass:: table-bordered

 +----------------------+-----------------------------------------------------------+----------------------------------------+
 | parámetros           | función                                                   | comentario                             |
 +======================+===========================================================+========================================+
 |IP address            | El bloqueo de una determinada dirección IP o un rango de  |                                        | 
 |                      | direcciones IP, lo que usted piensa es depredadora        |                                        |
 +----------------------+-----------------------------------------------------------+----------------------------------------+
 |Enable                | Habilitar firewall del sistema                            | Ptconfigure firewall enable            |
 +----------------------+-----------------------------------------------------------+----------------------------------------+
 |Disable               | Firewall del sistema Desactivar                           | Ptconfigure firewall disable           |
 +----------------------+-----------------------------------------------------------+----------------------------------------+
 |Allow                 | Permitir regla de firewall                                | Ptconfigure firewall allow –firewall-  |
 |                      |                                                           | rule=”ssh/tcp”                         |
 +----------------------+-----------------------------------------------------------+----------------------------------------+
 |Deny                  | Permitir intento de conexión que se ignora y el tiempo    | Ptconfigure firewall deny –firewall-   |
 |                      | de espera                                                 | rule=”ssh/tcp”                         |
 +----------------------+-----------------------------------------------------------+----------------------------------------+
 |Reject                | Terminar los intentos de conexión con un error al         | Ptconfigure firewall reject –firewall- |
 |                      | conector                                                  | rule=”ssh/tcp”                         |
 +----------------------+-----------------------------------------------------------+----------------------------------------+
 |Limit                 | Ufw negará conexiones si una dirección IP tiene 6 o       | Ptconfigure firewall limit –firewall-  |
 |                      | iniciar intentó más conexión en los últimos 30 segundos.  | rule=”ssh/tcp”                         |
 +----------------------+-----------------------------------------------------------+----------------------------------------+
 |Delete                | Eliminar una regla de firewall                            | Ptconfigure firewall delete –firewall- |
 |                      |                                                           | rule=”ssh/tcp”                         |
 +----------------------+-----------------------------------------------------------+----------------------------------------+
 |Insert                | Inserte una regla de firewall                             | Ptconfigure firewall insert –firewall- |
 |                      |                                                           | rule=”ssh/tcp”                         |
 +----------------------+-----------------------------------------------------------+----------------------------------------+
 |Reset                 | Cambiar una regla de firewall                             | Ptconfigure firewall reset –firewall-  |
 |                      |                                                           | rule=”ssh/tcp”                         |
 +----------------------+-----------------------------------------------------------+----------------------------------------+
 |default               | Política predeterminada, debe ser permitir, denegar o     | Ptconfigure firewall default –         |
 |                      | rechazar.                                                 | policy=”deny”|                         |
 +----------------------+-----------------------------------------------------------+----------------------------------------+


Beneficios
--------------

* El servidor de seguridad impide el acceso no deseado al sistema a través de una conexión de red mediante la identificación y prevención de 
  comunicación a través de los puertos de riesgo.
* Sistema de comunicarse a través de muchos puertos reconocidos diferentes, y el servidor de seguridad tiende a permitir que estos sin 
  preguntar o alertar al usuario.
* Los firewalls también pueden detectar la actividad "sospechosa" desde el exterior.
* El usuario puede configurar su dominio de acuerdo a su deseo.
