================
MysqlAdmins
================

sinopsis
------------

Este módulo ayuda a la instalación y al igual que la gestión de los usuarios administradores de mysql sin usar usuario root. Mediante el uso de esto, los usuarios pueden gestionar sus funciones administrativas.

Ayuda Comando
--------------------

El comando Ayuda guía a los usuarios en relación con el comando utilizado para la instalación de los administradores de mysql, y también sus ventajas. El comando utilizado para la opción de ayuda en virtud de este mysql administradores se muestra a continuación.

.. code-block:: bash

	ptconfigure MysqlAdmins help

La captura de pantalla tal como se indica a continuación puede conducir al usuario en el manejo del comando de ayuda para los administradores de mysql.

.. code-block:: bash


 kevell@corp:/# ptconfigure MysqlAdmins help
 ******************************


  This command allows you to install admin users for MySQL so that MySQL can
  be managed without using the Root User.

  MysqlAdmins, mysql-admins, mysqladmins

        - install
        Installs Mysql Admin Users.
        example: ptconfigure mysql-admins install

 ------------------------------
 End Help
 ******************************

instalación
-------------

Instalación de los administradores de MySQL a su máquina facilita los usuarios especificar y gestionar sus actos administrativos. El comando que se utiliza para la instalación de los administradores mysql está marcado a continuación.

.. code-block:: bash

	ptconfigure MysqlAdmins install

Además, las siguientes operaciones que se muestran en un formato tabular se produce.

.. cssclass:: table-bordered

 +----------------------+----------------------------------------------+----------------+-------------------------------------------+ 
 | Parámetros           | Parámetro Alternativa                        | Opciones       | Comentarios                               |
 +======================+==============================================+================+===========================================+
 |Install Admin User    | En el lugar de MysqlAdmins estos nombres     | Y(Yes)         | Si el usuario desea continuar el proceso  |
 |for MySQL? (Y/N)      | alternativos se pueden utilizar:             |                | de instalación se puede introducir        |
 |                      | mysql-admins,mysqladmins.                    |                | como Y.                                   |
 +----------------------+----------------------------------------------+----------------+-------------------------------------------+
 |Install MySQL Server? | En el lugar de MysqlAdmins estos nombres     | N(No)          | Si el usuario desea abandonar el proceso  |
 |(Y/N)                 | alternativos se pueden utilizar:             |                | de instalación se puede introducir como   |
 |                      | mysql-admins,mysqladmins.                    |                | N.|                                       |
 +----------------------+----------------------------------------------+----------------+-------------------------------------------+

Si el usuario siga el proceso de instalación, se pueden enmarcar sus funciones administrativas mediante la especificación de las siguientes limitaciones.

* MySQL Usuario root
* MySQL Root Pass
* MySQL Nueva User Admin
* MySQL Nueva admin Pass

Si el usuario desea procesar instalación de los administradores de MySQL en un sistema remoto que puede especificar:

* Host MySQL.

La siguiente captura de pantalla le da una representación pictórica sobre el proceso de instalación como se describe anteriormente.

.. code-block:: bash


 kevell@corp:/# ptconfigure mysql-admins install
 Install Admin User for MySQL? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         MySQL Admins!        *
 *******************************
 Enter MySQL Root User:
 root
 Enter MySQL Root Pass:
 root123
 Enter MySQL New Admin User:
 kevells
 Enter MySQL New Admin Pass:
 kevells123
 Enter MySQL Host: Enter nothing for 127.0.0.1

 Creating /tmp/ptconfigure-temp-script-74285705785.sh
 chmod 755 /tmp/ptconfigure-temp-script-74285705785.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-74285705785.sh Permissions
 Executing /tmp/ptconfigure-temp-script-74285705785.sh
 ERROR 1045 (28000): Access denied for user 'root'@'localhost' (using password: YES)
 Temp File /tmp/ptconfigure-temp-script-74285705785.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 MysqlAdmins: Success
 ------------------------------
 Installer Finished
 ******************************

Beneficios
----------

* En el caso de los administradores de MySQL ya está instalado en la máquina de los usuarios, a continuación, un mensaje se aparecen para 
  informar a los usuarios, ya que ya está instalado.
* Mediante el uso de este módulo los administradores pueden gestionar sus acciones administrativas como por los requisitos.
* Pueden realizar el proceso de instalación, incluso en un sistema remoto.
* Sin el uso de los usuarios root, los usuarios pueden instalar los administradores mysql.


