============
PHPEclipse
============

Sinopsis
-------------

PHPEclipse es un conjunto de plug-ins para el Marco de Eclipse que proporciona IDE integrado para desarrolladores de PHP. Eclipse y PHPEclipse están escritos en Java, y se ejecutarán en todos los entornos de escritorio gráficos. PHPEclipse es un software de código abierto, disponible libremente bajo la Licencia Pública Común.

La plataforma Eclipse proporciona a los usuarios un paradigma de interfaz de usuario consistente. Un IDE de desarrollo de software es una de las aplicaciones de escritorio más complejas mayoría de nosotros estamos propensos a usar, por lo que el tiempo necesario para que un desarrollador para convertirse eficiente con un IDE particular puede ser significativo. Eclipse no reduce este tiempo, pero proporciona un enfoque interfaz consistente que sólo necesitan ser aprendidas una vez con el fin de desarrollar de manera eficiente con una amplia gama de lenguajes y herramientas de programación. Como parte de este enfoque, Eclipse proporciona documentación detallada y tutoriales sobre todas sus funcionalidades genéricas, permitiendo proyectos de plugins, como PHPEclipse, centrarse sólo en sus áreas específicas de su dominio. Al aprender a utilizar Eclipse como plataforma de desarrollo, o aprender a desarrollar sus propias herramientas de plug-in para Eclipse, que está adquiriendo una habilidad útil y flexible.

Ayuda Comando
----------------------

Este comando ayuda a determinar el uso del módulo PHPEclipse. El usuario se llega a saber acerca de la diferente forma / formato de ejecutar este módulo. Este comando guía al usuario final a conocer el propósito de este comando. A continuación dado son el mando y la pantalla del mismo.

.. code-block:: bash
        
	        ptconfigure PHPeclipse help

La representación gráfica de la orden anterior se muestra a continuación,

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPEclipse help

 ******************************


  This command allows you to update PHPEclipse.

  phpeclipse, PHPEclipse, PHP-Eclipse

        - install
        Installs the latest version of PHPEclipse
        example: ptconfigure phpeclipse install

 ------------------------------
 End Help
 ******************************

instalación
----------------

Este comando ayuda en la instalación de la última versión de PHPEclipse en el sistema. El siguiente comando dado se ejecutará el proceso de instalación.

.. code-block:: bash
        
	        ptconfigure PHPEclipse install


Opciones
-----------

.. cssclass:: table-bordered

 +------------------------+-------------------------------------------------------+-------------+--------------------------------------+
 | Parámetros             | Parámetro Alternativa                                 | Opciones    | Comentarios                          |
 +========================+=======================================================+=============+======================================+
 |ptconfigure PHPEclipse  | Hay tres parámetros alternativos que pueden ser       | Y(Yes)      | El sistema se inicia proceso de      |
 |Install? (Y/N)          | utilizados en la línea de comandos. PHP-Eclipse,      |             | instalación                          |
 |                        | PHPEclipse, phpeclipse Por ejemplo: ptconfigure       |             |                                      |
 |                        | PHPEclipse install, ptconfigure PHP-Eclipse install   |             |                                      |
 +------------------------+-------------------------------------------------------+-------------+--------------------------------------+
 |ptconfigure PHPEclipse  | Hay tres parámetros alternativos que pueden ser       | N(No)       | El sistema detiene proceso de        |
 |Install? (Y/N)          | utilizados en la línea de comandos. PHP-Eclipse,      |             | instalación                          |
 |                        | PHPEclipse, phpeclipse Por ejemplo: ptconfigure       |             |                                      |
 |                        | PHPEclipse install, ptconfigure PHP-Eclipse install|  |             |                                      |
 +------------------------+-------------------------------------------------------+-------------+--------------------------------------+


Beneficios
--------------

* PHP, HTML, XML y CSS resaltado de sintaxis
* Finalización de código
* Navegador web integrado vista previa
* El control integrado de servidores Apache y MySQL
