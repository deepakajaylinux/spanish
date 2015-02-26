========
Dnsify
========

sinopsis
-----------

Esta módulos sobres las principales necesidades de los usuarios que gestionan DNS. Este tema es discutir acerca de cómo utilizar este módulo, y sobre varias funciones en el uso de dnsify.

Ayuda Comando
----------------------

El comando de ayuda guía a los usuarios en el manejo de este módulo, con el fin de manejar y realizar diversas funciones de una caja. En él se enumeran las salidas de los parámetros alternativos, y resalta la sintaxis para las diversas funciones de uso y modificación de una caja. La sintaxis de opción de ayuda en el marco del módulo dnsify se muestra a continuación,

.. code-block:: bash

	ptconfigure DNSify help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda bajo dnsify.

.. code-block:: bash

 kevell@corp:/# ptconfigure Dnsify help 
 ****************************** 

  This command provides a generic Box Management wrapper around all of the Box Providers (Cloud and Otherwise) so that we have a 
  generic way to create and destroy boxes. 

  DNSify, dnsify 

        - install-generic-autopilots 
        Install the generic Dnsify autopilot templates for a Tiny or Medium (Current Default) set of Environments 
        example: ptconfigure dnsify install-generic-autopilots 
        example: ptconfigure dnsify install-generic-autopilots 
                    --yes 
                    --guess # will set --destination-dir=*this dir +*build/config/ptconfigure/dnsify/autopilots/ 
                    --template-group=tiny 
                    --destination-dir=*path-to-destination* 

        - box-add 
        Installs a Box through a cloud provider 
        example: ptconfigure dnsify box-add --environment-name="*environment*" 
            --server-prefix="my-app" 
            --provider="DigitalOcean" // DigitalOcean, Rackspace, VSphere 
            --image-id="3101045" // DO=3101045 , RAX=ffd597d6-2cc4-4b43-b8f4-b1006715b84e 
            --size-id="66" // DO = 66, RAX = 2 
            --region-id="2" // DO = 2, RAX = LON 
            --box-amount=1 // An Integer number of boxes to create 
            --force-name="a-box-name" // optional, will override other options for name creation. may cause a conflict if creating more than 1 box. 
            --parallax // optional, when adding more than one box, if the provider supports it we can execute all requests in parallel 

        - box-remove 
        Removes a Box from the papyrus 
        example: ptconfigure dnsify box-remove --environment-name="staging" --environment-version="5.0" --provider="apt-get" 

        - box-destroy 
        Removes a Box from both papyrus and the cloud provider 
        example: ptconfigure dnsify box-destroy --environment-name="staging" 
            --destroy-all-boxes 
            --destroy 

        - list-papyrus 
        List all servers in papyrus, or those of a particular environment 
        example: ptconfigure dnsify list-papyrus --yes 
        example: ptconfigure dnsify list-papyrus --yes --environment-name="staging" 


 ------------------------------ 
 End Help 
 ****************************** 

Varias funciones de dnsify
------------------------------


Este tema describe acerca de las diversas funciones de dnsify bajo este módulo, como se indica a continuación


* Instale pilotos automáticos genéricos
* Caja Adición
* Caja de Extracción
* La destrucción de una caja
* lista


Instale pilotos automáticos genéricos
----------------------------------------

Esta función tiene por objeto la instalación de los pilotos automáticos aplicables a una pequeña o mediana conjunto de ambientes. Esto se puede implementar mediante la aplicación del comando como se indica a continuación,

.. code-block:: bash
	
	ptconfigure dnsify install-generic-autopilots 
                    --yes 
                    --guess # will set --destination-dir=*this dir +*build/config/ptconfigure/dnsify/autopilots/ 
                    --template-group=tiny 
                    --destination-dir=*path-to-destination* 

Como se muestra en la sintaxis mencionado de que el usuario tiene que especificar los siguientes campos para instalar los pilotos automáticos genéricos.

* Directorio de destino
* Plantilla grupo

cuadro Adición
-------------------

Esta función tiene por objeto la adición de una caja a través de un proveedor de la nube, simplemente usando el siguiente comando,

.. code-block:: bash

 example: ptconfigure dnsify box-add --environment-name="*environment*" 
            --server-prefix="my-app" 
            --provider="DigitalOcean" // DigitalOcean, Rackspace, VSphere 
            --image-id="3101045" // DO=3101045 , RAX=ffd597d6-2cc4-4b43-b8f4-b1006715b84e 
            --size-id="66" // DO = 66, RAX = 2 
            --region-id="2" // DO = 2, RAX = LON 
            --box-amount=1 // An Integer number of boxes to create 
            --force-name="a-box-name" // optional, will override other options for name creation. may cause a conflict if creating more than 1 box. 
            --parallax // optional, when adding more than one box, if the provider supports it we can execute all requests in parallel 

El usuario tiene que especificar los siguientes campos como se muestra en el comando anterior,

* Nombre del medio ambiente
* Prefijo de servidor
* proveedor
* Identificación imagen
* Cantidad caja (debe ser un valor entero para indicar el número de cajas que se añade)
* Nombre de la Fuerza (nombre de buzón)
* Paralaje (Es opcional, se puede utilizar cuando la adición de más de una casilla.)

cuadro de Extracción
---------------------------

Esta función tiene como objetivo la eliminación de una caja del papiro. Esto se puede implementar mediante el comando a continuación,

.. code-block:: bash

	ptconfigure dnsify box-remove --environment-name="staging" --environment-version="5.0" --provider="apt-get" 

El usuario tiene que especificar los siguientes campos como se muestra en el comando anterior,

* Nombre del medio ambiente
* Versión medio ambiente
* proveedor

La destrucción de una caja
-----------------------------------

Esta función tiene como objetivo la eliminación de una caja del papiro. Esta función se puede implementar simplemente usando el siguiente comando,

.. code-block:: bash

	ptconfigure dnsify box-destroy --environment-name="staging" 
            --destroy-all-boxes 
            --destroy

El comando se ha mencionado anteriormente se utiliza para la destrucción de todas las cajas de un entorno particular.


lista
-----
El principal objetivo de esta función es hacer una lista de todos los servidores de un papiro en particular o en un entorno. La sintaxis para la inclusión de todos los servidores se muestra a continuación,
.. code-block:: bash

	ptconfigure dnsify list-papyrus --yes --environment-name="staging"

El comando anterior mencionado enumerará fuera papiro de un entorno determinado.

parámetros alternativos
-------------------------------

Los parámetros alternativos para este módulo, cualquiera de los cuales se pueden utilizar en la declaración es,

* DNSify
* dnsify

Beneficios
-------------

* La sintaxis utilizada en la ayuda y otras operaciones de caja no distinguen entre mayúsculas y minúsculas.
* Es-acomodados tanto en OS Cent y así como en Ubuntu.
* Todas las funciones principales de la gestión de una caja en la gestión de DNS se envuelve bajo este único módulo.
