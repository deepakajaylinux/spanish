========
Awstats
========

sinopsis
----------

En este módulo se promueve la instalación de awstats, con la última versión. AWStats es un análisis web de código abierto herramienta de informes, adecuadas para el análisis de datos de los servicios de Internet como web, los servidores con los medios de comunicación, electrónico y FTP. AWStats analiza y analiza los archivos de registro del servidor, la elaboración de informes HTML.

AWStats (Advanced Web Statistics) es un potente analizador de archivo de registro del servidor web, con todas las funciones que te muestra todas las estadísticas de su web incluyendo: visitantes, páginas, golpea, hora, motores de búsqueda, palabras clave utilizadas para encontrar su sitio, enlaces rotos, robots y muchos más.

Veamos, los detalles de cómo instalar este awstats, las características y requisitos de awstats en los próximos temas.

Ayuda Comando
----------------------

El comando help guía a los usuarios en cuanto a la finalidad y al igual que sobre las opciones que se incluyen en el módulo AWStats. En él se enumeran los parámetros alternativos de módulo AWStats. También describe la sintaxis para instalar el módulo AWStats. El comando de ayuda para el módulo AWStats se muestra a continuación.

.. code-block:: bash
	
		ptconfigure AWStats help

La sintaxis para declarar el comando de ayuda no es sensible a mayúsculas, que es una ventaja añadida. La siguiente captura de pantalla a visualizar sobre el comando de ayuda bajo AWStats.

Instalación
--------------

El comando que se utiliza para la instalación de los AWStats a la máquina de los usuarios se muestra a continuación.

.. code-block:: bash

		ptconfigure AWStats install

Después de introducir el comando anterior, el siguiente proceso se produce como se muestra en el formato tabular.

.. cssclass:: table-bordered


 +-----------------------+-------------------------------------+-------------+--------------------------------------+
 | Parámetros            | parámetros alternativos             | Necesario   | Comentario                           |
 +=======================+=====================================+=============+======================================+
 |Install AWStats? (Y/N) | En lugar de AWStats, podemos        | Y(Yes)      | Si el usuario desea continuar el     |
 |                       | utilizar Awstats, awstats también.  |             | proceso de instalación se puede      |
 |                       |                                     |             | introducir como Y.                   |
 +-----------------------+-------------------------------------+-------------+--------------------------------------+
 |Install AWStats? (Y/N) | En lugar de AWStats, podemos        | N(No)       | Si el usuario desea abandonar el     |
 |                       | utilizar Awstats, awstats también.  |             | proceso de instalación se puede      |
 |                       |                                     |             | introducir como N.|                  |
 +-----------------------+-------------------------------------+-------------+--------------------------------------+



Si el usuario continúa la instalación, el siguiente proceso están involucrados durante la instalación:

* Lee la lista de paquetes.
* Construye el árbol de dependencias.
* Instala los paquetes adicionales necesarios
* Instala los paquetes sugeridos.
* Instala los nuevos paquetes.

Por último, la instalación de Awstats se completó con éxito como se muestra en las siguientes capturas de pantalla

Características del Awstats
---------------------------

Un análisis del registro completo permite AWStats para mostrarles la siguiente información:


* Número de visitas y de visitantes únicos
* Duración de las visitas y la última visita
* Los usuarios autenticados y últimas visitas autenticados
* Días de la semana y la hora punta (páginas, hits, KB por cada día y hora)
* Dominios / Países de anfitriones de los visitantes (páginas, hits, KB)
* Lista de los Ejércitos, últimas visitas y direcciones IP no resueltas lista
* Páginas más vistas, de entrada y salida
* Tipos de archivo
* Estadísticas de compresión Web (por mod_gzip o mod_deflate)
* Los navegadores utilizados (páginas, hits, kb para cada navegador)
* OS utilizado (páginas, hits, KB para cada sistema operativo)
* Visitas Robot
* Ataques de Gusanos
* Descargar y continuación de detección
* Los motores de búsqueda, frases y palabras clave utilizadas para encontrar su sitio
* Errores HTTP (Página no encontrada con el último árbitro, etc,)
* Informe de tamaño de pantalla
* Número de veces que su sitio está "añadido a favoritos marcadores"
* Relación de los navegadores que soporten: Java, Flash, lector RealG2,
  Lector Quicktime, lector WMA, lector de PDF
* Informe de Cluster para carga relación servidores equilibrada
* Otros informes personalizados ...


Es compatible con las siguientes características, así:

* Puede analizar todos los formatos de registro
* Obras de línea de comandos y desde un navegador como CGI (con dinámica
  filtros capacidades para algunos gráficos)
* Actualización de las estadísticas se puede hacer en la demanda de la interfaz web y
  no sólo de su planificador
* Sin límite de tamaño de archivo de registro, archivos de registro de soporte de división (sistema de balanceo de carga)
* Soporte 'casi ordenados' los archivos de registro, incluso para las páginas de entrada y salida
* Invertir búsqueda DNS antes o durante el análisis, soporta archivos de caché de DNS
* Detección País de localización de IP o nombre de dominio
* Enlaces Whois
* Una gran cantidad de opciones / filtros y plugins se puede utilizar Sitios web 
* Multi-nombradas soportados (servidores virtuales)
* Cross Site Scripting Ataques protección
* Varios idiomas
* No hay necesidad de bibliotecas Perl raras
* Informes dinámicos como resultado del CGI Informes 
* Estática en una o enmarcado HTML o XHTML
* Experimental de exportación a PDF
* Ver y colores pueden coincidir con el diseño del sitio (CSS)
* Ayuda y sugerencias en HTML informaron páginas
* Fácil de usar (sólo un archivo de configuración para editar)
* Análisis de la base de datos se puede almacenar en formato XML (para el procesamiento de XSLT, ...)
* Un módulo Webmin
* Libre (GNU GPL) con fuentes (los scripts de Perl)
* Disponible en todas las plataformas

Requisitos de Awstats
---------------------

Para usar AWStats script CGI, son necesarios los siguientes requisitos:

* El servidor debe registrar el acceso web en un archivo de registro se puede leer.
* Para ejecutar awstats, desde la línea de comandos, el sistema operativo debe ser capaz
  Para ejecutar scripts (archivos .pl) perl.
* Perl módulo "Encode" debe estar disponible.

Para ejecutar awstats como un CGI (por estadísticas en tiempo real), el servidor web también debe ser capaz de ejecutar dichos scripts.


 Si no, puede resolver este descargando la última versión de Perl en:

 http://www.activestate.com/ActivePerl/ (Windows)

 http://www.perl.com/pub/language/info/software.html (All OS)


Beneficios
----------

* Los parámetros utilizados en ayuda y de instalación y desinstalación operaciones no son sensibles, que es una ventaja añadida, mientras que 
  en comparación con otros.
* Es-acomodados tanto en Ubuntu y así como Cent OS.
* Este módulo se instala los Awstats en versión actualizada.
* Si el módulo ya existe en la máquina del usuario, se mostrará un mensaje, ya que ya existe.
* AWStats soporta la mayoría de los principales formatos de archivos de registro del servidor web, incluyendo (/ XLF / formato de registro ELF 
  NCSA combinado o Formato Común de Registro (CLF)) Apache,
  WebStar, IIS (formato de registro W3C), y muchos otros formatos de registro del servidor web común.
* Los desarrolladores pueden contribuir al proyecto AWStats través de SourceForge.net.
* Escrito en Perl, AWStats se pueden implementar en casi cualquier sistema operativo
* Se trata de una herramienta de administración de servidores, con los paquetes disponibles para la mayoría de las distribuciones de Linux.

* AWStats se pueden instalar en una estación de trabajo, tales como MS Windows, para uso local en situaciones en que los archivos de registro 
  se puede descargar desde un servidor remoto.
