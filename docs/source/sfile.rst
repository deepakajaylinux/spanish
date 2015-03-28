==========
File
==========

Sinopsis
-------------

El archivo es un programa estándar para reconocer el tipo de datos contenidos en un archivo de computadora. Los intentos del comando archivo para clasificar cada sistema objeto de archivo (es decir, archivo, directorio o enlace) que se proporciona a ella como un argumento (es decir, de entrada). Archivo prueba cada argumento en un intento de clasificarlo. Hay tres conjuntos de pruebas, realizadas en este orden: pruebas de sistemas de ficheros, pruebas de números mágicos y pruebas de lenguajes.

La primera es una prueba del sistema de archivos, que utiliza la llamada al sistema stat para obtener información de i-nodo del objeto (que contiene información acerca de un archivo).

La segunda prueba consiste en comprobar si hay un número mágico, que es un número incluido en o cerca del comienzo de muchos tipos de archivos que indica el formato de archivo (es decir, el tipo de archivo).

En el caso de que las dos primeras pruebas fallan para determinar el tipo de un archivo, se emplean pruebas de lenguaje para determinar si se trata de texto plano (es decir, compuesto en su totalidad de caracteres legibles), y, en caso afirmativo, qué tipo de texto sin formato , tales como HTML (lenguaje de marcado de hipertexto) o código fuente

Ayuda Comando
----------------------

Este comando ayuda a determinar el uso del módulo de archivo. El usuario se llega a saber acerca de las diferentes formas / formato para ejecutar este módulo. Este comando guía al usuario final a conocer el propósito de este comando. A continuación dado son el mando y la pantalla del mismo.

.. code-block:: bash
        
	ptconfigure file help


.. code-block:: bash

 kevell@corp:/# ptconfigure File help
 ******************************


  This command allows you to modify files or check their existence

  File, file

        - create
        Create a new system file
        example: ptconfigure file create --file="somename"

        - delete
        Delete a system file
        example: ptconfigure file delete --file="somename"

        - exists
        Check the existence of a file
        example: ptconfigure file exists --filename="somename"

        - append
        Append a line to a file
        example: ptconfigure file append --filename="somename" --line="a line"

        - should-have-line
        Ensure that a file contains a particular line
        example: ptconfigure file should-have-line --filename="somename" --line="a line"

 ------------------------------
 End Help
 ******************************



crear
------------

Cuando el usuario necesita para crear un nuevo archivo de sistema, el comando a continuación se indica se ejecutará el proceso.

.. code-block:: bash

	ptconfigure file create --file="somename"

Las siguientes órdenes dadas sobrescribir archivos que existen

.. code-block:: bash
         
	ptconfigure file create --file="somename” --overwrite-existing

El siguiente comando dado para escribir los datos en el archive

.. code-block:: bash
           
	ptconfigure file create –file="somename” --data="things to put in the file" 


.. code-block:: bash

 kevell@corp:/# ptconfigure file create --file="somename"

 [Pharaoh Logging] [File] Creating File somename
 File somename exists 
 ******************************


 File Modifications:
 --------------------------------------------

 File: Success

 ------------------------------
 File Mods Finished
 ******************************


borrar
----------

Cuando el usuario necesita para eliminar un archivo del sistema, el comando a continuación se indica se ejecutará el proceso.

.. code-block:: bash
	
		ptconfigure file delete --file="somename"

.. code-block:: bash

 kevell@corp:/# ptconfigure file delete --file="somename"

 [Pharaoh Logging] [File] Deleting File somename
 somename Deleted
 File somename not exists 
 ******************************


 File Modifications:
 --------------------------------------------

 File: Success

 ------------------------------
 File Mods Finished
 ******************************





existe
-----------

Cuando el usuario necesita para comprobar la existencia de un archivo, el siguiente comando dado se ejecutará el proceso.

.. code-block:: bash

		ptconfigure file exists --filename="somename"

.. code-block:: bash

 kevell@corp:/# ptconfigure file exists --filename="somename"

 Enter File Path:
 /home/kevells/Desktop/somename
 File /home/kevells/Desktop/somename exists 
 ******************************


 File Modifications:
 --------------------------------------------

 File: Success

 ------------------------------
 File Mods Finished
 ******************************




anexar
------------

Cuando el usuario necesita para añadir una línea en un archivo, el comando a continuación se indica se ejecutará el proceso.

.. code-block:: bash
	
		ptconfigure file append --filename="somename" --line="a line"

* La opción de línea - puede insertar una línea que se adjunta

.. code-block:: bash

 kevell@corp:/# ptconfigure file append --filename="somename" --line="a line"

 Enter File Path:
 /home/kevells/Desktop/somename                             
 Enter the input for append:
 this is for test
 [Pharaoh Logging] [File] Reading File /home/kevells/Desktop/somename
 [Pharaoh Logging] [File] Writing File /home/kevells/Desktop/somename
 ******************************


 File Modifications:
 --------------------------------------------

 File: Success

 ------------------------------
 File Mods Finished
 ******************************




En caso de-tener-line
----------------------------

Cuando el usuario necesita para asegurarse de que un archivo contiene una línea particular, el siguiente comando dado se ejecutará el proceso.

.. code-block:: bash
	
		ptconfigure file should-have-line --filename="somename" --line="a line"

* Opción Línea - Declaración de que necesita ser comprobada

Opciones
------------

.. cssclass:: table-bordered

 +--------------------------+----------------------------------------------+
 | parámetros               | Parámetro Alternativa                        |
 +==========================+==============================================+
 |Ptconfigure file help     | Cualquiera de los dos parámetros alternativa | 
 |                          | se puede utilizar en el comando - File, file |
 |                          | por ejemplo: Ptconfigure File Install/       |
 |                          | Ptconfigure file Install|                    |
 +--------------------------+----------------------------------------------+


Beneficios
--------------

* Especifique un archivo con formato especial que contiene pruebas sensibles a la posición;  No se realizaron pruebas sensibles a la posición 
  por defecto y pruebas sensibles al contexto.
