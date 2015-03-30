=========
Minify
=========

Sinopsis
------------------

Minify es la eliminación de personajes innecesarios del código fuente. Mini, cuando se usa como prefijo, significa pequeño. El objetivo de minify es hacer que el código fuente "más pequeño" y mejorar el rendimiento.

El término minify se asocia a menudo con los lenguajes de secuencias de comandos interpretado, como php, que se despliegan y se transmiten a través de Internet. Código que ha sido minified mediante la sustitución de carreras de espacios por un solo espacio, por ejemplo, es más ligera y requiere menos tiempo para un navegador para cargar. Herramientas populares minify para el desarrollo Web incluyen compresor, y ubuntu Compiler. Minify adapte a trabajar con Ubuntu y CentOS.

Comando Ayuda
-----------------------
Minify hace que el desarrollo conjunto de una brisa: Conceptualmente, minify es similar a la compresión. A diferencia de código que ha sido comprimido, sin embargo, el código que ha minified todavía puede ser trabajado con sin requerir el paso adicional de descompresión. Código fuente Minified también puede ser utilizado como una especie de ofuscación, aunque el término ofuscación se puede distinguir como una forma de falsa criptografía mientras que un ejemplo de código minified puede invertirse utilizando una bonita-impresora.

El siguiente comando ayuda guía al usuario para manejar minify.

.. code-block:: bash

                ptconfigure minify help

Esta captura de pantalla muestra el uso del comando ayuda

.. code-block:: bash

 kevell@corp:/# ptconfigure minify help

 ******************************


  This command allows you to update Minify.

  Minify, minify

        - install
        Installs the latest version of minify
        example: ptconfigure minify install

 ------------------------------
 End Help
 ******************************

instalación
------------------

Funciona con las convenciones existentes para la estructura del código, añadiendo herramientas eficaces para apoyar el ciclo de desarrollo de codificación. Con minify, el desarrollo de una codificación se hace tan fácil que será el diseño predeterminado de usuario cada vez que el usuario está escribiendo una cantidad significativa de código. Este comando se utiliza para instalar minify es la siguiente,

.. code-block:: bash

                ptconfigure minify install

La siguiente captura de pantalla y lo explica.

.. code-block:: bash



 kevell@corp:/# ptconfigure minify install 
 Install Minify? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         Minify!        * 
 ******************************* 
 Reading package lists... 
 Building dependency tree... 
 Reading state information... 
 The following packages were automatically installed and are no longer required: 
  libmemcached10 pear-channels php5-xdebug 
 Use 'apt-get autoremove' to remove them. 
 The following extra packages will be installed: 
  java-wrappers libjargs-java 
 Suggested packages: 
  libjargs-java-doc 
 The following NEW packages will be installed: 
  java-wrappers libjargs-java yui-compressor 
 0 upgraded, 3 newly installed, 0 to remove and 34 not upgraded. 
 Need to get 587 kB of archives. 
 After this operation, 776 kB of additional disk space will be used. 
 Get:1 http://archive.ubuntu.com/ubuntu/ trusty/main java-wrappers all 0.1.27 [9,908 B] 
 Get:2 http://archive.ubuntu.com/ubuntu/ trusty/main libjargs-java all 1.0.0-4 [14.3 kB] 
 Get:3 http://archive.ubuntu.com/ubuntu/ trusty/main yui-compressor all 2.4.7-1 [563 kB] 
 Fetched 587 kB in 41s (14.2 kB/s) 
 Selecting previously unselected package java-wrappers. 
 (Reading database ... 362717 files and directories currently installed.) 
 Preparing to unpack .../java-wrappers_0.1.27_all.deb ... 
 Unpacking java-wrappers (0.1.27) ... 
 Selecting previously unselected package libjargs-java. 
 Preparing to unpack .../libjargs-java_1.0.0-4_all.deb ... 
 Unpacking libjargs-java (1.0.0-4) ... 
 Selecting previously unselected package yui-compressor. 
 Preparing to unpack .../yui-compressor_2.4.7-1_all.deb ... 
 Unpacking yui-compressor (2.4.7-1) ... 
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ... 
 Setting up java-wrappers (0.1.27) ... 
 Setting up libjargs-java (1.0.0-4) ... 
 Setting up yui-compressor (2.4.7-1) ... 
 [Pharaoh Logging] Adding Package yui-compressor from the Packager Apt executed correctly 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 


 Single App Installer: 
 -------------------------------------------- 
 Minify: Success 
 ------------------------------ 
 Installer Finished 
 ****************************** 

opción
----------

Código fuente Minify es especialmente útil para lenguajes interpretados desplegados y transmitidos en Internet, ya que reduce la cantidad de datos que necesita ser transferido.

.. cssclass:: table-bordered

 +----------------------+---------------------------------+-------------+-----------------------------------------+
 | Parámetros           | Parámetro Alternativa           | Opciones    | Comentarios                             |
 +======================+=================================+=============+=========================================+
 |Install minify?(Y/N)  | En lugar de utilizar minify     | Y(Yes)      | Se instala minify bajo ptconfigure      |
 |                      | podemos utilizar Minify         |             |                                         |
 +----------------------+---------------------------------+-------------+-----------------------------------------+
 |Install minify?(Y/N)  | En lugar de utilizar minify     | N(No)       | La salida de sistema de la instalación  |
 |                      | podemos utilizar Minify|        |             |                                         |
 +----------------------+---------------------------------+-------------+-----------------------------------------+

		
Beneficios
-------------

* Minimizar comunica a través de la codificación de PHP.
* Minimizar consuela con Ubuntu y CentOS.
* Minimizar apoya sensibilidad no caso.
* Minimizar descuenta caracteres innecesarios desde el código fuente.
