==============
Templating
==============


sinopsis
---------------

El término de plantillas cuando se utiliza en el contexto de formato de archivo ptdeploy se refiere a una característica común de muchas aplicaciones de software que definen un formato de archivo no ejecutable único destinado específicamente para esa aplicación particular.

Formatos de plantillas son aquellos cuyo archivo indica que el tipo fil.e pretende ser un punto de partida muy alto desde el que crear otra
archivos.

Estos tipos de archivos suelen instalarse archivo de plantillas con nuevos valores. Se adapta a trabajar con Ubuntu y CentOS .

comando Ayuda
------------------------

El comando de ayuda conduce a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en los módulos de plantilla. El comando help enumera los parámetros alternativos de plantillas bajo módulo ptdeploy . También describe la sintaxis para la detección de la máquina del usuario . El comando de ayuda para crear plantillas se muestra a continuación .

.. code-block:: bash

	ptdeploy templating help


La siguiente captura de pantalla y explica sobre plantillas.


.. code-block:: bash

 kevell@corp:/# ptdeploy templating help
 ******************************


  This command allows you to install a templated file with new values.

  Templating, templating, template

        - install
        Installs a template
        example: ptconfigure template install

 ------------------------------
 End Help
 ******************************


instalación
----------------

En contexto ptdeploy , plantillas se refiere a la creación de una única imagen de máquina virtual como un sistema operativo invitado, luego guardarlo como una herramienta para múltiples máquinas virtuales que se ejecutan . La técnica se utiliza para instalar tanto en la gestión de la virtualización y el cloud computing , y es común en grandes almacenes de servidor. El siguiente comando ayuda al usuario a instalar plantillas.

.. code-block:: bash

	ptdeploy templating install

La siguiente captura de pantalla guía al usuario a instalar.


.. code-block:: bash

 kevell@corp:/# ptdeploy templating install

 Install Templating Functionality? (Y/N) 
 Y
 *******************************
 *   Golden Contact Computing  *
 *         Templating !        *
 *******************************
 ... All done!
 *******************************
 Thanks for installing , visit www.gcsoftshop.co.uk for more
 ******************************


 Single App Installer:
 --------------------------------------------


 Templating: Success

 ------------------------------
 Installer Finished
 ******************************



opción
------------

.. cssclass:: table-bordered

 +-----------------------------------+-------------------------+-----------+--------------------------------------------------+
 | parámetros	       		     | parámetros alternativos | Opciones  | Comentarios		   	              |
 +===================================+=========================+===========+==================================================+
 |Install templating functionality?  | Templating, templating  | Yes	   | Plantillas puede instalarse bajo ptdeploy .      |
 |                                   | template                |           |                                                  |
 +-----------------------------------+-------------------------+------- ---+--------------------------------------------------+
 |Install templating functionality?  | Templating, templating  | No	   | Se puede salir de la pantalla                    |
 |                                   | template|               |           |                                                  |
 +-----------------------------------+-------------------------+-----------+--------------------------------------------------+



Beneficios
-----------------

* El procesamiento de plantillas se utiliza en varios contextos para diferentes propósitos .
* El objetivo específico es normalmente depende de la aplicación de software o la plantilla en uso.
* no sensibles
* Trajes para trabajar con Ubuntu y CentOS .
* Versión actualizada con nuevos valores es posible.
