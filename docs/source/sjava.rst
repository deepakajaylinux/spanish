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
 Y
 *******************************
 *        Pharaoh Tools        *
 *         !!Java JDK!!        *
 *******************************
 Enter Java Install Directory (no trailing slash):

 Creating /tmp/ptconfigure-temp-script-37090112192.sh
 chmod 755 /tmp/ptconfigure-temp-script-37090112192.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-37090112192.sh Permissions
 Executing /tmp/ptconfigure-temp-script-37090112192.sh
 --2015-03-16 15:52:21--  https://bitbucket.org/phpengine/cleo-jdk-64/get/6c383e2868bd.zip
 Resolving bitbucket.org (bitbucket.org)... 131.103.20.167, 131.103.20.168
 Connecting to bitbucket.org (bitbucket.org)|131.103.20.167|:443... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: unspecified [application/zip]
 Saving to: ‘6c383e2868bd.zip’

    [          <=>                                                                                          ] 2,06,54,011 2.98KB/s   in 12m 14s

 2015-03-16 16:04:59 (27.5 KB/s) - ‘6c383e2868bd.zip’ saved [20654011]

 /tmp/oraclejdk: Scheme missing.
 FINISHED --2015-03-16 16:04:59--
 Total wall clock time: 12m 39s
 Downloaded: 1 files, 20M in 12m 14s (27.5 KB/s)
  End-of-central-directory signature not found.  Either this file is not
  a zipfile, or it constitutes one disk of a multi-part archive.  In the
  latter case the central directory and zipfile comment will be found on
  the last disk(s) of this archive.
 unzip:  cannot find zipfile directory in one of /tmp/oraclejdk.zip or
        /tmp/oraclejdk.zip.zip, and cannot find /tmp/oraclejdk.zip.ZIP, period.
 /tmp/ptconfigure-temp-script-37090112192.sh: 6: cd: can't cd to /tmp/oraclejdk
 mv: cannot stat ‘/tmp/oraclejdk/phpengine-cleo-jdk-64-6c383e2868bd/jdk-7u60-linux-x64.tar.gz’: No such file or directory
 tar: jdk-7u60-linux-x64.tar.gz: Cannot open: No such file or directory
 tar: Error is not recoverable: exiting now
 mkdir: missing operand
 Try 'mkdir --help' for more information.
 cp: missing destination file operand after ‘/tmp/oraclejdk/jdk1.7.0_60/*’
 Try 'cp --help' for more information.
 chmod: missing operand after ‘a+x’
 Try 'chmod --help' for more information.
 update-alternatives: error: alternative path /bin/java doesn't exist
 update-alternatives: error: alternative path /bin/javac doesn't exist
 update-alternatives: error: alternative path /bin/javaws doesn't exist
 update-alternatives: error: alternative /bin/java for java not registered; not setting
 update-alternatives: error: alternative /bin/javac for javac not registered; not setting
 update-alternatives: error: alternative /bin/javaws for javaws not registered; not setting
 Archive:  /tmp/oraclejdk.zip
 Temp File /tmp/ptconfigure-temp-script-37090112192.sh Removed
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
