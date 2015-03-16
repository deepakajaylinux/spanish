===========
Hostname
===========

sinopsis
---------------
Dado que las direcciones IP son bastante difíciles de recordar (y no son particularmente descriptiva), el Internet también permite al usuario especificar un ordenador por un nombre en lugar de una serie de números. Toda esta cadena se conoce como nombre de host del er comput. Hay dos opciones disponibles. Mostrar y Cambio. Mediante el uso de este módulo el usuario puede ver o modificar el nombre de host.

comando Ayuda
-----------------------

Este comando puede funcionar sobre los objetivos y los comandos disponibles bajo módulo de nombre de host. También explica el comando para modificar el nombre de host del módulo. Antes de modificar el nombre de host, el usuario lea este comando de ayuda explica su función.

.. code-block:: bash
         
                ptconfigure hostname help

La siguiente captura de pantalla puede traer a la mente la misma.

.. code-block:: bash

 kevell@corp:/# ptconfigure hostname help

 ******************************


  This command allows you to view or modify hostname

  Hostname, hostname

        - change
        Change the system hostname
        example: ptconfigure hostname change --hostname="my-laptop"

        - show
        Show the system hostname
        example: ptconfigure hostname show

 ------------------------------
 End Help
 ******************************


cambio
----------------

Los nombres de host se utilizan normalmente en una capacidad administrativa y pueden aparecer en las listas de computadora del navegador, listas de directorios activos, dirección IP a resoluciones de nombre de host, encabezados de correo electrónico, etc. Cuando el usuario quiere cambiar el nombre de host, puede utilizar el siguiente comando.

.. code-block:: bash

	ptconfigure hostname change –hostname=”kevellcorp”

Desde el comando anterior el nuevo nombre de host puede entrar.

.. code-block:: bash

 kevell@corp:/# ptconfigure hostname change –hostname=”kevellcorp”
 Enter Hostname:
 kevellcorp
 ******************************


 Hostname Modifications:
 --------------------------------------------

 Hostname: Success

 ------------------------------
 Hostname Mods Finished
 ******************************




show
-------------------

Este módulo es un proceso perceptible para ver el nombre de host en ptconfigure sólo por el uso de la orden dada a continuación,

.. code-block:: bash
         
                ptconfigure hostname show

Después de clave en el comando, se muestra el nombre de host.




opción
------------

.. cssclass:: table-bordered


 +---------------------------+---------------------------------+---------------+----------------------------------------------+
 | Parámetros                | Parámetro Alternativa           | Opciones      | Comentarios                                  |
 +===========================+=================================+===============+==============================================+
 |ptconfigure hostname       | En lugar de Hostname podemos    | Show          | Sistema comienza a mostrar el proceso de     |
 |                           | utilizar hostname               |               | nombre de host en ptconfigure                |
 +---------------------------+---------------------------------+---------------+----------------------------------------------+
 |ptconfigure hostname       | En lugar de Hostname podemos    | Change        | Sistema comienza a cambiar el proceso de     |
 |change –hostname=”Name”    | utilizar hostname               |               | nombre de host en ptconfigure|               |
 +---------------------------+---------------------------------+---------------+----------------------------------------------+


Beneficios
-------------

* Los nombres de host pueden ser nombres simples de una sola palabra o una frase, o pueden ser estructurada.
* Los nombres de host puede ser no sensible.
* Nombre de host puede ver y modificar fácilmente.

