==========
Grafana
==========

sinopsis
-----------
Grafana tiene un editor de consultas grafito avanzada que le permite navegar rápidamente el espacio métrico, añadir funciones. Cambiar parametros de función y mucho más.

Grafana es un código abierto, cuentan con métricas ricos salpicadero y editor gráfico de grafito, InfluxDB y OpenTSDB.

Veamos cómo este módulo facilita a los usuarios en la instalación del grafana.

Ayuda Comando
---------------------

El comando help guía a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en el módulo Grafana. En él se enumeran los parámetros alternativos de módulo Grafana. También describe la sintaxis para instalar el módulo Grafana. El comando de ayuda para el módulo Grafana se muestra a continuación.

.. code-block:: bash

		ptdeploy grafana help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda bajo módulo Grafana.

instalación
--------------

El comando que se utiliza para la instalación de los módulos grafana en la máquina de los usuarios se muestra a continuación:

.. code-block:: bash
	
		ptdeploy grafana install

Después de introducir el comando anterior, el siguiente proceso se produce como se muestra en el formato tabular.

.. cssclass:: table-bordered

 +-------------------------+-----------------------------------+------------+-----------------------------------------------------+
 | Parámetros              | Parámetro Alternativa             | Opciones   | Comentarios                                         |
 +=========================+===================================+============+=====================================================+
 |Install Grafana? (Y/N)   | En lugar de Grafana, podemos      | Y(Yes)     | Si el usuario desea continuar el proceso de         |
 |                         | utilizar grafana también.         |            | instalación se puede introducir como Y.             |
 +-------------------------+-----------------------------------+------------+-----------------------------------------------------+
 |Install Grafana? (Y/N)   | En lugar de Grafana, podemos      | N(No)      | Si el usuario desea abandonar el proceso de         |
 |                         | utilizar grafana también.         |            | instalación se puede introducir como N.|            |
 +-------------------------+-----------------------------------+------------+-----------------------------------------------------+

La siguiente captura de pantalla representa gráficamente el proceso anteriormente descrito de la instalación.


Beneficios
--------------

* Los parámetros utilizados en la ayuda y la instalación no son sensibles, que es una ventaja añadida, mientras que en comparación con otros.
* Es-acomodados tanto en Ubuntu y así como Cent OS.


Grafito Editor Target
-------------------------

* Grafito expresión diana analizador
* Característica ricos compositor consulta
* Rápidamente añadir y editar funciones y parámetros
* consultas con plantilla
* Verlo en acción

Graficando
-------------

* Renderizado rápido, incluso a grandes lapsos.
* Haga clic y arrastre para zoom.
* Y-eje múltiple.
* Barras, Líneas, Puntos.
* Inteligente eje formating
* Alterna de la serie y selector de color
* Valores Legend, y las opciones de formateo
* umbrales Grid, etiquetas de los ejes
* Anotaciones


Dashboards
--------------

* Crear, editar, guardar y cuadros de mando de búsqueda
* Palmos Cambio de columna y alto de fila
* Arrastrar y soltar los paneles para reordenar
* Uso InfluxDB o Elasticsearch como almacenamiento salpicadero
* Importación y exportación salpicadero (archivo json)
* Salpicadero Importar de grafito
* Plantillas
* cuadros de mando con guión
* listas Dashboard
* Controles rango de tiempo
