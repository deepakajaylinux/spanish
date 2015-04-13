=======
SVN
=======


sinopsis
------------

Este módulo ayuda a los usuarios en el manejo de las funciones de comprobación. Apache Subversion (SVN a menudo abreviado, después el comando nombre svn) es un software versionado y revisión sistema de control distribuido como software libre bajo la licencia Apache.[1] los desarrolladores usar Subversion para mantener versiones actuales e históricas de los archivos como código fuente, documentación y páginas web. Su objetivo es ser un sucesor en su mayoría compatible para el sistema ampliamente utilizado de versiones concurrentes (CVS). Veamos cómo este módulo facilita en el manejo de las funciones de comprobación.


comando Ayuda
---------------------

El comando ayuda guía a los usuarios sobre la finalidad y así como sobre las opciones que se incluyen en el SVN. Enumera los parámetros alternativos de SVN. También describe la sintaxis para utilizar las funciones de comprobación. El comando de ayuda para el módulo SVN se muestra a continuación.

.. code-block:: bash

	ptdeploy svn help

La sintaxis para declarar el comando help no es sensible a mayúsculas que es una ventaja añadida. La siguiente pantalla te visualizar sobre el comando ayuda bajo SVN.



.. code-block:: bash

 kevell@corp:/# ptdeploy svn help
 ******************************


  This command is part of Default Modules and handles Checkout Functions.

  Checkout, checkout, co

          - perform a checkout into configured projects folder. If you don't want to specify target dir but do want
          to specify a branch, then enter the text "none" as that parameter.
          example: ptdeploy svn co https://svnhub.com/phpengine/yourmum {optional target dir} {optional branch}
          example: ptdeploy svn co https://svnhub.com/phpengine/yourmum none {optional branch}

 ------------------------------
 End Help
 ******************************

Cómo utilizar las funciones de pago y envío
-------------------------------------------

La sintaxis para utilizar el check-out funciones bajo svn se expone a continuación.


.. code-block:: bash

	ptdeploy svn co https: // svnhub.com/ phpengine/yourmum



Después de introducir el mandato dado por encima, la ejecución de la función de comprobación comienza como se describe en la tabla, abajo




.. cssclass:: table-bordered

 +----------------------------+----------------------------------------+------------------+-------------------------------------------+
 | parámetros		      | parámetros alternativos		       | opciones         | comentarios                               |
 +============================+========================================+==================+===========================================+
 |Perform a clone/download    | En lugar de co , podemos utilizar la   | Y(Yes)		  | Si el usuario necesita para llevar a cabo |
 |of files? (Y/N)             | salida, Checkout también .             | 		  | un clon / descarga de los archivos        |
 |                            |                                        |                  | se puede introducir como Y.               |
 +----------------------------+----------------------------------------+------------------+-------------------------------------------+
 |Perform a clone/download    | En lugar de co , podemos utilizar la   | N(No)            | Si el usuario no está en la necesidad de  |
 |of files? (Y/N)             | salida, Checkout también .             |                  | realizar un clon / descarga de los        |
 |			      |					       |		  | archivos se puede introducir como N.|     |	
 +----------------------------+----------------------------------------+------------------+-------------------------------------------+

Si el usuario procede la función de verificación de entrada y, están involucrados los siguientes pasos como se describe a continuación.


Step 1:

Also change permissions/owner? (Y/N)

El usuario tiene que entrar como Y o N dependiendo de su voluntad de cambiar permisos y propietario.


Step 2:

What user is Apache Web Server running as?

El usuario tiene que introducir el nombre del usuario que ejecuta el servidor web apache.

Step 3:

Involucra el proceso de cambiar los permisos de la carpeta y propietario de la carpeta.

La captura de pantalla siguiente muestra gráficamente acerca del proceso y el trabajo de revisar las funciones.



.. code-block:: bash


 kevell@corp:/# ptdeploy  svn co --repository-url="http://core.svn.wordpress.org/trunk" --custom-clone-dir="/opt/"
 Perform a clone/download of files? (Y/N) 
 y
 Also change permissions/owner? (Y/N) 
 n
 View Template SvnView.tpl.php for  Not Found



Beneficios
-----------

* Es acomodada en ambos ubuntu y así como ciento OS. 
* Los parámetros utilizados en la declaración no es sensible a mayúsculas. 
* El usuario puede realizar y supervisar las funciones de comprobación utilizando este SVN.


