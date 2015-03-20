==============
JUser
==============

sinopsis
-------------

Un usuario es una persona que utiliza un servicio de ordenador o red. Los usuarios generalmente usan un sistema o un producto de software sin los conocimientos técnicos necesarios para lo entender completamente.


A menudo un usuario tiene una cuenta de usuario y se identifica al sistema mediante un nombre de usuario (o nombre de usuario). Otros términos para username incluyen nombre de usuario, nombre de pantalla.


Cuenta de un usuario permite a los usuarios autenticarse en un sistema y que se conceda autorización para acceder a los recursos proporcionados por o conectado a ese sistema; Sin embargo, la autenticación no implica la autorización. Para iniciar sesión en una cuenta, un usuario es típicamente necesaria para autenticar a sí mismo con una contraseña u otras credenciales para los propósitos de la gestión de recursos, seguridad, registro y contabilidad.


comando Ayuda
----------------------

Este comando permite para determinar el uso del módulo Juser. El usuario llegará a conocer el diferente formas/formato para ejecutar este módulo. Este comando guía al usuario final para conocer el propósito de este comando. A continuación dado son el comando y la captura de pantalla del mismo.


.. code-block:: bash
        
	jrush juser help

.. code-block:: bash

 kevell@corp:/# jrush juser help
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

  This command allows you to update JUser.

  JUser, juser

        - delete
        Deletes a user
        example: jrush juser delete

        - info
        Display the details of a user
        example: jrush juser info

        - change the password of a user
        Change a users password
        example: jrush juser password

 ------------------------------
 End Help
 ****************************************




Delete
----------------

Cuando el usuario necesita borrar un usuario en la máquina, la continuación dado comando se ejecutará el proceso de instalación.


.. code-block:: bash
        
	jrush juser delete ..config file=”bootstrap file path”

La representación pictórica del comando anterior se enumera a continuación,


.. code-block:: bash

 kevell@corp:/# jrush juser delete --config-file="/var/www/html/joomla/configuration.php"
 Enter a JUser ID. To enter email/username use --user-email or --username parameters
 2
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 JUser Delete:
 -------------------------

 The following user has been deleted:

 User ID: 0
 Name: 
 User Name: 
 Email: 
 ------------------------------
 JUser Delete Finished
 ****************************************


Info
----------------

Cuando el usuario necesita mostrar los detalles de un usuario en la máquina, la continuación dado comando se ejecutará el proceso de instalación.


.. code-block:: bash
        
	jrush juser info ..config file=”bootstrap file path”

La representación pictórica del comando anterior se enumera a continuación,


.. code-block:: bash


 kevell@corp:/# jrush juser info --config-file="/var/www/html/joomla/configuration.php"
 Enter a JUser ID. To enter email/username use --user-email or --username parameters
 1
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 JUser Info:
 -------------------------
 
 User ID: 
 Name: 
 User Name: 
 Email: 

 ------------------------------
 JUser Info Finished
 ****************************************

Password
----------------

Cuando el usuario necesita cambiar la contraseña de un usuario en la máquina, la continuación dado comando se ejecutará el proceso de instalación.


.. code-block:: bash
        
	jrush juser password ..config file=”bootstrap file path”


parámetros alternativos
-----------------------------

Ninguno de los dos parámetros alternativos pueden utilizarse en comando-juser and JUser

eg: jrush juser info ..config file=”bootstrap file path” / jrush JUser info ..config file=”bootstrap file path”                            

.. code-block:: bash

 kevell@corp:/# jrush juser password --config-file="/var/www/html/joomla/configuration.php"
 Enter a JUser ID. To enter email/username use --user-email or --username parameters
 5
 Enter a new Password. To enter as parameter use --password 
 12345
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 JUser Password:
 -------------------------

 User ID: 0
 Name: 
 User Name: 
 Email: 
 User Password: NOT SET

 ------------------------------
 JUser Password Finished
 ****************************************


beneficios
--------------

* Fácil para obtener la información sobre un usuario utilizando un único comando 
* fácil de cambiar la contraseña de un usuario de back-end usando solo comando 
* fácil de manejar a cuentas de usuario

