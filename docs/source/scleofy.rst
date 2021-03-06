=======
Cleofy
=======

sinopsis
-----------

Este módulo tiene por objeto facilitar a los usuarios en la creación de un conjunto estándar de archivos de piloto automático para su proyecto. Veamos cómo utilizar este módulo, y también acerca de las funciones de cleofy de los próximos temas.

Ayuda Comando
-----------------------

El comando de ayuda es un breve manual de usuario que facilita a los usuarios obtener conscientes en cuanto a la utilización de metodologías de manejo de este módulo para realizar diferentes funciones. También se enumeran las salidas de parámetros alternativos que se pueden utilizar en las declaraciones. Se destaca el ejemplo de sintaxis para el uso y acceso a diferentes funciones en virtud cleofy.

El comando utilizado para la declaración de opción de ayuda bajo cleofy se muestra a continuación,

.. code-block:: bash

	ptconfigure cleofy help


La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que esuna ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda bajo cleofy.

.. code-block:: bash


 kevell@corp:/# ptconfigure cleofy help

 ******************************


 This command is part of a default Module Core and provides you with a method by which you can create a standard set of Autopilot files for your project from the command line.  


 Cleofy, cleofy  

 - list        
 	List all of the autopilot files in your build/config/ptconfigure/autopilots        
	example: ptconfigure cleofy list        

 - standard        
	Create a default set of ptconfigure autopilots in build/config/ptconfigure/autopilots for your project.        
	example: ptconfigure cleofy standard        

 - tiny        
	Create a default set of ptconfigure autopilots in build/config/ptconfigure/autopilots for a project with a "tiny" style infrastructure.        	example: ptconfigure cleofy tiny        

 - medium        
	Create a default set of ptconfigure autopilots in build/config/ptconfigure/autopilots for a project with a "medium" style infrastructure.        	example: ptconfigure cleofy medium        

 - medium-web        
	Create a default set of ptconfigure autopilots in build/config/ptconfigure/autopilots for a project with a "medium" style infrastructure,
        with web but not database.        
 	example: ptconfigure cleofy medium-web        

 - db-cluster        
	Create a default set of ptconfigure autopilots in build/config/ptconfigure/autopilots for your project.        
 	example: ptconfigure cleofy db-cluster        
 --yes                    
 --guess                    
 --database-nodes-env=*db-nodes-environment-name*                    

 - install-generic-autopilots        
	Install the generic Cleofy autopilot templates for a Tiny or Medium (Current Default) set of Environments        
 example: ptconfigure cleofy install-generic-autopilots        
	example: ptconfigure cleofy install-generic-autopilots        
 --yes                    
 --guess # will set --destination-dir=*this dir +*build/config/ptconfigure/cleofy/autopilots/                    
 --template-group=tiny # tiny, medium, dbcluster, phlagrant || db-cluster, workstation                    
 --destination-dir=*path-to-destination*                    

 ------------------------------
 End Help
 ******************************

Funciones de cleofy
--------------------------


En este tema se describe acerca de las diversas funciones de cleofy bajo este módulo se enumeran a continuación,

* Lista
* Standard
* Tiny
* Medio
* Medium-web
* DB-cluster
* Install_generic_autopilots


lista
-----

Esta función tiene por objeto una lista de todos los archivos del piloto automático en su ubicación especificada (build / config / ptconfigure / pilotos automáticos). La sintaxis para la aplicación de esta función se muestra a continuación,

.. code-block:: bash

	ptconfigure cleofy list

estándar
------------

Esta función ayuda a crear un conjunto predeterminado de pilotos automáticos ptconfigure (en build / config / ptconfigure / pilotos automáticos) para el proyecto de los usuarios. Esta función se puede aplicar simplemente usando el siguiente comando,

.. code-block:: bash

	ptconfigure cleofy standard


.. code-block:: bash

 kevell@corp:/# ptconfigure cleofy standard

 Cleofy This? (Y/N) 
 y
 Environment 1  : 
 Default Settings for Any App not setup for environment  enter them now.
 Value for: Name of this Environment
 test1
 Value for: Default Temp Dir (should usually be /tmp/)

 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-bastion.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-build-server.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-cleo-dapper.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-db-load-balancer.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-db-node.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-git.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-standalone-server.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-web-load-balancer.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-cm-web-node.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-bastion.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-build-server.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-cleo-dapper-new.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-cleo-dapper-update.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-db-load-balancer.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-db-node.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-git.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-standalone-server.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-web-load-balancer.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-invoke-web-node.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-prep-any-box.php
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/test1-prep-ubuntu.php
 ******************************


 Success
 In Cleofy
 ******************************




diminuto
-------------

Esta función tiene como objetivo crear un conjunto predeterminado de pilotos automáticos ptconfigure (en build / config / ptconfigure / pilotos automáticos) para un proyecto de pequeña infraestructura. Para llevar a cabo estas funciones sigue el siguiente comando como abajo,

.. code-block:: bash

	ptconfigure cleofy tiny

.. code-block:: bash


 kevell@corp:/# ptconfigure cleofy tiny 

 Cleofy This? (Y/N) 
 y 
 Use existing environment settings? (Y/N) 
 y 
 Do you want to modify entries applicable to any app in environment kevells (Y/N) 
 n 
 Settings for cleo not setup for environment kevells enter them manually. 
 Environment 1 kevells : 
 Do you want to add another environment? (Y/N) 
 n 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-bastion.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-build-server.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-cleo-dapper.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-db-load-balancer.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-db-node.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-git.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-standalone-server.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-web-load-balancer.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-web-node.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-bastion.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-build-server.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-cleo-dapper-new.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-cleo-dapper-update.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-db-load-balancer.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-db-node.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-git.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-standalone-server.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-web-load-balancer.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-web-node.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-prep-any-box.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-prep-ubuntu.php 
 ****************************** 


 Success 
 In Cleofy 
 ****************************** 



medio
-------

 Esta función tiene como objetivo crear un conjunto predeterminado de pilotos automáticos ptconfigure (en build / config / ptconfigure / pilotos automáticos) para un proyecto de infraestructura de medio. Para llevar a cabo estas funciones sigue el siguiente comando como abajo,

.. code-block:: bash

	ptconfigure cleofy medium


.. code-block:: bash

 kevell@corp:/# ptconfigure cleofy medium 

 Cleofy This? (Y/N) 
 y 
 Use existing environment settings? (Y/N) 
 y 
 Do you want to modify entries applicable to any app in environment kevells (Y/N) 
 n 
 Settings for cleo not setup for environment kevells enter them manually. 
 Environment 1 kevells : 
 Do you want to add another environment? (Y/N) 
 n 
 Enter name of environment with your Stage web nodes 
 kevells 
 Enter name of environment with your Stage database nodes 
 kevells 
 Enter name of environment with your Prod web nodes 
 kevells 
 Enter name of environment with your Prod database nodes 
 kevells 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-bastion.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-build-server.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-cleo-dapper.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-db-load-balancer.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-db-node.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-git.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-standalone-server.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-web-load-balancer.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-web-node.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-bastion.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-build-server.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-cleo-dapper-new.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-cleo-dapper-update.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-db-load-balancer.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-db-node.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-git.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-standalone-server.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-web-load-balancer.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-web-node.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-prep-any-box.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-prep-ubuntu.php 
 ******************************    


 Success 
 In Cleofy 
 ****************************** 



Medium_Web
----------

Esta función tiene como objetivo crear un conjunto predeterminado de pilotos automáticos ptconfigure (en build / config / ptconfigure / Pilotos automáticos) PARA UN proyecto de infraestructura de medio con la web, Pero No La Base de Datos. Para Llevar un cabo ESTAS Funciones Sigue el siguiente comando Como abajo,

.. code-block:: bash

	ptconfigure cleofy medium-web


.. code-block:: bash


 kevell@corp:/# ptconfigure cleofy medium-web 

 Cleofy This? (Y/N) 
 y 
 Use existing environment settings? (Y/N) 
 y 
 Do you want to modify entries applicable to any app in environment kevells (Y/N) 
 n 
 Settings for cleo not setup for environment kevells enter them manually. 
 Environment 1 kevells : 
 Do you want to add another environment? (Y/N) 
 n 
 Enter name of environment with your Stage web nodes 
 kevells 
 Enter name of environment with your Prod web nodes 
 kevells 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-bastion.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-build-server.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-cleo-dapper.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-db-load-balancer.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-db-node.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-git.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-standalone-server.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-web-load-balancer.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-web-node.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-bastion.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-build-server.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-cleo-dapper-new.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-cleo-dapper-update.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-db-load-balancer.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-db-node.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-git.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-standalone-server.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-web-load-balancer.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-web-node.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-prep-any-box.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-prep-ubuntu.php 
 ****************************** 


 Success 
 In Cleofy 
 ****************************** 


DB_cluster
---------------

 Esta función tiene como objetivo crear un conjunto predeterminado de pilotos automáticos ptconfigure (en build / config / ptconfigure / pilotos automáticos) para el proyecto de los usuarios.  Para llevar a cabo estas funciones sigue el siguiente comando como abajo,

.. code-block:: bash

	ptconfigure cleofy db-cluster        
 --yes                    
 --guess                    
 --database-nodes-env=*db-nodes-environment-name*  

.. code-block:: bash


 kevell@corp:/# ptconfigure cleofy db-cluster 

 Cleofy This? (Y/N) 
 y 
 Use existing environment settings? (Y/N) 
 y 
 Do you want to modify entries applicable to any app in environment kevells (Y/N) 
 n 
 Settings for cleo not setup for environment kevells enter them manually. 
 Environment 1 kevells : 
 Do you want to add another environment? (Y/N) 
 n 
 Enter name of environment with your Databasenodes 
 kevells 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-bastion.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-build-server.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-cleo-dapper.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-db-load-balancer.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-db-node.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-git.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-standalone-server.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-web-load-balancer.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-cm-web-node.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-bastion.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-build-server.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-cleo-dapper-new.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-cleo-dapper-update.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-db-load-balancer.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-db-node.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-git.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-standalone-server.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-web-load-balancer.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-invoke-web-node.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-prep-any-box.php 
 /home/kevells/build/config/ptconfigure/cleofy/autopilots/generated/kevells-prep-ubuntu.php 
 ****************************** 


 Success 
 In Cleofy 
 ****************************** 


Install_generic_autopilots
----------------------------------

Esta función ayuda a la instalación de plantillas de piloto automático genéricos para pequeña o mediana conjunto de medio ambiente o simplemente usando el comando como se indica a continuación,

.. code-block:: bash
	
	ptconfigure cleofy install-generic-autopilots     
or,

.. code-block:: bash

	ptconfigure cleofy install-generic-autopilots
 --yes                    
 --guess # will set --destination-dir=*this dir +*build/config/ptconfigure/cleofy/autopilots/                    
 --template-group=tiny # tiny, medium, dbcluster, phlagrant || db-cluster, workstation                    
 --destination-dir=*path-to-destination*    

Para aplicar el comando como se indica más arriba, el usuario tiene que especificar los siguientes campos que se enumeran,

* Dir destino
* Grupo de plantillas



.. code-block:: bash


 kevell@corp:/# ptconfigure cleofy install-generic-autopilots 

 Enter Template Group: 
 (0) tiny 
 (1) medium 
 0 
 Enter Destination Directory: 
 /tmp/ 
 [Pharaoh Logging] Performing file copy from /opt/ptconfigure-enterprise/src/Modules/Cleofy/Templates/Generic/Tiny to /tmp/ 
 ****************************** 
  

 Cleofy Listing: 
 --------------------------------------------  

 Success 

 ------------------------------ 
 Cleofy Generic Autopilot Install Finished 
 ****************************** 


parámetros alternativos
-----------------------------

Los parámetros alternativos para este módulo, cualquiera de los cuales se pueden utilizar en la declaración es,

* Cleofy,
* cleofy

Beneficios
----------

* Los parámetros utilizados declarando ayuda y otras características diferentes de apt no distinguen entre mayúsculas y minúsculas.
* Es-acomodado tanto os Cent y así como en Ubuntu.
* Este módulo envuelve todas las necesidades de un proyecto en la creación de juego estándar de los pilotos automáticos.
