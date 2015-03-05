=================
PHPStorm
=================

sinopsis
----------------

PhpStorm mantiene al día con las últimas tendencias de PHP y ptconfigure, integra una variedad de herramientas modernas, y trae aún más extensibilidad con el apoyo de los principales frameworks PHP. Entorno de desarrollo de configuración automática (estándar de codificación, las asociaciones de archivos, etc.) es posible. Es cómodo con Ubuntu y CentOS.

Ayuda Comando
------------------------

Este comando puede funcionar sobre los objetivos y los comandos disponibles bajo módulo tormenta ptconfigure Php. También explica el comando para instalar el módulo tormenta Php. Antes de la instalación, el usuario puede leer este comando de ayuda explica su función.

.. code-block:: bash
   
	       ptconfigure PHPStorm help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda bajo PHP Storm.

.. code-block:: bash


 kevell@corp:/# ptconfigure PHPStorm help
 ******************************


  This command allows you to install Intellij, the JetBrains IDE

  PHPStorm, phpstorm

        - install
        Installs the latest version of Developer Tools
        example: ptconfigure gittools install

 ------------------------------
 End Help
 ******************************

instalación
------------------

Si el usuario desea instalar herramientas de git para su máquina, pueden utilizar el comando como se indica a continuación,

.. code-block:: bash

	ptconfigure gittools install

Después de introducir el comando anterior, los siguientes pasos son involucrados durante el proceso de instalación como se describe en la tabla,

.. cssclass:: table-bordered


 +--------------------------+-------------------------------------+-----------+-----------------------------------------------+
 | Parámetros               | Parámetro Alternativa               | Opciones  | Comentarios                                   |
 +==========================+=====================================+===========+===============================================+
 |Install Git Tools? (Y/N)  | En lugar de utilizar PhpStorm       | Y(Yes)    | Si el usuario desea continuar el proceso de   |
 |                          | Podemos utilizar phpstorm           |           | instalación se puede introducir como Y.       |
 +--------------------------+-------------------------------------+-----------+-----------------------------------------------+
 |Install Git Tools? (Y/N)  | En lugar de utilizar PhpStorm       | N(No)     | Si el usuario desea abandonar el proceso de   |
 |                          | Podemos utilizar phpstorm           |           | instalación se puede introducir como N.|      |
 +--------------------------+-------------------------------------+-----------+-----------------------------------------------+


La siguiente captura de pantalla representa gráficamente el proceso anteriormente descrito de la instalación.

.. code-block:: bash

 
 kevell@corp:/# ptconfigure gittools install
 Install Git Tools? (Y/N)
 Y
 *******************************
 *        Pharaoh Tools        *
 *         !Git Tools!!        *
 *******************************
 [Pharaoh Logging] Package git from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package git-core from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package gitk from the Packager Apt is already installed, so not installing
 [Pharaoh Logging] Package git-cola from the Packager Apt is already installed, so not installing
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 GitTools: Success
 ------------------------------
 Installer Finished
 ******************************

Beneficios
-------------------

* Más ajustes para mantener el código tan limpio como sea posible
* Mejor interfaz con el entorno de desarrollo de configuración automática.
* Mejores sugerencias de código y depuración
* Codificación Zen está disponible con DevOps.
* Múltiples cursores y atajos de teclado simples para crear, editar y navegar entre las cuestiones.
* Más atributos personalizados, flujos de trabajo personalizados y de gran alcance de personalización.
* Se utiliza para instalar la última versión de las herramientas para desarrolladores.

