============
OpenOffice
============

sinopsis
------------

Este módulo actúa como facilitador para instalar Openoffice .Open-office es la suite abierta premier de software relacionados con la oficina. Veamos el uso y las metodologías de la instalación de la oficina abierta en los próximos temas.

Ayuda Comando
----------------------

El comando help guía a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en el módulo de Open Office. En él se enumeran los parámetros alternativos de módulo de Open Office. También describe la sintaxis para instalar el módulo de Open Office. El comando de ayuda para el módulo de Open Office se muestra a continuación.

.. code-block:: bash

		ptconfigure OpenOffice help


La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda en virtud de Open Office.

.. code-block:: bash

 kevell@corp:/# ptconfigure openoffice help

 ******************************


  This command allows you to install OpenOffice.

  OpenOffice,openoffice,Openoffice

        - install
        Installs OpenOffice.
        example: ptconfigure openoffice install

 ------------------------------
 End Help
 ******************************

instalación
--------------

El comando utilizado para instalar el Open Office en el equipo del usuario se muestra a continuación:

.. code-block:: bash

		ptconfigure openoffice install

Después de introducir el comando anterior, el siguiente proceso se produce como se muestra en el formato tabular.

.. cssclass:: table-bordered

 +-----------------------+-------------------------------------------------+-------------+-----------------------------------------------+
 | Parámetros            | Parámetro Alternativa                           | Opciones    | Comentarios                                   |
 +=======================+=================================================+=============+===============================================+
 |Install Open Office?   | En lugar de openoffice, podemos utilizar        | Y(Yes)      | Si el usuario desea continuar el proceso      |
 |(Y/N)                  | OpenOffice, Openoffice también.                 |             | de instalación se puede introducir como Y.    |
 +-----------------------+-------------------------------------------------+-------------+-----------------------------------------------+
 |Install Open Office?   | En lugar de openoffice, podemos utilizar        | N(No)       | Si el usuario desea abandonar el proceso      |
 |(Y/N)                  | OpenOffice, Openoffice también.                 |             | de instalación se puede introducir como N.|   |
 +-----------------------+-------------------------------------------------+-------------+-----------------------------------------------+

Si el usuario procede de la instalación, durante el proceso de instalación se describe en las listas siguientes:

* Lee las listas de paquetes.
* Construye el árbol de dependencias.
* Lee la información de estado.
* Lista outs los paquetes que se instalan automáticamente.
* Lista outs el paquete adicional que está instalando.
* Lista outs los paquetes sugeridos.
* Lista outs los nuevos paquetes que está instalando.
* Los detalles sobre el número de archivos actualizados, recién instalados, retirados y no actualizados.
Finalmente, el proceso de instalación se completó. La siguiente captura de pantalla representar visualmente el proceso de instalación de la Oficina abierta.
.. code-block:: bash

Beneficios
--------------

* Los parámetros utilizados en la ayuda y la instalación no son sensibles, que es una ventaja añadida, mientras que en comparación con otros.
* Es-acomodados tanto en Ubuntu y así como Cent OS.
* Este módulo se instala el apc php en la versión actualizada.
* La principal ventaja de utilizar Apache OpenOffice como una suite de productividad viene del costo. Incluye procesador de textos, hoja de 
  cálculo, presentación, edición gráfica vectorial y componentes de gestión de base de datos.
* Es fácil para los principiantes a aprender a usar, pero es lo suficientemente potente como para hacer las tareas avanzadas usuarios 
  experimentados quieren. Está diseñado para que los comandos y funciones que debe utilizar en un componente del trabajo de software en toda 
  la suite.
