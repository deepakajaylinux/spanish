===================
Amazon ElastiCache
===================

sinopsis
-------------

ElastiCache es un servicio web que hace que sea fácil de implementar, operar y escalar una caché en memoria en la nube. El servicio mejora el rendimiento de las aplicaciones web al permitirle recuperar la información de rápido, administrado, en memoria caché, en lugar de depender totalmente de bases de datos basadas en disco más lentos. ElastiCache soporta dos open source en memoria caché motores:


Memcached - un objeto ampliamente adoptado de la memoria caché de sistema. ElastiCache es compatible con Memcached, protocolo herramientas populares que se utilizan hoy con entornos existentes Memcached funcionará perfectamente con el servicio.


Redis – una popular open source en memoria par clave-valor tienda que admite conjuntos de datos de estructuras tales como ordenadas y listas. Soporta ElastiCache maestro / esclavo de replicación y Multi-AZ que puede utilizarse para lograr Cruz AZ redundancia.


Amazon ElastiCache detecta automáticamente y sustituye los nodos fallidos, reducir la sobrecarga asociada a infraestructuras autogestionadas y proporciona un sistema flexible que mitiga el riesgo de bases de datos sobrecargados, tiempos de carga que sitio web lento y aplicación. Mediante la integración con Amazon CloudWatch, Amazon ElastiCache proporciona una visibilidad mejorada en indicadores de rendimiento clave asociadas con los nodos Memcached o Redis.


Usando Amazon ElastiCache, puede agregar una capa de almacenamiento en caché en la memoria a su infraestructura en cuestión de minutos utilizando la consola de administración de AWS.



comando Ayuda
----------------------

Este comando ayuda a determinar el uso de Amazon ElastiCache. El usuario llegará a saber acerca del manera/formato diferente para ejecutar este módulo. Este comando guía al usuario final para conocer el propósito de este comando. A continuación dado son el comando y la captura de pantalla del mismo.

.. code-block:: bash

 kevell@corp:/# ptconfigure AWSElastiCache help

 ******************************


    This is an extension provided for Handling AWS ElastiCache.

    AWSElastiCache, awselasticache, aws-elasticache

        - create-cache-cluster
        Lets you add cache Cluster to AWS ElastiCache
        example: ptconfigure AWSElastiCache create-cache-cluster
                    --yes
                    --guess
        - create-health-check
        Lets you add Health Check to AWS Route53
        example: ptconfigure AWSRoute53 create-health-check
                    --yes
                    --guess

          - reboot-cache-cluster
        Lets you reboot cache Cluster to AWS ElastiCache
        example: ptconfigure AWSRoute53 delete-hosted-zone
                    --yes
                    --guess

         - delete-cache-cluster
        Lets you delete cache Cluster to AWS ElastiCache
        example: ptconfigure AWSElastiCache delete-cache-cluster
                    --yes
                    --guess

         - delete-replication-group
        Lets you delete replication group to AWS ElastiCache
        example: ptconfigure AWSElastiCache delete-replication-group
                    --yes
                    --guess

        - list
        Will display data about your AWS ElastiCache
        example: ptconfigure AWSElastiCache list
                    --yes
                    --guess

        Note: region must be one of the following...
        us-east-1, ap-northeast-1, sa-east-1, ap-southeast-1, ap-southeast-2, us-west-2, us-gov-west-1, us-west-1, cn-north-1, eu-west-1

 ------------------------------
 End Help
 ******************************

Create-cache-cluster 
---------------------------

Este comando permite para añadir memoria caché Cluster a AWS ElastiCache. La continuación dado comando se ejecutará el proceso.

.. code-block:: bash

	ptconfigure AWSElastiCache create-cache-cluster –yes --guess 


Create-health-check 
---------------------------

Este comando permite para añadir chequeo a AWS Route53. La continuación dado comando se ejecutará el proceso.

.. code-block:: bash
	
	ptconfigure AWSRoute53 create-health-check –yes –guess

Reboot-cache-cluster 
---------------------------

Este comando permite para reiniciar caché Cluster a AWS ElastiCache.
 
.. code-block:: bash     

	ptconfigure AWSRoute53 delete-hosted-zone --yes --guess 


Delete-cache-cluster 
-------------------------

Este comando permite para borrar caché de clúster a AWS ElastiCache. La continuación dado comando se ejecutará el proceso.

.. code-block:: bash     
	
	ptconfigure AWSElastiCache delete-cache-cluster --yes --guess


Delete-replication-group 
-----------------------------------

Este comando permite para borrar grupo de replicación a AWS ElastiCache. La continuación dado comando se ejecutará el proceso.

.. code-block:: bash 
	
	ptconfigure AWSElastiCache delete-replication-group --yes --guess
        
List
---------------------

Este comando permite para mostrar pantalla datos acerca de su ElastiCache de AWS. La continuación dado comando se ejecutará el proceso.

.. code-block:: bash 

	ptconfigure AWSElastiCache list --yes --guess

parámetros alternativos
------------------------------       

Hay tres parámetros alternativos que pueden utilizarse en la línea de comandos.

AWSElastiCache, awselasticache, aws-elasticache 

Beneficios
--------------

Fácil de implementar: Amazon ElastiCache lo pone muy fácil implementar un entorno compatible con caché Memcached o Redis. Utilice la consola de administración de AWS o simples llamadas a la API para acceder a las capacidades de un cluster de caché nube listo para la producción en minutos sin tener que preocuparse sobre el provisioning de infraestructura o instalación y mantenimiento de software de caché.


Administrado: Amazon ElastiCache automatiza las tareas de gestión desperdiciador de tiempo--tales como gestión de parches, detección de fallos y recuperación--permitiéndole seguir el desarrollo de aplicaciones de mayor valor.


Compatible: Con Amazon ElastiCache, obtienes acceso nativo a los entornos en la memoria caché de Memcached o Redis. Esto facilita la compatibilidad con sus aplicaciones y herramientas existentes.

Elástico: Con una simple llamada de API o un par de clics de AWS Management Console, puede agregar o eliminar caché de nodos en el clúster de caché de nube para satisfacer la carga de las aplicaciones. Autodescubrimiento de Memcached permite detección automática de nodos de memoria caché por ElastiCache los clientes cuando los nodos se agregan o quitan de un clúster de Amazon ElastiCache.

Confiable: Amazon ElastiCache tiene varias características que mejoran la fiabilidad para implementaciones de producción crítica, incluyendo la recuperación y detección de fallos automática. Amazon ElastiCache se ejecuta en la misma infraestructura altamente confiable usada por otros servicios Web de Amazon. Integrado: Amazon ElastiCache está diseñado para uso sin fisuras con otros servicios Web de Amazon, incluyendo servicio de base de datos relacional de Amazon (Amazon RDS), DynamoDB de Amazon, Amazon Elastic Compute Cloud (Amazon EC2), Amazon CloudWatch y Amazon Simple Notification Service (Amazon SNS).

Seguro: Amazon ElastiCache proporciona una serie de mecanismos para garantizar su racimo de caché.
Amazon ElastiCache proporciona interfaces de servicio web que le permiten configurar la configuración del firewall que controlan el acceso a la red para el clúster de caché.

Amazon ElastiCache le permite ejecutar su racimo de caché en nube privada Virtual de Amazon (Amazon VPC). Amazon VPC permite aislar el clúster de caché especificando los intervalos de direcciones IP que desea utilizar para los nodos de memoria caché y conectar a las aplicaciones existentes dentro de Amazon VPC. Para aprender más sobre Amazon ElastiCache en VPC, consulte la guía de usuario de Amazon ElastiCache.



Rentable: Amazon ElastiCache ahorra el coste administrativo de configuración y administración de un clúster de varios nodos caché. Puede ampliar y reducir el número de nodos de memoria caché en el clúster de caché para ofrecer un rendimiento óptimo como el uso de aplicaciones cambios de patrones, pagando sólo por los recursos que realmente consume. El precio de la demanda le permite pagar para capacidad de memoria/computar por hora sin compromisos a largo plazo. Esto hace que el uso de Amazon ElastiCache muy rentable y libera de los costos y la complejidad de la planificación, compra y mantenimiento de hardware.


Multi-AZ: Amazon ElastiCache proporciona funcionalidades de replicación para el motor Redis y funcionalidad Multi-AZ. Usted puede tomar ventaja de varias zonas de la disponibilidad de AWS para obtener la disponibilidad y escalar más allá de las limitaciones de capacidad de un nodo único caché. En caso de pérdida del nodo principal, ElastiCache detectará automáticamente el fracaso y failover a leer una réplica para proporcionar mayor disponibilidad sin necesidad de intervención manual.


Backup y Restore: Amazon ElastiCache para Redis le ayuda a proteger sus datos mediante la creación de instantáneas de los clústeres. Mediante unos pocos clics en la consola o simples llamadas a la API, usted puede configurar instantáneas automáticas, así como iniciar una copia de seguridad cada vez que usted elige. Las instantáneas entonces pueden utilizarse para la siembra de nueva ElastiCache para clústeres de Redis.



Principales casos de uso: Amazon ElastiCache puede utilizarse para mejorar significativamente el rendimiento de muchas cargas de trabajo pesado leer aplicaciones (por ejemplo, las redes sociales, juegos, compartir medios y portales Q&A) o cargas informáticas (por ejemplo, un motor de recomendación) y latencia. Almacenamiento en caché mejora el rendimiento de la aplicación mediante el almacenamiento de piezas críticas de datos en memoria para acceso de baja latencia. Información en la memoria caché puede incluir los resultados de las consultas de base de datos/O-intensivos o los resultados de los cálculos de cómputo intensivo. Las aplicaciones que necesitan un servidor de estructura de datos, encontrará el motor Redis más útiles.

