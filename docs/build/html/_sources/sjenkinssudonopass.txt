==================
JenkinsSudoNoPass
==================

sinopsis
------------

Jenkins es un servidor de creación popular. JenkinsÂ proporciona servicios de integración continua foros de desarrollo de software. Jenkinssudonopass tolera el usuario para unir una entrada al archivo sudo sistema. Esto puso a los jenkins usuario para funcionar con fuera passward. Esto es adecuado para Ubuntu y centOS.

comando Ayuda
-----------------------

El comando ayuda a controlar los usuarios en cuanto a la finalidad y, así como acerca de las opciones que se incluyen en el módulo jenkinssudonopass. Las listas de comandos de ayuda fuera de los parámetros alternativos de jenkinssudonopass. También se describe la sintaxis para utilizar jenkinssudonopass a Securify. El comando de ayuda para jenkinssudonopass es la siguiente.

.. code-block:: bash

		ptconfigure Jenkinssudonopass help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda bajo jenkinssudonopass.

.. code-block:: bash

 kevell@corp:/# ptconfigure JenkinsSudoNoPass help
 ******************************


  This command allows you to add an entry to the system sudo file that will
  allow your Jenkins user to have passwordless sudo. This is required for
  quite a few of the Jenkins builds provided by Golden Contact, as Jenkins
  will perform test execution, software installs and more, silently.

  JenkinsSudoNoPass, jenkinssudonopass, jenkins-sudo-nopass, jenkins-sudo-passwordless

        - install
        Installs the Jenkins sudo without password entry
        example: ptconfigure jenkins-sudo-nopass install

 ------------------------------
 End Help
 ******************************

instalación
-----------------

Este comando autoriza a instalar jenkins sudo sin entrada de palabra pase. Cuando el usuario desea instalar jenkinssudonopass el comando siguiente guía al usuario para instalar.

.. code-block:: bash

                ptconfigure Jenkinssudonopass install

Después de escribir este comando el sistema pide que los usuarios desean. El otro proceso explica la instalación a través de la pantalla.

.. code-block:: bash

 kevell@corp:/# ptconfigure jenkinssudonopass install
 Install Sudo w/o Pass for Jenkins User? (Y/N) 
 Y
 *******************************
 *        Pharaoh Tools        *
 *         Jenk Sudo Ps        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-2682022801.sh
 chmod 755 /tmp/ptconfigure-temp-script-2682022801.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-2682022801.sh Permissions
 Executing /tmp/ptconfigure-temp-script-2682022801.sh
 The following will be written to /etc/sudoers
 Please check if it looks wrong
 It may break your system if wrong !!!
 jenkins ALL=NOPASSWD: ALL
 Temp File /tmp/ptconfigure-temp-script-2682022801.sh Removed
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 JenkinsSudoNoPass: Success
 ------------------------------
 Installer Finished
 ******************************


Opciones
-----------
.. cssclass:: table-bordered

 +--------------------------+------------------------------------+------------+--------------------------------------------+
 | Parámetros               | Parámetro Alternativa              | Opciones   | Comentarios                                |
 +==========================+====================================+============+============================================+
 |Install sudo w/o for      | En lugar de jenkinssudonopass, las | Y(Yes)     | Si el usuario desea continuar el proceso   |
 |Jenkins user? (Y/N)       | siguientes alternativas también se |            | de instalación se puede introducir como Y. |
 |                          | pueden utilizar: JenkinsSudoNoPass |            |                                            |
 |                          | , jenkinssudonopass,               |            |                                            |
 |                          | jenkins-sudo-nopass,               |            |                                            |
 |                          | jenkins-sudo-passwordless          |            |                                            |
 +--------------------------+------------------------------------+------------+--------------------------------------------+
 |Install sudo w/o for      | En lugar de jenkinssudonopass, las | N(No)      | Si el usuario desea abandonar el proceso   |
 |Jenkins user? (Y/N)       | siguientes alternativas también se |            | de instalación se puede introducir como N. |
 |                          | pueden utilizar: JenkinsSudoNoPass |            |                                            |
 |                          | , jenkinssudonopass,               |            |                                            |
 |                          | jenkins-sudo-nopass,               |            |                                            |
 |                          | jenkins-sudo-passwordless|         |            |                                            |
 +--------------------------+------------------------------------+------------+--------------------------------------------+


Beneficios
-------------

* Abrir fuente proceso de integración continua.
* Jenkinssudonopass es una automatización construye.
* Por scripting construye y eliminar problemas de errores humanos, las computadoras son apenas mejor en la ejecución de tareas repetitivas.
* Jenkinssudonopass necesita gastar tiempo en sus despliegues
* Versatilidad y flexibilidad.
