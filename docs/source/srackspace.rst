============
Rackspace
============

sinopsis
-------------

Rackspace ofrece alto rendimiento , infraestructura confiable para tener éxito en la nube. Se necesita , plataformas optimizadas con todas las funciones , y un equipo de expertos para ejecutar cargas de trabajo.

Rackspace tiene dos líneas principales de negocio - Servidores Cloud y Servidores Dedicados. Rackspace ayuda a diseñar , construir y operar cargas de trabajo en entornos tanto en función de las necesidades individuales del cliente .

Servidores Cloud - El nivel de servicio Infraestructura gestionada proporciona un conjunto básico de servicios necesarios para configurar los clientes en la nube , incluyendo consejos arquitectura, asistencia en seguridad y asistencia para el desarrollo de código (a través de APIs y SDKs ) . El nivel de soporte de operaciones Gestionado ofrece todos los servicios de infraestructura administrados además de soporte proactivo adicional.

Servidores Dedicados - El nivel de servicio Managed consiste en el apoyo a la carta , donde se proporcionan servicios proactivos .


Ayuda Comando
----------------------

Este comando ayuda a determinar el uso de Rackspace . El usuario se llega a saber acerca de la diferente forma / formato de ejecutar este módulo. Este comando guía al usuario final a conocer el propósito de este comando. A continuación dado son el mando y la pantalla del mismo .

.. code-block:: bash


 kevell@corp:/# ptconfigure Rackspace help

 ******************************


    This is an extension provided for Handling Servers on Rackspace.

    Rackspace, rackspace

        - box-add
        Lets you add boxes to Rackspace, and adds them to your papyrusfile
        example: ptconfigure rackspace box-add
                    --yes
                    --rackspace-ssh-key-path="/home/dave/.ssh/bastion.pub"
                    --rackspace-ssh-key-name="bastion"

        - box-destroy
        Will destroy box/es in an environment for you, and remove them from the papyrus file
        example: ptconfigure rackspace box-destroy --yes --guess --rackspace-ssh-key-path="/home/dave/.ssh/bastion.pub" --rackspace-ssh-key-name="bastion"

        - box-destroy-all
        Will destroy all boxes in your Rackspace account - Careful - its irreversible
        example: ptconfigure rackspace box-destroy-all --yes --guess

        - save-ssh-key, sshkey, ssh-key
        Will let you save a local ssh key to your Rackspace account, so you can ssh in to your nodes with it
        securely and without a password
        example: ptconfigure rackspace save-ssh-key
                    --yes
                    --rackspace-ssh-key-path="/home/dave/.ssh/bastion.pub"
                    --rackspace-ssh-key-name="bastion"

        - list
        Will display data about your Rackspace account
        example: ptconfigure rackspace list
        example: ptconfigure rackspace list --yes
                    --guess # use project saved connection details if possible
                    --rackspace-list-data-type=sizes # servers, sizes, images, domains, regions, ssh_keys

        - list-containers
        Will display Container data about your Rackspace account
        example: ptconfigure rackspace list-containers
        example: ptconfigure rackspace list-containers --yes
                    --guess # use project saved connection details if possible

        - list-objects
        Will display object of Containers data about your Rackspace account
        example: ptconfigure rackspace list-objects
        example: ptconfigure rackspace list-objects --yes
                    --guess # use project saved connection details if possible

 ------------------------------
 End Help
 ******************************


Box- add
----------------

Este comando ayuda a añadir cajas de Rackspace , y los agrega a su archivo de papiro. El siguiente comando dado se ejecutará el proceso.

.. code-block:: bash

 ptconfigure rackspace box-add --yes --rackspace-ssh-key-path="/home/dave/.ssh/bastion.pub" --rackspace-ssh-key-name="bastion"

Box- destruir
-------------------

Este comando ayuda a destruir la caja / es en un entorno para usted, y eliminarlos del archivo de papiro. El siguiente comando dado se ejecutará el proceso.

.. code-block:: bash

 ptconfigure rackspace box-destroy --yes --guess --rackspace-ssh-key-path="/home/dave/.ssh/bastion.pub" --rackspace-ssh-key-name="bastion"

Box- destruir - todo
-----------------------

Este comando ayuda a destruir todas las cajas en su cuenta de Rackspace . La parte más crítica es que es irreversible.

.. code-block:: bash     

 ptconfigure rackspace box-destroy-all --yes --guess

Save- ssh- clave
---------------------

Este comando ayuda a ahorrar una clave ssh local a su cuenta de Rackspace , así que usted puede ssh a los nodos con él de forma segura y sin una contraseña . Hay tres parámetros alternativo utilizado para este comando en particular - - clave ssh , sshkey , llave ssh . El siguiente comando dado se ejecutará el proceso.

.. code-block:: bash     
	
	ptconfigure rackspace save-ssh-key --yes --rackspace-ssh-key-path="/home/dave/.ssh/bastion.pub" --rackspace-ssh-key-name="bastion"

lista 
---------------------

Este comando ayuda a datos sobre su cuenta de Rackspace . El siguiente comando dado se ejecutará el proceso.

.. code-block:: bash 
	
	ptconfigure rackspace list
        
.. code-block:: bash 

	ptconfigure rackspace list --yes --guess # use project saved connection details if possible --rackspace-list-data-type=sizes # servers, sizes, images, domains, regions, ssh_keys


Lista de los contenedores
-------------------------------

Este comando ayuda a mostrar los datos de contenedores sobre su cuenta de Rackspace . El siguiente comando dado se ejecutará el proceso.

.. code-block:: bash 
	
 	ptconfigure rackspace list-containers

.. code-block:: bash 

	ptconfigure rackspace list-containers --yes --guess # use project saved connection details if possible


Lista de los objetos-
-----------------------

Este comando ayuda a visualizar objeto de datos de Contenedores sobre su cuenta de Rackspace . El siguiente comando dado se ejecutará el proceso.

.. code-block:: bash 

 	ptconfigure rackspace list-objects

.. code-block:: bash 

	ptconfigure rackspace list-objects --yes --guess # use project saved connection details if possible

Parámetro Alternativa
------------------------------       

Hay dos parámetros alternativos que pueden ser utilizados en la línea de comandos .

Rackspace, rackspace


Beneficios
--------------

Rackspace ofrece una solución completa para clientes exigentes una infraestructura especialmente diseñada de alto rendimiento diseñado para bases de datos relacionales respaldados y apoyados por los ingenieros que se especializan en las cargas de trabajo de MySQL. Rackspace es un servicio completamente gestionado para los clientes que quieren centrarse en el desarrollo de sus aplicaciones y no preocuparse por la infraestructura subyacente. El servicio ofrece a las copias de seguridad y restauraciones de la demanda , la vigilancia integrada, almacenamiento redundante , escalabilidad para crecer en base a sus necesidades de aplicación y el control total de su base de datos .
