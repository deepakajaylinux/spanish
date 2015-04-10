====================
EnvironmentConfig
====================

sinopsis
-------------

Este módulo facilita a los usuarios en la configuración de su entorno necesario para su proyecto. Veamos cómo configurar el entorno, cómo eliminar el medio ambiente no deseado, cómo utilizar la opción de lista para mostrar los entornos disponibles en los próximos temas.

comando Ayuda
--------------------

El comando de ayuda guía a los usuarios en cuanto a la finalidad del módulo, sus parámetros alternativos que se utilizan en la declaración. En él se destacan las tres funciones de configuración del entorno que son lista, configurar, borrar. También especifica la sintaxis para utilizar tres funciones principales. La sintaxis utilizada para declarar la ayuda se muestra a continuación:

.. code-block:: bash

		ptdeploy envconfig help

La siguiente captura de pantalla muestra gráficamente sobre el funcionamiento de comando ayuda.

.. code-block:: bash

 kevell@corp:/# ptdeploy EnvironmentConfig help
 **************************************************

  This command is part of a default Module and provides you with a method by which you can
  configure environments for your project from the command line. Currently compliant with
  both ptdeploy and ptconfigure.


  EnvironmentConfig, environmentconfig, environment-config, envconfig, env-config

        - list
        List current environments
        example: ptdeploy envconfig list --yes

        - configure, config
        Configure the environments for your project to use
        example: ptdeploy envconfig config
        example: ptdeploy envconfig config --keep-current-environments

        - delete, del
        Configure the environments for your project to use
        example: ptdeploy envconfig delete
        example: ptdeploy envconfig del --environment-name="staging"

 ------------------------------
 End Help
 ******************************


Cómo configurar el entorno
----------------------------------------------

A los efectos de la configuración de los ambientes, el usuario puede utilizar el siguiente comando:

.. code-block:: bash

		ptdeploy envconfig config

Después de introducir el comando anterior las siguientes operaciones se lleva a cabo como se muestra:
Paso 1: Configure Environments Here? (Y/N)

El usuario tiene a la entrada de S o N.

Paso 2: Use existing environment Settings? (Y/N)

El usuario tiene a la entrada de S o N.

Si la entrada del usuario como Y se procederá con ya existente.

Si de entrada como N, lo hará pide información sobre el medio ambiente como

Value for: Name of the environment

Value for: Default temp dir(Location)

Después de los pasos anteriores, el usuario tiene que introducir los siguientes detalles:

Enter target?

Enter user?

Enter password?

Add Another Server? (Y/N)

El usuario tiene a la entrada de S o N.

Por último, la configuración del entorno consigue el éxito como se muestra en la siguiente captura de pantalla.

.. code-block:: bash


 kevell@corp:/# ptdeploy envconfig config

 Configure Environments Here? (Y/N) 
 y
 Do you want to add another environment? (Y/N) 
 y
 Environment 3  : 
 Default Settings for Any App not setup for environment  enter them now.
 Value for: Name of this Environment
 deepak
 Value for: Default Temp Dir (should usually be /tmp/)
 /tmp/
 Enter Servers - this is an array of entries
 Enter target ?
 192.168.1.7
 Enter user ?
 deepak
 Enter password ?
 123
 Add Another Server? (Y/N)
 n
 ******************************
 Success
 In Environment Configuration
 ****************************** 



Al configurar un entorno, si el usuario desea configurar con el entorno actual, pueden utilizar el siguiente comando:

.. code-block:: bash

		ptdeploy envconfig config --keep-current-environments

Después de introducir el comando anterior, lo hará pide los siguientes datos como se muestra en el formato de tabla:


.. cssclass:: table-bordered

 +-----------------------------------------------+------------+-----------------------------------------------------------------------+
 | Parámetros                                    | Opciones   | Comentarios                                                           |
 +===============================================+============+=======================================================================+
 |Configure Environments Here? (Y/N)             | Y(Yes)     | Si el usuario desea configurar los entornos en el entorno actual se   |
 |                                               |            | puede introducir como Y                                               |
 +-----------------------------------------------+------------+-----------------------------------------------------------------------+
 |Configure Environments Here? (Y/N)	         | N(No)      | Si el usuario no desea configurar los entornos en el entorno actual   |
 |                                               |            | se puede introducir como N                                            |
 +-----------------------------------------------+------------+-----------------------------------------------------------------------+
 |Use existing environment settings? (Y/N)       | Y(Yes)     | Si el usuario desea utilizar la configuración del entorno existentes  |
 |                                               |            | se puede introducir como Y.                                           |
 +-----------------------------------------------+------------+-----------------------------------------------------------------------+
 |Use existing environment settings? (Y/N)       | N(No)      | Si el usuario no desea utilizar los valores del entorno existentes    |
 |                                               |            | se puede introducir como N.                                           |
 +-----------------------------------------------+------------+-----------------------------------------------------------------------+
 |Do you want to add another environment? (Y/N)  | Y(Yes)     | Si el usuario desea agregar otro entorno, se puede introducir como Y. |
 +-----------------------------------------------+------------+-----------------------------------------------------------------------+
 |Do you want to add another environment? (Y/N)  | N(No)      | Si el usuario no desea agregar otro entorno, se puede introducir      |
 |                                               |            | como N.|                                                              |
 +-----------------------------------------------+------------+-----------------------------------------------------------------------+


La siguiente captura de pantalla representa gráficamente el proceso mencionado anteriormente:

.. code-block:: bash


 kevell@corp:/# ptdeploy envconfig config --keep-current-environments

 Configure Environments Here? (Y/N) 
 y
 Use existing environment settings? (Y/N) 
 y
 Do you want to add another environment? (Y/N) 
 n
 ******************************
 Success
 In Environment Configuration
 ****************************** 



Cómo eliminar configuración del entorno
-------------------------------------------------------

Si el usuario necesita para borrar la configuración del entorno, se puede introducir el siguiente comando:

.. code-block:: bash

	ptdeploy envconfig del --environment-name="kevells"

El usuario puede especificar el nombre del entorno que desean eliminar como se muestra arriba.

Después de introducir el comando anterior, se le preguntará

Paso 1: Delete Environments Here?

y muestra un mensaje de advertencia como

.. code-block:: bash

 WARNING: Deleting an environment from papyrus is final. You may be looking for boxify box-destroy instead (Y/N) 

El usuario tiene que especificar Sí o No

Paso 2: Environment Kevells(Name of the specified environment that is supposed to delete) found. Are you sure want to delete it? (Y/N)

El usuario tiene que especificar Sí o No

Por último, el entorno especificado se elimina como se muestra en la captura de pantalla.

.. code-block:: bash


 kevell@corp:/# ptdeploy envconfig del --environment-name="kevells"

 Delete Environments Here?
 WARNING: Deleting an environment from papyrus is final. You may be looking for boxify box-destroy instead (Y/N) 
 y
 Environment kevells found. Are you sure you want to delete it? (Y/N) 
 y
 [Pharaoh Logging] Removing environment kevells.
 ****************************
 Success
 In Environment Configuration
 ****************************



Otra forma de eliminar un medio ambiente sin especificar el nombre del medio ambiente es como se muestra mediante el comando:

.. code-block:: bash

	ptdeploy envconfig delete

Después de introducir el comando anterior, se le preguntará

Paso 1: Delete Environments Here?

y muestra un mensaje de advertencia como

.. code-block:: bash

 WARNING: Deleting an environment from papyrus is final. You may be looking for boxify box-destroy instead (Y/N) 

El usuario tiene que especificar Sí o No

Por último, el medio ambiente se elimina como se muestra en la captura de pantalla:

.. code-block:: bash

 kevell@corp:/# ptdeploy envconfig delete

 Delete Environments Here?
 WARNING: Deleting an environment from papyrus is final. You may be looking for boxify box-destroy instead (Y/N) 
 y
 Enter Environment Name To delete
 deepak
 Environment deepak found. Are you sure you want to delete it? (Y/N) 
 y
 [Pharaoh Logging] Removing environment deepak.
 ******************************
 Success
 In Environment Configuration
 ****************************** 



Cómo listar configuración del entorno
--------------------------------------------------

Si el usuario desea ver la lista de los detalles con respecto a la configuración del entorno, pueden de entrada como se muestra:

.. code-block:: bash

	ptdeploy envconfig list

Después de introducir el comando anterior, lo hará pide

List Environment Here? (Y/N)

si el usuario especifica como Y, generará la pantalla de salida como se muestra en la captura de pantalla:

.. code-block:: bash


 kevell@corp:/# ptdeploy envconfig list --yes
 ************************************************

 array(3) {
  [0]=>
  array(2) {
    ["any-app"]=>
    array(2) {
      ["gen_env_name"]=>
      string(13) "default-local"
      ["gen_env_tmp_dir"]=>
      string(5) "/tmp/"
    }
    ["servers"]=>
    array(1) {
      [0]=>
      array(3) {
        ["target"]=>
        string(9) "127.0.0.1"
        ["user"]=>
        string(5) "local"
        ["password"]=>
        string(5) "local"
      }
    }
  }
  [1]=>
  array(2) {
    ["any-app"]=>
    array(2) {
      ["gen_env_name"]=>
      string(18) "default-local-8080"
      ["gen_env_tmp_dir"]=>
      string(5) "/tmp/"
    }
    ["servers"]=>
    array(1) {
      [0]=>
      array(3) {
        ["target"]=>
        string(14) "127.0.0.1:8080"
        ["user"]=>
        string(5) "local"
        ["password"]=>
        string(5) "local"
      }
    }
  }
  [2]=>
  array(2) {
    ["any-app"]=>
    array(2) {
      ["gen_env_name"]=>
      string(6) "deepak"
      ["gen_env_tmp_dir"]=>
      string(5) "/tmp/"
    }
    ["servers"]=>
    array(1) {
      [0]=>
      array(3) {
        ["target"]=>
        string(11) "192.168.1.7"
        ["user"]=>
        string(6) "deepak"
        ["password"]=>
        string(3) "123"
      }
    }
  }
 }

 In Environment Configuration
 ******************************



parámetros alternativos
--------------------------------
 
En lugar de envconfig los siguientes parámetros se puede utilizar en la declaración:

* EnvironmentConfig
* environmentconfig
* environment-config
* env-config

Beneficios
------------

* Es-acomodados tanto en OS ciento y así como en ubuntu.
* Los parámetros utilizados en la declaración no son sensibles, que es una ventaja añadida, mientras que en comparación con otros.
* Este módulo conduce a los usuarios cómo configurar el entorno, cómo eliminar el medio ambiente no deseado, cómo utilizar la opción de 
  lista para mostrar los entornos disponibles.

