============
VNCPasswd
============

sinopsis
----------------

La utilidad vncpasswd debe utilizarse para crear y cambiar las contraseñas para la autenticación del servidor VNC. Utiliza estas contraseñas cuando se inicia con el gerente de escritorio local cuando se arranca desde el guión servidor VNC. vncpasswd permite introducir una o dos contraseñas. La utilidad vncpasswd pide interactivamente si se debe establecer el segundo contraseña. Esto es más cómodo con ubunt y centos.

comando Ayuda
----------------------

Comando de Ayuda incluye una extensa, sistema de ayuda basado en la consola, que recuerda a las páginas de manual en Ubuntu. Los temas de ayuda incluyen ayuda para instalar el passward para la área remota o local. Fácil de escribir los comandos sin argumentos.

.. code-block:: bash

                ptconfigure  VNC-passwd help

La siguiente captura de pantalla puede visualizarlo.

.. code-block:: bash

 kevell@corp:/# ptconfigure VNCPasswd help

 ******************************


  This command allows you to install VNCPasswd, the popular Remote/Local Desktop Manager Solution.

  VNCPasswd, vncpasswd, vnc-passwd

        - install
        Installs VNCPasswd through a package manager
        example: ptconfigure vnc install

 ------------------------------
 End Help
 ******************************


instalación
-----------------

Instalación permite al usuario instalar vncpassward. Es muy popular en Escritorio remoto o local. Se instala el passwd vnc a través del paquete manager.The primera contraseña es la primaria, la segunda contraseña se puede utilizar para vista de sólo authentication.It cómodo con Ubuntu y CentOS.

.. code-block:: bash

                ptconfigure  VNC-passwd install

Después de clave en el comando el sistema puede pedir al usuario para la entrada. Si la entrada del usuario como Y puede instalar el VNCpassward de lo contrario puede salir. siguiente captura de pantalla puede visualizarlo.

.. code-block:: bash

 kevell@corp:/# ptconfigure VNC-passwd install

 Install VNCPasswd? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *          ! VNCPasswd !        *
 *******************************
 E: Could not get lock /var/cache/apt/archives/lock - open (11: Resource temporarily unavailable)
 E: Unable to lock directory /var/cache/apt/archives/
 Reading package lists...
 Building dependency tree...
 Reading state information...
 The following packages were automatically installed and are no longer required:
  gyp libc-ares-dev libc-ares2 libjs-node-uuid libv8-3.14-dev
  linux-headers-3.13.0-32 linux-headers-3.13.0-32-generic
  linux-image-3.13.0-32-generic linux-image-extra-3.13.0-32-generic
  node-abbrev node-ansi node-archy node-async node-block-stream
  node-combined-stream node-cookie-jar node-delayed-stream node-forever-agent
  node-form-data node-fstream node-fstream-ignore node-github-url-from-git
  node-glob node-graceful-fs node-gyp node-inherits node-ini
  node-json-stringify-safe node-lockfile node-lru-cache node-mime
  node-minimatch node-mkdirp node-mute-stream node-node-uuid node-nopt
  node-normalize-package-data node-npmlog node-once node-osenv node-qs
  node-read node-read-package-json node-request node-retry node-rimraf
  node-semver node-sha node-sigmund node-slide node-tar node-tunnel-agent
  node-which nodejs nodejs-dev ttf-dejavu-core
 Use 'apt-get autoremove' to remove them.
 The following NEW packages will be installed:
  expect
 0 upgraded, 1 newly installed, 0 to remove and 79 not upgraded.
 9 not fully installed or removed.
 [Pharaoh Logging] Adding Package expect from the Packager Apt did not execute correctly
 Enter VNC User:

 Enter VNC Pass:

 Creating /tmp/ptconfigure-temp-script-40114506906.sh
 chmod 755 /tmp/ptconfigure-temp-script-40114506906.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-40114506906.sh Permissions
 Executing /tmp/ptconfigure-temp-script-40114506906.sh
 sudo: unknown user: /usr/bin/expect
 sudo: unable to initialize policy plugin
 Temp File /tmp/ptconfigure-temp-script-40114506906.sh Removed
 [Pharaoh Logging] Removing Package expect
 E: Could not get lock /var/cache/apt/archives/lock - open (11: Resource temporarily unavailable)
 E: Unable to lock directory /var/cache/apt/archives/
 Reading package lists...
 Building dependency tree...
 Reading state information...
 Package 'expect' is not installed, so not removed
 The following packages were automatically installed and are no longer required:
  gyp libc-ares-dev libc-ares2 libjs-node-uuid libv8-3.14-dev
  linux-headers-3.13.0-32 linux-headers-3.13.0-32-generic
  linux-image-3.13.0-32-generic linux-image-extra-3.13.0-32-generic
  node-abbrev node-ansi node-archy node-async node-block-stream
  node-combined-stream node-cookie-jar node-delayed-stream node-forever-agent
  node-form-data node-fstream node-fstream-ignore node-github-url-from-git
  node-glob node-graceful-fs node-gyp node-inherits node-ini
  node-json-stringify-safe node-lockfile node-lru-cache node-mime
  node-minimatch node-mkdirp node-mute-stream node-node-uuid node-nopt
  node-normalize-package-data node-npmlog node-once node-osenv node-qs
  node-read node-read-package-json node-request node-retry node-rimraf
  node-semver node-sha node-sigmund node-slide node-tar node-tunnel-agent
  node-which nodejs nodejs-dev ttf-dejavu-core
 Use 'apt-get autoremove' to remove them.
 0 upgraded, 0 newly installed, 0 to remove and 79 not upgraded.
 9 not fully installed or removed.
 [Pharaoh Logging] Package expect from the Packager Apt is not installed, so not removed.
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 VNCPasswd: Success
 ------------------------------
 Installer Finished
 ******************************

Opciones
---------------

.. cssclass:: table-bordered

 +-------------------------+-------------------------------------+--------------+------------------------------------------------+
 | Parámetros              | Parámetro Alternativa               | Opciones     | Comentarios                                    |
 +=========================+=====================================+==============+================================================+
 |Install VNCpasswd?(Y/N)  | VNCPasswd, vncpasswd, vnc-passwd    | Y(Yes)       | Si el usuario desea continuar el proceso de    |
 |                         |                                     |              | instalación se puede introducir como Y.        |
 +-------------------------+-------------------------------------+--------------+------------------------------------------------+
 |Install VNCpasswd?(Y/N)  | VNCPasswd, vncpasswd, vnc-passwd    | N(No)        | Si el usuario desea abandonar el proceso de    |
 |                         |                                     |              | instalación se puede introducir como N.|       |
 +-------------------------+-------------------------------------+--------------+------------------------------------------------+





Beneficios
-----------------

* El soporte multi-idioma
* Autenticación VNC
* Rendimiento optimizado
* La transferencia de archivos es posible
* Estrategias de implementación de gran alcance

