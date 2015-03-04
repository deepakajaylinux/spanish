==============
Phake
==============

sinopsis
-------------

Phake es un marco de burla para PHP. Permite la creación de objetos que imitan a un objeto real de una manera predecible y controlada. Esto le permite tratar las llamadas a métodos externos realizados por el sistema bajo prueba (SUT) como otra forma de entrada a tu SUT y salida de su SUT. Esto se hace por métodos que suministran entrada indirecta en su prueba de tropezar y mediante la verificación de los parámetros a los métodos que reciben salida indirecta de la prueba.

Ayuda Comando
----------------------

Este comando ayuda a determinar el uso del módulo Phake. El usuario se llega a saber acerca de las diferentes formas / formato para ejecutar este módulo. Este comando guía al usuario final a conocer el propósito de este comando. A continuación dado son el mando y la pantalla del mismo.

.. code-block:: bash
        
	        ptconfigure Phake help

.. code-block:: bash


 kevell@corp:/# ptconfigure Phake help
 ******************************


  This command allows you to install or update Phake.

  Phake, phake

        - install
        Installs the latest version of phake
        example: ptconfigure phake install

        - ensure
        Installs the latest version of phake, only if a version is not installed
        example: ptconfigure phake ensure

 ------------------------------
 End Help
 ******************************

instalación
----------------

Cuando el usuario necesita para instalar Phake en la máquina, el siguiente comando dado se ejecutará el proceso de instalación.

.. code-block:: bash
         
   	        ptconfigure Phake install

El sistema pide el nombre del directorio, si usted quiere establecer su PATH puede definir su camino. Defina su trayectoria seguida por el símbolo "/". Pulse Intro si no hay cambios por hacer.

"What is the program data directory? Found "/opt/phake" - use this?

A continuación, el sistema pide la ejecución de nombre de directorio, si usted quiere establecer su PATH puede definir su camino. Defina su trayectoria seguida por el símbolo "/". Pulse Intro si no hay cambios por hacer

"What is the program executer directory? Found "/usr/bin" - Use this? "

La siguiente captura de pantalla muestra la misma.

.. code-block:: bash

 kevell@corp:/# ptconfigure Phake install
 Install Phake ? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *          Phake         *
 *******************************
 What is the program data directory? Found "/opt/phake" - use this? (Enter nothing for yes, no end slash)

 What is the program executor directory? Found "/usr/bin" - use this? (Enter nothing for yes, No Trailing Slash)

 git clone 'http://github.com/jaz303/phake.git'  /tmp/phake/phakeCloning into '/tmp/phake/phake'...
 remote: Counting objects: 552, done.
 remote: Total 552 (delta 0), reused 0 (delta 0)
 Receiving objects: 100% (552/552), 91.36 KiB | 76.00 KiB/s, done.
 Resolving deltas: 100% (314/314), done.
 Checking connectivity... done.
 Program Data folder populated
 Program Executor Deleted if existed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Phake: Success
 ------------------------------
 Installer Finished
 ******************************

Opciones
-----------
.. cssclass:: table-bordered

 +---------------------+------------------------------------------------------+-----------+------------------------------------------------+
 | Parámetros          | Parámetro Alternativa                                | Opciones  | Comentarios                                    |
 +=====================+======================================================+===========+================================================+
 |Install Phake? (Y/N) | Cualquiera de los dos parámetros alternativa se      | Y(Yes)    | Una vez que el usuario proporciona la opción,  |
 |                     | puede utilizar en mandamiento Phake, phake por       |           | sistema comienza proceso de instalación        |
 |                     | ejemplo: ptconfigure phake Install                   |           |                                                |
 +---------------------+------------------------------------------------------+-----------+------------------------------------------------+
 |Install Phake? (Y/N) | Cualquiera de los dos parámetros alternativa se      | N(No)     | Una vez que el usuario proporciona la opción,  |
 |                     | puede utilizar en mandamiento Phake, phake por       |           | Sistema detiene proceso de instalación         |
 |                     | ejemplo: ptconfigure phake Install|                  |           |                                                |
 +---------------------+------------------------------------------------------+-----------+------------------------------------------------+


Beneficios
--------------

* Phake es una gran biblioteca de burla y se puede integrar fácilmente en PHPUnit.
* Su nuevo enfoque de la burla y talones de prototipos y la separación entre las fases Stubbing y verificación es muy refrescante y fácil de 
  usar.
