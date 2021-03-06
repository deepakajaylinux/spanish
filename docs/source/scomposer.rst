========
Composer
========

sinopsis
----------

Compositor es un administrador de la dependencia a nivel de aplicación para el lenguaje de programación PHP que ofrece un formato estándar para la gestión de dependencias de software PHP y bibliotecas necesarias.

Se permite declarar las bibliotecas dependientes necesita su proyecto y los instalará en su proyecto para usted. Composer es multiplataforma y nos esforzamos para que funcione igual de bien en Windows, Linux y OSX.

Ayuda Comando
----------------------
Este comando ayuda a determinar el uso del módulo de compositor. El usuario se llega a saber acerca de las diferentes formas / formato para ejecutar este módulo. Este comando guía al usuario final con respecto a los parámetros alternativos y comandos para la instalación. A continuación dado son el mando y la pantalla del mismo.

.. code-block:: bash
              
		 ptconfigure composer help

.. code-block:: bash

 kevell@corp:/# ptconfigure composer help
 ******************************


  This command allows you to update Composer.

  Composer, composer

        - install
        Installs the latest version of composer
        example: ptconfigure composer install

 ------------------------------
 End Help
 ******************************

instalación
--------------

Cuando el usuario tiene que instalar el módulo compositor en la máquina, el siguiente comando dado se ejecutará el proceso de instalación.

.. code-block:: bash
               
		 ptconfigure composer install

Durante la instalación, el sistema pide el nombre del directorio, si usted quiere configurar su PATH, puede definir su camino. Defina su camino tiene que ser seguido por el símbolo "/". Pulse Intro para utilizar la ruta por defecto.

"What is the program data directory? "/opt/composer" - use this?

Durante la instalación, el sistema pide la ejecución de nombre de directorio, si usted quiere configurar su PATH, puede definir su camino. Defina su camino tiene que ser seguido por el símbolo "/". Pulse Intro para utilizar la ruta por defecto.

"What is the program executer directory? Found "/usr/bin" - Use this? "
                              

.. cssclass:: table-bordered

 +---------------------------+------------------------------+----------------+-----------------------------------------+
 | Parámetros                | alternativos de parámetros   | Opción         | Comentarios                             |
 +===========================+==============================+================+=========================================+
 |ptconfigure composer       | Composer, composer           | Y              | El sistema se inicia proceso de         | 
 |Install? (Y/N)             |                              |                | instalación                             |
 +---------------------------+------------------------------+----------------+-----------------------------------------+
 |ptconfigure composer       | Composer, composer           | N              | El sistema detiene proceso de           |
 |Install? (Y/N)             |                              |                | instalación|                            |
 +---------------------------+------------------------------+----------------+-----------------------------------------+
 

La captura de pantalla para el comando de instalación se enumeran a continuación,

.. code-block:: bash

 kevell@corp:/$ ptconfigure composer install
 Install Composer - Update to latest version ? (Y/N) 
 Y
 ******************************
 *        Pharaoh Tools        *
 *          Composer!         *
 *******************************
 What is the program data directory? Found "/opt/composer" - use this? (Enter nothing for yes, no end slash)

 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'https://github.com/phpengine/composer-phar.git'  /tmp/composer/composerCloning into '/tmp/composer/composer'...

 remote: Counting objects: 6, done.
 remote: Total 6 (delta 0), reused 0 (delta 0), pack-reused 6
 Unpacking objects: 100% (6/6), done.
 Checking connectivity... done.
 Program Data Folder /opt/composer Deleted if existed
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Composer: Success
 ------------------------------
 Installer Finished
 ******************************

Beneficios
--------------

* Se instala dependencias (por ejemplo, bibliotecas) para una aplicación.
* También permite a los usuarios instalar
