==============
Loadrunner
==============

sinopsis
----------

HP LoadRunner es un rendimiento y pruebas automatizadas de automatización de productos de Hewlett - Packard para las pruebas de carga de aplicaciones : examinar el comportamiento del sistema y el rendimiento , mientras que la generación de carga real. LoadRunner soporta varias herramientas de desarrollo , tecnologías y protocolos de comunicación. 

comando Ayuda
--------------

El comando help guía a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en el módulo LoadRunner . También describe la sintaxis para instalar el módulo LoadRunner . El comando de ayuda para LoadRunner se muestra a continuación .


.. code-block:: bash

	ptconfigure Loadrunner help

La representación gráfica de la orden anterior se enumeran a continuación ,

.. code-block:: bash

 kevell@corp:/# ptconfigure Loadrunner help 
 ****************************** 


  This command allows you to install HardyCssRegression from a GC Repo. 

  Loadrunner 

        - install 
        Installs the latest GC Repo version of Loadrunner 
        example: ptconfigure Loadrunner install 

 ------------------------------ 
 End Help 
 ******************************   



instalación
--------------

El comando utilizado para instalar el módulo LoadRunner en el terminal aparece a continuación ,

.. code-block:: bash

	ptconfigure loadrunner install 

La representación gráfica de la orden anterior se enumeran a continuación ,

.. code-block:: bash

 kevell@corp:/# ptconfigure loadrunner install 
 Install Loadrunner? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         Loadrunner !         * 
 ******************************* 
 Creating /tmp/ptconfigure-temp-script-32374780925.sh 
 chmod 755 /tmp/ptconfigure-temp-script-32374780925.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-32374780925.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-32374780925.sh 
 mkdir: cannot create directory â€˜loadrunnerâ€™: File exists 
 Cloning into 'loadrunner'... 
 remote: Counting objects: 1284, done. 
 remote: Total 1284 (delta 0), reused 0 (delta 0), pack-reused 1284 
 Receiving objects: 100% (1284/1284), 5.63 MiB | 21.00 KiB/s, done. 
 Resolving deltas: 100% (592/592), done. 
 Checking connectivity... done. 
 Temp File /tmp/ptconfigure-temp-script-32374780925.sh Removed 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 


 Single App Installer: 
 -------------------------------------------- 
 Loadrunner: Success 
 ------------------------------ 
 Installer Finished 
 ****************************** 


Beneficios
----------

* No hay necesidad de instalarlo en el servidor bajo prueba . Se utiliza monitores nativos. Por Ej: Perfmon para ventanas o demonio rstatd
  para Unix
* Utiliza ANSI C como la idioma1 programación por defecto y otros lenguajes como Java y VB .
* Interfaz de análisis donde se pueden ver los informes en fácil de entender diagramas y gráficos de color excelente supervisión y .
  Soporta la mayoría de la protocols2 .
* Hace correlation3 mucho más fácil. Vamos a profundizar en correlación a través de una serie de mensajes más tarde.
* Niza GUI genera la escritura a través de una grabación de un solo clic , por supuesto que tendría que modificar el script de acuerdo a sus
  necesidades.
