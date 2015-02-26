===============
Mysqlserver
===============

sinopsis
------------

Este módulo actúa como facilitador para instalar mysql-servidor con la versión actualizada a través de apt-get. Si el servidor mysql ya existe en su equipo, se comprueba la disponibilidad de módulo recién actualizado.

Ayuda Comando
---------------------

El comando help guía a los usuarios en cuanto a la metodología en uso y también acerca de las acciones que se pueden realizar en virtud de estos módulos. También describe los nombres alternativos para mysql-server. El comando para el uso de la opción de ayuda se da a continuación

.. code-block:: bash

	ptconfigure mysql-server help

Este comando hace que los usuarios sean conscientes de su propósito y también sobre el comando utilizado para instalar el servidor mysql.
La captura de pantalla que figura a continuación muestra un pictograma sobre el comando ayuda.

.. code-block:: bash


 kevell@corp:/# ptconfigure MysqlServer help
 ******************************


  This command allows you to install the MySQL Server. Currently only
  Mysql Workbench, the Database management GUI provided by Oracle for
  Mysql.

  MysqlServer, mysql-server, mysqlserver

        - install
        Install some Mysql Server Tools through apt-get.
        example: ptconfigure mysql-server install

  Notes, during mysql install a root password will be set. First, it'll look
  for the parameter --mysql-root-pass, if this is not set, it'll look in the
  ptconfigure config for a mysql-default-root-pass setting, and failing both of
  those it will just set the password for root to ptconfigure.

 ------------------------------
 End Help
 ******************************

instalación
------------

El comando utilizado para instalar el servidor MySQL es la siguiente.

.. code-block:: bash

	ptconfigure mysql-server install

Durante la instalación, se produce el siguiente proceso
----------------------------------------------------------------

* Este módulo ayuda a instalar algunas herramientas para el servidor MySQL a través de apt-get.
* Inicialmente una contraseña de root se establecerá.
* Durante la instalación, se buscará un parámetro de la raíz del pase --mysql.
* Si la raíz de paso --mysql no está disponible, buscará la config ptconfigure para la configuración de la raíz del pase-mysql por defecto.
* En el caso de los dos pasos mencionados anteriormente no se, se procederá al establecer contraseña de root para ptconfigure.

Opciones adicionales
--------------------------

Veamos acerca de las opciones adicionales que intervienen en la instalación del servidor mysql.

.. cssclass:: table-bordered

 +------------------------+--------------------------------------+------------+--------------------------------------+
 | Parámetros             | Parámetro Alternativa                | Opciones   | Comentarios                          |
 +========================+======================================+============+======================================+
 |Install MySQL Server?   | En el lugar del MySQL Server estos   | Y(Yes)     | Si el usuario desea continuar el     |
 |(Y/N)                   | nombres alternativos pueden ser      |            | proceso de instalación se puede      |
 |                        | utilizados: MySQLServer,             |            | introducir como Y.                   |
 |                        | mysql-server, mysqlserver.           |            |                                      |
 +------------------------+--------------------------------------+------------+--------------------------------------+
 |Install MySQL Server?   | En el lugar del MySQL Server estos   | N(No)      | Si el usuario desea abandonar el     |
 |(Y/N)                   | nombres alternativos pueden ser      |            | proceso de instalación se puede      |
 |                        | utilizados: MySQLServer,             |            | introducir como N.                   |
 |                        | mysql-server, mysqlserver.|          |            |                                      |
 +------------------------+--------------------------------------+------------+--------------------------------------+

La siguiente captura de pantalla le da una presentación gráfica sobre el proceso de instalación.

.. code-block:: bash

Si el servidor MySQL está ya existe en su máquina, entonces se lanza un mensaje al usuario, ya que ya está instalado. La siguiente captura de pantalla representa el proceso de garantizar:

.. code-block:: bash

Beneficios
------------

* Durante la instalación del servidor mysql, se instala con la versión actualizada.
* Asegura antes de instalar, y compruebe la disponibilidad de módulos.
* En el caso de los nuevos módulos incluidos en la versión actualizada, se instalará de forma individual el módulo que falta.
* Comprueba la disponibilidad de funciones de la biblioteca en el servidor mysql.
