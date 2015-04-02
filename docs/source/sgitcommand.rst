===============
GitCommand
===============

sinopsis
-------------

Git es un sistema gratuito y de código abierto distribuido de control de versiones diseñado para manejar todo, desde pequeñas a grandes proyectos con rapidez y eficiencia . 


comando Ayuda
---------------

El comando help guía a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en el módulo de git . En él se enumeran los parámetros alternativos de módulo git . El comando de ayuda para el módulo de git se muestra a continuación .

.. code-block:: bash

	ptconfigure gitcommand help

La representación gráfica de la orden anterior se enumeran a continuación ,

.. code-block:: bash

 kevell@corp:/# ptconfigure gitcommand help

 ******************************



  This command handles Git Functionality

  Git, GitCommand, git-command, gitcommand

  - checkout-branch
    checkout a branch
    example: ptconfigure git checkout-branch --branch=*branchname*

  - create-checkout-branch
    checkout a branch, creating a new branch if needed
    example: ptconfigure git create-checkout-branch --branch=*branchname*

  - delete-branch
    delete a branch
    example: ptconfigure git delete-branch --branch=*branchname*
    
  - ensure-branch
    ensure a branch
    example: ptconfigure git ensure-branch --branch=*branchname*
    
  - add
    add new files to a git repository
    example: ptconfigure git add 
	
  - commit
    commit new messages to a git repository
    example: ptconfigure git  commit --message=*some commit message*

  - push
    push to a git repo
    example: ptconfigure git push --branch=*origin yourbranch*
  
  - pull
    pull a git repo
    example: ptconfigure git pull --branch=*origin yourbranch*

 ------------------------------
 End Help
 ******************************


Checkout-branch
-------------------

El comando git checkout le permite navegar entre las ramas creadas por rama git . Este comando checkout una rama y el proceso de ejecución es como se muestra a continuación ,

.. code-block:: bash

	ptconfigure git checkout-branch --branch=*branchname*

La representación gráfica de la orden anterior se enumeran a continuación ,

.. code-block:: bash

 kevell@corp:/# ptconfigure git checkout-branch

 Perform a git command? (Y/N) 
 y
 What branch?
 kevellbranch
 [Pharaoh Logging] [GitCommand] Attempting to create branch kevellbranch
 Switched to branch 'kevellbranch'
 Now in: /opt/ptconfigure-enterprise 

 ******************************


 0 : In GitCommand View
 ******************************



Create-checkout-branch
---------------------------

El git checkout permite crear rama que obtiene una rama, la creación de una nueva rama de ser necesario. El proceso de ejecución de este comando es como se muestra a continuación ,


.. code-block:: bash

	ptconfigure git create-checkout-branch --branch=*branchname*

La representación gráfica de la orden anterior se enumeran a continuación ,

.. code-block:: bash

 kevell@corp:/# ptconfigure git checkout-branch

 Perform a git command? (Y/N) 
 y
 What branch?
 kevellbranch
 [Pharaoh Logging] [GitCommand] Attempting to create branch kevellbranch
 Switched to branch 'kevellbranch'
 Now in: /opt/ptconfigure-enterprise 

 ******************************


 0 : In GitCommand View
 ******************************


.. code-block:: bash

 kevell@corp:/# ptconfigure git create-checkout-branch

 Perform a git command? (Y/N) 
 y
 What branch?
 karthi
 [Pharaoh Logging] [GitCommand] Attempting to create branch karthi
 Switched to a new branch 'karthi'
 Now in: /opt/ptconfigure-enterprise

 ******************************


 0 : In GitCommand View
 ******************************


delete-branch
-----------------

Este comando se utiliza para borrar una rama si existe. El proceso de ejecución de este comando es como se muestra a continuación ,

.. code-block:: bash

	ptconfigure git delete-branch --branch=*branchname*

La representación gráfica de la orden anterior se enumeran a continuación ,

.. code-block:: bash

 kevell@corp:/# ptconfigure git delete-branch

 Perform a git command? (Y/N) 
 y
 What branch?
 kevell
 [Pharaoh Logging] [GitCommand] Branch kevell exists, deleting...
 git branch -d mmmm
 Now in: /opt/ptconfigure-enterprise 

 ******************************


 0 : In GitCommand View
 ******************************


ensure-branch
----------------

Este comando se utiliza para asegurar una rama existe , si no se crea una nueva rama . El proceso de ejecución de este comando se enumeran a continuación ,

.. code-block:: bash

	ptconfigure git ensure-branch --branch=*branchname*

La representación gráfica de la orden anterior se enumeran a continuación ,

.. code-block:: bash

 kevell@corp:/# ptconfigure git ensure-branch

 Perform a git command? (Y/N) 
 y
 What branch?
 kevell
 [Pharaoh Logging] [GitCommand] Branch kevell does not exist, creating...
 Switched to a new branch 'kevell'
 Now in: /opt/ptconfigure-enterprise

 ******************************


 0 : In GitCommand View
 ******************************

.. code-block:: bash

 kevell@corp:/# ptconfigure git ensure-branch

 Perform a git command? (Y/N) 
 y
 What branch?
 karthi
 [Pharaoh Logging] [GitCommand] Branch karthi already exists, continuing...
 Now in: /opt/ptconfigure-enterprise

 ******************************


 1 : In GitCommand View
 ******************************

Add
------

El comando git add se utiliza para añadir nuevos archivos al repositorio git . El proceso de ejecución de este comando se enumeran a continuación ,

.. code-block:: bash

	ptconfigure git add 

La representación gráfica de la orden anterior se enumeran a continuación ,

.. code-block:: bash

 kevell@corp:/# ptconfigure git add
 
 Enter the file path to add ? (Enter nothing to add all new & modified files in the git repo).
 test1
 [Pharaoh Logging] All new files in the git repository were added
 ******************************


 0 : In GitCommand View
 ******************************

Commit
---------

Este comando se utiliza para cometer nuevos mensajes en el repositorio git . El proceso de ejecución de este comando es como se muestra a continuación ,

.. code-block:: bash

	ptconfigure git  commit --message=*some commit message*

La representación gráfica de la orden anterior se enumeran a continuación ,

.. code-block:: bash

 kevell@corp:/# ptconfigure git commit

 Enter message to commit:
 testing
 [Pharaoh Logging] Git commit successfully
 ******************************


 0 : In GitCommand View
 ******************************


Push
----------

Este comando se utiliza para impulsar los archivos al repositorio git . El proceso de ejecución de este comando se muestra a continuación ,

.. code-block:: bash

	ptconfigure git push --branch=*origin yourbranch*

La representación gráfica de la orden anterior se enumeran a continuación ,

.. code-block:: bash

 kevell@corp:/# ptconfigure git push

 What branch?
 origin master
 Username for 'https://github.com': muralivel
 Password for 'https://muralivel@github.com': 
 Counting objects: 5, done.
 Delta compression using up to 2 threads.
 Compressing objects: 100% (3/3), done.
 Writing objects: 100% (5/5), 394 bytes | 0 bytes/s, done.
 Total 5 (delta 0), reused 0 (delta 0)
 To https://github.com/muralivel/kumar.git
  * [new branch]      master -> master
 [Pharaoh Logging] Git push to branch origin master successfully
 ******************************


 0 : In GitCommand View
 ******************************


Pull
----------

Este comando se utiliza para tirar de un repositorio git . El proceso de ejecución de este comando es como se muestra a continuación ,

.. code-block:: bash

	ptconfigure git pull --branch=*origin yourbranch*

La representación gráfica de la orden anterior se enumeran a continuación ,

.. code-block:: bash


 kevell@corp:/# ptconfigure git pull

 What branch?
 origin master
 remote: Counting objects: 3, done.
 remote: Compressing objects: 100% (2/2), done.
 Unpacking objects: 100% (3/3), done.
 remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
 From https://github.com/muralivel/kumar
 * branch            master     -> FETCH_HEAD
   4f390f3..c3e9feb  master     -> origin/master
 [Pharaoh Logging] Git pull from branch origin master successfully
 ******************************


 0 : In GitCommand View
 ******************************



parámetros alternativos
--------------------------

Hay cuatro parámetros alternativos que pueden ser utilizados en la línea de comandos .

Git, GitCommand, git-command, gitcommand


Beneficios
--------------

* Gratuito y de código abierto
* Rápido y pequeño
* Copia de seguridad implícita
* Seguridad
* No hay necesidad de un hardware potente
* Ramificación Más fácil



