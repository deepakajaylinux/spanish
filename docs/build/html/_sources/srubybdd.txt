=========
RubyBDD
=========

sinopsis
------------------

Rubí Behaviour Driven Development (BDD) te ofrece la mejor de Test Driven Development, Domain Driven Design, y prueba de aceptación de técnicas de planificación Driven, por lo que el usuario puede instalar Rubí BDD para un mejor software con auto-documentado, pruebas ejecutables que aportan los usuarios y desarrolladores juntos con un lenguaje PHP. Se consuela con Ubuntu y CentOS.

comando Ayuda
------------------------

El comando de ayuda conduce a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en los módulos de Ruby BDD. El comando help enumera los parámetros alternativos de Ruby Bdd bajo módulo ptconfigure. También se describe la sintaxis para la instalación de updation del usuario. El comando de ayuda para Ruby Bdd se muestra a continuación.

.. code-block:: bash

		ptconfigure Ruby Bdd help

La siguiente captura de pantalla muestra el esfuerzo total de Rubí Bdd.

.. code-block:: bash

 kevell@corp:/# ptconfigure RubyBDD help

 ******************************


  This command allows you to install Ruby RVM.

  RubyBDD, rubybdd, ruby-bdd

        - install
        Installs Ruby BDD Gems
        example: ptconfigure ruby-bdd install

 ------------------------------
 End Help
 ******************************

instalación
-------------------

Instalación incluye la instalación de Rubí Bdd requerida para hacer la instalación en una versión actualizada. Es un proceso de manifiesto para instalar el módulo de Ruby Bdd bajo ptconfigure sólo por el uso de la orden dada a continuación,

.. code-block:: bash

	ptconfigure Ruby Bdd Install

Después de vitalizar el comando se catequizar entrada.
Cuando la entrada de usuario como si automáticamente se instalará Rubí Bdd con la comprobación del sistema. Si no salir de la instalación. La siguiente captura de pantalla demuestra.

.. code-block:: bash

 kevell@corp:/# ptconfigure ruby-bdd install

 Install Ruby BDD? (Y/N)
 Y
 *******************************
 *        Pharaoh Tools        *
 *          !Ruby BDD!!        *
 *******************************
 ERROR:  Error installing cucumber:
	ERROR: Failed to build gem native extension.

        /usr/bin/ruby1.9.1 extconf.rb
 /usr/lib/ruby/1.9.1/rubygems/custom_require.rb:36:in `require': cannot load such file -- mkmf (LoadError)
	from /usr/lib/ruby/1.9.1/rubygems/custom_require.rb:36:in `require'
	from extconf.rb:1:in `<main>'


 Gem files will remain installed in /var/lib/gems/1.9.1/gems/gherkin-2.12.2 for inspection.
 Results logged to /var/lib/gems/1.9.1/gems/gherkin-2.12.2/ext/gherkin_lexer_ar/gem_make.out
 INFO:  `gem install -y` is now default and will be removed
 INFO:  use --ignore-dependencies to install only the gems you list
 Building native extensions.  This could take a while...
 [Pharaoh Logging] Adding Package cucumber from the Packager Gem did not execute correctly
 ERROR:  Error installing capybara:
	ERROR: Failed to build gem native extension.

        /usr/bin/ruby1.9.1 extconf.rb
 /usr/lib/ruby/1.9.1/rubygems/custom_require.rb:36:in `require': cannot load such file -- mkmf (LoadError)
	from /usr/lib/ruby/1.9.1/rubygems/custom_require.rb:36:in `require'
	from extconf.rb:4:in `<main>'


 Gem files will remain installed in /var/lib/gems/1.9.1/gems/nokogiri-1.6.6.2 for inspection.
 Results logged to /var/lib/gems/1.9.1/gems/nokogiri-1.6.6.2/ext/nokogiri/gem_make.out
 INFO:  `gem install -y` is now default and will be removed
 INFO:  use --ignore-dependencies to install only the gems you list
 Building native extensions.  This could take a while...
 [Pharaoh Logging] Adding Package capybara from the Packager Gem did not execute correctly
 ERROR:  While executing gem ... (Gem::DependencyError)
     Unable to resolve dependencies: calabash-android requires rubyzip (~> 0.9.9); xamarin-test-cloud requires rubyzip (~> 1.1)
 INFO:  `gem install -y` is now default and will be removed
 INFO:  use --ignore-dependencies to install only the gems you list
 [Pharaoh Logging] Adding Package calabash from the Packager Gem did not execute correctly
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************
 

 Single App Installer:
 --------------------------------------------
 RubyBDD: Success
 ------------------------------
 Installer Finished
 ******************************

Opciones
---------------

.. cssclass:: table-bordered

 +--------------------------+-------------------------------------------+--------------+--------------------------------------------+
 | Parámetros               | Parámetro Alternativa                     | Opciones     | Comentarios                                |
 +==========================+===========================================+==============+============================================+
 |Install RubyBdd?(Y/N)     | En lugar de utilizar RubyBdd podemos usar | Y(Yes)       | Se instalará RubyBdd bajo ptconfigure en   |
 |                          | ruby-bdd,rubybdd                          |              | herramientas Faraón                        |
 +--------------------------+-------------------------------------------+--------------+--------------------------------------------+
 |Install RubyBdd?(Y/N)     | En lugar de utilizar RubyBdd podemos usar | N(No)        | La salida de sistema de la instalación     |
 |                          | ruby-bdd,rubybdd|                         |              |                                            |
 +--------------------------+-------------------------------------------+--------------+--------------------------------------------+


Beneficios
----------------

* Rubybdd es acomodado en Ubuntu y CentOS
* Rubybdd apoya sensibilidad no caso
* Rubybdd es flexible
* Otra gran ventaja de tener BDD son el desarrollo impulsado por el usuario puede actualizar como versión más reciente de rubybdd, y nivel de 
  parche, de rubí.
* Rubybdd utiliza para la instalación
