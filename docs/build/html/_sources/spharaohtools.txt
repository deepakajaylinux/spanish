===================
PharaohTools
===================

sinopsis
------------

El módulo herramienta Faraón asistencias en la instalación Ptdeploy, Pttest, Jrush, generando informes ptconfigure. Facilita a los usuarios para garantizar la disponibilidad antes de instalaciones. Sólo módulos faltantes se pueden instalar en concreto.

Ayuda Comando
---------------------

El comando help guía a los usuarios sobre cómo hacer uso de este módulo en particular bajo ptconfigure.
También los hace conscientes de las opciones que se pueden realizar en este módulo específico.

La captura de pantalla como se muestra a continuación le da una representación gráfica sobre el uso del comando de ayuda.

.. code-block:: bash

 kevell@corp:/# ptconfigure PharaohTools help
 ******************************


  This command allows you to install the Pharaoh Tools which are ready. These include
  ptconfigure - this Configuration Management tool, ptdeploy - the Automated Deployment tool,
  and pttest, the test configuration and automation tool.

  PharaohTools, pharaohtools, pharaoh-tools

        - install
        Installs the latest version of all of the Pharaoh Tools
        example: ptconfigure pharaoh-tools install

 ------------------------------
 End Help
 ******************************

instalación
-------------

El módulo herramienta faraón actúa como una ruta más corta que envuelve la instalación de ptdeploy, pttest, Jrush. Si cualquier módulo en particular no se encuentra entre los tres, se instalará el módulo específico solo que es una ventaja añadida. El proceso de garantizar juega un papel importante en el acaparamiento de datos con respecto a la disponibilidad de módulos.

El comando que se utiliza para el proceso de instalación en herramienta Faraón se da a continuación,

.. code-block:: bash

		ptconfigure pharaoh-tools install


.. cssclass:: table-bordered

 +--------------------------+------------------------------------------+-------------+-------------------------------------------------+
 | Parámetros               | Parámetro Alternativa                    | Opciones    | Comentarios                                     |
 +==========================+==========================================+=============+=================================================+
 |Install Pharaoh Tools?    | PharaohTools, pharaohtools,              | Y(Yes)      | Si el usuario desea continuar con el proceso    |
 |(Y/N)                     | pharaoh-tools                            |             | de instalación, se puede introducir como Y      |
 +--------------------------+------------------------------------------+-------------+-------------------------------------------------+
 |Install Pharaoh Tools?    | PharaohTools, pharaohtools,              | N(No)       | Si el usuario desea salir del proceso de        | 
 |(Y/N)                     | pharaoh-tools                            |             | instalación, pueden dejar simplemente usando N| |
 +--------------------------+------------------------------------------+-------------+-------------------------------------------------+

Durante la instalación de la herramienta de Faraón los siguientes pasos se lleva a cabo:

Asegurar
---------

* La herramienta faraón asegura que los módulos disponibles.
* Además de garantizar, No comprobará sobre las versiones.

Ptdeploy      
-------------------

* El módulo ptdeploy indica que es instalado, en el caso de la existencia.
* También comprueba la versión para ptdeploy módulo.
* Si el módulo ptdeploy no está disponible en la máquina, entonces automáticamente ptdeploy progresará a instalar.

Pttest
---------------

* Después de completar la instalación ptdeploy, se asegurará el módulo pttest.
* El módulo pttest indica que es instalado, en el caso de la existencia.
* Si el módulo pttest no está disponible en la máquina, entonces automáticamente pttest progresará instalar.

Jrush
---------
* Después de completar la instalación pttest, se asegurará el módulo Jrush.
* El módulo Jrush indica que es instalado, en el caso de la existencia.
* Si el módulo Jrush no está disponible en la máquina, entonces automáticamente Jrush progresará instalar.
Si todos los tres módulos ya existen, a continuación, se mostrará el mensaje excepcional como se da en la siguiente imagen,

.. code-block:: bash

 kevell@corp:/# ptconfigure pharaoh-tools install
 Install Pharaoh Tools? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         Pharaoh Tools        *
 *******************************
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module ptdeploy reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module pttest reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module ptconfigure reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module JRush reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PharaohTools: Success
 ------------------------------
 Installer Finished
 ******************************


Opciones Adicionales
----------------------------

Durante la instalación de ptdeploy, pttest, Jrush las siguientes opciones se requieren como entrada del usuario. Veamos acerca de las opciones adicionales que se pueden especificar por los usuarios si desean, se representa en forma de tabla como se muestra a continuación.

.. cssclass:: table-bordered


 +--------------------------+--------------------------------+---------------+---------------------------------------------------------------+
 | Parámetros               | camino                         | Opciones      | Comentarios                                                   |
 +==========================+================================+===============+===============================================================+
 |Program data directory    | “/opt/pttest (módulo           | Y(Yes)        | Si el usuario de proceder con la instalación del directorio   | 
 |(Por defecto)             | correspondiente)”              |               | de datos de programa predeterminado que puede introducir      |
 |                          |                                |               | como Sí                                                       |
 +--------------------------+--------------------------------+---------------+---------------------------------------------------------------+
 |Program data directory    | específica de usuario          | N(Fin barra)  | Si el usuario desea continuar con su propio directorio de     |
 |                          |                                |               | datos del programa, pueden de entrada como N, y en la mano    |
 |                          |                                |               | especificar que poseen ubicación.                             |
 +--------------------------+--------------------------------+---------------+---------------------------------------------------------------+
 |Program executor          | “/usr/bin”                     | Yes           | Si el usuario de proceder con la instalación del directorio   |
 |directory (Por defecto)   |                                |               | ejecutor programa predeterminado que puede introducir como Sí |
 +--------------------------+--------------------------------+---------------+---------------------------------------------------------------+
 |Program executor          | específica de usuario          | N(Fin barra)  | Si el usuario desea continuar con su propio directorio        |
 |directory                 |                                |               | ejecutor del programa, pueden de entrada como N, y en la mano |
 |                          |                                |               | especificar que poseen ubicación.|                            |
 +--------------------------+--------------------------------+---------------+---------------------------------------------------------------+


Durante la instalación se especificará la ubicación de git clone, muestra el número de objetos, que reciben los objetos, la resolución de los deltas, conectividad.

La siguiente captura de pantalla que explica gráficamente sobre el proceso para la instalación de la herramienta de Faraón.

.. code-block:: bash

 kevell@corp:/# ptconfigure pharaoh-tools install
 Install Pharaoh Tools? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         Pharaoh Tools        *
 *******************************
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module ptdeploy reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module pttest reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module ptconfigure reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 [Pharaoh Logging] Ensure module install is not checking versions
 [Pharaoh Logging] Module JRush reports itself as Installed
 [Pharaoh Logging] Not installing as already installed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PharaohTools: Success
 ------------------------------
 Installer Finished
 ******************************


Beneficios
--------------

* Facilita a los usuarios para asegurarse antes de la instalación.
* En caso de cualquier módulo en particular no se encuentra, el usuario puede proceder a instalar ese módulo en particular solo.
* El usuario puede especificar su propia vía o ubicación para el directorio de datos del programa y el directorio de albacea.
* Si algún módulo en particular ya existe en la máquina, entonces la herramienta de instalación generará un mensaje de excepción, ya que ya 
  está instalado.
* Evita sobreescritura no deseado de módulos, por lo tanto, es el ahorro de tiempo.
