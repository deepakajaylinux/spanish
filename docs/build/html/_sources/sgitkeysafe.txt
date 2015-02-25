============
GitKeySafe
============

sinopsis
-----------

Git caja fuerte de llaves que le ayuda a instala clave Git seguro. Esto permite que el permiso de una manera segura. Estos sistemas tienen la capacidad de los usuarios para acceder a la autorización del sistema de archivos. El permiso de lectura otorga la capacidad de leer un archivo. El permiso de escritura otorga la capacidad de modificar un archivo. El permiso de ejecución otorga la capacidad de ejecutar un archivo. Se consuela con Ubuntu y CentOS.

comando Ayuda
----------------------

El comando de ayuda conduce a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en los módulos Gitkeysafe. El comando help enumera los parámetros alternativos de Gitkeysafe bajo módulo ptconfigure. También se describe la sintaxis para la instalación de KeySafe del usuario. El comando de ayuda para Gitkeysafe se muestra a continuación.

.. code-block:: bash

		ptconfigure GitkeySafe help

La sintaxis para el comando de ayuda no entre mayúsculas y minúsculas, que añade una ventaja para este módulo. La siguiente captura de pantalla a visualizar al usuario sobre el comando de ayuda bajo la sintaxis para el comando de ayuda no entre mayúsculas y minúsculas, que añade una ventaja para este módulo. La siguiente captura de pantalla a visualizar al usuario sobre el comando de ayuda bajo gitkeysafe.

.. code-block:: bash

 kevell@corp:/# ptconfigure GitKeySafe help

 ******************************


  This module installs Git Key-Safe Server to the program git-key-safe

  GitKeySafe, git-key-safe, gitkeysafe

        - install
        Installs Git Key-Safe Server
        example: ptconfigure gitkeysafe install

        script example: git-safe-key -i /path/to/key clone http://git.com/repo.git

 ------------------------------
 End Help
 ******************************

instalación
---------------

Instalación implica típicamente código se copie / generada a partir de los archivos de instalación a los nuevos archivos en el equipo local para facilitar el acceso por el sistema operativo .. Su uso, el usuario tiene que asegurarse y tener una copia de seguridad, por lo que los datos del usuario siempre puede ser restaurado . El siguiente comando utiliza para instalar clave git seguro.

.. code-block:: bash

		ptconfigure gitkeysafe install

Durante la instalación de este módulo se apareció la siguiente captura de pantalla.

.. code-block:: bash

 kevell@corp:/# ptconfigure gitkeysafe install

 Install Git Key-Safe Server? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         Git Key-Safe Server!        *
 *******************************
 Git Key-Safe script /usr/bin/git-key-safe added
 Git Key-Safe script /usr/bin/git-key-safe permissions changed to 775
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 GitKeySafe: Success
 ------------------------------
 Installer Finished
 ******************************

opción
------------

.. cssclass:: table-bordered

 +-------------------------+-----------------------------------------+-------------+------------------------------------------+
 | Parámetros              | Parámetro Alternativa                   | Opciones    | Comentarios                              |
 +=========================+=========================================+=============+==========================================+
 |Install gitkeysafe       | En lugar de utilizar gitkeysafe podemos | Y(Yes)      | Se instala gitkeysafe bajo ptconfigure   |
 |                         | utilizar GitKeySafe,git-key-safe        |             |                                          |
 +-------------------------+-----------------------------------------+-------------+------------------------------------------+
 |Install gitkeysafe       | En lugar de utilizar gitkeysafe podemos | N(No)       | La salida de sistema de la instalación   |
 |                         | utilizar GitKeySafe,git-key-safe|       |             |                                          |
 +-------------------------+-----------------------------------------+-------------+------------------------------------------+


Beneficios
--------------

* Sensitibilidad caso
* Utiliza la instalación segura clave Git
* Ver el permiso del usuario
* Trabajar con Ubuntu y CentOS
* La seguridad es posible
