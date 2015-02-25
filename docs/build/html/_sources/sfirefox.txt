==========
FireFox
==========

sinopsis
-----------

En este módulo se utiliza para instalar firefox. Ubuntu lanza versiones actualizadas periódicamente. Implementa los estándares web actuales y previstos. Apoyo a largo plazo incluye actualizaciones para el nuevo hardware, parches de seguridad y actualizaciones de la infraestructura de cloud computing. Es cómodo con Ubuntu y CentOS.

Ayuda Comando
----------------------

Este comando puede funcionar sobre los objetivos y los comandos disponibles bajo módulo de Firefox. También explica el comando para instalar firefox. Antes de la instalación, el usuario puede leer este comando de ayuda explica su función.

.. code-block:: bash

              ptconfigure firefox help

La siguiente imagen también ayuda a entender este módulo con claridad.

.. code-block:: bash

	 kevell@corp:/# ptconfigure firefox help

	 ******************************


	 This command is part of Core and provides you  with a method by which you can install Firefox from your package
         manager

	 Firefox, firefox

        - install
        Installs Firefox
        example: ptconfigure firefox install

	------------------------------
	End Help
	******************************

instalación
-------------------

Es un proceso evidente para instalar módulo firefox bajo Ptconfigure simplemente usando la orden dada a continuación,

.. code-block:: bash

              ptconfigure firefox install

Después de clave en el comando, puede pregunta

Install firefox? (Y/N)

En caso de que la entrada del usuario como Y, se puede instalar Firefox desde el paquete. Si no, se puede salir de la pantalla. Las siguientes capturas de pantalla pueden explicarlo.

.. code-block:: bash
	
	kevell@corp:/# ptconfigure firefox install

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
	Cloning into 'firefox'...
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
	Firefox: Success
	------------------------------
	Installer Finished
	******************************

Opciones
--------------

.. cssclass:: table-bordered

 +-----------------------------+----------------------------------+------------+--------------------------------------------+
 | Parámetros                  | Parámetro Alternativa            | Opciones   | Comentarios                                |
 +=============================+==================================+============+============================================+
 |ptconfigure firefox Install  | En vez de usar firefox podemos   | Y(Yes)     | El sistema se inicia proceso de            |
 |                             | utilizar Firefox, firefox        |            | instalación se puede introducir como Y     |
 +-----------------------------+----------------------------------+------------+--------------------------------------------+
 |ptconfigure Firefox Install  | En vez de usar firefox podemos   | N(No)      | El sistema detiene proceso de instalación  |
 |                             | utilizar Firefox, firefox|       |            |                                            |
 +-----------------------------+----------------------------------+------------+--------------------------------------------+


Beneficios
-------------

* Firefox utiliza el soporte para nuevo hardware y la integración de todas las actualizaciones publicadas en la serie hasta la fecha.
* Es cómodo con Ubuntu y CentOS.
* Firefox no es sensible a mayúsculas.
* Privacidad y medidas de seguridad, búsqueda inteligente
