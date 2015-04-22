========
Drupal
========

Sinopsis
------------

Módulo de Drupal es una parte de módulos por defecto. Proporciona pilotos automáticos para Drupal que se adapta por builderfy y pilotos automáticos dapperfy. Además de la builderfy y dapperfy, proporciona configuración de base de Drupal para el módulo de configuración de DB.

Drupal es un marco de gestión de contenido libre y de código abierto escrito en PHP y distribuido bajo la Licencia Pública General GNU. Se utiliza como marco de fondo de al menos el 2,1% de todos los sitios web en todo el mundo que van desde blogs personales hasta, y sitios del gobierno corporativos, políticos incluidos WhiteHouse.gov y data.gov.uk. También se utiliza para la gestión del conocimiento y la colaboración empresarial.

Drupal funciona en cualquier plataforma informática que soporta tanto un servidor web capaz de ejecutar PHP (incluyendo Apache, Litespeed, IIS, Lighttpd, Hiawatha, Cherokee o Nginx) y una base de datos (como MySQL, MongoDB, MariaDB, PostgreSQL, SQLite, o Microsoft SQL Server) para almacenar contenido y la configuración.

Veamos cómo dapperfy el drupal bajo estos módulos en diferentes aspectos.

Ayuda Comando
--------------------

El comando de ayuda es una breve y así como abstracto interesante para el usuario. Proporciona información sobre su papel principal, los detalles de parámetros alternativos que se pueden utilizar en las declaraciones, Sus tres funciones principales (builderfy, dapperfy, ejecutar), y también la sintaxis para el uso y la declaración de esas tres funciones interesantes. La sintaxis utilizada para la declaración de opción de ayuda, es la siguiente.

.. code-block:: bash

	ptdeploy Drupal help

Después de introducir el comando dado anteriormente, el usuario puede ver el resultado de visualización de opciones de ayuda, junto con los detalles descritos anteriormente, puede obtener visualmente estos resultados de opción de ayuda, como se muestra en la siguiente captura de pantalla.

.. code-block:: bash

 kevell@corp:/# ptdeploy Drupal help
 ******************************


  This module is a Default Modules and provides autopilots for drupal tailored Builderfy and Dapperfy Autopilots.
  Also provides Drupal Database Configuration for the DBConfigure Module.

  Drupal, drupal

  This module adds multiple actions to both builderfy and dapperfy. This will let you produce autopilots for both
  which are tailored to Drupal.

  // dapperfy - create our auto deploy files
  ptdeploy dapperfy drupal --yes --guess

  // builderfy - create templates to install build
  sudo ptdeploy builderfy continuous --yes --jenkins-home="/var/lib/jenkins" --target-job-name="my-project-continuous" --project-description="This is the Continuous Delivery build for My Project" --primary-scm-url="http://146.185.129.66:8080/git/root/first-pharaoh-cd.git" --source-branch-spec="origin/master" --source-scm-url="http://146.185.129.66:8080/git/root/first-pharaoh-cd.git" --days-to-keep="-1" --amount-to-keep="10" --autopilot-test-invoke-install-file="build/config/ptdeploy/autopilots/tiny-staging-invoke-code-no-dbconf.php" --autopilot-prod-invoke-install-file="build/config/ptdeploy/autopilots/tiny-prod-invoke-code-no-dbconf.php" --error-email="phpengine@hotmail.co.uk" --only-autopilots

  // execute the build creator
  ptdeploy autopilot execute build/config/ptdeploy/builderfy/autopilots/tiny-jenkins-invoke-continuous.php

 ------------------------------
 End Help
 ******************************

Cómo Dapperfy Drupal
--------------------------------
 
Veamos acerca de los diferentes aspectos de este módulo en dapperfying el drupal. El comando utilizado para este propósito es el mismo para todos los aspectos como se muestra a continuación,

.. code-block:: bash

	ptdeploy dapperfy drupal

Después de entrar en la orden dada anteriormente, los siguientes datos se preguntaron durante la ejecución como se muestra en la tabla,

.. cssclass:: table-bordered

 +----------------------------+------------------------------------------+-----------+-------------------------------------------------+
 | Parámetros                 | Parámetro Alternativa                    | Opciones  | Comentarios                                     |
 +============================+==========================================+===========+=================================================+
 |Dapperfy This for Drupal?   | En lugar deDrupal, podemos utilizar      | Y(Yes)    | Si el usuario necesita dapperfy la Drupal       | 
 |(Y/N)	                      | drupal también.                          |           | se puede introducir como Y.                     |
 +----------------------------+------------------------------------------+-----------+-------------------------------------------------+
 |Dapperfy This for Drupal?   | En lugar deDrupal, podemos utilizar      | N(No)     | Si el usuario no está en necesidad de           |
 |(Y/N)	                      | drupal también.                          |           | dapperfy la drupal se puede introducir como N.| |
 +----------------------------+------------------------------------------+-----------+-------------------------------------------------+


Si los fondos de usuarios dapperfying el drupal introduciendo como Y, los siguientes pasos están involucrados en la ejecución,

Paso 1:

Do you want to add another environment? (Y/N)

El usuario tiene a la entrada de Y o N, dependiendo de su necesidad de añadir otro entorno.

La siguiente captura de pantalla muestra visualmente sobre este proceso de dapperfying el drupal.

.. code-block:: bash

 kevell@corp:/# ptdeploy dapperfy drupal
 Dapperfy This for Drupal? (Y/N) 
 Y
 Use existing environment settings? (Y/N) 
 n
 Do you want to add another environment? (Y/N) 
 n
 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 ******************************


 Success
 In Dapperfy
 ******************************

La segunda forma de declarar la dapperfying de Drupal se explica a continuación, y el comando utilizado para que sea lo mismo que

.. code-block:: bash

	ptdeploy dapperfy drupal

Después de entrar en la orden dada anteriormente, los siguientes datos se preguntaron durante la ejecución como se muestra en la tabla,

.. cssclass:: table-bordered

 +-----------------------------+--------------------------------------+-------------+------------------------------------------------------+
 | Parámetros                  | Parámetro Alternativa                | Opciones    | Comentarios                                          |
 +=============================+======================================+=============+======================================================+
 |Dapperfy This for Drupal?    | En lugar deDrupal, podemos utilizar  | Y(Yes)      | Si el usuario necesita dapperfy la Drupal            |
 |(Y/N)	                       | drupal también.                      |             | se puede introducir como Y.                          |
 +-----------------------------+--------------------------------------+-------------+------------------------------------------------------+
 |Dapperfy This for Drupal?    | En lugar deDrupal, podemos utilizar  | N(No)       | Si el usuario no está en necesidad de dapperfy       |
 |(Y/N)	                       | drupal también.                      |             | la drupal se puede introducir como N.                |
 +-----------------------------+--------------------------------------+-------------+------------------------------------------------------+
 |Use existing environment     |                                      | Y(Yes)      | Si el usuario desea continuar con la configuración   |
 |settings? (Y/N)              |                                      |             | del entorno existentes que pueden ingresarse como Y. |
 +-----------------------------+--------------------------------------+-------------+------------------------------------------------------+
 |Use existing environment     |                                      | N(No)       | Si el usuario desea proceder con los nuevos valores  |
 |settings? (Y/N)              |                                      |             | de entorno que puede introducir como N.|             |
 +-----------------------------+--------------------------------------+-------------+------------------------------------------------------+

Tras la finalización de las investigaciones dadas anteriormente, los siguientes pasos descritos ejecutarán,

Paso 1:

Do you want to modify entries applicable to any app in environment default-local (Y/N)

El usuario tiene a la entrada de S o N.

Paso 2:

Environment 1 default-local:

En este paso, el valor del medio ambiente y directorio temporal se preguntó y el usuario tendrá que introducirlos.

Paso 3:

Enter Servers-this is an array of entries

Enter target?

Enter User?

Enter Password?

El usuario tiene que introducir los inquirido de datos.

Paso 4:

Add Another Server? (Y/N)

El usuario tiene a la entrada de S o N en función de su deseo.

Paso 5:

Do you want to modify entries applicable to any app in environment default-local -0000 (Y/N)

El usuario tiene a la entrada de S o N.

Paso 6:

Los ajustes para el medio ambiente se pueden definir manualmente si es necesario para introducir los valores no predeterminados.

Los datos del preguntaron durante la ejecución de la aplicación de configuración se definen de la siguiente manera,

Value for Git repo URL

Value for Optional Private SSH Key for Git Repo.

Value for Git Custom Branch

Value for Apache VHost URL

Value for Apache VHost Hostname/IP

Value for how many revisions to keep

Value for DB IP Address

Value for DB App User Name

Value for DB App User Pass

Paso 7:

Do you want to add another environment? (Y/N)

El usuario tiene a la entrada de Y o N en función de sus necesidades.

La siguiente pantalla le dará una representación pictórica de los pasos explicados anteriormente.

.. code-block:: bash

 kevell@corp:/# ptdeploy dapperfy drupal

 Dapperfy This for Drupal? (Y/N) 
 Y
 Use existing environment settings? (Y/N) 
 Y
 Do you want to modify entries applicable to any app in environment default-local (Y/N) 
 Y
 Environment 1 default-local : 
 Default Settings for Any App not setup for environment default-local enter them now.
 Value for: Name of this Environment
 kevell
 Value for: Default Temp Dir (should usually be /tmp/)

 Enter Servers - this is an array of entries
 Enter target ?
 /root/gg
 Enter user ?
 root
 Enter password ?
 123
 Add Another Server? (Y/N)
 n
 Do you want to modify entries applicable to any app in environment default-local-8080 (Y/N) 
 n
 Settings for dapper not setup for environment default-local-8080 enter them manually.
 Environment 2 default-local-8080 : 
 Value for: Project Container directory, (inc slash)
 /root/vv
 Value for: Git Repo URL
 
 Value for: Optional Private SSH Key for Git Repo

 Value for: Git Custom Branch
 
 Value for: Apache VHost URL (Don't Include http://)
 
 Value for: Apache VHost Hostname/IP
 
 Value for: How many revisions to keep
 
 Value for: DB IP Address
 
 Value for: DB App User Name (Will be created if not existing)
 
 Value for: DB App User Pass
 
 Value for: DB Name (Will be created if not existing)
 
 Value for: DB Admin User Name
 
 Value for: DB Admin User Pass
 
 Do you want to add another environment? (Y/N) 
 n
 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 ******************************
 
 
 Success
 In Dapperfy
 ******************************

La tercera forma de ejecución se explica a partir de los próximos pasos. El comando es igual

.. code-block:: bash

	ptdeploy dapperfy drupal

Después de entrar en la orden dada anteriormente, los siguientes datos se preguntaron durante la ejecución como se muestra en la tabla,

.. cssclass:: table-bordered

 +-------------------------+--------------------------------------------+-----------+-------------------------------------------------------+
 | Parámetros              | Parámetro Alternativa                      | Opciones  | Comentarios                                           |
 +=========================+============================================+===========+=======================================================+
 |Dapperfy This for        | En lugar deDrupal, podemos utilizar        | Y(Yes)    | Si el usuario necesita dapperfy la Drupal se puede    |
 |Drupal? (Y/N)	           | drupal también.                            |           | introducir como Y.                                    |
 +-------------------------+--------------------------------------------+-----------+-------------------------------------------------------+
 |Dapperfy This for        | En lugar deDrupal, podemos utilizar        | N(No)     | Si el usuario no está en necesidad de dapperfy        |
 |Drupal? (Y/N)	           | drupal también.                            |           | la drupal se puede introducir como N.                 |
 +-------------------------+--------------------------------------------+-----------+-------------------------------------------------------+
 |Use existing environment |                                            | Y(Yes)    | Si el usuario desea continuar con la configuración    |
 |settings? (Y/N)	   |                                            |           | del entorno existentes que pueden ingresarse como Y.  |
 +-------------------------+--------------------------------------------+-----------+-------------------------------------------------------+
 |Use existing environment |                                            | N(No)     | Si el usuario desea proceder con los nuevos valores   |
 |settings? (Y/N)	   |                                            |           | de entorno que puede introducir como N.|              |
 +-------------------------+--------------------------------------------+-----------+-------------------------------------------------------+

Tras la finalización de las investigaciones dadas anteriormente, los siguientes pasos descritos ejecutarán,

Paso 1:

Do you want to add another environment settings? (Y/N)

El usuario tiene a la entrada de S o N.

Paso 2:

Environment 3 default-local:

En este paso, el valor del medio ambiente y directorio temporal se preguntó y el usuario tendrá que introducirlos.

Los ajustes para el medio ambiente se pueden definir manualmente si es necesario para introducir los valores no predeterminados.

Los datos del preguntaron durante la ejecución de la aplicación de configuración se definen de la siguiente manera,

Value for Project Container Directory.

Value for Git repo URL

Value for Optional Private SSH Key for Git Repo.

Value for Git Custom Branch

Value for Apache VHost URL

Value for Apache VHost Hostname/IP

Value for how many revisions to keep

Value for DB IP Address

Value for DB App User Name

Value for DB App User Pass

La siguiente pantalla le dará una representación pictórica de los pasos explicados anteriormente.

.. code-block:: bash

 kevell@corp:/# ptdeploy dapperfy drupal
 Dapperfy This for Drupal? (Y/N) 
 y
 Use existing environment settings? (Y/N) 
 n
 Do you want to add another environment? (Y/N) 
 y
 Environment 3  : 
 Default Settings for Any App not setup for environment  enter them now.
 Value for: Name of this Environment
 kevell
 Value for: Default Temp Dir (should usually be /tmp/)

 Value for: Project Container directory, (inc slash)

 Value for: Git Repo URL

 Value for: Optional Private SSH Key for Git Repo

 Value for: Git Custom Branch

 Value for: Apache VHost URL (Don't Include http://)

 Value for: Apache VHost Hostname/IP

 Value for: How many revisions to keep

 Value for: DB IP Address

 Value for: DB App User Name (Will be created if not existing)

 Value for: DB App User Pass

 Value for: DB Name (Will be created if not existing)

 Value for: DB Admin User Name

 Value for: DB Admin User Pass

 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 ******************************


 Success
 In Dapperfy
 ******************************

El cuarto tipo de dapperfying el drupal se explica a continuación, y el comando utilizado es el mismo que

.. code-block:: bash

	ptdeploy dapperfy drupal

Después de entrar en la orden dada anteriormente, los siguientes datos se preguntaron durante la ejecución como se muestra en la tabla,

.. cssclass:: table-bordered

 +---------------------------+--------------------------------------+------------+----------------------------------------------------------+
 | Parámetros                | Parámetro Alternativa                | Opciones   | Comentarios                                              |
 +===========================+======================================+============+==========================================================+
 |Dapperfy This for          | En lugar deDrupal, podemos utilizar  | Y(Yes)     | Si el usuario necesita dapperfy la Drupal se puede       | 
 |Drupal? (Y/N)	             | drupal también.                      |            | introducir como Y.                                       |
 +---------------------------+--------------------------------------+------------+----------------------------------------------------------+
 |Dapperfy This for          | En lugar deDrupal, podemos utilizar  | N(No)      | Si el usuario no está en necesidad de dapperfy la        |
 |Drupal? (Y/N)	             | drupal también.                      |            | drupal se puede introducir como N.                       |
 +---------------------------+--------------------------------------+------------+----------------------------------------------------------+
 |Use existing environment   |                                      | Y(Yes)     | Si el usuario desea continuar con la configuración       |
 |settings? (Y/N)	     |                                      |            | del entorno existentes que pueden ingresarse como Y.     |
 +---------------------------+--------------------------------------+------------+----------------------------------------------------------+
 |Use existing environment   |                                      | N(No)      | Si el usuario desea proceder con los nuevos valores      |
 |settings? (Y/N)	     |                                      |            | de entorno que puede introducir como N.|                 |
 +---------------------------+--------------------------------------+------------+----------------------------------------------------------+


Si los fondos de usuarios dapperfying el drupal introduciendo como Y, los siguientes pasos están involucrados en la ejecución,

Paso 1:

Do you want to add another environment? (Y/N)

El usuario tiene a la entrada de Y o N, dependiendo de su necesidad de añadir otro entorno.

La siguiente captura de pantalla muestra visualmente sobre este proceso de dapperfying el drupal.

.. code-block:: bash

 kevell@corp:/# ptdeploy dapperfy drupal
 Dapperfy This for Drupal? (Y/N) 
 y
 Use existing environment settings? (Y/N) 
 n
 Do you want to add another environment? (Y/N) 
 n
 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Builderfy
 //build/config/ptdeploy/dapperfy/autopilots/generated/Dapperfy
 ******************************


 Success
 In Dapperfy
 ******************************

Builderfy
----------

Crea plantillas drupal instalar build. El usuario puede añadir más plantillas . Cuando hacemos cambios en el repositorio de usuarios , la implementación de una nueva versión de la Producción destino para el usuario . El comando utilizado para builderfy es como sigue ,


.. code-block:: bash

        ptdeploy builderfy continuous-drupal

.. code-block:: bash



 kevell@corp:/# ptdeploy builderfy continuous-drupal
 Install Builderfy? (Y/N) 
 y
 *******************************
 *   Golden Contact Computing  *
 *           Builderfy!          *
 *******************************
 Enter the data handling type
 (0) code 
 (1) replication 
 (2) capture 
 0
 checkWhat is your Jenkins home? Found "/var/lib/jenkins" - use this? 

 What is the target Job Name?
 my-project-continuous
 Enter a description for your project
 This is the Continuous Delivery build for My Project
 Enter a Primary SCM URL for your project
 http://146.185.129.66:8080/git/root/first-pharaoh-cd.git
 Enter a Source Branch Spec for your project
 origin/master
 Enter a Source SCM URL for your project
 http://146.185.129.66:8080/git/root/first-pharaoh-cd.git
 Enter the number of days to keep builds for
 1
 Enter the max number of builds results to keep
 10
 Enter the path of the autopilot test environment invoke install file (Relative to project root)
 build/config/ptdeploy/autopilots/tiny-staging-invoke-code-no-dbconf.php
 Enter the path of the autopilot prod environment invoke install file (Relative to project root)
 build/config/ptdeploy/autopilots/tiny-staging-invoke-code-no-dbconf.php
 Enter the data handling type
 (0) code 
 (1) replication 
 (2) capture 
 0
 Enter build failure Email address. Whitespace-separated list of recipient addresses
 phpengine@hotmail.co.uk
 Copying Files...
 Enter the data handling type
 (0) code 
 (1) replication 
 (2) capture 
 0
 Changing Folder Permissions...
 Changing Folder Owner...
 Changing Folder Group...
 ... All done!
 *******************************
 Thanks for installing , visit www.gcsoftshop.co.uk for more
 ****************************** 


 Success
 In Builderfy
 ******************************




Beneficios
-----------

* Es-acomodados tanto en ubuntu y al igual que en ciento OS.
* Los parámetros utilizados en la declaración no distingue entre mayúsculas y minúsculas.
* Los ajustes para el medio ambiente pueden ser definidos durante la ejecución de la dapperfying.

