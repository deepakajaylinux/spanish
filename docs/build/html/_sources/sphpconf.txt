============
phpconf
============

sinopsis
----------

Este módulo ayuda a la instalación y al igual que la gestión de la configuración de php. El usuario puede enmarcar su configuración según sus necesidades en el momento de la ejecución de la instalación.

Ayuda Comando
-------------------

El comando de ayuda guía al usuario en el trabajo con este php config. También especifica el comando que se utiliza para la instalación. El comando de ayuda también enumera los parámetros alternativos que se pueden utilizar. El comando utilizado para la opción de ayuda bajo la config php es la siguiente.

.. code-block:: bash

	ptconfigure PHPConf help

La captura de pantalla, tal como figura a continuación muestra la representación pictórica en cuanto a la utilización de la ayuda en php config.

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPConf help
 ******************************


  This command is part of Core and provides you  with a method by which you can install Apache HTTP Server

  PHPConf, php-configure, php-configuration, php-conf, phpconf

        - install
        Installs a configuration for PHP
        example: ptconfigure phpconf install

 ------------------------------
 End Help
 ******************************


instalación
-------------

Instalación de la config php es más beneficioso para los usuarios, ya que pueden enmarcar la configuración según sus necesidades. El comando utilizado para la instalación se da a continuación:

.. code-block:: bash

		ptconfigure PHPConf install

Después de introducir el comando, como se muestra por encima de las siguientes operaciones se produce como se muestra en el formato tabular.

.. code-block:: bash

 kevell@corp:/# ptconfigure PHPConf install
 Install PHP Conf? (Y/N)
 y
 *******************************
 *Pharaoh Tools*
 * PHP Conf!*
 *******************************
 Set non-default value for user_ini.filename? Default is .user.ini (Y/N)
 y
 What value for user_ini.filename?

 Set non-default value for user_ini.cache_ttl? Default is 300 (Y/N)
 
 Set non-default value for engine? Default is On (Y/N)

 Set non-default value for short_open_tag? Default is On (Y/N)

 Set non-default value for asp_tags? Default is Off (Y/N)

 Set non-default value for precision? Default is 14 (Y/N)

 Set non-default value for y2k_compliance? Default is On (Y/N)

 Set non-default value for output_buffering? Default is 4096 (Y/N)

 Set non-default value for output_handler? Default isâ€‚â€‚(Y/N)

 Set non-default value for zlib.output_compression? Default is Off (Y/N)

 Set non-default value for zlib.output_compression_level? Default is -1 (Y/N)

 Set non-default value for zlib.output_handler? Default isâ€‚â€‚(Y/N)

 Set non-default value for implicit_flush? Default is Off (Y/N)

 Set non-default value for unserialize_callback_func? Default isâ€‚â€‚(Y/N)

 Set non-default value for serialize_precision? Default is 17 (Y/N)

 Set non-default value for allow_call_time_pass_reference? Default is Off (Y/N)

 Set non-default value for safe_mode? Default is Off (Y/N)

 Set non-default value for safe_mode_gid? Default is Off (Y/N)

 Set non-default value for safe_mode_exec_dir? Default isâ€‚â€‚(Y/N)

 Set non-default value for safe_mode_allowed_env_vars? Default is PHP_ (Y/N)

 Set non-default value for safe_mode_protected_env_vars? Default is LD_LIBRARY_PATH (Y/N)

 Set non-default value for open_basedir? Default isâ€‚â€‚(Y/N)

 Set non-default value for disable_functions? Default is pcntl_alarm,pcntl_fork,pcntl_waitpid,pcntl_wait,pcntl_wifexited,pcntl_wifstopped,pcntl_wifsignaled,pcntl_wexitstatus,pcntl_wtermsig,pcntl_wstopsig,pcntl_signal,pcntl_signal_dispatch,pcntl_get_last_error,pcntl_strerror,pcntl_sigpr ocmask,pcntl_sigwaitinfo,pcntl_sigtimedwait,pcntl_exec,pcntl_getpriority,pcntl_setpriority, (Y/N)

 Set non-default value for disable_classes? Default isâ€‚â€‚(Y/N)

 Set non-default value for ignore_user_abort? Default is On (Y/N)

 Set non-default value for realpath_cache_size? Default is 16k (Y/N)

 Set non-default value for realpath_cache_ttl? Default is 120 (Y/N)

 Set non-default value for zend.enable_gc? Default is On (Y/N)

 Set non-default value for expose_php? Default is On (Y/N)

 Set non-default value for max_execution_time? Default is 30 (Y/N)

 Set non-default value for max_input_time? Default is 60 (Y/N)

 Set non-default value for max_input_nesting_level? Default is 64 (Y/N)

 Set non-default value for max_input_vars? Default is 1000 (Y/N)

 Set non-default value for memory_limit? Default is 128M (Y/N)



 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 PHPConf: Success
 ------------------------------
 Installer Finished
 ******************************

Opciones
-----------
.. cssclass:: table-bordered

 +-----------------------+--------------------------------------------+-----------+-----------------------------------------------+
 | Parámetros            | Parámetro Alternativa                      | Opciones  | Comentarios                                   |
 +=======================+============================================+===========+===============================================+
 |Install PHPConf? (Y/N) | En lugar de PHP Conf estos nombres         | Y(Yes)    | Si el usuario desea continuar el proceso      |
 |                       | alternativos pueden ser utilizados:        |           | nstalación que puede introducir como Y        |
 |                       | php-configure, php-conf php-configuration, |           |                                               |
 |                       | phpconf                                    |           |                                               |
 +-----------------------+--------------------------------------------+-----------+-----------------------------------------------+
 |Install PHPConf? (Y/N) | En lugar de PHP Conf estos nombres         | N(No)     | Si el usuario desea abandonar el proceso      |
 |                       | alternativos pueden ser utilizados:        |           | de instalación se puede introducir como N.    |
 |                       | php-configure, php-conf php-configuration, |           |                                               |
 |                       | phpconf|                                   |           |                                               |
 +-----------------------+--------------------------------------------+-----------+-----------------------------------------------+


Si el usuario continúa el proceso de instalación, durante la ejecución de la instalación, el módulo especifica el valor por defecto de la configuración y también se pregunta al usuario hablar de los valores no predeterminados para la configuración según sus necesidades. Las especificaciones para la configuración durante la instalación de A continuación se relacionan:

* Relación calidad user_ini.filename
* Valor de user_ini.cache_ttl?
* Valor para el motor.
* Valor de short_open_tag.
* Valor de asp_tags.
* Valor de la precisión.
* Valor de y2k_compliance.
* Valor de output_buffering.
* Valor de output_handler.
* Valor de zlib.output_compression.
* Valor de zlib.output_compression_level.
* Valor de zlib.output_handler.
* Valor de implicit_flush.
* Valor de unserialize_callback_func.
* Valor de la precisión serialize.
* Valor de allow_call_time_pass_reference.
* Valor de safe_mode.
* Valor de safe_mode_gid.
* Valor de safe_mode_exec_dir?
* Valor de safe_mode_allowed_env_vars.
* Valor de BASEDIR abierto.
* Valor para desactivar funciones.
* Valor de disable_classes?
* Valor de ignore_user_abort
* Valor de realpath_cache_size?
* Valor de realpath_cache_ttl.
* Valor de zend.enable_gc.
* Valor de expose_php.
* Valor de max_execution_time.
* Valor de max_input_time.
* Valor de max_input_nesting_level.
* Valor de max_input_vars.
* Valor de memory_limits.

Después de mirar los valores por defecto para las funciones de configuración, el usuario puede decidir sus acciones. Si son roble con valores predeterminados que pueden ingresarse como N. Si se requieren para especificar los valores de configuración que pueden ingresarse como Y. La captura de pantalla como se muestra a continuación explica el proceso descrito anteriormente visualmente.

Beneficios
--------------

* Los parámetros utilizados para definir la instalación y el comando de ayuda no distingue entre mayúsculas y minúsculas.
* Los usuarios pueden enmarcar las funciones de configuración en el tiempo de ejecución de la instalación.
* Funciona bien tanto en OS Cent y ventanas.
