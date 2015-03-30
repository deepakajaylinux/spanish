===============
Appsettings
===============

sinopsis
-----------------

AppSetting que nos permite mantener la configuración de ancho configurables y de aplicación que una aplicación requiere con el fin de realizar las tareas correctamente. Esto ayuda a facilitar el mantenimiento y despliegue de la aplicación. Mediante el uso de appSetting podemos definir los valores definidos por el usuario .


comando Ayuda
------------------

Este comando ayuda a determinar el uso de appsettings . En él se enumeran los parámetros y sintaxis alternativas para el funcionamiento de appsettings módulo. El comando de ayuda para appsettings se muestra a continuación .


.. code-block:: bash

	ptdeploy appsettings help

La representación gráfica del comando de ayuda se da a continuación ,


.. code-block:: bash


 kevell@corp:/# ptdeploy appsettings help

 ******************************


  This command is part of Default Modules and provides you  with a method by which you can configure Application Settings.
  You can configure default application settings, ie: mysql admin user, host, pass

  AppSettings, appsettings
	
        - set
        Set a configuration value
        example: ptdeploy appsettings set

        - get
        Get the value of a setting you have configured
        example: ptdeploy appsettings get

        - delete
        Delete a setting you have configured
        example: ptdeploy appsettings delete

        - list
        Display a list of all default available settings
        example: ptdeploy appsettings list

 ------------------------------
 End Help
 ******************************


Set
---------

El comando set ayuda para establecer un valor de configuración. El siguiente comando se ejecutará el proceso.

.. code-block:: bash

	ptdeploy appsettings set

La representación gráfica de la orden anterior se enumeran a continuación ,



.. code-block:: bash

 kevell@corp:/# ptdeploy appsettings set

 Do you want to Configure Application Settings? (Y/N) 
 y
 What's the App Config Variable?

 (0) **ENTER PLAIN TEXT** 
 (1) mysql-admin-user 
 (2) mysql-admin-host 
 (3) mysql-admin-pass 
 (4) linux-user 
 (5) linux-user-dir 
 (6) program-dir 
 (7) temp-base-dir 
 (8) distro 
 (9) op-sys 
 (10) linux-type 
 5
 What Value do you want to give this variable?
 /tmp/
 ******************************

 Seems Fine...
 In Application Config
 ******************************


Get
--------

El comando Get ayuda a obtener el valor de un ajuste que ya ha configurado . El siguiente comando se ejecutará el proceso.


.. code-block:: bash

	ptdeploy appsettings get


La representación gráfica de la orden anterior se enumeran a continuación ,

.. code-block:: bash

 kevell@corp:/# ptdeploy appsettings get

 Do you want to Configure Application Settings? (Y/N) 
 y
 What's the App Config Variable?

 (0) **ENTER PLAIN TEXT** 
 (1) mysql-admin-user 
 (2) mysql-admin-host 
 (3) mysql-admin-pass 
 (4) linux-user 
 (5) linux-user-dir 
 (6) program-dir 
 (7) temp-base-dir 
 (8) distro 
 (9) op-sys 
 (10) linux-type 
 4
 ******************************


 Variable Name: linux-user
 Variable Value: karuna
 
 In Application Config
 ******************************


Delete
--------

El comando delete ayuda a eliminar un ajuste que ha configurado. El siguiente comando se ejecutará el proceso.

.. code-block:: bash

	ptdeploy appsettings delete

La representación gráfica de la orden anterior se enumeran a continuación ,

.. code-block:: bash


 kevell@corp:/# ptdeploy appsettings delete

 Do you want to Configure Application Settings? (Y/N) 
 y
 What's the App Config Variable?

 (0) **ENTER PLAIN TEXT** 
 (1) mysql-admin-user 
 (2) mysql-admin-host 
 (3) mysql-admin-pass 
 (4) linux-user 
 (5) linux-user-dir 
 (6) program-dir 
 (7) temp-base-dir 
 (8) distro 
 (9) op-sys 
 (10) linux-type 
 5
 ******************************


 Seems Fine...
 In Application Config
 ******************************



List
-------

El comando lista ayuda a mostrar una lista de todos los valores predeterminados disponibles . El commad continuación se ejecutará el proceso.


.. code-block:: bash

	ptdeploy appsettings list

La representación gráfica de la orden anterior se enumeran a continuación ,


.. code-block:: bash

 kevell@corp:/# ptdeploy appsettings list

 Do you want to Configure Application Settings? (Y/N) 
 y
 ******************************


 Variable Type is: allSet 
   linux-user is: karuna 
   mysql-admin-user is: mani 
 Variable Type is: allTotal 
   mysql-admin-user 
   mysql-admin-host 
   mysql-admin-pass 
   linux-user 
   linux-user-dir 
   program-dir 
   temp-base-dir 
   distro 
   op-sys 
   linux-type 

 In Application Config
 ******************************



parámetros alternativos
--------------------------

Hay dos parámetros alternativos que pueden ser utilizados en la línea de comandos .

AppSettings, appsettings


Beneficios
-----------

* Acceso fuertemente tipado
* Sensitibilidad caso


