=================
PTBuild
=================

sinopsis
------------------

Esta herramienta ayuda al usuario a instalar y actualizar ptbuild bajo ptconfigure en herramientas faraón. Automatización de la construcción debe incluir la automatización de la integración, que a menudo incluye el despliegue en un entorno de producción similar. En muchos casos, el script de construcción no sólo compila binarios, pero también genera documentación, páginas web, las estadísticas y los medios de distribución, tales como Red Hat. Se consuela con Ubuntu y CentOS.

comando Ayuda
-----------------------

El comando de ayuda conduce a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en los módulos ptbuild. Las listas de comandos de ayuda fuera de los parámetros alternativos de ptbuild bajo módulo ptconfigure. También se describe la sintaxis para la instalación de updation del usuario. El comando de ayuda para ptbuild se muestra a continuación.

.. code-block:: bash

 		ptconfigure ptbuild help

La siguiente captura de pantalla muestra el esfuerzo total de ptbuild.

.. code-block:: bash

 kevell@corp:/# ptconfigure ptbuild help

 ******************************


  This command allows you to install or update ptbuild.

  ptbuild, Ptbuild

        - install
        Installs the latest version of ptbuild
        example: ptconfigure ptbuild install

        - ensure
        Ensures ptbuild is installed
        example: ptconfigure ptbuild ensure

        - uninstall
        Uninstalls the latest version of ptbuild
        example: ptconfigure ptbuild uninstall
 ------------------------------
 End Help
 ******************************

instalación
--------------------

Esta es una herramienta que se encuentra bajo ptconfigure y tira hacia abajo copias limpias de la base de código de usuario y no completa construye, a partir de cero, todo el tiempo. Este comando se utiliza para instalar la última versión de ptbuild. El comando utilizado para la instalación es el siguiente.

.. code-block:: bash

	ptconfigure ptbuild install

 Después introduce el comando, el sistema puede pedir

install ptbuild?(Y/N)

Si el usuario da Y entonces se instalará ptbuild. La siguiente captura de pantalla demuestran.

.. code-block:: bash


.. cssclass:: table-bordered

 +------------------------+------------------------------+--------------+--------------------------------------------------------+
 | Parámetros             | Directorio (por defecto)     | Opciones     | Comentarios                                            |
 +========================+==============================+==============+========================================================+
 |Program data directory  | “/opt/ptbuild(módulo         | Y(Yes)       | Si el usuario de proceder con la instalación del       |
 |(Por defecto)           | correspondiente)”            |              | directorio de datos de programa predeterminado que     |
 |                        |                              |              | puede introducir como Sí                               |
 +------------------------+------------------------------+--------------+--------------------------------------------------------+
 |Program data directory  | específica de usuario        | N(Fin barra) | Si el usuario desea continuar con su propio directorio |
 |                        |                              |              | de datos del programa, pueden de entrada como N, y en  |
 |                        |                              |              | la mano especificar que poseen ubicación.              |
 +------------------------+------------------------------+--------------+--------------------------------------------------------+
 |Program executor        | “/usr/bin”                   | Y(Yes)       | Si el usuario de proceder con la instalación del       | 
 |directory (Por defecto) |                              |              | directorio ejecutor programa predeterminado que puede  |
 |                        |                              |              | introducir como Sí                                     |
 +------------------------+------------------------------+--------------+--------------------------------------------------------+
 |Program executor        | específica de usuario        | N(Fin barra) | Si el usuario desea continuar con su propio directorio |
 |directory               |                              |              | ejecutor del programa, pueden de entrada como N, y en  |
 |                        |                              |              | la mano especificar que poseen ubicación.|             |
 +------------------------+------------------------------+--------------+--------------------------------------------------------+


Desinstalar
--------------

Este comando se utiliza para desinstalar la versión más reciente de ptbuild. El comando que se utiliza para la desinstalación es el siguiente.

.. code-block:: bash

		ptconfigure ptbuild Uninstall

Después introduce el comando, el sistema puede pedir

Uninstall ptbuild?(Y/N)

Si el usuario da Y entonces ptbuild será desinstalado. La siguiente captura de pantalla demuestran.

.. code-block:: bash


.. cssclass:: table-bordered


 +------------------------+------------------------------+--------------+--------------------------------------------------------+
 | Parámetros             | Directorio (por defecto)     | Opciones     | Comentarios                                            |
 +========================+==============================+==============+========================================================+
 |Program data directory  | “/opt/ptbuild(módulo         | Y(Yes)       | Si el usuario para proceder con los datos del programa | 
 |(Por defecto)           | correspondiente)”            |              | de desinstalación directorio predeterminado para ser   |
 |                        |                              |              | introducido como Sí                                    |
 +------------------------+------------------------------+--------------+--------------------------------------------------------+
 |Program data directory  | específica de usuario        | N(Fin barra) | Si el usuario desea continuar con su propio directorio |
 |                        |                              |              | de datos del programa, pueden de entrada como N, y en  |
 |                        |                              |              | la mano especificar que poseen ubicación.              |
 +------------------------+------------------------------+--------------+--------------------------------------------------------+
 |Program executor        | “/usr/bin”                   | Y(Yes)       | Si el usuario para proceder con el directorio          | 
 |directory (Por defecto) |                              |              | predeterminado desinstalación del programa en          |
 |                        |                              |              | ejecución que se puede introducir en Sí                |
 +------------------------+------------------------------+--------------+--------------------------------------------------------+
 |Program executor        | específica de usuario        | N(Fin barra) | Si el usuario desea continuar con su propio directorio |
 |directory               |                              |              | ejecutor del programa, pueden de entrada como N, y en  |
 |                        |                              |              | la mano especificar que poseen ubicación.|             |
 +------------------------+------------------------------+--------------+--------------------------------------------------------+


asegurar
----------

Proceso que se utiliza para comprobar el ptbuild instalado en el sistema del usuario o no Ensure. El siguiente comando ayuda al usuario para asegurarse.

.. code-block:: bash

		ptconfigure ptbuild ensure

La siguiente captura de pantalla muestra sus funciones.

.. code-block:: bash


parámetros alternativos
-----------------------

Los parámetros alternativos que se pueden utilizar en la declaración son:

  Ptbuild

  Ptbuild

Beneficios
----------------

* Se utiliza para instalar ptbuilds posible.
* Adecuado para trabajar con Ubuntu y CentOS.
* Sensitibilidad caso.
* Automatización en la versión actualizada.
* Fiabilidad, disponibilidad, capacidad de servicio con otras conexiones.


