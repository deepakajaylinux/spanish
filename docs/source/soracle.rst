===========
Oracle
===========

sinopsis
----------------

Módulo de Oracle utiliza para actualizar oráculo. Es la primera base de datos diseñada para la computación grid empresa, la manera más flexible y económica para gestionar la información y las aplicaciones. Grid computing Enterprise crea grandes grupos de la industria estándar, modular de almacenamiento y servidores. Con esta arquitectura, cada nuevo sistema puede ser rápidamente aprovisionados desde la piscina de los componentes. No hay necesidad de que los picos de trabajo, ya que la capacidad puede ser fácilmente añadidos o reasignarse los fondos de recursos según sea necesario. Es cómodo con Ubuntu y CentOS.

comando Ayuda
-----------------------

Este comando ayuda guía al usuario para actualizar Oracle. Esto también comprueba ejecución, resolver y petición.
El comando de ayuda para Oracle se muestra a continuación.

.. code-block:: bash

		ptconfigure Oracle help

Después de entradas el comando anterior, comienza a funcionar para actualizar oráculo. Es la catequesis de las funciones en las capturas de pantalla.

.. code-block:: bash

instalación
------------------

La instalación incluye la instalación de Oracle requiere para hacer la instalación en una versión actualizada. Es un proceso de manifiesto para instalar el módulo de Oracle bajo ptconfigure Oracle con sólo usar la orden dada a continuación,

.. Code-block:: bash

	ptconfigure Oracle Install


Después de vitalizar el comando se catequizar entrada.

Cuando la entrada de usuario como si automáticamente se instalará Oracle con la comprobación del sistema. Si no salir de la instalación. La siguiente captura de pantalla de demostrar Oracle y sus funciones.

.. code-block:: bash


 kevell@corp:/# ptconfigure Oracle install
 Install Oracle? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         Oracle!        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-74494590076.sh
 chmod 755 /tmp/ptconfigure-temp-script-74494590076.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-74494590076.sh Permissions
 Executing /tmp/ptconfigure-temp-script-74494590076.sh
 --2015-01-28 19:28:31--  http://oss.oracle.com/el4/RPM-GPG-KEY-oracle
 Resolving oss.oracle.com (oss.oracle.com)... 137.254.120.35
 Connecting to oss.oracle.com (oss.oracle.com)|137.254.120.35|:80... connected.
 HTTP request sent, awaiting response... 302 Found
 Location: https://oss.oracle.com/el4/RPM-GPG-KEY-oracle [following]
 --2015-01-28 19:28:32--  https://oss.oracle.com/el4/RPM-GPG-KEY-oracle
 Connecting to oss.oracle.com (oss.oracle.com)|137.254.120.35|:443... connected.
 HTTP request sent, awaiting response... 200 OK
 Length: 1743 (1.7K) [text/plain]
 Saving to: â€˜STDOUTâ€™

 100%[=====================================================================================================>] 1,743       --.-K/s   in0s       
 2015-01-28 19:28:35 (4.27 MB/s) - written to stdout [1743/1743]
 W: GPG error: http://oss.oracle.com unstable Release: The following signatures were invalid: KEYEXPIRED 1378511808 KEYEXPIRED 1378511808    	KEYEXPIRED 1378511808
 W: Failed to fetch http://oss.oracle.com/debian/dists/unstable/main/binary-amd64/Packages  HttpError404

 W: Failed to fetch http://oss.oracle.com/debian/dists/unstable/non-free/binary-amd64/Packages  HttpError404

 E: Some index files failed to download. They have been ignored, or old ones used instead.
 OK
 Ign http://dl.google.com stable InRelease
 Hit http://dl.google.com stable Release.gpg
 Hit http://dl.google.com stable Release
 Hit http://dl.google.com stable/main amd64 Packages
 Hit http://dl.google.com stable/main i386 Packages
 Ign http://repos.zend.com server InRelease
 Hit http://repos.zend.com server Release.gpg
 Hit http://repos.zend.com server Release
 Ign http://dl.google.com stable/main Translation-en_US
 Ign http://dl.google.com stable/main Translation-en
 Hit http://repos.zend.com server/non-free amd64 Packages
 Hit http://repos.zend.com server/non-free i386 Packages
 Ign http://extras.ubuntu.com trusty InRelease
 Ign http://security.ubuntu.com trusty-security InRelease
 Ign http://us.archive.ubuntu.com trusty InRelease
 Get:1 http://oss.oracle.com unstable InRelease
 Ign http://oss.oracle.com unstable InRelease
 Hit http://extras.ubuntu.com trusty Release.gpg
 Ign http://us.archive.ubuntu.com trusty-updates InRelease
 Get:2 http://security.ubuntu.com trusty-security Release.gpg [933 B]
 Hit http://extras.ubuntu.com trusty Release
 Ign http://us.archive.ubuntu.com trusty-backports InRelease
 Get:3 http://security.ubuntu.com trusty-security Release [62.0 kB]
 Hit http://extras.ubuntu.com trusty/main Sources
 Hit http://us.archive.ubuntu.com trusty Release.gpg
 Hit http://extras.ubuntu.com trusty/main amd64 Packages
 Hit http://extras.ubuntu.com trusty/main i386 Packages
 Get:4 http://oss.oracle.com unstable Release
 Ign http://oss.oracle.com unstable Release
 Get:5 http://us.archive.ubuntu.com trusty-updates Release.gpg [933 B]
 Hit http://us.archive.ubuntu.com trusty-backports Release.gpg
 Get:6 http://oss.oracle.com unstable/main amd64 Packages
 Hit http://us.archive.ubuntu.com trusty Release
 Get:7 http://us.archive.ubuntu.com trusty-updates Release [62.0 kB]
 Get:8 http://oss.oracle.com unstable/non-free i386 Packages
 Ign http://repos.zend.com server/non-free Translation-en_US
 Get:9 http://oss.oracle.com unstable/main Translation-en_US
 Ign http://repos.zend.com server/non-free Translation-en
 Ign http://extras.ubuntu.com trusty/main Translation-en_US
 Ign http://extras.ubuntu.com trusty/main Translation-en
 Get:10 http://security.ubuntu.com trusty-security/main Sources [64.8 kB]
 Hit http://us.archive.ubuntu.com trusty-backports Release
 Hit http://us.archive.ubuntu.com trusty/main Sources
 Hit http://us.archive.ubuntu.com trusty/restricted Sources
 Hit http://us.archive.ubuntu.com trusty/universe Sources
 Hit http://us.archive.ubuntu.com trusty/multiverse Sources
 Hit http://us.archive.ubuntu.com trusty/main amd64 Packages
 Hit http://us.archive.ubuntu.com trusty/restricted amd64 Packages
 Hit http://us.archive.ubuntu.com trusty/universe amd64 Packages
 Hit http://us.archive.ubuntu.com trusty/multiverse amd64 Packages
 Hit http://us.archive.ubuntu.com trusty/main i386 Packages
 Err http://oss.oracle.com unstable/main amd64 Packages
   HttpError404
 Hit http://us.archive.ubuntu.com trusty/restricted i386 Packages
 Err http://oss.oracle.com unstable/non-free amd64 Packages
   HttpError404
 Ign http://oss.oracle.com unstable/main Translation-en_US
 Ign http://oss.oracle.com unstable/main Translation-en
 Hit http://us.archive.ubuntu.com trusty/universe i386 Packages
 Ign http://oss.oracle.com unstable/non-free Translation-en_US
 Hit http://us.archive.ubuntu.com trusty/multiverse i386 Packages
 Hit http://us.archive.ubuntu.com trusty/main Translation-en
 Get:11 http://security.ubuntu.com trusty-security/restricted Sources [2,061 B]
 Ign http://oss.oracle.com unstable/non-free Translation-en
 Hit http://us.archive.ubuntu.com trusty/multiverse Translation-en
 Hit http://us.archive.ubuntu.com trusty/restricted Translation-en
 Get:12 http://security.ubuntu.com trusty-security/universe Sources [17.4 kB]
 Hit http://us.archive.ubuntu.com trusty/universe Translation-en
 Get:13 http://us.archive.ubuntu.com trusty-updates/main Sources [159 kB]
 Get:14 http://security.ubuntu.com trusty-security/multiverse Sources [723 B]
 Get:15 http://security.ubuntu.com trusty-security/main amd64 Packages [200 kB]
 Get:16 http://us.archive.ubuntu.com trusty-updates/restricted Sources [2,061 B]
 Get:17 http://us.archive.ubuntu.com trusty-updates/universe Sources [97.6 kB]
 Get:18 http://security.ubuntu.com trusty-security/restricted amd64 Packages [8,875 B]
 Get:19 http://security.ubuntu.com trusty-security/universe amd64 Packages [85.3 kB]
 Get:20 http://security.ubuntu.com trusty-security/multiverse amd64 Packages [1,161 B]
 Get:21 http://security.ubuntu.com trusty-security/main i386 Packages [190 kB]
 Get:22 http://us.archive.ubuntu.com trusty-updates/multiverse Sources [3,553 B]
 Get:23 http://us.archive.ubuntu.com trusty-updates/main amd64 Packages [406 kB]
 Get:24 http://security.ubuntu.com trusty-security/restricted i386 Packages [8,846 B]
 Get:25 http://security.ubuntu.com trusty-security/universe i386 Packages [85.3 kB]
 Get:26 http://security.ubuntu.com trusty-security/multiverse i386 Packages [1,412 B]
 Hit http://security.ubuntu.com trusty-security/main Translation-en
 Hit http://security.ubuntu.com trusty-security/multiverse Translation-en
 Hit http://security.ubuntu.com trusty-security/restricted Translation-en
 Hit http://security.ubuntu.com trusty-security/universe Translation-en
 Get:27 http://us.archive.ubuntu.com trusty-updates/restricted amd64 Packages [8,875 B]
 Get:28 http://us.archive.ubuntu.com trusty-updates/universe amd64 Packages [241 kB]
 Get:29 http://us.archive.ubuntu.com trusty-updates/multiverse amd64 Packages [9,382 B]
 Get:30 http://us.archive.ubuntu.com trusty-updates/main i386 Packages [398 kB]
 Get:31 http://us.archive.ubuntu.com trusty-updates/restricted i386 Packages [8,846 B]
 Get:32 http://us.archive.ubuntu.com trusty-updates/universe i386 Packages [241 kB]
 Get:33 http://us.archive.ubuntu.com trusty-updates/multiverse i386 Packages [9,558 B]
 Hit http://us.archive.ubuntu.com trusty-updates/main Translation-en
 Hit http://us.archive.ubuntu.com trusty-updates/multiverse Translation-en
 Hit http://us.archive.ubuntu.com trusty-updates/restricted Translation-en
 Hit http://us.archive.ubuntu.com trusty-updates/universe Translation-en
 Hit http://us.archive.ubuntu.com trusty-backports/main Sources
 Hit http://us.archive.ubuntu.com trusty-backports/restricted Sources
 Hit http://us.archive.ubuntu.com trusty-backports/universe Sources
 Hit http://us.archive.ubuntu.com trusty-backports/multiverse Sources
 Hit http://us.archive.ubuntu.com trusty-backports/main amd64 Packages
 Hit http://us.archive.ubuntu.com trusty-backports/restricted amd64 Packages
 Hit http://us.archive.ubuntu.com trusty-backports/universe amd64 Packages
 Hit http://us.archive.ubuntu.com trusty-backports/multiverse amd64 Packages
 Hit http://us.archive.ubuntu.com trusty-backports/main i386 Packages
 Hit http://us.archive.ubuntu.com trusty-backports/restricted i386 Packages
 Hit http://us.archive.ubuntu.com trusty-backports/universe i386 Packages
 Hit http://us.archive.ubuntu.com trusty-backports/multiverse i386 Packages
 Hit http://us.archive.ubuntu.com trusty-backports/main Translation-en
 Hit http://us.archive.ubuntu.com trusty-backports/multiverse Translation-en
 Hit http://us.archive.ubuntu.com trusty-backports/restricted Translation-en
 Hit http://us.archive.ubuntu.com trusty-backports/universe Translation-en
 Ign http://us.archive.ubuntu.com trusty/main Translation-en_US
 Ign http://us.archive.ubuntu.com trusty/multiverse Translation-en_US
 Ign http://us.archive.ubuntu.com trusty/restricted Translation-en_US
 Ign http://us.archive.ubuntu.com trusty/universe Translation-en_US
 Fetched 2,380 kB in 3min 52s (10.3 kB/s)
 Temp File /tmp/ptconfigure-temp-script-74494590076.sh Removed
 E: Failed to fetch http://oss.oracle.com/debian/dists/unstable/non-free/binary-i386/oracle-xe_10.2.0.1-1.1_i386.deb  GnuTLS recv error  (-9):   A TLS packet with unexpected length was received.

 E: Unable to fetch some archives, maybe run apt-get update or try with --fix-missing?
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following extra packages will be installed:
   gcc-4.9-base:i386 libaio:i386 libc6:i386 libgcc1:i386
 Suggested packages:
  glibc-doc:i386 locales:i386
 The following NEW packages will be installed:
   gcc-4.9-base:i386 libaio:i386 libc6:i386 libgcc1:i386 oracle-xe:i386
 0 upgraded, 5 newly installed, 0 to remove and 15 not upgraded.
 16 not fully installed or removed.
 Need to get 225 MB of archives.
 After this operation, 415 MB of additional disk space will be used.
 WARNING: The following packages cannot be authenticated!
   libaio:i386 oracle-xe:i386
 Get:1 http://us.archive.ubuntu.com/ubuntu/ trusty-updates/main gcc-4.9-base i386 4.9.1-0ubuntu1 [14.9 kB]
 Get:2 http://us.archive.ubuntu.com/ubuntu/ trusty-updates/main libc6 i386 2.19-0ubuntu6.5 [4,003 kB]
 Get:3 http://oss.oracle.com/debian/ unstable/main libaio i386 0.3.104-1 [6,018 B]
 Get:4 http://oss.oracle.com/debian/ unstable/non-free oracle-xe i386 10.2.0.1-1.1 [221 MB]
 Err http://oss.oracle.com/debian/ unstable/non-free oracle-xe i386 10.2.0.1-1.1
   GnuTLS recv error (-9): A TLS packet with unexpected length was received.
 Get:5 http://us.archive.ubuntu.com/ubuntu/ trusty-updates/main libgcc1 i386 1:4.9.1-0ubuntu1 [47.9 kB]
 Fetched 4,071 kB in 8min 36s (7,880 B/s)
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ****************************** 


 Single App Installer:
 --------------------------------------------
 Oracle: Success
 ------------------------------
 Installer Finished

 ******************************

opción
--------
.. cssclass:: table-bordered

 +-----------------------+-------------------------------------------+-----------+------------------------------------------+
 | Parámetros            | Parámetro Alternativa                     | Opciones  | Comentarios                              |
 +=======================+===========================================+===========+==========================================+
 |Install Oracle?(Y/N)   | En lugar de utilizar Oracle podemos       | Y(Yes)    | Se instalará Oracle bajo ptconfigure     |
 |                       | utilizar oracle, Ora-cle                  |           | en herramientas faraón                   |
 +-----------------------+-------------------------------------------+-----------+------------------------------------------+
 |Install Oracle?(Y/N)   | En lugar de utilizar Oracle podemos       | N(No)     | La salida de sistema de la instalación   |
 |                       | utilizar oracle, Ora-cle|                 |           |                                          |
 +-----------------------+-------------------------------------------+-----------+------------------------------------------+


Beneficios
---------------

* La portabilidad es posible.
* Copia de seguridad y recuperación también disponibles.
* Alta velocidad en rendimiento.
* Soporte Multiple Database.
* Sensitibilidad caso.
* Relevante trabajar con Ubuntu y CentOS.
