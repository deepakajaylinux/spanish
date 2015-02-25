==========
IntelliJ
==========

Sinopsis
------------

En este módulo se acelere la instalación de IntelliJ que es un Brains Jet IDE con una versión más reciente. La Plataforma IntelliJ es una plataforma para la construcción, IDEs cuenta el idioma inteligentes con un conjunto completo ofÂ componentes, que incluye sistema virtual de archivos, marco de interfaz de usuario, editor de texto, léxico, análisis sintáctico, árboles de sintaxis abstracta y otra infraestructura específica del idioma, marcos de aplicación del navegación, completado de código, las inspecciones, las intenciones, refactorizaciones, integración de control de versiones, marco depurador, corredor gráfica de prueba de unidad.

El código fuente de la plataforma IntelliJ está cubierto por la licencia Apache 2.0. Esto significa que usted puede construir tanto de código abierto y los productos comerciales en la parte superior de la plataforma sin pagar regalías a JetBrains. Veamos acerca de las funcionalidades de IntelliJ bajo este módulo.

Ayuda Comando
--------------------

El comando help guía a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en el módulo de IntelliJ. En él se enumeran los parámetros alternativos de módulo de IntelliJ. También describe la sintaxis para instalar el módulo de IntelliJ. El comando de ayuda para el módulo de IntelliJ se muestra a continuación.

.. code-block:: bash

 		ptconfigure IntelliJ help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda en virtud de IntelliJ.

.. code-block:: bash

 kevell@corp:/# ptconfigure IntelliJ help
 ******************************


  This command allows you to install Intellij, the JetBrains IDE

  IntelliJ, intellij

        - install
        Installs the latest version of Developer Tools
        example: ptconfigure gittools install

 ------------------------------
 End Help
 ******************************

instalación
---------------

El comando utilizado para instalar el JRush a la máquina de los usuarios se muestra a continuación.

.. code-block:: bash

		ptconfigure IntelliJ install

Después de introducir el comando anterior, las siguientes operaciones se produce:

* Se solicita al usuario que introduzca la versión IntelliJ.
* Asegura la disponibilidad de módulos y no comprueba la versión.
* Si no existe el módulo en la máquina de los usuarios, comienza la instalación.
* Durante la instalación lo hará pide al usuario que introduzca instalar el Java Directory.

Por último, la instalación de IntelliJ se completó. La captura de pantalla como se muestra a continuación muestra el proceso de instalación de IntelliJ.

.. code-block:: bash

 kevell@corp:/# ptconfigure IntelliJ install
 Install IntelliJ IDE? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         IntelliJ IDE        *
 *******************************
 Enter IntelliJ Version
 PHP Notice:  Undefined offset: 0 in /opt/ptconfigure/ptconfigure/src/Core/Base/Model/Base.php on line 187
 (0)  
 PHP Notice:  Undefined offset: 1 in /opt/ptconfigure/ptconfigure/src/Core/Base/Model/Base.php on line 187
 (1)  

 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module Java reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 Creating /tmp/ptconfigure-temp-script-98824051629.sh
 chmod 755 /tmp/ptconfigure-temp-script-98824051629.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-98824051629.sh Permissions
 Executing /tmp/ptconfigure-temp-script-98824051629.sh
 Cloning into 'intellij'...
 remote: Counting objects: 1026, done.
 remote: Total 1026 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (1026/1026), 205.06 MiB | 410.00 KiB/s, done.
 Resolving deltas: 100% (60/60), done.
 Checking connectivity... done.
 Checking out files: 100% (744/744), done.
 Temp File /tmp/ptconfigure-temp-script-98824051629.sh Removed
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 IntelliJ: Success
 ------------------------------
 Installer Finished
 ******************************

parámetros
----------------------------

En lugar de IntelliJ podemos utilizar, intelliJ

Beneficios
------------

* Este módulo facilita al usuario en la instalación de IntelliJ con la última versión.
* Los parámetros utilizados en la declaración de la ayuda y las instalaciones no son sensibles, que se añade la ventaja, mientras que en 
  comparación con otros.
* Es-acomodados tanto en OS ciento y así como en ubuntu.
* El estado requiere se supervisan con claridad durante la instalación.
* Durante la instalación, el usuario puede introducir la versión que desee y, así como Java Instale Directory.
