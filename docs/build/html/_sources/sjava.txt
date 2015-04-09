=====	
JAVA
=====

sinopsis
------------

Ayuda Este módulo en la instalación de la versión de Oracle Java JDK 1.7. Será también facilita la configuración de java, javac, javaws junto con la nueva versión de Oracle.

Ayuda Comando
---------------------

El comando help guía a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en el módulo de Java. El comando help enumera los parámetros alternativos de módulo Java. También describe la sintaxis para instalar Java JDK 1.7. El comando de ayuda para el módulo de Java se muestra a continuación.

.. code-block:: bash

		ptconfigure Java help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda bajo módulo de java.

.. code-block:: bash

 kevell@corp:/# ptconfigure java help
 ******************************


 This command allows you to install Java JDK 1.7 .

 Java, java, java17

        - install
        Installs a version of Oracle Java JDK 1.7. It will also configure java,
        javac and javaws to be provided by the new Oracle version.
        example: ptconfigure java17 install

 ------------------------------
 End Help
 ******************************

instalación
----------------

Instalación de la versión de Oracle Java JDK 1.7 a la máquina de los usuarios se puede hacer simplemente usando el comando como se muestra a continuación.

.. code-block:: bash
	
		ptconfigure Java install

Después de introducir el comando anterior, el siguiente proceso se produce como se muestra en el formato tabular.

.. cssclass:: table-bordered

 +------------------------+--------------------------------------------+------------+--------------------------------------+
 | Parámetros             | Parámetro Alternativa                      | Opciones   | Comentarios                          |
 +========================+============================================+============+======================================+
 |Install The Oracle Java | En lugar de Oracle Java JDK 1.7, las       | Y(Yes)     | Si el usuario desea continuar el     |
 |JDK 1.7? (Y/N)          | siguientes alternativas también se pueden  |            | proceso de instalación se puede      |
 |                        | utilizar: Java, Java, java17               |            | introducir como Y                    |
 +------------------------+--------------------------------------------+------------+--------------------------------------+
 |Install The Oracle Java | En lugar de Oracle Java JDK 1.7, las       | N(No)      | Si el usuario desea abandonar el     |
 |JDK 1.7? (Y/N)          | siguientes alternativas también se pueden  |            | proceso de instalación se puede      |
 |                        | utilizar: Java, Java, java17               |            | introducir como N.|                  |
 +------------------------+--------------------------------------------+------------+--------------------------------------+

.. code-block:: bash

 kevell@corp:/# ptconfigure java17 install
 Install The Oracle Java JDK 1.7? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         !!Java JDK!!        *
 *******************************
 Enter Java Install Directory (no trailing slash):
 /opt
 Creating /tmp/ptconfigure-temp-script-96883431452.sh
 chmod 755 /tmp/ptconfigure-temp-script-96883431452.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-96883431452.sh Permissions
 Executing /tmp/ptconfigure-temp-script-96883431452.sh
 --2015-04-09 16:27:08--  https://bitbucket.org/phpengine/cleo-jdk-64/get/6c383e2868bd.zip
 Resolving bitbucket.org (bitbucket.org)... 131.103.20.168, 131.103.20.167
 Connecting to bitbucket.org (bitbucket.org)|131.103.20.168|:443... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: 141966331 (135M) [application/zip]
 Saving to: Ã¢â‚¬Ëœ/tmp/oraclejdk/6c383e2868bd.zipÃ¢â‚¬â„¢

 100%[====================================================================================================>] 14,19,66,331  110KB/s   in 12m 36s

 2015-04-09 16:39:46 (183 KB/s) - Ã¢â‚¬Ëœ/tmp/oraclejdk/6c383e2868bd.zipÃ¢â‚¬â„¢ saved [141966331/141966331]

 Archive:  /tmp/oraclejdk.zip
 6c383e2868bd47e56385921e11ec155ac54faa13
   creating: /tmp/oraclejdk/phpengine-cleo-jdk-64-6c383e2868bd/
  inflating: /tmp/oraclejdk/phpengine-cleo-jdk-64-6c383e2868bd/jdk-7u60-linux-x64.tar.gz  
 update-alternatives: using /opt/bin/java to provide /usr/bin/java (java) in auto mode
 update-alternatives: using /opt/bin/javac to provide /usr/bin/javac (javac) in auto mode 
 update-alternatives: using /opt/bin/javaws to provide /usr/bin/javaws (javaws) in auto mode
 Temp File /tmp/ptconfigure-temp-script-96883431452.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************

 Single App Installer:
 --------------------------------------------
 Java: Success
 ------------------------------
 Installer Finished
 ******************************



Beneficios
-------------
* Los parámetros utilizados en ayuda de instalación y operaciones no son sensibles, que es una ventaja añadida, mientras que en comparación 
  con otros.
* Es-acomodados tanto en Ubuntu y así como Cent OS.
* Configuración de java, javac, javaws se puede hacer con la ayuda de una nueva versión de Oracle.
