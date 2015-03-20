=================
Amazon S3 
=================

Sinopsis
-------------

Amazon Simple Storage Service (Amazon S3), proporciona a los desarrolladores y los equipos de con el almacenamiento de objetos altamente escalable, segura y durable. Amazon S3 es fácil de usar, con una interfaz de servicios web simple para almacenar y recuperar cualquier cantidad de datos desde cualquier sitio en la web. Con Amazon S3, usted sólo paga por el almacenamiento en realidad usas. No hay ningún honorario mínimo y ninguna disposición costo.

Amazon S3 puede usarse sola o junto con otros servicios AWS como Amazon Elastic Compute Cloud (Amazon EC2), Amazon Elastic Block Store (Amazon EBS) y Amazon glaciar, así como repositorios de almacenamiento de información de terceros y las entradas. Amazon S3 proporciona almacenamiento objeto rentable para una amplia variedad de casos de uso, incluyendo aplicaciones cloud, distribución de contenidos, backup, archiving y recuperación ante desastres y análisis de datos grande.

comando Ayuda
----------------------

Este comando permite para determinar el uso de AWS S3. El usuario llegará a saber acerca del manera/formato diferente para ejecutar este módulo. Este comando guía al usuario final para conocer el propósito de este comando. A continuación dado son el comando y la captura de pantalla del mismo.

.. code-block:: bash

 kevell@corp:/# ptconfigure AWSS3 help

 ******************************


    This is an extension provided for Handling AWSS3.

    AWSS3, awss3 aws-s3

        - ensure-bucket-exists
        Lets you add bucket to AWSS3 if doesnt exists
        example: ptconfigure AWSS3 ensure-bucket-exists
                    --yes
                    --guess
        - add-object
        Lets you upload object to bucket
        example: ptconfigure AWSS3 add-object
                    --yes
                    --guess


        - remove-bucket
          Lets you remove bucket
          example: ptconfigure AWSS3 remove-bucket
                    --yes
                    --guess

        - remove-object-all
       Lets you remove all object from a bucket
          example: ptconfigure AWSS3 remove-object-all
                    --yes
                    --guess


            - remove-object
       Lets you remove a object from a bucket
          example: ptconfigure AWSS3 remove-object
                    --yes
                    --guess

        - list
        Will display data about your AWS S3
        example: ptconfigure AWSS3 list
                  --yes
                  --guess


        Note: region must be one of the following...
        us-east-1, ap-northeast-1, sa-east-1, ap-southeast-1, ap-southeast-2, us-west-2, us-gov-west-1, us-west-1, cn-north-1, eu-west-1


 ------------------------------
 End Help
 ******************************


Ensure-bucket-exists
---------------------------

Este comando ayuda a añadir cubo a AWSS3 si no existe. La continuación dado comando se ejecutará el proceso.

.. code-block:: bash

	ptconfigure AWSRoute53 create-hosted-zone --yes --guess


Add-object 
---------------------------

Este comando permite para cargar objeto para cubo. La continuación dado comando se ejecutará el proceso.

.. code-block:: bash
	
	ptconfigure AWSS3 add-object --yes –guess

Remove-bucket 
---------------------------

Este comando contribuye a eliminar el cubo. La continuación dado comando se ejecutará el proceso.
 
.. code-block:: bash     

	ptconfigure AWSS3 remove-bucket --yes --guess

Remove-object-all
--------------------------

Este comando ayuda a quitar todos los objetos de un cubo. La continuación dado comando se ejecutará el proceso.

.. code-block:: bash     
	
	ptconfigure AWSS3 remove-object-all --yes --guess

Remove-object	
--------------------------

Este comando permite para eliminar un objeto de un cubo. La continuación dado comando se ejecutará el proceso.

.. code-block:: bash     
	
	ptconfigure AWSS3 remove-object --yes --guess 

List
---------

Este comando permite para visualizar datos sobre su S3 AWS. La continuación dado comando se ejecutará el proceso.

.. code-block:: bash 

	ptconfigure AWSS3 list --yes --guess

parámetros alternativos
------------------------------

Hay tres parámetros alternativos que pueden utilizarse en la línea de comandos.

AWSS3, awss3 aws-s3 

beneficios
--------------

Durable: Amazon S3 proporciona infraestructura durable para almacenar datos importantes y está diseñado para la durabilidad del 99.999999999% de objetos. Los datos se almacenan redundante a través de múltiples instalaciones y múltiples dispositivos en cada planta.

Bajo costo: Amazon S3 permite almacenar grandes cantidades de datos a un costo muy bajo. Usted paga por lo que necesita, sin compromisos mínimos o honorarios prepagos.

Disponible: Amazon S3 está diseñado para la disponibilidad de 99.99% de los objetos más de un año determinado.  Amazon S3 también está respaldado por el Amazon S3 Service Level Agreement, asegurando que usted puede confiar en él cuando lo necesite. Y usted puede elegir una región AWS a optimizar para latencia, minimizar costos o requerimientos regulatorios.

Seguro: Amazon S3 soporta transferencia de datos sobre SSL y encriptación automática de los datos una vez que se haya cargado. También puede configurar el cubo políticas para administrar los permisos del objeto y controlar el acceso a sus datos usando AWS identidad y acceso gestión (IAM).

Escalable: Con Amazon S3, se pueden almacenar tantos datos como quieras y acceder a él cuando lo necesite. Puedes dejar de adivinar sus necesidades futuras de almacenamiento y escala hacia arriba y hacia abajo según sea necesario, aumentando la agilidad del negocio.
Enviar notificaciones de eventos: Amazon S3 puede enviar notificaciones de eventos cuando se cargan objetos a Amazon S3. Las notificaciones de eventos de Amazon S3 pueden entregadas usando Amazon SQS o Amazon SNS, o enviadas directamente a AWS Lambda, que permite a gatillo flujos de trabajo, alertas u otro proceso. Por ejemplo, necesitas las notificaciones de eventos de Amazon S3 para desencadenar la transcodificación de archivos multimedia cuando se carguen, procesamiento de archivos de datos cuando estén disponibles, o sincronización de Amazon S3 objetos con otros almacenes de datos.

Alto rendimiento: Amazon S3 soporta varias partes subidos para maximizar la flexibilidad y el rendimiento de la red y le permite elegir la región AWS para almacenar los datos cerca del usuario final y minimizar la latencia de la red. Y Amazon S3 está integrado con Amazon CloudFront, un servicio de entrega de contenido web que distribuye el contenido a los usuarios finales con una latencia baja, altas velocidades de transferencia y sin compromisos de uso mínimo.

Integrado: Amazon S3 se integra con otros servicios AWS para simplificar la carga y descarga de datos de Amazon S3 y que sea más fácil construir las soluciones que utilizan los servicios de una gama de AWS. Amazon S3 integraciones incluyen Amazon CloudFront, Amazon Kinesis, Amazon RDS, glaciar de Amazon, Amazon EBS, Amazon DynamoDB, Amazon Redshift, Amazon ruta 53, Amazon EMR y AWS Lambda.
Fácil de usar: Amazon S3 es fácil de usar con una consola de administración basada en web y aplicaciones móviles y resto completo APIs y SDKs para una fácil integración con tecnologías de terceros.

