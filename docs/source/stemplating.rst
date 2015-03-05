===========
Templating
===========

sinopsis
---------------

El término de plantillas cuando se utiliza en el contexto de formato de archivo ptconfigure se refiere a una característica común de muchas aplicaciones de software que definen un formato de archivo no ejecutable único destinado específicamente para esa aplicación particular.
Formatos de plantillas son aquellos cuyo archivo indica que el tipo de archivo está pensado como un punto de partida muy alta de la que para crear otros archivos.

Estos tipos de archivos suelen instalarse archivo de plantillas con nuevos valores. Se adapta a trabajar con Ubuntu y CentOS.

comando Ayuda
------------------------

El comando de ayuda conduce a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en los módulos de plantilla. El comando help enumera los parámetros alternativos de plantillas bajo módulo Ptconfigure. También describe la sintaxis para la detección de la máquina del usuario.

El comando de ayuda para crear plantillas se muestra a continuación.

.. code-block:: bash

	ptconfigure templating help

La siguiente captura de pantalla y explica sobre plantillas.

.. code-block:: bash

 kevell@corp:/# ptconfigure templating help
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

En contexto ptconfigure, plantillas se refiere a la creación de una única imagen de máquina virtual como un sistema operativo invitado, luego guardarlo como una herramienta para múltiples máquinas virtuales que se ejecutan. La técnica se utiliza para instalar tanto en la gestión de la virtualización y el cloud computing, y es común en grandes almacenes de servidor.

El siguiente comando ayuda al usuario a instalar plantillas.

.. code-block:: bash

	ptconfigure templating install

La siguiente captura de pantalla guía al usuario a instalar.

.. code-block:: bash



Opciones
------------

.. cssclass:: table-bordered

 +----------------------+----------------------------------------+----------+------------------------------------------------+
 | Parámetros           | Parámetro Alternativa                  | Opciones | Comentarios                                    |
 +======================+========================================+==========+================================================+
 |Install templating    | En lugar de utilizar templating, el    | Y(Yes)   | Si el usuario desea continuar el proceso de    |
 |functionality (Y/N)	| usuario puede utilizar Templating,     |          | instalación se puede introducir como Y.        |
 |                      | templating, template                   |          |                                                |
 +----------------------+----------------------------------------+----------+------------------------------------------------+
 |Install templating    | En lugar de utilizar templating, el    | N(No)    | Si el usuario desea abandonar el proceso de    |
 |functionality (Y/N)	| usuario puede utilizar Templating,     |          | instalación se puede introducir como N.        |
 |                      | templating, template|                  |          |                                                |
 +----------------------+----------------------------------------+----------+------------------------------------------------+




Beneficios
-----------------

* El procesamiento de plantillas se utiliza en varios contextos para diferentes propósitos.
* El objetivo específico es normalmente depende de la aplicación de software o la plantilla en uso.
* No sensibles
* Se adapta a trabajar con Ubuntu y CentOS.
* Versión actualizada con nuevos valores es posible.


