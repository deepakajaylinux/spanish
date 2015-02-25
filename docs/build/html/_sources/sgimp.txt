=======
GIMP
=======

Sinopsis
-----------

Este módulo permite a los usuarios instalar GIMP que es un editor de imágenes populares.

GIMP acrónimo de GNU Image Manipulation Program) es utilizado para el retoque y edición de imágenes, el dibujo de forma libre, cambiar el tamaño, recortar, fotomontajes, la conversión entre diferentes formatos de imagen, y las tareas más especializadas.

GIMP se distribuye gratuitamente a (y por) a nadie, y nadie puede mirar a su contenido y su código fuente y puede agregar características o solucionar problemas. Es liberado bajo licencias LGPLv3 y GPLv3 +. GIMP se inició en 1995 como el proyecto de la escuela de dos estudiantes universitarios; ahora GIMP es una aplicación de pleno derecho, disponibles en todas las distribuciones de GNU / Linux y en las versiones recientes de Microsoft Windows y Mac OS X.

Veamos cómo este módulo facilita la instalación de GIMP de los próximos temas.

Ayuda Comando
---------------------

El comando de ayuda es un breve manual de usuario que representa a los usuarios en cuanto a la finalidad de este módulo, sus listas de outs sus parámetros alternativos que se pueden utilizar en las declaraciones, junto con la sintaxis para instalar GIMP través de apt-get. La sintaxis para utilizar la opción de ayuda en virtud de este módulo se muestra a continuación,

.. code-block:: bash

	ptconfigure GIMP help


La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda en virtud de GIMP.

instalación
--------------

El comando que se utiliza para la instalación de GIMP a través de apt-get usando este módulo es simple con sólo usar el siguiente comando,

.. code-block:: bash

	ptconfigure GIMP install


Después de introducir el comando anterior, los siguientes pasos se realizan como se muestra en la tabla,

.. cssclass:: table-bordered

 +--------------------------+----------------------------------------+-------------+----------------------------------------------+
 | Parámetros               | Parámetro Alternativa                  | Opciones    | Comentarios                                  |
 +==========================+========================================+=============+==============================================+
 |GIMP Install? (Y/N)       | En lugar de GIMP podemos usar gimp     | Y(Yes)      | InsIf el deseo del usuario para continuar    |
 |                          | también.                               |             | la instalación, se puede introducir como Y.  |
 +--------------------------+----------------------------------------+-------------+----------------------------------------------+
 |GIMP Install? (Y/N)       | En lugar de GIMP podemos usar gimp     | N(No)       | Si el usuario desea para salir de la         |
 |                          | también.                               |             | instalación, se puede introducir como N.|    |
 +--------------------------+----------------------------------------+-------------+----------------------------------------------+

La siguiente captura de pantalla muestra visualmente sobre el proceso de instalación.

Beneficios
--------------

* Los parámetros utilizados declarando ayuda y otras características diferentes de apt no distinguen entre mayúsculas y minúsculas.
* Es-acomodado tanto os Cent y así como en Ubuntu.


GIMP también proporciona herramientas "inteligentes" que utilizan un algoritmo más complejo de hacer cosas que de otro modo sería lento o imposible. Estos incluyen a:

* La herramienta de clonación, que copia píxeles utilizando un pincel
* Pincel corrector, que copia píxeles de un área y corrige el tono y color
* La herramienta de clon perspectiva, que funciona como la herramienta de clonación, pero corrige la distancia cambia
* Blur y afilar herramientas desenfoques y agudiza usando un cepillo
* Dodge y herramienta de grabación es un cepillo que hace diana píxeles más claros (dodges) o más oscuras (quemaduras)


GIMP transformar herramientas incluyen:

* Alinear
* Movimiento
* Recortar
* Girar
* Escala
* Shear
* Perspectiva
* Voltear
