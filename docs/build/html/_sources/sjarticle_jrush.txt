===============
JArticle
===============

sinopsis
-------------

Gestiona los datos de jarticle. Esto permite utilizar un artículo como un módulo. Joomla ofrece una muy amplia gama de opciones para crear diferentes tipos de contenido y estructurarlo en su sitio Web.


En Joomla, un artículo es una pieza de contenido de texto, posiblemente con enlaces a otros recursos (por ejemplo, imágenes). Los artículos son las unidades básicas de información en el sistema de contenido y el nivel inferior en la jerarquía del contenido. Cada artículo está en una categoría. Una categoría puede estar en otra categoría por lo que es un sub categoría. También es posible tener artículos Uncategorized. Estos artículos existen sin asociarse con cualquier categoría.



comando Ayuda
----------------------

Este comando permite para determinar el uso del módulo jarticle. El usuario llegará a conocer el diferente formas/formato para ejecutar este módulo. Este comando guía al usuario final para conocer el propósito de este comando. A continuación dado son el comando y la captura de pantalla del mismo.


.. code-block:: bash
        
	jrush  jarticle help


.. code-block:: bash

 kevell@corp:/# jrush  jarticle help
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

  This command allows you to manage Joomla JArticles (Component, Module or Plugin).

  JArticle, jarticle

        - disable
        Deletes a jarticle
        example: jrush jarticle disable

        - enable
        Enables a jarticle
        example: jrush jarticle enable

        - info
        Display the details of a jarticle
        example: jrush jarticle info


 ------------------------------
 End Help
 ****************************************



Enable
----------------

Cuando el usuario necesita habilitar un artículo en particular, la continuación dado comando se ejecutará el proceso de instalación.


.. code-block:: bash
        
	jrush jarticle enable ..config file=”bootstrap file path”


Info
------

Si el usuario necesita saber acerca de la información de un artículo. La continuación dado comando le ayudará a

.. code-block:: bash
        
	jrush jarticle info ..config file=”bootstrap file path”


La representación pictórica del comando anterior se enumera a continuación,


.. code-block:: bash

 kevell@corp:/# jrush jarticle info --config-file="/var/www/html/joomla/configuration.php"
 Enter a JArticle ID. To enter title/alias/asset-id use --jarticle-title, --jarticle-alias or --jarticle-asset-id parameters
 2
 ****************************************
 GC JRush - The Joomla Command Line Shell
 ****************************************

 JArticle Information:
 -------------------------

 Article ID: 2
 Asset ID: 35
 Alias: about-us
 Title: About Us
 Created By: 825
 Created By Alias: Joomla
 State: 1
 ------------------------------
 JArticle Manage Finished
 ****************************************


Disable
----------------

Cuando el usuario necesita desactivar un artículo en particular, la continuación dado comando se ejecutará el proceso de instalación.


.. code-block:: bash
        
	jrush jarticle disable ..config file=”bootstrap file path”

parámetros alternativos
----------------------------

Ninguno de los dos parámetros alternativos pueden utilizarse en comando-

jarticle, JArticle

eg:  jrush jarticle disable/ jrush JArticle disable                                 




beneficios
--------------

* Proporcionar un método opcional para organizar tus artículos 
* contiene parte del texto y puede contener imágenes y otros tipos de contenido
* ayuda a obtener la información de un artículo de manera fácil 
* puede activar y desactivar un artículo en un solo paso
