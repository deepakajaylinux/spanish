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


Beneficios
-------------
* Los parámetros utilizados en ayuda de instalación y operaciones no son sensibles, que es una ventaja añadida, mientras que en comparación 
  con otros.
* Es-acomodados tanto en Ubuntu y así como Cent OS.
* Configuración de java, javac, javaws se puede hacer con la ayuda de una nueva versión de Oracle.
