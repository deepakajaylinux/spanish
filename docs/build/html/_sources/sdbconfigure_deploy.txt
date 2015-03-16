============
DBConfigure
============


sinopsis
-------------

Esta base de datos de los módulos de función apodos . Configuración se puede derivar de esta base de datos se puede colocar en el mismo conjunto como una base de datos derivada de DbContext para definir la configuración de Entity Framework para una aplicación. La configuración se realiza llamando a métodos protegidos y configuración de propiedades protegidas de esta base de datos en el constructor de tipo derivado de usuario. El tipo de uso también se pueden registrar en el archivo de configuración de la aplicación. Esto es suficiente con Ubuntu y CentOS .


comando Ayuda
-----------------------

El comando de ayuda guía al usuario para manejar la base de datos en ptdeploy . Este comando ayuda guía al usuario para crear un conf . Esto también restablecer la base de datos actual . Las bases de datos se utilizan para apoyar las operaciones internas de las organizaciones y de refuerzo de las interacciones en línea con clientes y proveedores . El comando de ayuda para dbconfigure se muestra a continuación .

.. code-block:: bash
	
	ptdeploy  DBConfigure help

Después de entradas el comando anterior, comienza a funcionar para manejar la base de datos . Es la catequesis de las funciones en las capturas de pantalla .

La siguiente captura de pantalla muestra sobre DBConfigure .


.. code-block:: bash

 kevell@corp:/# ptdeploy DBConfigure help
 ******************************


  This command is part of Default Modules and handles Databasing Functions.

  DBConfigure, db-configure, dbconfigure, db-conf

      - configure, conf
      set up db user & pw for a project, use admins to create new resources as needed.
      example: ptdeploy db-conf conf drupal
      example: ptdeploy db-conf conf --yes --platform=joomla30 --mysql-host=127.0.0.1 --mysql-admin-user="" --mysql-user="impi_dv_user" --mysql-pass="impi_dv_pass" --mysql-db="impi_dv_db"

      - reset
      reset current db to generic values so ptdeploy can write them. may need to be run before db conf.
      example: ptdeploy db-conf reset drupal
      example: ptdeploy db-conf reset --yes --platform=joomla30



parámetro Alternativa
-----------------------------------

Hay cuatro parámetros alternativos disponibles .

DBConfigure, db-configure, dbconfigure, db-conf.


Configurar, conf
-----------------------

Este proceso creó usuario de base de datos y passward para un proyecto. Utilice también administrador para crear nuevos recursos si necesitan . La siguiente captura de pantalla muestra su función.

.. code-block:: bash

      - configure, conf
      set up db user & pw for a project, use admins to create new resources as needed.
      example: ptdeploy db-conf conf drupal
      example: ptdeploy db-conf conf --yes --platform=joomla30 --mysql-host=127.0.0.1 --mysql-admin-user="" --mysql-user="impi_dv_user" --m	     ysql-pass="impi_dv_pass" --mysql-db="impi_dv_db"


El siguiente comando utiliza para configurar .

.. code-block:: bash

	ptdeploy  db-conf Conf

Después de clave en el por encima de dicho comando el siguiente proceso , puede ser ejercido . Se ha demostrado en las capturas de pantalla .

Después de la entrada como "Y" , Se pregunta MySql usuario admin , Mysql anfitrión, aplicación Db usuario , contraseña y aplicación db , nombre Db . El usuario introduce la entrada de éstos este proceso comenzará sus funciones

reajustar
-----------

Este proceso utiliza para restablecer la base de datos actual a los valores genéricos. En tales casos ptdeploy puede escribir antes de la configuración de base de datos de ejecución. El nombre de la base de datos se puede introducir en la misma línea de comandos.

El siguiente comando utiliza para reiniciar .

.. code-block:: bash

	ptdeploy  db-conf reset


La siguiente captura de pantalla muestra la función de este proceso.


.. code-block:: bash

      - reset
      reset current db to generic values so ptdeploy can write them. may need to be run before db conf.
      example: ptdeploy db-conf reset drupal
      example: ptdeploy db-conf reset --yes --platform=joomla30



opción
---------------

.. cssclass:: table-bordered

 +--------------------------------------+-------------------+-------------------------------------------------+
 | parámetros			        | opción	    | Comentarios			              |
 +======================================+===================+=================================================+
 |Do you want to configure a database?  | Yes		    | Configurado la base de datos undder ptdeploy.   |
 +--------------------------------------+-------------------+-------------------------------------------------+
 |Do you want to configure a database?	| No		    | Salga de la pantalla de configuración|	      |
 +--------------------------------------+-------------------+-------------------------------------------------+



Beneficios
--------------

* La configuración de base de datos Advantage es un alto rendimiento , bajo costo de mantenimiento , configuración de base de datos remoto  
  que permite al usuario construir fácilmente y desplegar aplicaciones cliente / servidor y aplicaciones basadas en la Web .
* Es fácil de usar con Ubuntu y CentOS .
* Sensitibilidad caso es un gran mérito de este módulo
* Es compatible con interfaces estándar como PHP
* Es fácil de manejar con funciones de base de datos
