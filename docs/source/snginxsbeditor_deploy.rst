===============
NginxSBEditor
===============

Sinopsis
----------

Este módulo es una parte bien de módulos predeterminados y encarga de las funciones de Nginx ServerBlocks. Vamos a ver sobre las metodologías para el uso de esto y también sobre las funciones bajo este editor nginx en próximos temas.


comando Ayuda
---------------------

El comando help envuelve toda la información necesaria con respecto a NginxSBEditor como sus principales usos, la lista de parámetros alternativos que pueden utilizarse en la declaración, qué función primaria de NginxSBEditor (Ex: agregar, quitar, lista, activar, desactivar) y también la sintaxis utilizada para declarar esas funciones interesantes. El siguiente comando se utiliza para declarar la opción ayuda en NginxSBEditor,


.. code-block:: bash

	ptdeploy NginxSBEditor help


La captura de pantalla siguiente muestra gráficamente sobre el funcionamiento del comando help.


.. code-block:: bash

 kevell@corp:/# ptdeploy NginxSBEditor help
 ******************************


  This command is part of Default Modules and handles Nginx ServerBlocks Functions.

  NginxSBEditor, nginx-sb-editor, nginxsbe

          - add
          create a Server Block
          example: ptdeploy nginxsbe add
          sb-docroot
          sb-url
          sb-ip-port

          - rm
          remove a Server Block
          example: ptdeploy nginxsbe rm

          - list
          List current Server Blocks
          example: ptdeploy nginxsbe list

          - enable
          enable a Server Block
          example: ptdeploy nginxsbe enable

          - disable
          disable a Server Block
          example: ptdeploy nginxsbe disable

 ------------------------------
 End Help
 ******************************

Cómo utilizar
---------------

Como representado y explicado en el anterior comando help, el NginxSBEditor, tiene las siguientes funciones,


* Add
* Remove
* List
* Enable
* Disable


Vamos a ver cómo utilizar estas funciones interesantes bajo NginxSBEditor.


Add
----

El papel de esta función es crear o agregar un nuevo bloque de servidor. El comando y el trabajo de agregar funciones es representado por debajo,


.. code-block:: bash

	ptdeploy NginxSBEditor add

Después de introducir el mandato dado por encima, se muestra a continuación, el funcionamiento de esta función agregar



.. cssclass:: table-bordered

 +------------------------+----------------------------------------------+-----------+-------------------------------------------------------+
 | parámetros		  | parámetro alternativo	                 | opciones  | comentarios       		                     |
 +========================+==============================================+===========+=======================================================+
 |Do you want to add a 	  | En lugar de NginxSBEditor , podemos utilizar | Y(Yes)    | Si el usuario tiene que agregar un nuevo servidor     |
 |ServerBlock? (Y/N)      | nginx-sb-editor, nginxsbe también            |           | bloque se puede introducir como Y.                    |
 +------------------------+----------------------------------------------+-----------+-------------------------------------------------------+
 |Do you want to add a 	  | En lugar de NginxSBEditor , podemos utilizar | N(No)     | Si el usuario no está en necesidad de añadir una      |
 |ServerBlock? (Y/N)	  | nginx-sb-editor, nginxsbe también            | 	     | nuevo bloque de servidor que puede introducir como N| |
 +------------------------+----------------------------------------------+-----------+-------------------------------------------------------+

Si el usuario continúa agregando los bloques del servidor durante el proceso de agregar los siguientes pasos están involucrados.


Step 1:

What is document root?

El usuario se especifica la raíz, si no desean continuar con el valor por defecto.

Step 2:

What URL do you want to add as server name?

El usuario debe especificar la dirección url que se supone para añadir.

Step 3:

What IP? Port should be set?

El usuario se especificar la IP, si no desean continuar con el valor por defecto.

Step 4:

What is your ServerBlock Template directory?

El usuario se especifique el directorio, si no desean continuar con el valor por defecto.

Step 5:

Please check the ServerBlock
El usuario ha Compruebe la pantalla de salida del bloque de servidor que se añade y asegurar.


Step 6:

Is this Okay? (Y/N)

Si el usuario está feliz con el resultado generado, puede introducir como Y demás N.

Step 7:

What is your ServerBlock directory?

El usuario se especifique el directorio.


Step 8:

Do you want to enable a server block? (Y/N)

El usuario tiene que entrar como Y o N dependiendo de sus necesidades.


Step 9:

What is your Enabled Symlink ServerBlock directory.

Si un bloque de servidor está activado, el usuario debe especificar su directorio.


La captura de pantalla siguiente muestra visualmente el proceso explicado anteriormente.


.. code-block:: bash

 kevell@corp:/# ptdeploy nginxsbe add
 Do you want to add a ServerBlock? (Y/N) 
 Y
 What's the document root? Enter nothing for /
 /root/Nginx
 What URL do you want to add as server name?
 www.ngx.com
 What IP:Port should be set? Enter nothing for 127.0.0.1:80

 What is your ServerBlock Template directory? Enter nothing for default templates
 /root/Nginxdir
 Please Choose ServerBlock Template: 
 --- Default Server Block Templates: ---
 (0) docroot-no-suffix
 (1) docroot-src-sfx
 (2) docroot-web-suffix
 (3) docroot-www-suffix
 (4) docroot-docroot-suffix

 3
 Please check ServerBlock: server {
        listen   127.0.0.1:80 ; ## listen for ipv4; this line is default and implied
        #listen   [::]:80 default ipv6only=on; ## listen for ipv6

        root /root/Nginx/www ;
        index index.html index.htm index.php;

        # Make site accessible from http://localhost/
        server_name www.ngx.com ;

        # pass the PHP scripts to FastCGI server listening on 127.0.0.1:9000
        #
        location ~ \.php$ {
                try_files $uri =404;
                fastcgi_split_path_info ^(.+\.php)(/.+)$;
                fastcgi_pass 127.0.0.1:9000;
                fastcgi_index index.php;
                include fastcgi_params;
        }

 }

 Is this Okay? (Y/N) 
 Y
 What is your ServerBlock directory?
 /root/Nginxdir
 Do you want to enable a ServerBlock? (Y/N) 
 Y
 What is your Enabled Symlink ServerBlock directory?
 /home/Nginxsymlink
 Server Block Enabled Symlink Created
 ******************************
 

 1ServerBlock Creator Finished
 ******************************




Remove
----------

Al eliminar la función se utiliza para quitar los bloques de servidor no deseados. Esto puede hacerse utilizando el comando siguiente,


.. code-block:: bash

	ptdeploy NginxSBEditor rm

Después de introducir el comando anterior, el siguiente proceso de eliminación, como se muestra en la table



.. cssclass:: table-bordered

 +------------------------+----------------------------------------------+-----------+----------------------------------------------------+
 | parámetros             | parámetro alternativo                        | opciones  | comentarios                                        |
 +========================+==============================================+===========+====================================================+
 |Do you want to delete   | En lugar de NginxSBEditor , podemos utilizar | Y(Yes)    | Si el usuario tiene que eliminar el servidor       |
 |a ServerBlock/s? (Y/N)  | nginx-sb-editor, nginxsbe también            |           | bloque se puede introducir como Y.                 |
 +------------------------+----------------------------------------------+-----------+----------------------------------------------------+
 |Do you want to delete   | En lugar de NginxSBEditor , podemos utilizar | N(No)     | Si el usuario no está en la necesidad de eliminar  |
 |a ServerBlock/s? (Y/N)  | nginx-sb-editor, nginxsbe también            |           | el bloque de servidor que puede introducir como N| |
 +------------------------+----------------------------------------------+-----------+----------------------------------------------------+


Si el usuario procede eliminar los bloques de servidor durante este proceso están implicados los siguientes pasos.


Step 1:

Deleting ServerBlock

What is your ServerBlock directory?

El usuario tiene que especificar el directorio.


Step 2:

Please Choose ServerBlock

--All Server Blocks: ---

(0) www.ngn.com

(1) www.ngx.com

(2) www.nx.com

El usuario debe especificar los valores de 0 a 2 dependiendo de sus necesidades.


Step 3:

!! Sure? Definitely delete ServerBlock? (Y/N) !!

El usuario debe especificar Y o N dependiendo de sus necesidades.


Step 4:

Do you want to disable a ServerBlock? (Y/N)

El usuario debe especificar Y o N dependiendo de sus necesidades.


Step 5:

What is your Enabled Symlink ServerBlock directory?

El usuario tiene que especificar el directorio.


La siguiente captura representa visualmente sobre el proceso de eliminación.



.. code-block:: bash

 kevell@corp:/# ptdeploy nginxsbe rm
 Do you want to delete ServerBlock/s? (Y/N) 
 Y
 Deleting ServerBlock
 What is your ServerBlock directory?
 /root/Nginxdir
 Please Choose ServerBlock:
 ---All Server Blocks: ---
 (0) www.ngn.com
 (1) www.ngx.com
 (2) www.nx.com

 2
 !! Sure? Definitely delete ServerBlock? (Y/N) !!
 Y
 Do you want to disable a ServerBlock? (Y/N) 
 Y
 What is your Enabled Symlink ServerBlock directory?
 /root/home/Nginxsymlink
 Server Block www.nx.com Disabled if existed
 Server Block www.nx.com Deleted if existed
 *******************************


 1ServerBlock Creator Finished
 ******************************


List
----

La función de la opción de la lista es enumerar los bloques instalado el servidor actual. Se da el comando utilizado para la lista de abajo,


.. code-block:: bash

	ptdeploy NginxSBEditor list

Después de introducir el comando anterior, el siguiente proceso de opción de la lista.


Step 1:

What is your ServerBlock directory?

El usuario tiene que especificar el directorio.

Step 2:

What is your Enabled Symlink ServerBlock directory?

El usuario tiene que especificar el directorio.

Después de estos pasos, se muestran él enumera de ServerBlocks instalado actualmente.


La captura de pantalla siguiente muestra el funcionamiento de la opción de la lista visualmente.


.. code-block:: bash


 kevell@corp:/# ptdeploy nginxsbe list
 What is your ServerBlock directory?
 /root/Nginxdir
 What is your Enabled Symlink ServerBlock directory?

 Current Installed ServerBlocks:
 --- Enabled Server Blocks: ---
 (0) www.ngn.com
 (1) www.ngx.com
 --- All Available Server Blocks: ---
 (2) www.ngn.com
 (3) www.ngx.com
 ******************************


 1ServerBlock Creator Finished
 ******************************


Enable
----------

La función de habilitación se utiliza para habilitar un serverblock . El comando utilizado para permitir se muestra a continuación,

.. code-block:: bash

	ptdeploy nginxsbe enable

.. code-block:: bash


 kevell@corp:/# ptdeploy nginxsbe enable

 Do you want to enable a ServerBlock? (Y/N) 
 y
 What is your Enabled Symlink ServerBlock directory? Found "/etc/nginx/sites-enabled" - Enter nothing to use this

 Please Choose ServerBlock:
 --- All Server Blocks: ---
 (0) ServerBlocktemp
 (1) aaaaaa
 (2) as
 (3) ddd
 (4) default
 (5) default.dpkg-old
 (6) dfdkdfsd.com
 (7) dfsdfssfdfdfdf.com
 (8) google
 (9) karuna
 (10) kkkkkkk
 (11) kumark
 (12) sites-available
 (13) vijay
 (14) www.amazon.com
 (15) www.deepak.com
 (16) www.google.com
 (17) www.kkk.com

 1
 Server Block Enabled Symlink Created
 ******************************
 ServerBlock Creator Finished
 ******************************


Disable
-----------

La función de bloqueo se utiliza para desactivar un bloque de servidor. El comando para deshabilitar se enumeran a continuación ,

.. code-block:: bash

	ptdeploy nginxsbe disable

.. code-block:: bash


 kevell@corp:/# ptdeploy nginxsbe disable

 Do you want to disable a ServerBlock? (Y/N) 
 y
 What is your Enabled Symlink ServerBlock directory? Found "/etc/nginx/sites-enabled" - Enter nothing to use this

 Please Choose ServerBlock:
 --- All Server Blocks: ---
 (0) ServerBlocktemp
 (1) aaaaaa
 (2) as
 (3) ddd
 (4) default
 (5) default.dpkg-old
 (6) dfdkdfsd.com
 (7) dfsdfssfdfdfdf.com
 (8) google
 (9) karuna
 (10) kkkkkkk
 (11) kumark
 (12) sites-available
 (13) vijay
 (14) www.amazon.com
 (15) www.deepak.com
 (16) www.google.com
 (17) www.kkk.com

 1
 Server Block aaaaaa Disabled  if exist
 ******************************
 ServerBlock Creator Finished
 ******************************


Beneficios
----------

* Es acomodada en ambos ubuntu y así como ciento OS. 
* Los parámetros utilizados en la declaración no es sensible a mayúsculas. 
* Los usuarios pueden visualizar la lista de bloques de servidor disponibles y actualmente instaladas, incluso antes de añadir o eliminar 
  un bloque de servidor.


