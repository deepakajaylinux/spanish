==========
Joomla
==========

sinopsis
----------------

Joomla ofrece el sitio web de integración. Muchos servicios de alojamiento web ofrecen un solo clic en instalar, consiguiendo que el usuario nuevo sitio en marcha y funcionando en pocos minutos.

Incluyendo su facilidad de uso y extensibilidad, Joomla han hecho el software del sitio Web más popular. Lo mejor de todo, piloto automatico, builderfy y dapperfy están disponibles en ptdeploy y hace una mejor solución. Esto es cómodo con Ubuntu y CentOS.

comando Ayuda
------------------------

Este comando ayuda guía al usuario para proporcionar una integración de Joomla. Ha personalizado Piloto automático, builderfy y dapperfy están disponibles en ptdeploy .También proporciona una configuración de base de datos para el módulo de configuración db.
El comando de ayuda para Oracle se muestra a continuación.

.. code-block:: bash

		ptdeploy joomla help

Después de entradas el comando anterior, comienza a funcionar para integrar sitio web joomla. Es la catequesis las funciones de joomla en las capturas de pantalla.

.. code-block:: bash

 kevell@corp:/# ptdeploy Joomla help
 ******************************


  This module is a Default one, and provides integration for Joomla websites. It has tailored Builderfy and Dapperfy
  Autopilots and also provides Joomla Database Configuration for the DBConfigure Module.

  Joomla, joomla

  This module adds multiple actions to both builderfy and dapperfy. This will let you produce autopilots for both
  which are tailored to Joomla.

  // dapperfy - create our auto deploy files
  ptdeploy dapperfy joomla --yes --guess

  // builderfy - create templates to install build
  sudo ptdeploy builderfy continuous --yes --jenkins-home="/var/lib/jenkins" --target-job-name="my-project-continuous" --project-description="This is the Continuous Delivery build for My Project" --primary-scm-url="http://146.185.129.66:8080/git/root/first-pharaoh-cd.git" --source-branch-spec="origin/master" --source-scm-url="http://146.185.129.66:8080/git/root/first-pharaoh-cd.git" --days-to-keep="-1" --amount-to-keep="10" --autopilot-test-invoke-install-file="build/config/ptdeploy/autopilots/tiny-staging-invoke-code-no-dbconf.php" --autopilot-prod-invoke-install-file="build/config/ptdeploy/autopilots/tiny-prod-invoke-code-no-dbconf.php" --error-email="phpengine@hotmail.co.uk" --only-autopilots

  // execute the build creator
  ptdeploy autopilot execute build/config/ptdeploy/builderfy/autopilots/tiny-jenkins-invoke-continuous.php

 ------------------------------
 End Help
 ******************************

instalación
-------------------

Este módulo añade múltiples acciones a ambos builderfy y dapperfy. Esto es fácil de instalar y configurar, incluso si el usuario no es un user.Since avanzada Joomla es tan fácil de usar, como diseñador web o programador, el usuario puede crear rápidamente sitios para sus clientes. El comando utilizado para instalar joomla es el siguiente,

.. code-block:: bash

		ptdeploy joomla install

Después de vitalizar el comando se catequizar entrada.

Cuando la entrada de usuario como si automáticamente se instalará joomla del sistema. Si no salir de la instalación. La siguiente captura de pantalla de demostrar Joomla y sus funciones.

Dapperfy
---------------

Este dapperfy utiliza para crear el auto usuario desplegar archivos. Dapperfy puede trabajar para una gran cantidad de proyectos sin configuraciones complejas con un par de minutos por valor de establecer. Utilizando Dapperfy es muy rápido, y es probablemente el mejor punto de partida, incluso para configuraciones complejas como el usuario siempre puede simplemente modificar los archivos después con sus propias personalizaciones. El siguiente comando utiliza para dapperfy.

.. code-block:: bash

		ptdeploy dapperfy joomla

Después de entrada como por encima de dicho comando se pide dapperfy ejecución se muestra por la pantalla.

.. code-block:: bash

 kevell@corp:/# ptdeploy dapperfy joomla
 Dapperfy This for Joomla? (Y/N) 
 Y
 Do you want to add another environment? (Y/N) 
 n
 Standard Dapperfies:
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-enforce-revisions.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-rollback-newest.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-invoke-rollback-previous.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-enforce-revisions.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-rollback-newest.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-rollback-previous.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-uninstall-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-uninstall-code.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-nodepool-install-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-ptvirtualize-host-install-host-file-entry.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-ptvirtualize-host-uninstall-host-file-entry.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-ptvirtualize-install-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-install-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-uninstall-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-uninstall-code.php
 Joomla Dapperfies:
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-node-install-code-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-install-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-workstation-install-code-dbconf.php
 Standard Dapperfies:
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-enforce-revisions.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-rollback-newest.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-invoke-rollback-previous.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-enforce-revisions.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-rollback-newest.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-rollback-previous.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-uninstall-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-uninstall-code.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-nodepool-install-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-ptvirtualize-host-install-host-file-entry.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-ptvirtualize-host-uninstall-host-file-entry.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-ptvirtualize-install-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-install-code-no-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-uninstall-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-uninstall-code.php
 Joomla Dapperfies:
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-node-install-code-dbconf.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-install-code-data.php
 /vv/build/config/ptdeploy/dapperfy/autopilots/generated/default-local-8080-workstation-install-code-dbconf.php
 ******************************
 

 Success
 In Dapperfy
 ******************************

Builderfy
--------------

Crea plantillas para instalar build. El usuario puede añadir más plantillas. Cuando hacemos cambios en el repositorio de usuarios, la implementación de una nueva versión de la Producción destino para el usuario. El comando utilizado para builderfy es como sigue,

.. code-block:: bash

		ptdeploy builderfy joomla

La siguiente captura de pantalla explica su función.

.. code-block:: bash

ejecutar
------------

Este proceso ejecuta piloto automático creador de construcción. Acceso rápido es posible. La orden para la ejecución de la siguiente manera,

.. code-block:: bash

		ptdeploy autopilot execute

La siguiente captura de pantalla a explicar sus funciones.

.. code-block:: bash


Opciones
------------

.. cssclass:: table-bordered

 +----------------------------+-------------------------+-------------+-----------------------------------------------------+
 | Parámetros                 | Parámetro Alternativa   | Opciones    | Comentarios                                         |
 +============================+=========================+=============+=====================================================+
 |Dapperfy this for           | Joomla, joomla          | Y(Yes)      | Si el usuario desea proceder dapperfying se puede   |
 |joomla? (Y/N)               |                         |             | introducir como Y.                                  |
 +----------------------------+-------------------------+-------------+-----------------------------------------------------+
 |Dapperfy this for           | Joomla, joomla          | N(No)       | La salida del sistema de la dapperfy                |
 |joomla? (Y/N)               |                         |             |                                                     |
 +----------------------------+-------------------------+-------------+-----------------------------------------------------+
 |Do you want to add another  |                         | Y(Yes)      | Si el usuario desea añadir un nuevo entorno         |
 |environment?(Y/N)           |                         |             | en el que puede introducir como Y.                  |
 +----------------------------+-------------------------+-------------+-----------------------------------------------------+
 |Do you want to add another  |                         | N(No)       | Si el usuario no está en necesidad de añadir        |
 |environment?(Y/N)           |                         |             | nuevo entorno en el que puede introducir como N.|   |
 +----------------------------+-------------------------+-------------+-----------------------------------------------------+


Beneficios
------------

* Soporte Bueno para profesionales de TI
* Proceso multilingüe
* Fácil actualización
* La línea de sistema de Speedy
* No mayúsculas y minúsculas
* Conveniente para Ubuntu y CentOS.


El equipo de Joomla sí abre todo un nuevo mundo de expresión, ya que le la libertad de usar hace que el diseño sueño hecho realidad de usuario permite
