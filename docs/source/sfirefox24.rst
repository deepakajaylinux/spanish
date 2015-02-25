===================
FireFox24
===================

sinopsis
----------

En este módulo se utiliza para instalar firefox24. Ubuntu lanza versiones actualizadas periódicamente. Implementa los estándares web actuales y previstos. Apoyo a largo plazo incluye actualizaciones para el nuevo hardware, parches de seguridad y actualizaciones de la infraestructura de cloud computing. Es cómodo con Ubuntu y CentOS.

Ayuda Comando
---------------------

Este comando puede funcionar sobre los objetivos y los comandos disponibles bajo módulo Firefox24. También explica el comando para instalar firefox24. Antes de la instalación, el usuario puede leer este comando de ayuda explica su función.

.. code-block:: bash
           
      ptconfigure firefox24 help

La siguiente imagen también ayuda a entender este módulo con claridad.

.. code-block:: bash

	Kevell@corp:/# ptconfigure firefox24 help
	******************************


	 This command allows you to install Firefox24.

	 Firefox24, ff24, firefox24

        - install
        Installs the latest version of Firefox 24
        example: ptconfigure firefox24 install

	------------------------------
	End Help
	******************************

instalación
--------------

Es un proceso evidente para instalar módulo firefox24 bajo Ptconfigure simplemente usando la orden dada a continuación,

.. code-block:: bash
       
  ptconfigure firefox24 install

Después de clave en el comando, puede pregunta

Install firefox24? (Y/N)

En caso de que la entrada del usuario como Y, se puede instalar firefox24 del paquete. Si no, se puede salir de la pantalla. Las siguientes capturas de pantalla pueden explicarlo.

.. code-block:: bash
        
        kevell@corp:/# ptconfigure Firefox24 install

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
        Cloning into 'firefox24'...
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
        Firefox24: Success
        ------------------------------
        Installer Finished
        ******************************


Opciones
--------------

.. cssclass:: table-bordered

 +-------------------------+----------------------------------------+-------------+-------------------------------------+
 | parámetros              | Parámetro Alternativa                  | Opciones    | Comentarios                         |
 +=========================+========================================+=============+=====================================+
 |ptconfigure firefox24    | En lugar de utilizar firefox24 podemos | Y(Yes)      | El sistema se inicia proceso de     |
 |Install                  | utilizar FF24, Firefox24               |             | instalación Bajo ptconfigure        |
 +-------------------------+----------------------------------------+-------------+-------------------------------------+
 |ptconfigure firefox24    | En lugar de utilizar firefox24 podemos | N(No)       | El sistema detiene proceso de       |
 |Install                  | utilizar FF24, Firefox24               |             | instalación Bajo ptconfigure|       |
 +-------------------------+----------------------------------------+-------------+-------------------------------------+

Beneficios
---------------

* Firefox24 utiliza soporte para nuevo hardware y la integración de todas las actualizaciones publicadas en la serie hasta la fecha.
* Firefox24 no es sensible a mayúsculas.
* Privacidad y medidas de seguridad, búsqueda inteligente es posible.
* Es cómodo con Ubuntu y CentOS.




