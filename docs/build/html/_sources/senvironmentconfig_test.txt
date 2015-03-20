===================
EnvironmentConfig
===================


sinopsis
-------------

Este módulo facilita a los usuarios en la configuración de su entorno necesario para su proyecto. Veamos cómo configurar el entorno, cómo eliminar el ambiente no deseado, cómo utilizar la opción lista para enumerar los entornos disponibles en próximos temas.


comando Ayuda
--------------------

El comando ayuda guía a los usuarios sobre la finalidad del módulo, sus parámetros alternativos que se utilizan en la declaración. Se destacan las tres funciones de la configuración del entorno que son lista, configurar, borrar. También especifica la sintaxis para utilizar tres funciones principales. A continuación se muestra la sintaxis utilizada para declarar la ayuda:



.. code-block:: bash

	ptconfigure envconfig help

La captura de pantalla siguiente muestra gráficamente sobre el funcionamiento del comando help.



.. code-block:: bash


 kevell@corp:/# ptconfigure envconfig help
 ******************************


  This command is part of a default Module and provides you with a method by which you can
  configure environments for your project from the command line. Currently compliant with
  both ptdeploy and ptconfigure.

  EnvironmentConfig, environmentconfig, environment-config, envconfig, env-config

        - list
        List current environments
        example: ptconfigure envconfig list --yes

        - list-local
        List current local environments
        example: ptconfigure envconfig list-local --yes

        - configure, config
        Configure bespoke environments for your project to use
        example: ptconfigure envconfig config
        # below to create an empty environment to add instances to
        example: ptconfigure envconfig config --yes
                    --keep-current-environments # do not overwrite the current environments stored in papyrusfile
                    --no-manual-servers # so it will not ask you to interactively enter connection details of instances
                    --add-single-environment # otherwise it will loop for more until you specify not to
                    --environment-name="some-name" # name of the environment to create
                    --tmp-dir=/tmp/ # we're deprecating this soon

        - configure-default, config-default
        Configure default environments for your project to use
        example: ptconfigure envconfig config-default
        example: ptconfigure envconfig config-default --yes --environment-name="local-80/local-8080"

        - delete, del
        Configure the environments for your project to use
        example: ptconfigure envconfig delete
        example: ptconfigure envconfig del --environment-name="staging"


 ------------------------------
 End Help
 ******************************




Cómo configurar el entorno 
----------------------------------------------

A fin de configurar el entorno, el usuario puede utilizar el siguiente comando:


.. code-block:: bash

	ptconfigure envconfig config


Después de introducir el comando sobre las siguientes operaciones lleva a cabo como se muestra:


Step 1: Configure Environments Here? (Y/N)

El usuario tiene que introducir Y o N.

Step 2: Use existing environment Settings? (Y/N)

El usuario tiene que introducir Y o N.

Si el usuario de entrada y se procederá con la ya existente.

Si de entrada como N, se pide información sobre el medio ambiente como

Value for: Name of the environment

Value for: Default temp dir(Location)

Después de los pasos anteriores, el usuario tiene que introducir los siguientes datos:


Enter target?

Enter user?

Enter password?

Add Another Server? (Y/N)

El usuario tiene que introducir Y o N.


Por último, la configuración del entorno obtiene éxito como se muestra en la siguiente captura de pantalla.



.. code-block:: bash

 kevell@corp:/# ptconfigure envconfig config
 Configure Environments Here? (Y/N) 
 Y
 Environment 1  : 
 Default Settings for Any App not setup for environment  enter them now.
 Value for: Name of this Environment
 kevells
 Value for: Default Temp Dir (should usually be /tmp/)

 Enter Servers - this is an array of entries
 Enter target ?
 /home/kevells
 Enter user ?
 kevells
 Value for: Default Temp Dir (should usually be /tmp/)

 Enter Servers - this is an array of entries
 Enter target ?
 /home/kevells
 Enter user ?
 kevells
 Enter password ?
 123456
 Add Another Server? (Y/N)
 N
 ******************************


 Success
 In Environment Configuration
 ******************************




Mientras configura un entorno, si el usuario desea configurar con el entorno actual, puede utilizar el siguiente comando:


.. code-block:: bash

	ptconfigure envconfig config --keep-current-environments




Después de introducir el comando anterior, se pide a los siguientes datos como se muestra en el formato tabular:


.. cssclass:: table-bordered

 +-------------------------------------+------------+----------------------------------------------------------------+
 | parámetros                          | opciones   | comentarios                                                    |
 +=====================================+============+================================================================+
 |Configure Environments Here? (Y/N)   | Y          | Si el usuario desea configurar los entornos en la corriente    |
 |                                     |            | entorno en el que puede introducir como Y                      |
 +-------------------------------------+------------+----------------------------------------------------------------+
 |Configure Environments Here? (Y/N)   | N          | Si el usuario no desea configurar los entornos expuestos a     |
 |                                     |            | entorno actual se puede introducir como N                      |
 +-------------------------------------+------------+----------------------------------------------------------------+
 |Use existing environment             | Y          | Si el usuario desea utilizar la configuración del entorno      |
 |settings? (Y/N)                      |            | existentes se puede introducir como Y.                         |
 +-------------------------------------+------------+----------------------------------------------------------------+
 |Use existing environment             | N          | Si el usuario no desea utilizar el entorno existente           |
 |settings? (Y/N)                      |            | configuración que puede introducir como N.                     |
 +-------------------------------------+------------+----------------------------------------------------------------+
 |Do you want to add another           | Y          | Si el usuario desea agregar otro ambiente , que pueden         |
 |environment? (Y/N)                   |            | de entrada como Y.                                             |
 +-------------------------------------+------------+----------------------------------------------------------------+
 |Do you want to add another           | N          | Si el usuario no desea añadir otro ambiente , que pueden       |
 |environment? (Y/N)                   |            | de entrada como N.|                                            |
 +-------------------------------------+------------+----------------------------------------------------------------+ 


La siguiente captura representa gráficamente el proceso antes mencionado:



.. code-block:: bash


 kevell@corp:/# ptconfigure envconfig config --keep-current-environments
 Configure Environments Here? (Y/N) 
 Y
 Use existing environment settings? (Y/N) 
 Y
 Do you want to add another environment? (Y/N) 
 N
 ******************************


 Success
 In Environment Configuration
 ******************************


Cómo eliminar la configuración del entorno 
-------------------------------------------------------

Si el usuario necesita borrar la configuración del entorno, puede introducir el siguiente comando:

.. code-block:: bash

ptconfigure envconfig del --environment-name="kevells"

El usuario puede especificar el nombre del medio ambiente que desean eliminar como se muestra arriba.


Después de introducir el comando anterior, se preguntará


Step 1: Delete Environments Here?

y muestra una advertencia del mensaje como


.. code-block:: bash

 WARNING: Deleting an environment from papyrus is final. You may be looking for boxify box-destroy instead (Y/N) 



El usuario debe especificar Y o N

Step 2: Environment Kevells(Name of the specified environment that is supposed to delete) found. Are you sure want to delete it? (Y/N)

El usuario debe especificar Y o N


Finalmente, el entorno especificado consigue eliminar como se muestra en la captura de pantalla.


.. code-block:: bash



 kevell@corp:/# ptconfigure envconfig del --environment-name="kevells"
 Delete Environments Here?
 WARNING: Deleting an environment from papyrus is final. You may be looking for boxify box-destroy instead (Y/N) 
 Y
 Environment kevells found. Are you sure you want to delete it? (Y/N) 
 Y
 [Pharaoh Logging] Removing environment kevells.
 ******************************


 Success
 In Environment Configuration
 ******************************


Cómo enumerar configuración del entorno 
--------------------------------------------------

Si el usuario desea ver la lista de los detalles sobre la configuración del entorno, puede introducir como se muestra:

.. code-block:: bash

ptconfigure envconfig list --yes


Después de introducir el comando anterior, mostrará la salida como se muestra en la captura de pantalla:

.. code-block:: bash
	


 kevell@corp:/# ptconfigure envconfig list --yes
 ******************************


 array(0) {
 }

 In Environment Configuration
 ******************************


Alternative Parameters
--------------------------------

En lugar de envconfig los siguientes parámetros pueden utilizarse en la declaración:

* EnvironmentConfig
* environmentconfig
* environment-config
* env-config

beneficios
------------

* Es acomodada en ambos OS ciento y así como en ubuntu. 
* Los parámetros utilizados en la declaración no son mayúsculas y 
  minúsculas que es una ventaja añadida mientras que comparado con otros. * Este módulo conduce a los usuarios cómo configurar el entorno, cómo
  eliminar el ambiente no deseado, cómo utilizar la opción lista para 
  enumerar los ambientes disponibles.
                                                                      


