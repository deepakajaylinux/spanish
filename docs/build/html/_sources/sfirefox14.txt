===================
FireFox14
===================

sinopsis
----------

En este módulo se utiliza para instalar firefox14. Ubuntu lanza versiones actualizadas periódicamente. Implementa los estándares web actuales y previstos. Apoyo a largo plazo incluye actualizaciones para el nuevo hardware, parches de seguridad y actualizaciones de la infraestructura de cloud computing. Es cómodo con Ubuntu y CentOS.

Ayuda Comando
---------------------

Este comando puede funcionar sobre los objetivos y los comandos disponibles bajo módulo Firefox14. También explica el comando para instalar firefox14. Antes de la instalación, el usuario puede leer este comando de ayuda explica su función.

.. code-block:: bash
           
      ptconfigure firefox14 help

La siguiente imagen también ayuda a entender este módulo con claridad.

.. code-block:: bash

	Kevell@corp:/# ptconfigure firefox14 help
	******************************


	 This command allows you to install Firefox14.

	 Firefox14, ff14, firefox14

        - install
        Installs the latest version of Firefox 14
        example: ptconfigure firefox14 install

	------------------------------
	End Help
	******************************

instalación
--------------

Es un proceso evidente para instalar módulo firefox14 bajo Ptconfigure simplemente usando la orden dada a continuación,

.. code-block:: bash
       
  ptconfigure firefox14 install

Después de clave en el comando, puede pregunta

Install firefox14? (Y/N)

En caso de que la entrada del usuario como Y, se puede instalar firefox14 del paquete. Si no, se puede salir de la pantalla. Las siguientes capturas de pantalla pueden explicarlo.

.. code-block:: bash
        
        kevell@corp:/# ptconfigure Firefox14 install

        Install Firefox? (Y/N) 
        y
        *******************************
        *        Pharaoh Tools        *
        *          Firefox            *
        *******************************
        Creating /tmp/ptconfigure-temp-script-51942043520.sh
        chmod 755 /tmp/ptconfigure-temp-script-51942043520.sh 2>/dev/null
        Changing /tmp/ptconfigure-temp-script-51942043520.sh Permissions
        Executing /tmp/ptconfigure-temp-script-51942043520.sh
        Cloning into 'firefox14'...
        remote: Counting objects: 78, done.
        remote: Total 78 (delta 0), reused 0 (delta 0)
        Unpacking objects: 100% (78/78), done.
        Checking connectivity... done.
        Temp File /tmp/ptconfigure-temp-script-51942043520.sh Removed
        Program Executor Deleted if existed
        ... All done!
        *******************************
        Thanks for installing , visit www.pharaohtools.com for more
        ******************************


        Single App Installer:
        --------------------------------------------
        Firefox14: Success
        ------------------------------
        Installer Finished
        ******************************


Opciones
--------------

.. cssclass:: table-bordered

 +--------------------------+----------------------------------------+------------+--------------------------------------+
 | parámetros               | Parámetro Alternativa                  | Opciones   | Comentarios                          |
 +==========================+========================================+============+======================================+
 |ptconfigure firefox14     | En lugar de utilizar firefox14 podemos | Y(Yes)     | El sistema se inicia proceso de      |
 |Install                   | utilizar FF14, Firefox14               |            | instalación Bajo ptconfigure         |
 +--------------------------+----------------------------------------+------------+--------------------------------------+
 |ptconfigure firefox14     | En lugar de utilizar firefox14 podemos | N(No)      | El sistema detiene proceso de        |
 |Install                   | utilizar FF14, Firefox14               |            | instalación Bajo ptconfigure|        |
 +--------------------------+----------------------------------------+------------+--------------------------------------+


Beneficios
---------------

* Firefox14 utiliza soporte para nuevo hardware y la integración de todas las actualizaciones publicadas en la serie hasta la fecha.
* Firefox14 no es sensible a mayúsculas.
* Privacidad y medidas de seguridad, búsqueda inteligente es posible.
* Es cómodo con Ubuntu y CentOS.


