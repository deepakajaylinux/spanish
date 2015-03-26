===============
Jasmine
===============

sinopsis
---------

Jazmín es un framework de desarrollo impulsado por el comportamiento para pruebas de código JavaScript.  El jazmín es una fuente de European framework para javascript de pruebas.  No depende en los navegadores, DOM o cualquier framework de JavaScript. Por lo tanto es adecuado para sitios web, proyectos de Node.js, o en cualquier lugar puede ejecutar ese JavaScript.

comando Ayuda
--------------

Este comando permite para determinar el uso del módulo de jazmín. Enumera los parámetros alternativos de jazmín. También describe la sintaxis para el funcionamiento del módulo de jazmín. El comando ayuda para jasmine se muestra a continuación.

.. code-block:: bash

        ptconfigure Jasmine  help

La representación pictórica del comando anterior se enumera a continuación,

.. code-block:: bash

 kevell@corp:/# ptconfigure Jasmine help
 ******************************


  This command allows you to install Jasmine from a GC Repo.

  Jasmine

        - install
        Installs the latest GC Repo version of Jasmine.
        example: ptconfigure Jasmine install

 ------------------------------
 End Help
 ******************************


Instalación
---------------

El comando utilizado para instalar el módulo de jazmín en el terminal se enumera a continuación,

.. code-block:: bash

        ptconfigure Jasmine install

El comando anterior pretende instalar la última versión de jazmín y sus dependencias.

La representación pictórica del comando anterior se enumera a continuación,

.. code-block:: bash

 kevell@corp:/# ptconfigure jasmine install
 Install Jasmine? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Jasmine        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-79546324044.sh
 chmod 755 /tmp/ptconfigure-temp-script-79546324044.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-79546324044.sh Permissions
 Executing /tmp/ptconfigure-temp-script-79546324044.sh
 Cloning into 'jasmine'...
 remote: Counting objects: 12178, done.
 remote: Total 12178 (delta 0), reused 0 (delta 0), pack-reused 12178
 Receiving objects: 100% (12178/12178), 6.60 MiB | 8.00 KiB/s, done.
 Resolving deltas: 100% (7866/7866), done.
 Checking connectivity... done.
 Archive:  jasmine-standalone-2.0.0.zip
  inflating: MIT.LICENSE             
  inflating: lib/jasmine-2.0.0/jasmine_favicon.png  
  inflating: lib/jasmine-2.0.0/jasmine.js  
  inflating: lib/jasmine-2.0.0/jasmine-html.js  
  inflating: lib/jasmine-2.0.0/jasmine.css  
  inflating: lib/jasmine-2.0.0/console.js  
  inflating: lib/jasmine-2.0.0/boot.js  
  inflating: SpecRunner.html         
  inflating: src/Player.js           
  inflating: src/Song.js             
  inflating: spec/PlayerSpec.js      
  inflating: spec/SpecHelper.js      
 Temp File /tmp/ptconfigure-temp-script-79546324044.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Jasmine: Success
 ------------------------------
 Installer Finished
 ******************************


Objetivos
-----------

* Deberían alentar buenas prácticas pruebas 
* debe ser simple comenzar con 
* deben integrarse fácilmente con sistemas de construcción continua


