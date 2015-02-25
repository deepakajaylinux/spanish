================
DigitalOcean
================

sinopsis
------------

Este módulo ayuda a los usuarios en el manejo de los servidores en el océano digital. Se envuelve todas las necesidades básicas de los usuarios en el manejo de cajas en el océano digital.

Los temas próximos discute acerca de cómo utilizar este módulo, las diversas características del océano digital bajo este módulo.

Ayuda Comando
----------------------

El comando ayuda actúa como un breve manual de usuario. En él se describe sobre el objetivo principal de este módulo. En él se enumeran las salidas de parámetros alternativos que se pueden utilizar en las declaraciones. Además, también se pone de relieve las diferentes características de la utilización del océano digital bajo este módulo junto con la sintaxis para su uso. El comando utilizado para la declaración de opción de ayuda se muestra a continuación,

.. code-block:: bash

		ptconfigure DigitalOcean help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda bajo Océano Digital.

.. code-block:: bash

 kevell@corp:/# ptconfigure DigitalOcean help
 ******************************


    This is an extension provided for Handling Servers on Digital Ocean.

    DigitalOcean, digitaloceanv1, digital-ocean-v1

        - box-add
        Lets you add boxes to Digital Ocean, and adds them to your papyrusfile
        example: ptconfigure digital-ocean box-add
                    --yes
                    --digital-ocean-ssh-key-path="/home/dave/.ssh/bastion.pub"
                    --digital-ocean-ssh-key-name="bastion"

        - box-destroy
        Will destroy box/es in an environment for you, and remove them from the papyrus file
        example: ptconfigure digital-ocean box-destroy --yes --guess --digital-ocean-ssh-key-path="/home/dave/.ssh/bastion.pub" --digital-ocean-ssh-key-name="bastion"

        - box-destroy-all
        Will destroy all boxes in your digital ocean account - Careful - its irreversible
        example: ptconfigure digital-ocean box-destroy-all --yes --guess

        - save-ssh-key
        Will let you save a local ssh key to your Digital Ocean account, so you can ssh in to your nodes
        securely and without a password
        example: ptconfigure digital-ocean save-ssh-key
                    --yes
                    --digital-ocean-ssh-key-path="/home/dave/.ssh/bastion.pub"
                    --digital-ocean-ssh-key-name="bastion"

        - list
        Will display data about your digital ocean account
        example: ptconfigure digital-ocean list
        example: ptconfigure digital-ocean list --yes
                    --guess # use project saved connection details if possible
                    --type=sizes # droplets, sizes, images, domains, regions, ssh_keys

 ------------------------------
 End Help
 ******************************

Características del océano digital
-------------------------------------------

Como se muestra en el comando de ayuda anterior, este módulo tiene varias características en el uso de océano digital como se indica a continuación

* Box_Add
* Box_Destroy
* Box_Destroy_All
* Save_ssh_Key
* Lista


Box_Add
------------

Esta función tiene por objeto la adición de cajas para el océano digital y en la mano les agregar al archivo papiro. Esto se puede implementar simplemente utilizando la sintaxis como se indica a continuación,

.. code-block:: bash

	ptconfigure digital-ocean box-add
                    --yes
                    --digital-ocean-ssh-key-path="/home/dave/.ssh/bastion.pub"
                    --digital-ocean-ssh-key-name="bastion"


Para implementar el comando anterior, el usuario tiene que especificar los siguientes campos en el formato de la sintaxis mencionada.

* Camino digital océano SSH-clave
* Nombre digital océano clave ssh

Box_Destroy
----------------

Esta característica tiene como objetivo destruir las cajas en un entorno determinado y en la mano eliminarlos del archivo de papiro. Esto se puede implementar simplemente utilizando la sintaxis como se indica a continuación,

.. code-block:: bash

	ptconfigure digital-ocean box-destroy --yes --guess --digital-ocean-ssh-key-path="/home/dave/.ssh/bastion.pub" 
        --digital-ocean-ssh-key-name="bastion"

Para implementar el comando anterior, el usuario tiene que especificar los siguientes campos en el formato de la sintaxis mencionada.

* Camino digital océano SSH-clave
* Nombre digital océano clave ssh

Box_Destroy_All
----------------------

Esta característica tiene como objetivo la destrucción de todas las cajas en la cuenta océano digital. El usuario debe tener cuidado al implementar esta cuenta, ya que es un proceso irreversible. Para implementar esta función, el usuario tiene que aplicar el comando como se indica a continuación,

.. code-block:: bash
   
	ptconfigure digital-ocean box-destroy-all --yes --guess

Save_Ssh_key
-------------------

Esta función permite a los usuarios guardar un ssh local a su océano digital por lo que los usuarios pueden ssh en sus nodos de forma segura y sin contraseña. Esto se puede lograr mediante el comando de abajo,

.. code-block:: bash

	ptconfigure digital-ocean save-ssh-key
                    --yes
                    --digital-ocean-ssh-key-path="/home/dave/.ssh/bastion.pub"
                    --digital-ocean-ssh-key-name="bastion"

Para implementar el comando anterior, el usuario tiene que especificar los siguientes campos en el formato de la sintaxis mencionada.

* Camino digital océano SSH-clave
* Nombre digital océano clave ssh

lista
-----

Esta función permite a los usuarios hacer una lista de todos los datos de su cuenta océano digital. Esto se puede implementar simplemente usando el siguiente comando,

.. code-block:: bash

	ptconfigure digital-ocean list


or

.. code-block:: bash

        ptconfigure digital-ocean list --yes
                    --guess # use project saved connection details if possible
                    --type=sizes # droplets, sizes, images, domains, regions, ssh_keys

parámetros alternativos
----------------------------

Los parámetros alternativos para este módulo, cualquiera de los cuales se pueden utilizar en la declaración es,

DigitalOcean,   digitaloceanv1,   digital-ocean-v1

Beneficios
--------------

* Los parámetros utilizados declarando ayuda y otras características diferentes de apt no distinguen entre mayúsculas y minúsculas.
* Es-acomodado tanto os Cent y así como en Ubuntu.
* Este módulo envuelve todas las necesidades de los usuarios en el manejo de Océano digital.
