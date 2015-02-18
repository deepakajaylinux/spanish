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

	cleopatra cleofy help


La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que esuna ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda bajo cleofy.

.. code-block:: bash


 kevell@corp:/# cleopatra cleofy help

 ******************************


 This command is part of a default Module Core and provides you with a method by which you can create a standard set of Autopilot files for your project from the command line.  


 Cleofy, cleofy  

 - list        
 	List all of the autopilot files in your build/config/cleopatra/autopilots        
	example: cleopatra cleofy list        

 - standard        
	Create a default set of cleopatra autopilots in build/config/cleopatra/autopilots for your project.        
	example: cleopatra cleofy standard        

 - tiny        
	Create a default set of cleopatra autopilots in build/config/cleopatra/autopilots for a project with a "tiny" style infrastructure.        	example: cleopatra cleofy tiny        

 - medium        
	Create a default set of cleopatra autopilots in build/config/cleopatra/autopilots for a project with a "medium" style infrastructure.        	example: cleopatra cleofy medium        

 - medium-web        
	Create a default set of cleopatra autopilots in build/config/cleopatra/autopilots for a project with a "medium" style infrastructure,
        with web but not database.        
 	example: cleopatra cleofy medium-web        

 - db-cluster        
	Create a default set of cleopatra autopilots in build/config/cleopatra/autopilots for your project.        
 	example: cleopatra cleofy db-cluster        
 --yes                    
 --guess                    
 --database-nodes-env=*db-nodes-environment-name*                    

 - install-generic-autopilots        
	Install the generic Cleofy autopilot templates for a Tiny or Medium (Current Default) set of Environments        
 example: cleopatra cleofy install-generic-autopilots        
	example: cleopatra cleofy install-generic-autopilots        
 --yes                    
 --guess # will set --destination-dir=*this dir +*build/config/cleopatra/cleofy/autopilots/                    
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

Esta función tiene por objeto una lista de todos los archivos del piloto automático en su ubicación especificada (build / config / cleopatra / pilotos automáticos). La sintaxis para la aplicación de esta función se muestra a continuación,

.. code-block:: bash

	cleopatra cleofy list

estándar
------------

Esta función ayuda a crear un conjunto predeterminado de pilotos automáticos cleopatra (en build / config / cleopatra / pilotos automáticos) para el proyecto de los usuarios. Esta función se puede aplicar simplemente usando el siguiente comando,

.. code-block:: bash

	cleopatra cleofy standard


diminuto
-------------

Esta función tiene como objetivo crear un conjunto predeterminado de pilotos automáticos cleopatra (en build / config / cleopatra / pilotos automáticos) para un proyecto de pequeña infraestructura. Para llevar a cabo estas funciones sigue el siguiente comando como abajo,

.. code-block:: bash

	cleopatra cleofy tiny

medio
-------

 Esta función tiene como objetivo crear un conjunto predeterminado de pilotos automáticos cleopatra (en build / config / cleopatra / pilotos automáticos) para un proyecto de infraestructura de medio. Para llevar a cabo estas funciones sigue el siguiente comando como abajo,

.. code-block:: bash

	cleopatra cleofy medium


Medium_Web
----------

Esta función tiene como objetivo crear un conjunto predeterminado de pilotos automáticos cleopatra (en build / config / cleopatra / Pilotos automáticos) PARA UN proyecto de infraestructura de medio con la web, Pero No La Base de Datos. Para Llevar un cabo ESTAS Funciones Sigue el siguiente comando Como abajo,

.. code-block:: bash

	cleopatra cleofy medium-web

DB_cluster
---------------

 Esta función tiene como objetivo crear un conjunto predeterminado de pilotos automáticos cleopatra (en build / config / cleopatra / pilotos automáticos) para el proyecto de los usuarios.  Para llevar a cabo estas funciones sigue el siguiente comando como abajo,

.. code-block:: bash

	cleopatra cleofy db-cluster        
 --yes                    
 --guess                    
 --database-nodes-env=*db-nodes-environment-name*  

Install_generic_autopilots
----------------------------------

Esta función ayuda a la instalación de plantillas de piloto automático genéricos para pequeña o mediana conjunto de medio ambiente o simplemente usando el comando como se indica a continuación,

.. code-block:: bash
	
	cleopatra cleofy install-generic-autopilots     
or,

.. code-block:: bash

	cleopatra cleofy install-generic-autopilots
 --yes                    
 --guess # will set --destination-dir=*this dir +*build/config/cleopatra/cleofy/autopilots/                    
 --template-group=tiny # tiny, medium, dbcluster, phlagrant || db-cluster, workstation                    
 --destination-dir=*path-to-destination*    

Para aplicar el comando como se indica más arriba, el usuario tiene que especificar los siguientes campos que se enumeran,

* Dir destino
* Grupo de plantillas


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
