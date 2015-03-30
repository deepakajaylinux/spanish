============
MediaTools
============

sinopsis
------------

Este módulo tiene como objetivo instalar GC recomendado Media Tool como VLC Media Player que mejora la productividad de los usuarios del sistema. VLC Media Player soporta varios métodos de compresión de audio y vídeo y formatos de archivo, incluyendo DVD-Vídeo, CD de vídeo y protocolos streaming. VLC media player (comúnmente conocido como VLC) es un portátil, libre y de código abierto, multiplataforma reproductor multimedia y servidor de streaming de medios de comunicación escrita por el proyecto VideoLAN. Veamos cómo este módulo ayuda a la instalación de VLC.

Ayuda Comando
--------------------

El comando de ayuda conduce a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en el módulo de herramientas de medios. Las listas de comandos de ayuda fuera de los parámetros alternativos de herramientas de medios. También se describe la sintaxis para la instalación de VLC. El comando de ayuda para el módulo de herramientas de medios se muestra a continuación.

.. code-block:: bash
  
 ptconfigure mediatools help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda en virtud de las herramientas de medios.

.. code-block:: bash


	Kevell@corp:/# ptconfigure MediaTools help
	******************************


	This command allows you to install a few GC recommended Media Tools
        for productivity in your system. Currently, we're only including
        VLC Media Player

         MediaTools, media-tools, mediatools, mediatools, media-tools

        - install
        Installs some media tools
        example: ptconfigure mediatools install

	------------------------------
	End Help

	------------------------------

instalación
---------------

El siguiente comando utiliza para instalar las herramientas de medios.

.. code-block:: bash

	ptconfigure mediatools install

La captura de pantalla a visualizar su función.

.. code-block:: bash


        - install
        Installs some media tools
        example: ptconfigure mediatools install

        ------------------------------
        End Help


Si el usuario continúa el proceso de instalación, el siguiente proceso ocurre durante la instalación.

* Extrae plantillas de paquetes
* Lee las listas de paquetes.
* Construye árbol de dependencias.
* Lee la información de estado.
* Enumera los paquetes que se instalan automáticamente.
* Enumera los paquetes adicionales que se instalan.
* Enumera los paquetes sugeridos.
* Enumera los nuevos paquetes que están instalados.
* Por último, los informes se muestran claramente con el estado y los resultados.
* La siguiente captura de pantalla explica el proceso mencionado anteriormente pictóricamente.

.. code-block:: bash


 kevell@corp:/# ptconfigure mediatools install 
 Install Media Tools? (Y/N) 
 y 
 ******************************* 
 *        Pharaoh Tools        * 
 *         Media Tools!        * 
 ******************************* 
 [Pharaoh Logging] Packages vlc, libdvdread4 from the Packager Apt are already installed, so not installing 
 Creating /tmp/ptconfigure-temp-script-57996813529.sh 
 chmod 755 /tmp/ptconfigure-temp-script-57996813529.sh 2>/dev/null 
 Changing /tmp/ptconfigure-temp-script-57996813529.sh Permissions 
 Executing /tmp/ptconfigure-temp-script-57996813529.sh 
 --2015-03-27 13:21:10--  http://download.videolan.org/pub/debian/stable//Packages 
 Resolving download.videolan.org (download.videolan.org)... 88.191.250.2 
 Connecting to download.videolan.org (download.videolan.org)|88.191.250.2|:80... connected. 
 HTTP request sent, awaiting response... 200 OK 
 Length: 3520 (3.4K) [application/octet-stream] 
 Saving to: â€˜/tmp/dvdcss-2TJ4IX/Packagesâ€™ 

 100%[=======================================================================================================>] 3,520       --.-K/s   in 0s      

 2015-03-27 13:21:11 (77.0 MB/s) - â€˜/tmp/dvdcss-2TJ4IX/Packagesâ€™ saved [3520/3520] 

 --2015-03-27 13:21:12--  http://download.videolan.org/pub/debian/stable/stable/libdvdcss2_1.2.13-0_amd64.deb 
 Resolving download.videolan.org (download.videolan.org)... 88.191.250.2 
 Connecting to download.videolan.org (download.videolan.org)|88.191.250.2|:80... connected. 
 HTTP request sent, awaiting response... 200 OK 
 Length: 44462 (43K) [application/octet-stream] 
 Saving to: â€˜/tmp/dvdcss-2TJ4IX/libdvdcss.debâ€™ 

 100%[=======================================================================================================>] 44,462      65.6KB/s   in 0.7s   

 2015-03-27 13:21:13 (65.6 KB/s) - â€˜/tmp/dvdcss-2TJ4IX/libdvdcss.debâ€™ saved [44462/44462] 

 Selecting previously unselected package libdvdcss2. 
 (Reading database ... 362949 files and directories currently installed.) 
 Preparing to unpack .../dvdcss-2TJ4IX/libdvdcss.deb ... 
 Unpacking libdvdcss2 (1.2.13-0) ... 
 Setting up libdvdcss2 (1.2.13-0) ... 
 Processing triggers for libc-bin (2.19-0ubuntu6.6) ... 
 Temp File /tmp/ptconfigure-temp-script-57996813529.sh Removed 
 ... All done! 
 ******************************* 
 Thanks for installing , visit www.pharaohtools.com for more 
 ****************************** 

 
 Single App Installer: 
 -------------------------------------------- 
 MediaTools: Success 
 ------------------------------ 
 Installer Finished 
 ****************************** 


Opciones
-----------

.. cssclass:: table-bordered

 +---------------------+--------------------------------------+------------+-----------------------------------------+
 | Parámetros          | Parámetro Alternativa                | Opciones   | Comentarios                             |
 +=====================+======================================+============+=========================================+
 |Install Media        | En lugar de herramientas de medios,  | Y(Yes)     | Si el usuario desea continuar el        |
 |Tools? (Y/N)         | las siguientes alternativas también  |            | proceso de instalación se puede         |
 |                     | pueden utilizarse: MediaTools,       |            | introducir como Y                       |
 |                     | media-tools, mediatools.             |            |                                         |
 +---------------------+--------------------------------------+------------+-----------------------------------------+
 |Install Media        | En lugar de herramientas de medios,  | N(No)      | Si el usuario desea abandonar el        |
 |Tools? (Y/N)         | las siguientes alternativas también  |            | proceso de instalación se puede         |
 |                     | pueden utilizarse: MediaTools,       |            | introducir como N                       |
 |                     | media-tools, mediatools.|            |            |                                         |
 +---------------------+--------------------------------------+------------+-----------------------------------------+

Beneficios
------------

* Los parámetros utilizados en ayuda de instalación y operaciones no son sensibles, que es una ventaja añadida, mientras que en comparación 
  con otros.
* El uso de este módulo de la productividad del sistema se puede mejorar.
* Es-acomodados tanto en Ubuntu y así como Cent OS.
* Este módulo facilita la instalación de GC recomendado herramientas de medios.
