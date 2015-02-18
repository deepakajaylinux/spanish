======
Copy
======

sinopsis
-------------
Copy es la orden introducida en un shell de Linux para copiar un archivo de un lugar a otro, posiblemente en un sistema de archivos diferente. El archivo original se mantiene sin cambios, y el nuevo archivo puede tener el mismo o un nombre diferente. Copiar es el comando que hace una copia de sus archivos o directorios.

Las formas archivos se copian en Linux dependen de su distribución y sistema de archivos. Todas las versiones de Linux pueden copiar archivos desde la línea de comandos. También hay una serie de administradores de archivos tanto de texto basado en GUI y que podría ser utilizado.
Por ejemplo, digamos que usted tiene un archivo denominado imagen.jpg en su directorio de trabajo, y que desea hacer una copia de la misma llama foto-02.jpg. Usted tendría que ejecutar el comando y el archivo se copiará. Aquí, picture.jpg es la fuente de la operación de copia y la imagen-02.jpg es el destino. Ambos archivos existen ahora en su directorio de trabajo.

Los archivos de origen y de destino también pueden residir en diferentes directorios. Por ejemplo, hacer una copia de la /home/chuck/pictures/picture.jpg archivo en el directorio / home / chuck / backup. El archivo de destino también será nombrado imagen.jpg.

Ayuda Comando
----------------------

Este comando ayuda a determinar el uso del módulo de copia. El usuario se llega a saber acerca de la diferente forma / formato de ejecutar este módulo. Este comando guía al usuario final a conocer el propósito de este comando. A continuación dado son el mando y la pantalla del mismo.

.. code-block:: bash
        
	        cleopatra copy help

La representación gráfica del comando de copia de pantalla aparece a continuación,

.. code-block:: bash

 kevell@corp:/# cleopatra copy help
 ******************************


  This command handles file copying functions.

  Copy, copy

        - put
        Will ask you for details for servers, then copy a file or directory from local to remote
        example: cleopatra copy put
        example: cleopatra copy put --yes --source="/tmp/file" --target="/home/user/file"

 ------------------------------
 End Help
 ******************************

poner
--------

Cuando el usuario necesita para copiar un archivo en nuestra fuente a otro destino, el comando a continuación se indica se ejecutará el proceso.

.. code-block:: bash
        
	        cleopatra copy put

El sistema pide la ruta del archivo de origen y la ruta del archivo de destino.

.. code-block:: bash


 kevell@corp:/# cleopatra copy put
 Copy files? (Y/N) 
 Y
 Enter source file path
 /kevell.html
 Enter target file path
 /home/desktop
 [Pharaoh Logging] [Copy] Executing cp -r /kevell.html /home/desktop
 ******************************


 Copy Result: Success
 ------------------------------
 Copy Finished
 ******************************

Hay otra opción, en la que se puede dar la ruta de origen y de destino en la línea de commandos.

.. code-block:: bash

 kevell@corp:/# cleopatra copy put --yes --source="/kevell.html" --target="/opt"
 [Pharaoh Logging] [Copy] Executing cp -r /kevell.html /opt
 ******************************


 Copy Result: Success
 ------------------------------
 Copy Finished
 ******************************

Parámetro Alternativa
--------------------------------

Hay dos parámetros alternativa que se puede utilizar en la línea de commandos.

Copy , copy.

Por ejemplo: cleopatra copy put/ cleopatra Copy help


Beneficios
---------------

* Este comando ayuda a hacer una copia de sus archivos o directorios.
* Copia de un archivo o directorio desde el origen al destino utilizando solo comando
* Si desea copiar un archivo de una carpeta a otra con el mismo nombre, sólo el nombre del directorio de destino es lo suficientemente bueno
* Un directorio (y todo su contenido) se pueden copiar desde el origen al destino con la opción recursiva -r

