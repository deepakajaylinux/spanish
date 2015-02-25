=======
Jmeter
=======

sinopsis
------------

Este módulo se ocupa de la instalación de la jmeter con la versión actualizada. JMeter puede ser utilizado como una herramienta de prueba de unidad para las conexiones de base de datos JDBC, FTP, LDAP, servicios Web, JMS, HTTP conexiones TCP genéricos y procesos nativos del sistema operativo. Veamos cómo este módulo ayuda al usuario en la instalación y el uso de la Jmeter.

Ayuda Comando
---------------------

El comando help guía a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en el módulo Jmeter. En él se enumeran los parámetros alternativos de módulo jmeter. También describe la sintaxis para instalar el módulo jmeter. El comando de ayuda para el módulo jmeter se muestra a continuación.

.. code-block:: bash

		ptconfigure Jmeter help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda bajo Jmeter.

.. code-block:: bash

 kevell@corp:/# ptconfigure Jmeter help

 ******************************


  This command allows you to update Jmeter.

  Jmeter, jmeter

        - install
        Installs the latest version of Jmeter
        example: ptconfigure jmeter install

 ------------------------------
 End Help
 ******************************

instalación
----------------

El comando utilizado para instalar el jmeter en la máquina de los usuarios se muestra a continuación:

.. code-block:: bash

		ptconfigure jmeter install


Después de introducir el comando anterior, el siguiente proceso se produce como se muestra en el formato tabular.

.. cssclass:: table-bordered

 +---------------------------+----------------------------------+--------------+----------------------------------------------+
 | Parámetros                | Parámetro Alternativa            | Opciones     | Comentarios                                  |
 +===========================+==================================+==============+==============================================+
 |Install Jmeter? (Y/N)      | En lugar de jmeter, podemos      | Y(Yes)       | Si el usuario desea continuar el proceso de  | 
 |                           | utilizar Jmeter también.         |              | instalación se puede introducir como Y.      |
 +---------------------------+----------------------------------+--------------+----------------------------------------------+
 |Install Jmeter? (Y/N)      | En lugar de jmeter, podemos      | N(No)        | Si el usuario desea abandonar el proceso de  |
 |                           | utilizar Jmeter también.         |              | instalación se puede introducir como N.|     |
 +---------------------------+----------------------------------+--------------+----------------------------------------------+

Si el usuario procede de la instalación, durante el proceso de instalación se describe en las listas siguientes:

* Construye el árbol de dependencias.
* Lee la información de estado.
* Lista outs los paquetes que se instalan automáticamente.
* Lista outs los nuevos paquetes que está instalando.
* Detalles sobre el número de archivos actualizados, recién instalados, retirados y no actualizados.
* Lee la lista de paquetes y muestra la lista de paquetes que ya están instalados.

La siguiente captura de pantalla representa gráficamente el proceso anteriormente descrito de la instalación.

.. code-block:: bash

Beneficios
--------------

* Los parámetros utilizados en la ayuda y la instalación no son sensibles, que es una ventaja añadida, mientras que en comparación con otros.
* Es-acomodados tanto en Ubuntu y así como Cent OS.
* Este módulo se instala el Jmeter en versión actualizada.
* Si el módulo ya existe en la máquina del usuario, se mostrará un mensaje, ya que ya existe.
* JMeter apoya parametrización variable afirmaciones (validación de respuesta), por las cookies hilo, variables de configuración y una 
  variedad de informes.
* Desarrolladores fuera de sitio pueden extender fácilmente JMeter con plugins personalizados.
