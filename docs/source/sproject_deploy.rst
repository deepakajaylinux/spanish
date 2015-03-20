==============
Project
==============

Sinopsis
-------------

En los negocios contemporáneos y ciencia que un proyecto se define como una empresa colaborativa, que involucren investigación o diseño, que se planea cuidadosamente para lograr un objetivo particular. Proyectos pueden definirse más como algo temporal en lugar de los sistemas sociales permanentes o sistemas de trabajo que están constituidos por equipos dentro o a través de las organizaciones para llevar a cabo tareas particulares bajo las limitaciones de tiempo. Un proyecto generalmente se llama (o se transforma en) un programa.


Este comando es parte de módulos predeterminados y encarga de las funciones de inicialización de proyecto, como configurar un proyecto, o un contenedor de proyecto e instalación también Jenkins construir archivos en una instancia en ejecución Jenkins.


comando Ayuda
----------------------

Este comando permite para determinar el uso del módulo de proyecto. El usuario llegará a conocer el diferente formas/formato para ejecutar este módulo. Este comando guía al usuario final para conocer el propósito de este comando. A continuación dado son el comando y la captura de pantalla del mismo.

.. code-block:: bash
	
	ptdeploy project help
       

 kevell@corp:/# ptdeploy Project help
 ******************************


  This command is part of Default Modules and handles Project initialisation functions, like configuring a project, or a project
  container and also installing Jenkins build files into a running Jenkins instance.

  Project, project, proj


          - container
          make a container folder for revisions (like /var/www/applications/*APP NAME*)
          example: ptdeploy proj container
          example: ptdeploy proj container --yes --proj-container="/var/www/applications/the-app"

          - init
          initialize Dapper project
          example: ptdeploy proj init
          example: ptdeploy proj init --yes

          - build-install
          copy jenkins project stored in repo to running jenkins so you can run builds
          example: ptdeploy proj build-install
          example: ptdeploy proj build-install
                        --jenkins-fs-dir=/var/lib/jenkins # --guess will set this to /var/lib/jenkins
                        --original-build-dir="/var/www/applications/the-app/build/config/ptconfigure/Project/jenkins-builds"
                        --target-job-name="Project_Build"
                        --new-job-dir="Project_Build_Alternate_Name"  # If target one is not available

 ------------------------------
 End Help
 ******************************


Container
----------------

Este comando le ayuda a crear una carpeta de contenedor para las revisiones (como /var/www/applications/*APP NAME*). 

Cuando el usuario necesita instalar, el usuario puede ejecutar los siguientes comandos para DBIstall. El sistema ejecutará el proceso de instalación.


.. code-block:: bash
	
	ptdeploy proj container

 kevell@corp:/# ptdeploy proj container
 Do you want to Modify Project Container Settings? (Y/N) 
 Y
 Do you want to initialize this as a ptdeploy project Container? (Y/N) 
 Y
 What is your Project Container directory?
 /root/gg
 Project Container directory created
 /root/gg space /root/ggMoving to Container
 /root/gg
 Showing Container Directory
 Project Container file created
 ******************************


 Seems Fine...Project Editor Finished
 ******************************



init
----------------

Cuando el usuario necesita inicializar proyecto dapper, el usuario puede ejecutar los siguientes comandos. El sistema ejecutará el proceso.


.. code-block:: bash

	ptdeploy proj init


.. code-block:: bash

 kevell@corp:/# ptdeploy proj init
 Do you want to Modify Project Settings To initialise Project? (Y/N) 
 Y
 Do you want to initialize this as a ptdeploy project? (Y/N) 
 Y
 ******************************


 Seems Fine...Project Editor Finished
 ******************************



Build-Install
----------------

Cuando el usuario necesita copia Jenkins proyecto almacenado en repo dirigir Jenkins, el usuario puede ejecutar los siguientes comandos. El sistema ejecutará el proceso.


.. code-block:: bash
	
	ptdeploy proj build-install

parámetros alternativos
--------------------------------

Hay dos parámetros alternativos que pueden utilizarse en el mando.


Project, project and proj

eg: ptdeploy Project help/  ptdeploy proj help
                       
beneficios
--------------

* Ayuda a hace una carpeta contenedor para revisiones 
* ayuda a inicializar proyecto dapper


