================
Amazon DynamoDB
================

sinopsis
-------------

Amazon DynamoDB es un servicio rápido y flexible de base de datos NoSQL para todas las aplicaciones que necesitan latencia milisegundo consistente, de un solo dígito en cualquier escala. Es una base de datos totalmente gestionado y soporta tanto documento y modelos de datos de clave y valor. Su modelo de datos flexible y fiable rendimiento hacen un gran ajuste para el móvil, web, juegos de azar, ad-tech, muchos y muchas otras aplicaciones.


comando Ayuda
----------------------	

Este comando ayuda a determinar el uso de AWS DynamoDB. El usuario llegará a saber acerca del manera/formato diferente para ejecutar este módulo. Este comando guía al usuario final para conocer el propósito de este comando. A continuación dado son el comando y la captura de pantalla del mismo.


.. code-block:: bash


 kevell@corp:/# ptconfigure AWSDynamoDb help

 ******************************


    This is an extension provided for Handling AWSDynamoDb.

    AWSDynamoDb, awsdynamodb,aws-dynamodb

        - describe-table
        Describe a table
        example: ptconfigure AWSDynamoDb describe-table
                    --yes
                    --guess
        - delete-table
        Lets you delete a table
        example: ptconfigure AWSDynamoDb delete-table
                    --yes
                    --guess


        - create-table
          Lets you create a table
          example: ptconfigure AWSDynamoDb create-table
                    --yes
                    --guess




        - list
        Will display data about your AWS AWSDynamoDb
        example: ptconfigure AWSDynamoDb list
                  --yes
                  --guess


        Note: region must be one of the following...
        us-east-1, ap-northeast-1, sa-east-1, ap-southeast-1, ap-southeast-2, us-west-2, us-gov-west-1, us-west-1, cn-north-1, eu-west-1


 ------------------------------
 End Help
 ******************************

Describe-table 
-------------------

Este comando permite para describir una mesa. La continuación dado comando se ejecutará el proceso.


.. code-block:: bash

	 ptconfigure AWSDynamoDb describe-table --yes --guess

Delete-table 
-------------------

Este comando permite para borrar una tabla. La continuación dado comando se ejecutará el proceso.


.. code-block:: bash

	ptconfigure AWSDynamoDb delete-table --yes --guess

Create-table
---------------------

Este comando permite para crear una tabla. La parte más crítica es que es irreversible.

.. code-block:: bash     

	ptconfigure AWSDynamoDb create-table --yes --guess 

List 
---------------------

Este comando permite para Mostrar datos acerca de su AWSDynamoDb de AWS. La continuación dado comando se ejecutará el proceso.

.. code-block:: bash 
	
	ptconfigure AWSDynamoDb list --yes --guess

parámetros alternativos
------------------------------

Hay dos parámetros alternativos que pueden utilizarse en la línea de comandos.

AWSDynamoDb, awsdynamodb,aws-dynamodb 

Beneficios
--------------

Escaneo de índice secundario – una manera más simple para analizar tablas DynamoDB: Amazon DynamoDB permite recuperar todos los elementos de una tabla mediante la operación de análisis. Con secundario Index Scan, ahora puede utilizar la operación de análisis de índices secundarios y recuperar todos los datos de seleccionados atributos y elementos que se proyectan en un índice secundario. Escaneo de índice secundario trabaja en índices secundarios globales y locales. Índices secundarios pueden analizarse desde la consola de DynamoDB o llamando a la API de exploración con un parámetro adicional para especificar el índice.


Indexación en línea – una manera flexible para administrar los índices globales de secundaria: Amazon DynamoDB le permite crear índices secundarios Global (GSI) en mesa de crear tiempo. GSIs permiten escribir ricas consultas con filtros. Con indexación en línea, usted puede agregar o borrar GSIs a una tabla de DynamoDB en cualquier momento utilizando la consola de DynamoDB o a través de una simple llamada de API. Mientras el GSI es ser añadido o eliminado, el DynamoDB mesa todavía manejar tráfico directo y proporcionar servicio continuo en el nivel de rendimiento con provisioning.


Para registrarse para la previsualización de secuencias de DynamoDB: DynamoDB arroyos proporciona un tiempo ordenó la secuencia de cambios de nivel de elemento en cualquier mesa de DynamoDB. Los cambios son desduplicados y almacenados durante 24 horas. Esta capacidad permite a los desarrolladores ampliar el poder de DynamoDB con replicación Cruz-región, analytics continua con integración de corrimiento al rojo, las notificaciones de cambios y muchos otros.

