======
Xvfb
======

sinopsis
------------

Este módulo facilita en la instalación del XVFB, que se conoce como solución de máquina virtual popular. El módulo proporciona una solución para trabajar en una máquina virtual. XVFB conocida como memoria intermedia de trama virtual X es un servidor de pantalla que implementa el protocolo servidor X11. En contraste con otros servidores de visualización Xvfb realiza todas las operaciones gráficas en la memoria sin mostrar ninguna salida de pantalla. Veamos cómo este módulo ayuda a instalar el XVFB través de apt-get.

Ayuda Comando
--------------------

El comando help guía a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en el módulo XVFB. Las listas de comandos de ayuda fuera de los parámetros alternativos de módulo XVFB. También describe la sintaxis para instalar módulo XVFB El comando de ayuda para el módulo XVFB se muestra a continuación.

.. code-block:: bash

		ptconfigure Xvfb help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda bajo módulo XVFB.

.. code-block:: bash

 kevell@corp:/# ptconfigure Xvfb help
 ******************************


  This command allows you to install Xvfb, the popular Virtual Machine Solution.

  Xvfb, xvfb

        - install
        Installs Xvfb through apt-get
        example: ptconfigure xvfb install

 ------------------------------
 End Help
 ******************************



instalación
----------------

El comando utilizado para instalar el XVFB a la máquina de los usuarios se muestra a continuación.

.. code-block:: bash

		ptconfigure xvfb install

Después de introducir el comando anterior, las siguientes operaciones se produce como se muestra en el formato tabular.

.. cssclass:: table-bordered

 +--------------------------+---------------------------------------+-----------+--------------------------------------------------+
 | Parámetros               | Parámetro Alternativa                 | Opciones  | Comentarios                                      |
 +==========================+=======================================+===========+==================================================+
 |Install Xvfb? (Y/N)	    | En lugar de utilizar Xvfb, el usuario | Y(Yes)    | Si el usuario desea continuar el proceso de      |
 |                          | puede utilizar xvfb.                  |           | instalación se puede introducir como Y.          |
 +--------------------------+---------------------------------------+-----------+--------------------------------------------------+
 |Install Xvfb? (Y/N)	    | En lugar de utilizar Xvfb, el usuario | N(No)     | Si el usuario desea abandonar el proceso de      |
 |                          | puede utilizar xvfb.                  |           | instalación se puede introducir como N.|         |
 +--------------------------+---------------------------------------+-----------+--------------------------------------------------+


Si el usuario continúa el proceso de instalación, durante la ejecución de la instalación produce el siguiente proceso:

* Lee las listas de paquetes.
* Construye el árbol de dependencias.
* Lee la información de estado.
* Lista de nuevos paquetes instalados.
* Número de archivos actualizados, recién instalados, retirados, sin actualizar.

Por último, la situación se informó claramente y añadiendo paquete XVFB del empaquetador Apt se ejecutan correctamente. La siguiente captura de pantalla que muestra sobre el proceso de instalación de XVFB.

Si el módulo XVFB ya existe en la máquina de los usuarios, se mostrará un mensaje como el XVFB paquete del empaquetador Apt ya está instalado. La captura de pantalla de la siguiente es un buen ejemplo de ese tipo de mensajes.

.. code-block:: bash

 kevell@corp:/# ptconfigure xvfb install
 Install Xvfb? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *          ! Xvfb !        *
 *******************************
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following NEW packages will be installed:
  xvfb
 0 upgraded, 1 newly installed, 0 to remove and 8 not upgraded.
 Need to get 747 kB of archives.
 After this operation, 2,191 kB of additional disk space will be used.
 Get:1 http://in.archive.ubuntu.com/ubuntu/ trusty-updates/main xvfb amd64 2:1.15.1-0ubuntu2.6 [747 kB]
 Fetched 747 kB in 36s (20.6 kB/s)
 Selecting previously unselected package xvfb.
 (Reading database ... 211203 files and directories currently installed.)
 Preparing to unpack .../xvfb_2%3a1.15.1-0ubuntu2.6_amd64.deb ...
 Unpacking xvfb (2:1.15.1-0ubuntu2.6) ...
 Processing triggers for man-db (2.6.7.1-1ubuntu1) ...
 Setting up xvfb (2:1.15.1-0ubuntu2.6) ...
 [Pharaoh Logging] Adding Package xvfb from the Packager Apt executed correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Xvfb: Success
 ------------------------------
 Installer Finished
 ******************************





Beneficios
-----------

* Los parámetros utilizados para la declaración de la ayuda de mandatos, la instalación no son sensibles, que es una ventaja añadida, mientras 
  que en comparación con otros.
* Es-acomodados tanto en OS Cent y así como en Ubuntu.
* Si el paquete XVFB ya existe en la máquina del usuario, lo hará no sobrescribe, en lugar de que se mostrará un mensaje que ya existen.

Xvfb se utiliza principalmente para la prueba:

* Dado que comparte código con el servidor real X, que puede ser utilizado para probar las partes del código que no están relacionados con el 
  hardware específico.
* Puede ser utilizado para probar los clientes en diversas condiciones que de otro modo requerirían una gama de hardware diferente; por ejemplo,  puede ser utilizado para probar si los clientes funcionan correctamente a profundidades o tamaños de pantalla que rara vez son compatibles 
  con el hardware.
* Antecedentes funcionamiento de los clientes. (El programa xwd o un programa similar para capturar una captura de pantalla se pueden utilizar 
  para ver realmente el resultado)
* Ejecución de programas que requieren un servidor X para estar activo incluso cuando no se utilizan. (por ejemplo, informes HTML trébol)
