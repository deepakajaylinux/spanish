==============
ModuleManager
==============

sinopsis
-----------

El ámbito principal de la gerente módulo es permitir al usuario gestionar sus módulos. Sus funciones principales incluyen la instalación, activar, desactivar, garantizar, desinstalación. vamos a ver sobre estas importantes funciones del administrador de módulos de una manera elaborada a partir de los próximos temas.

Ayuda Comando
----------------------

El comando ayuda de este gestor de módulos es un breve manual de usuario que guía al usuario en cuanto a la finalidad, de gestor de módulos, describe al usuario sobre las funciones principales, tales como instalar, activar, desactivar, garantizar, desinstale junto con la sintaxis para declarar ellos. También enumera outs los parámetros alternativos de gestor de módulos. El comando para declarar la opción de ayuda en virtud de administrador de módulos se muestra a continuación:

.. code-block:: bash

		ptconfigure ModuleManager help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda bajo gestor de módulos.

.. code-block:: bash


 kevell@corp:/# ptconfigure ModuleManager help

 ******************************


  The Module Manager allows you to manage modules. Install, Ensure, Uninstall, Enable, Disable.

  ModuleManager, module-manager, modulemanager

        - install
        Installs the latest version of a module. If a module of the same name already exists in your Extensions directory,
        an error will be thrown.
        example: ptconfigure module-manager install --module-name="MyModule" --module-source="http://git.cleo-modules.com/MyModule.git"

        - ensure
        Ensures the existence of a module. The module will only be installed if it currently doesn't exist.
        example: ptconfigure module-manager ensure --module-name="MyModule" --module-source="http://git.cleo-modules.com/MyModule.git"

        - uninstall
        Uninstalls a Module. This will delete all of the files for this Module
        example: ptconfigure module-manager enable --module-name="MyModule"

        - enable
        Enables a Module. All installed Modules are enabled by default.
        example: ptconfigure module-manager enable --module-name="MyModule"

        - disable
        Disables a Module. The files for this module will still exist, but none will be automatically loaded during execution.
        example: ptconfigure module-manager disable --module-name="MyModule"

 ------------------------------
 End Help
 ******************************

instalación
----------------

El comando utilizado para instalar el gestor de módulos en la máquina de los usuarios se muestra a continuación:

.. code-block:: bash

		ptconfigure module-manager install

Después de introducir el comando anterior, el siguiente proceso se produce como se muestra en el formato tabular.

.. cssclass:: table-bordered

 +---------------------------+--------------------------------------+--------------+----------------------------------------------+
 | Parámetros                | Parámetro Alternativa                | Opciones     | Comentarios                                  |
 +===========================+======================================+==============+==============================================+
 |Install ModuleManager?     | En lugar de module-manager, podemos  | Y(Yes)       | Si el usuario desea continuar el proceso     |
 |(Y/N)                      | utilizar modulemanager,              |              | de instalación se puede introducir como Y.   |
 |                           | ModuleManager también.               |              |                                              |
 +---------------------------+--------------------------------------+--------------+----------------------------------------------+
 |Install ModuleManager?     | En lugar de module-manager, podemos  | N(No)        | Si el usuario desea abandonar el proceso     |
 |(Y/N)                      | utilizar modulemanager,              |              | de instalación se puede introducir como N.   |
 |                           | ModuleManager también.|              |              |                                              | 
 +---------------------------+--------------------------------------+--------------+----------------------------------------------+

Si el usuario procede de la instalación, durante el proceso de instalación, el siguiente proceso se realiza como se muestra en el formato tabular:
.. cssclass:: table-bordered


 +---------------------------+-----------------------------------+----------------+--------------------------------------------------+
 | Parámetros                | camino                            | Opciones       | Comentarios                                      |
 +===========================+===================================+================+==================================================+
 |Program executor director  | “/usr/bin”                        | Y(Yes)         | Si el usuario de proceder con la instalación     |
 |(Por defecto)              |                                   |                | del directorio ejecutor programa predeterminado  |
 |                           |                                   |                | que puede introducir como Sí                     |
 +---------------------------+-----------------------------------+----------------+--------------------------------------------------+
 |Program executor directory | específica de usuario             | No(End Slash)  | Si el usuario de proceder con la instalación     |
 |(Por defecto)              |                                   |                | de su propio directorio ejecutor del programa    |
 |                           |                                   |                | se puede introducir como N, y en la mano         |
 |                           |                                   |                | especificar que poseen ubicación|                |
 +---------------------------+-----------------------------------+----------------+--------------------------------------------------+


Finalmente voluntad instalación se completó como se muestra en la siguiente captura de pantalla.

permitir
-----------

El proceso de activación tiene por objeto permitir el módulo. Todos los módulos instalados están habilitadas por defecto con el comando a continuación:

.. code-block:: bash

	ptconfigure module-manager enable --module-name="MyModule"

Después de introducir este comando, el módulo que se especifica se habilita.

inhabilitar
-------------

El proceso tiene como objetivo desactivar la desactivación del módulo. Los archivos de los módulos con discapacidad sigue siendo existe, pero que no serán cargados en el momento de la ejecución. Esto se puede lograr por el siguiente comando

.. code-block:: bash

	ptconfigure module-manager disable --module-name="MyModule"

Después de introducir este comando, el módulo que se especifica se desactiva.

asegurar
----------

El papel de asegurar que el proceso es comprobar la disponibilidad de módulos. Después de que el proceso de garantizar se completó se instalarán los módulos sólo si los módulos reportan como no se instala. El proceso de garantizar se puede hacer mediante el uso de la orden dada a continuación:

.. code-block:: bash

		ptconfigure module-manager ensure

Durante el proceso de garantizar, las versiones de los módulos no se comprueban. La siguiente captura de pantalla representan gráficamente el proceso de garantizar.

.. code-block:: bash

 kevell@corp:/# ptconfigure module-manager ensure

 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module ModuleManager reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 ******************************


 Single App Installer:
 --------------------------------------------
 ModuleManager: Success
 ------------------------------
 Installer Finished
 ******************************

Desinstalar
-------------

El proceso de desinstalación se utiliza para borrar todos los archivos de los módulos. El comando utilizado para desinstalar el gestor de módulos se muestra a continuación:

.. code-block:: bash

		ptconfigure module-manager uninstall

Después de introducir el comando anterior, el siguiente proceso se produce como se muestra en el formato tabular.

.. cssclass:: table-bordered

 +----------------------------------+-------------------------------------------+--------------+--------------------------------------------+
 | Parámetros                       | Parámetro Alternativa                     | Opciones     | Comentarios                                |
 +==================================+===========================================+==============+============================================+
 |Un Install ModuleManager? (Y/N)   | En lugar de module-manager, podemos       | Y(Yes)       | Si el usuario desea continuar el proceso   |
 |                                  | utilizar modulemanager, ModuleManager     |              | de desinstalación se puede introducir como |
 |                                  | también.                                  |              | Y                                          |
 +----------------------------------+-------------------------------------------+--------------+--------------------------------------------+
 |Un Install ModuleManager? (Y/N)   | En lugar de module-manager, podemos       | N(No)        | Si el usuario desea abandonar el proceso   |
 |                                  | utilizar modulemanager, ModuleManager     |              | de desinstalación se puede introducir      |
 |                                  | también                                   |              | como N.|                                   |
 +----------------------------------+-------------------------------------------+--------------+--------------------------------------------+

Si el usuario procede de la instalación, durante el proceso de instalación, el siguiente proceso se realiza como se muestra en el formato tabular:

.. cssclass:: table-bordered


 +---------------------------+----------------------------+--------------+-------------------------------------------------------+
 | Parámetros                | camino                     | Opciones     | Comentarios                                           |
 +===========================+============================+==============+=======================================================+
 |Program executor directory | “/usr/bin”                 | Y(Yes)       | Si el usuario para proceder desinstalación con el     |
 |(Por defecto)              |                            |              | directorio ejecutor programa predeterminado que       |
 |                           |                            |              | puede introducir como Sí                              |
 +---------------------------+----------------------------+--------------+-------------------------------------------------------+
 |Program executor directory | específica de usuario      | No (End      | Si el usuario para proceder desinstalación con su     |
 |(Por defecto)              |                            | slash)       | propio directorio ejecutor del programa se puede      |
 |                           |                            |              | introducir como N, y en la mano especificar que       |
 |                           |                            |              | poseen ubicación|                                     |
 +---------------------------+----------------------------+--------------+-------------------------------------------------------+

Por último, la desinstalación se completó como se muestra en la siguiente captura de pantalla.

.. code-block:: bash

Beneficios
-------------

* Los parámetros utilizados en la ayuda y la instalación, desinstalación, activar, desactivar, asegúrese de que no entre mayúsculas y 
  minúsculas, que es una ventaja añadida, mientras que en comparación con otros.
* Es-acomodados tanto en Ubuntu y así como Cent OS.
* El proceso de garantizar facilita la disponibilidad de cheques de los módulos antes de la instalación.
* Si el usuario desea desactivar un módulo en particular que pueden desactivarlos sin borrar sus archivos correspondientes.
* Durante la instalación, desinstale el usuario puede especificar la ubicación de directorio ejecutor del programa.
