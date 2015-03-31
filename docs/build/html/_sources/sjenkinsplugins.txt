================
JenkinsPlugins
================

Sinopsis
-------------

Jenkins es popular para construir servidor. Jenins es una herramienta de integración continua fuente escrito en Java. Jenkins proporciona servicios de integración continua para el desarrollo de software.

Plugins han sido puestos a Jenkins que extender su uso a los proyectos escritos en idiomas que no sean Java. Plugins están disponibles para la integración de Jenkins con la mayoría de los sistemas de control de versiones y las grandes bases de datos. Muchas herramientas de construcción están soportados a través de sus respectivos plugins. Plugins también pueden cambiar la forma Jenkins ve o añadir nuevas funcionalidades. Construye puede generar informes de pruebas en diversos formatos compatibles con plugins (apoyo JUnit se incluye en la actualidad) y Jenkins puede mostrar los informes y generar tendencias y hacerlos en la GUI.

Ayuda Comando
--------------------

Este comando ayuda a determinar el uso del módulo JenkinsPlugins. El usuario se llega a saber acerca de las diferentes formas / formato para ejecutar este módulo. Este comando guía al usuario final a conocer el propósito de este comando. A continuación dado son el mando y la pantalla del mismo.

.. code-block:: bash
             
   		ptconfigure JenkinsPlugins help

.. code-block:: bash

 
 kevell@corp:/# ptconfigure JenkinsPlugins help
 ******************************


  This command allows you to install a bunch of plugins that we recommend for
  PHP builds in Jenkins.

  JenkinsPlugins, jenkinsplugins, jenkins-plugins, jenkins-plugs

        - install
        Installs the latest version of Jenkins Plugins for PHP recommended by Golden Contact
        example: ptconfigure jenkins-plugins install

 ------------------------------
 End Help
 ******************************

instalación
----------------

  Este comando le permite instalar un montón de plugins que recomendamos para PHP construye en Jenkins. Si el usuario tiene que instalar el módulo Jenkins en la máquina, el siguiente comando dado se ejecutará el proceso de instalación.


.. code-block:: bash
        
		ptconfigure JenkinsPlugins install

La captura de pantalla de la orden anterior se enumeran a continuación,

.. code-block:: bash


 kevell@corp:/# ptconfigure jenkins-plugins install
 Install Jenkins Plugins? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Jenkns Plgs!        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-71115535759.sh
 chmod 755 /tmp/ptconfigure-temp-script-71115535759.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-71115535759.sh Permissions
 Executing /tmp/ptconfigure-temp-script-71115535759.sh
 Cloning into 'jplugins'...
 remote: Counting objects: 39, done.
 remote: Total 39 (delta 0), reused 0 (delta 0), pack-reused 39
 Unpacking objects: 100% (39/39), done.
 Checking connectivity... done.
 * Restarting Jenkins Continuous Integration Server jenkins
   ...done.
 Temp File /tmp/ptconfigure-temp-script-71115535759.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 JenkinsPlugins: Success
 ------------------------------
 Installer Finished
 ******************************


Opciones
-----------

.. cssclass:: table-bordered

 +------------------------+------------------------------------------------------------+-----------+--------------------------------------+
 | Parámetros             | Parámetro Alternativa                                      | Opciones  | Comentarios                          |
 +========================+============================================================+===========+======================================+
 |ptconfigure             | Cualquiera de los cuatro parámetros alternativa se         | Y(Yes)    | Una vez que el usuario proporciona   |
 |JenkinsPlugins Install  | puede utilizar en comando JenkinsPlugins, jenkinsplugins,  |           | la opción, sistema comienza proceso  |
 |                        | jenkins-plugins, jenkins-plugs Por ejemplo:                |           | de instalación                       |
 |                        | ptconfigure jenkins-plugins Install                        |           |                                      |
 +------------------------+------------------------------------------------------------+-----------+--------------------------------------+
 |ptconfigure             | Cualquiera de los cuatro parámetros alternativa se         | N(No)     | Una vez que el usuario proporciona   |
 |JenkinsPlugins Install  | puede utilizar en comando JenkinsPlugins, jenkinsplugins,  |           | la opción, Sistema Detiene proceso   |
 |                        | jenkins-plugins, jenkins-plugs Por ejemplo:                |           | de instalación                       |
 |                        | ptconfigure jenkins-plugins Install|                       |           |                                      |
 +------------------------+------------------------------------------------------------+-----------+--------------------------------------+


Beneficios
--------------

* El plug-in le dará un informe sobre cuánto se utilizará todos los plugins en todos sus trabajos. Por lo tanto, se analizará la extensión 
  utilizada puntos de cada puesto de trabajo.
* Este plugin te da la posibilidad de analizar el uso de los plugins instalados.
* Sensitibilidad caso
* Well-to-do en Ubuntu y CentOS.
