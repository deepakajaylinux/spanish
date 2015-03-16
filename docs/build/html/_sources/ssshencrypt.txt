===========
SshEncrypt
===========

Sinopsis
----------------

Sshencrypt ayudar al usuario a instalar la clave privada cifrada. Es el proceso de codificación de mensajes y la información de tal manera que sólo las partes autorizadas puedan leerlo. Sshencrypt sí misma no evitar la interceptación, pero niega el contenido del mensaje al interceptor. En un esquema de cifrado, el mensaje o información, que se refiere como texto sin formato, se cifra utilizando un algoritmo de encriptación, la generación de ciphertxt que sólo se puede leer si descifrado. Se consuela con Ubuntu y CentOS.

Comando Ayuda
-----------------------

El comando de ayuda guía al usuario para introducir ptconfigure manejar. Este comando ayuda guía al usuario para instalar sshencrypt. Esto también desencriptar la clave. El cifrado se puede utilizar para proteger los datos "en reposo", tales como archivos en los ordenadores y dispositivos de almacenamiento. En los últimos años ha habido numerosos informes de datos confidenciales, tales como registros personales de los clientes están expuestos a través de la pérdida o robo de ordenadores portátiles o unidades de respaldo. El comando de ayuda para Sshencrypt se muestra a continuación.

.. code-block:: bash

		ptconfigure  sshencrypt help


Después de entradas el comando anterior, comienza a funcionar para instalar una clave privada encriptada. Es la catequesis de las funciones en las capturas de pantalla.

La siguiente captura de pantalla muestra sobre sshencrypted

.. code-block:: bash


parámetro Alternativa
-----------------------------------

Hay muchas alternativas disponibles en sshencrypt. Cada alternativa muestra una ventaja añadida a estos módulos. Ellos son,

SshEncrypt, ssh-cifrar, sshencrypt.

Cifrar
-------------

Se utiliza para instalar un sshkey cifrado. En principio, es posible descifrar el mensaje sin poseer la llave, pero, para un esquema de cifrado bien diseñado, se requieren grandes recursos computacionales y habilidad. Cifrar por orden de la misma dada a continuación.

.. code-block:: bash

		ptconfigure  ssh-encrypt install

La representación gráfica de la orden anterior se enumeran a continuación,

.. code-block:: bash

        - encrypt
        Installs an encrypted SSH Key.
        example: ptconfigure ssh-encrypt install

Después de vitalizar el comando se catequizar entrada.

Cuando la entrada de usuario como si se instala automáticamente encriptada con la comprobación del sistema. Si no salir de la instalación.

unencrypt
----------------

Solía instala clave ssh sin cifrar. Un destinatario autorizado puede descifrar fácilmente el mensaje con la clave proporcionada por el emisor a los receptores, pero no a los interceptores no autorizadas. Desencriptar con sólo orden dada a continuación.

.. code-block:: bash

		ptconfigure  ssh-encrypt install

La representación gráfica de la orden anterior se enumeran a continuación,

.. code-block:: bash

        - unencrypt
        Installs an encrypted SSH Key.
        example: ptconfigure ssh-encrypt install


Beneficios
----------------

* El secreto puede mantenerse.
* Well-to-do en Ubuntu y CentOS.
* Sensitibilidad caso.
* La parte receptora tiene acceso a la clave de descifrado que permite que los mensajes que se deben leer.
