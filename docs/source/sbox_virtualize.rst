=======
Box
=======

sinopsis
------------

Este módulo ayuda a los usuarios en el manejo y gestión de las cajas que están disponibles en el ptvirtualize. Veamos cómo funciona este módulo en el manejo de las funciones de la caja.


comando Ayuda
---------------------

El comando ayuda guía a los usuarios sobre la finalidad y así como sobre las opciones que se incluyen en el módulo de caja. Enumera los parámetros alternativos del módulo de caja. También describe la sintaxis para utilizar al agregar, quitar, paquete, lista comandos. El comando de ayuda para el módulo de caja se muestra a continuación.


.. code-block:: bash
		
	ptvirtualize Box help

La sintaxis para declarar el comando help no es sensible a mayúsculas que es una ventaja añadida. La siguiente pantalla te visualizar sobre el comando ayuda debajo de caja.



.. code-block:: bash

 kevell@corp:/# ptvirtualize Box help

 ******************************
 Pharaoh Tools - Virtualize
 ******************************


  This command allows you to manage the Base boxes available to you in ptvirtualize

  Box, box

        - add
        Initialises the Box as usable by ptvirtualize
        example: ptvirtualize box add
        example: ptvirtualize box add --yes --guess
            --source="/home/dave/file.box" # where the box file is
            --target="opt/ptvirtualize/boxes" # will guess the dir next to ptvirtualize install dir
            --name="vanillaubuntu"

        - remove
        Removes the box as usable by ptvirtualize
        example: ptvirtualize box remove

        - package
        Packages a box as usable by ptvirtualize
        example: ptvirtualize box package
        example ptvirtualize box package --yes --guess
            --name="Vanilla Ubuntu 12.04 amd 64"
            --vmname="a4dc638f-2721-40c4-a943-2f2565c83fee" # use name or id of virtual machine
            --provider="virtualbox" # guess will use virtualbox
            --group="ptvirtualize"
            --slug="" # guess can generate this based on name field
            --description="A Vanilla install of Ubuntu..."
            --home_location="http://www.someplace.net/" # guess will set this to http://www.ptvirtualizeboxes.co.uk/
            --target="/opt/ptvirtualize/boxes" # save location, will guess /opt/ptvirtualize/boxes

        - list
        List boxes installed in ptvirtualize
        example: ptvirtualize box list

 ------------------------------
 End Help
 ******************************

Funciones de ptvirtualize caja 
----------------------------------

Como se muestra en el comando anterior ayuda las funciones del cuadro de ptvirtualize incluye lo siguiente:


* Add
* Remove
* Package
* List

Add
-----

El complemento se utiliza para inicializar la caja como utilizable por ptvirtualize. Puede utilizarse la siguiente sintaxis para agregar un cuadro de ptvirtualize.


.. code-block:: bash

		ptvirtualize box add

or

.. code-block:: bash

	ptvirtualize box add --yes --guess
	--source="/home/dave/file.box	(This line describes where the box is)
	--target="opt/ptvirtualize/boxes"	(This line guess the dir next to ptvirtualize install dir)
	--name="vanillaubuntu"

In the above mentioned ways the box can be added to a ptvirtualize.

Remove
-----------

Esta función se utiliza para quitar el cuadro como utilizable por ptvirtualize. Esto puede hacerse utilizando el comando se muestra a continuación:

.. code-block:: bash

		ptvirtualize box remove

En las formas mencionadas puede eliminarse el cuadro de un ptvirtualize.


Package
-----------

Esta función se utiliza para empaquetar la caja como utilizable por ptvirtualize. Esto puede implementarse usando el siguiente comando:


.. code-block:: bash

		ptvirtualize box package

or

.. code-block:: bash

	ptvirtualize box package --yes --guess
	name="Vanilla Ubuntu 12.04 amd 64"
	vmname="a4.............." (This two lines represents the name and id of virtual machine)
	--provider="virtualbox" (guess will use virtual box)
	--group="ptvirtualize"
	--slug="" (The guess can generate this based on the name field)
	--description="A vanilla install of Ubuntu..."
	--home_location="http://www.someplace.net/" (guess will set this to http://www.ptvirtualizeboxes.co.uk/
	--target="/opt/ptvirtualize/boxes" (The location for saving)



Finalmente, una caja de empaquetado como utilizable por la ptvirtualize.


List
-----

Esta función se utiliza para enumerar las cajas que se instalan en ptvirtualize. Esto puede hacerse usando el siguiente comando,


.. code-block:: bash

		ptvirtualize box list

Utilizando el comando anterior, se mostrará la lista de las cajas ptvirtualize que están recién instalados.


parámetros alternativos
-------------------------------

* Box
* box


En la lista antes mencionada, cualquiera de los parámetros alternativos pueden utilizarse en la declaración.

beneficios
-----------

* Los parámetros utilizados en la ayuda no es sensible a mayúsculas que es una ventaja añadida mientras que comparado con otros. 
* Está acomodada en ambos Ubuntu y así como ciento so. 
* La sintaxis para usar agregar, quitar, paquete, la lista no son mayúsculas y minúsculas.

