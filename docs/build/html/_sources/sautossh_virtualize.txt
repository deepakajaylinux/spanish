==========
AutoSSH
==========


sinopsis
-----------

Este módulo facilita a los usuarios a autoSSH una caja de ptvirtualize. Autossh es un front-end para SSH que puede controlar la conexión y reinicie el túnel si cae o deja de responder.


autossh utiliza ssh para construir un bucle de ssh expediciones (uno de local a remoto, uno de control remoto al local), y luego envía datos que espera volver de prueba.


Veamos las funciones de auto ssh en próximos temas.


comando Ayuda
-------------------

El comando ayuda guía a los usuarios sobre la finalidad y así como sobre las opciones que se incluyen en el módulo de Auto SSH. Enumera los parámetros alternativos del módulo Auto SSH. También describe la sintaxis para utilizar la cli, sftp_put, sftp_get los comandos. El comando de ayuda para el módulo de Auto SSH se muestra a continuación.



.. code-block:: bash

	ptvirtualize AutoSSH help


La sintaxis para declarar el comando help no es sensible a mayúsculas que es una ventaja añadida. La siguiente pantalla te visualizar sobre el comando ayuda bajo Auto SSH.



.. code-block:: bash


 kevell@corp:/# ptvirtualize AutoSSH help

 ******************************
 Pharaoh Tools - Virtualize
 ******************************


  This command allows you to autoSSH a ptvirtualize box

  AutoSSH, auto-ssh, autossh, ssh, SSH

        - cli
        Open an SSH Cli to your ptvirtualize Box
        example: ptvirtualize auto-ssh cli --yes --guess

        - sftp-put
        SFTP Put a file on to your ptvirtualize Box
        example: ptvirtualize auto-ssh sftp-put --yes --guess --source=/path/to/source --target=/path/to/target

        - sftp-get
        SFTP Get a file from your ptvirtualize Box
        example: ptvirtualize auto-ssh sftp-get --yes --guess --source=/path/to/source --target=/path/to/target

 ------------------------------
 End Help
 ******************************


Funciones de autossh
----------------------

Como se muestra en el comando de ayuda anterior, las principales funciones de este auto ssh módulo incluye


* cli
* sftp_put
* sftp_get


Cli
------

Después de activar o construir un auto ssh en el entorno de los usuarios, puede crear la cli que se utiliza para abrir un SSH Cli a la caja de ptvirtualize de los usuarios mediante el siguiente comando:


.. code-block:: bash

	ptvirtualize auto-ssh cli --yes --guess


La cli se utiliza para enumerar a los clientes disponibles en un entorno particular donde el ssh es generados automáticamente.

Sftp_put
-----------

Esta función se utiliza para colocar o mover los archivos requeridos o los datos desde el origen al destino de un entorno particular donde el ssh es generados automáticamente. Esto puede hacerse mediante el comando siguiente:


.. code-block:: bash

		ptvirtualize auto-ssh sftp-put --yes --guess --source="path/to/source --target=/path/to/target

El comando mostrado arriba pondrá un archivo en el cuadro de ptvirtualize de los usuarios. La captura de pantalla siguiente muestra visualmente el proceso.



Sftp_get
-----------

Esta función se utiliza para obtener o buscar los archivos requeridos o los datos desde el origen al destino de un entorno particular donde el ssh es generados automáticamente. Esto puede hacerse mediante el comando siguiente:


.. code-block:: bash

		ptvirtualize auto-ssh sftp-get --yes --guess --source="path/to/source --target=/path/to/target

El comando mostrado arriba se obtiene o recibe un archivo desde el cuadro de ptvirtualize de los usuarios. La captura de pantalla siguiente muestra visualmente el proceso.



parámetros alternativos
-----------------------------

* AutoSSH
* auto-ssh
* autossh
* ssh
* SSH

En la lista antes mencionada cualquiera de los parámetros alternativos pueden utilizarse en la declaración.


beneficios
-----------

* Los parámetros utilizados en la ayuda y las operaciones de instalación instalación y Naciones Unidas no son mayúsculas y minúsculas que es un  a  ventaja añadida mientras que comparado con otros. 
* Está acomodada en ambos Ubuntu y así como ciento so. 
* La lista de funciones de cli outs los clientes disponibles en un entorno determinado con la ayuda de auto SSH. 
* Sftp_put, Sftp_get puede colocar y buscar los archivos respectivamente entre origen y destino de un entorno determinado mediante el uso de
  auto SSH. 
* La sintaxis para declarar la cli, puesto, consigue son claramente representados en el comando de ayuda.

