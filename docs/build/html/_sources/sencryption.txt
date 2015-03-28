============
Encryption
============

Sinopsis
------------
Este módulo permite a los usuarios cifrar o descifrar un archivo.

El cifrado es el proceso de codificación de mensajes y la información de tal manera que sólo las partes autorizadas puedan leerlo. Cifrado en sí misma no evitar la interceptación, pero niega el contenido del mensaje al interceptor. En un esquema de cifrado, el mensaje o información, que se refiere como texto sin formato, se codifica mediante un algoritmo de encriptación, la generación de texto cifrado que sólo se puede leer si descifrado. Por razones técnicas, un esquema de encriptación normalmente utiliza una clave pseudo-aleatorios generados por un algoritmo. En principio, es posible descifrar el mensaje sin poseer la llave, pero, para un esquema de cifrado bien diseñado, se requieren grandes recursos computacionales y habilidad. Un destinatario autorizado puede descifrar fácilmente el mensaje con la clave proporcionada por el emisor a los receptores, pero no a los interceptores no autorizadas.

Veamos cómo utilizar este módulo en cifrar y descifrar un archivo o una cadena.

Ayuda Comando
----------------------

El comando de ayuda es un breve manual de usuario que ayuda a los usuarios en el manejo de este módulo. Se especifica los parámetros alternativos que se pueden utilizar en declarar. También especifica las posibles funciones conforme a este módulo de cifrado, junto con la sintaxis para usarlos. El comando utilizado para la declaración de opción de ayuda se muestra a continuación,

.. code-block:: bash

	ptconfigure encryption help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda bajo cifrado.

.. code-block:: bash



 kevell@corp:/# ptconfigure encryption help

 ******************************


 This command allows you to encrypt or decrypt a file.  

 Encryption, encrypt  

 - install        
	Encrypts a file or string        
 	example: sudo ptconfigure encryption install --yes --unencrypted-data=/var/www/a-website/build/config/ptconfigure/SSH/raw/bastion        
	 --encryption-target-file=/tmp/encrypted --encryption-key=/root/.ptconfigure/SSH/key --encryption-file-permissions=""                
	 --encryption-file-owner="" --encryption-file-group=""                

 - uninstall        
	Decrypts an encrypted file or string        
	example: sudo ptconfigure encryption uninstall --yes --encrypted-data=/tmp/encrypted        
	 --encryption-target-file=/var/www/a-website/build/config/ptconfigure/SSH/raw/bastion --encryption-key=/root/.ptconfigure/SSH/key                	 --encryption-file-permissions="" --encryption-file-owner="" --encryption-file-group=""                

 ------------------------------
 End Help
 ******************************

instalar
--------


Esta función permite a los usuarios cifrar un archivo o una cadena simplemente usando el comando como se indica a continuación,

.. code-block:: bash

	 sudo ptconfigure encryption install --yes --unencrypted-data=/var/www/a-website/build/config/ptconfigure/SSH/raw/bastion
 	--encryption-target-file=/tmp/encrypted --encryption-key=/root/.ptconfigure/SSH/key --encryption-file-permissions=""                
	 --encryption-file-owner="" --encryption-file-group=""                

Para implementar esta función, el usuario tiene que especificar los siguientes campos en el formato de la sintaxis mencionada,

* Archivo de destino cifrado
* Clave de cifrado
* Clave SSH
* Permiso de archivo cifrado
* Propietario del archivo cifrado
* Grupo de archivos de cifrado


.. code-block:: bash

 kevell@corp:/# sudo ptconfigure encryption install --yes --unencrypted-data="/home/kevells/Desktop/graphs" --encryption-target-file="/home/kevells/Desktop/graphs" --encryption-key=/root/.ptconfigure/SSH/key --encryption-file-permissions="755" --encryption-file-owner="kevells" --encryption-file-group="kevells"

 *******************************
 *        Pharaoh Tools        *
 *         Encryption !        *
 *******************************
 [Pharaoh Logging] Package php5-mcrypt from the Packager Apt is already installed, so not installing
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 Encryption: Success
 ------------------------------
 Installer Finished
 ******************************



Desinstalar
---------------

Esta función permite a los usuarios para descifrar un archivo o cadena cifrada. Esto se puede lograr mediante el comando de abajo,

.. code-block:: bash

	sudo ptconfigure encryption uninstall --yes --encrypted-data=/tmp/encrypted
	 --encryption-target-file=/var/www/a-website/build/config/ptconfigure/SSH/raw/bastion --encryption-key=/root/.ptconfigure/SSH/key                	 --encryption-file-permissions="" --encryption-file-owner="" --encryption-file-group=""                

Para implementar esta función, el usuario tiene que especificar los siguientes campos en el formato de la sintaxis mencionada,

* Archivo de destino cifrado
* Clave de cifrado
* Clave SSH
* Permiso de archivo cifrado
* Propietario del archivo cifrado
* Grupo de archivos de cifrado


parámetros alternativos
------------------------------


Los parámetros alternativos para este módulo, cualquiera de los cuales se pueden utilizar en la declaración es,


* Encryption
* encrypt

Beneficios
--------------

* Los parámetros utilizados en ayuda y de cifrado y descifrado de la ONU operaciones no son sensibles, que es una ventaja añadida, mientras que 
  compararon a los demás.
* Es-acomodados tanto en Ubuntu y así como Cent OS.
* Se trata de un modo seguro, porque sólo una persona autorizada pueda utilizarlos.
