=================
AMAZON ROUTE 53 
=================

sinopsis
-------------

Amazon ruta 53 es una nube altamente disponible y escalable servicio web Domain Name System (DNS). Está diseñado para dar los desarrolladores y empresas una forma extremadamente fiable y rentable para los usuarios finales de la ruta a las aplicaciones de Internet traduciendo nombres como www.example.com a las direcciones IP numéricas como 192.0.2.1 que utilizan computadoras para conectar entre sí.

Amazon ruta 53 efectivamente conecta las peticiones del usuario funcionando en AWS – como instancias de Amazon EC2, balanceo de carga elástica equilibradores de carga o cubos de Amazon S3 – infraestructura y puede utilizarse también para los usuarios de ruta a la infraestructura fuera de AWS. Puede utilizar Amazon ruta 53 configurar DNS los controles sanitarios para tráfico de ruta hacia los extremos sanos o controlar independientemente la salud de su aplicación y sus extremos. Amazon ruta 53 hace posible para que usted pueda administrar el tráfico en todo el mundo a través de una variedad de tipos de enrutamiento, incluyendo enrutamiento basado en latencia, Geo DNS y Weighted Round Robin — todos los cuales pueden combinarse con Failover de DNS para permitir una variedad de arquitecturas de baja latencia y tolerante. Amazon ruta 53 también ofrece registro de nombres de dominio – usted puede comprar y administrar nombres de dominio como ejemplo.com y Amazonas ruta 53 se configurará automáticamente la configuración de DNS de sus dominios.

comando Ayuda
----------------------

Este comando permite para determinar el uso del Amazonas ruta 53. El usuario llegará a saber acerca del manera/formato diferente para ejecutar este módulo. Este comando guía al usuario final para conocer el propósito de este comando. A continuación dado son el comando y la captura de pantalla del mismo.

.. code-block:: bash

 kevell@corp:/# ptconfigure AWSRoute53 help

 ******************************


    This is an extension provided for Handling AWS ROUTE53.

    AWSRoute53, awsroute53, aws-route53

        - create-hosted-zone
        Lets you add Hosted zone to AWS Route53
        example: ptconfigure AWSRoute53 create-hosted-zone
                    --yes
                    --guess
        - create-health-check
        Lets you add Health Check to AWS Route53
        example: ptconfigure AWSRoute53 create-health-check
                    --yes
                    --guess
          - delete-hosted-zone
        Lets you delete Hosted zone to AWS Route53
        example: ptconfigure AWSRoute53 delete-hosted-zone
                    --yes
                    --guess
         - delete-health-check
        Lets you delete Health Check to AWS Route53
        example: ptconfigure AWSRoute53 delete-health-check
                    --yes
                    --guess

        - list
        Will display data about your AWS Route53
        example: ptconfigure AWSRoute53 list
                    --yes
                    --guess

        Note: region must be one of the following...
        us-east-1, ap-northeast-1, sa-east-1, ap-southeast-1, ap-southeast-2, us-west-2, us-gov-west-1, us-west-1, cn-north-1, eu-west-1

 ------------------------------
 End Help
 ******************************

Create-hosted-zone 
---------------------------

Este comando permite para añadir zona alojado a AWS Route53. La continuación dado comando se ejecutará el proceso.

.. code-block:: bash

	ptconfigure AWSRoute53 create-hosted-zone --yes --guess

Create-health-check 
---------------------------

Este comando permite para añadir chequeo a AWS Route53. La continuación dado comando se ejecutará el proceso.

.. code-block:: bash
	
	ptconfigure AWSRoute53 create-health-check --yes --guess

Delete-hosted-zone 
---------------------------

Este comando permite para borrar zona alojado a AWS Route53. La continuación dado comando se ejecutará el proceso.

.. code-block:: bash     

	ptconfigure AWSRoute53 delete-hosted-zone --yes --guess 

Delete-health-check 
-------------------------

Este comando permite para borrar chequeo a AWS Route53. La continuación dado comando se ejecutará el proceso.

.. code-block:: bash     
	
	ptconfigure AWSRoute53 delete-health-check --yes --guess

List
---------

Este comando permite para Mostrar datos acerca de su Route53 de AWS. La continuación dado comando se ejecutará el proceso.

.. code-block:: bash 

	ptconfigure AWSRoute53 list --yes --guess

parámetros alternativos
-----------------------------

Hay tres parámetros alternativos que pueden utilizarse en la línea de comandos.

AWSRoute53, awsroute53, aws-route53 

Beneficios
--------------

Altamente disponibles y confiable: Amazon ruta 53 se construye utilizando la infraestructura altamente confiable y disponible de AWS. La naturaleza distribuida de nuestros servidores DNS ayuda a garantizar una capacidad constante para los usuarios finales a su aplicación. Ruta 53 está diseñado para proporcionar el nivel de fiabilidad requerido por las aplicaciones importantes. Amazon ruta 53 está respaldado por el Amazonas ruta 53 Service Level Agreement.

Escalable: Ruta 53 está diseñado para escalar automáticamente para manejar volúmenes muy grandes consulta sin intervención alguna de ti.

Diseñado para su uso con otros servicios Web de Amazon: Amazon ruta 53 está diseñado para trabajar bien con otras características AWS y ofrendas. Puede utilizar Amazon ruta 53 para asignar nombres de dominio a sus instancias de EC2 de Amazon, Amazon S3 cubos, Amazon CloudFront distribuciones y otros recursos AWS. Al utilizar el servicio de identidad de AWS y acceso gestión (IAM) con Amazon ruta 53, tienes control de grano fino sobre quién puede actualizar sus datos de DNS. Puede utilizar Amazon ruta 53 para asignar su ápice de zona (ejemplo.com versus www.example.com) a su instancia de equilibrio de carga de elástico, Amazon CloudFront distribución o cubo de Amazon S3 Web utilizando una característica denominada registro de Alias.

Simple: Con inscripción de autoservicio, ruta 53 puede comenzar a responder sus consultas DNS dentro de minutos. Puede configurar sus ajustes DNS con la consola de administración de AWS o nuestra API fácil de usar. También mediante programación puede integrar la ruta 53 API en su aplicación web global. Por ejemplo, dispones API de ruta 53 para crear un nuevo registro DNS cada vez que se crea una nueva instancia de EC2.

Rápido: Usando una red global anycast de servidores DNS alrededor del mundo, Amazon ruta 53 está diseñado para enrutar automáticamente los usuarios a la ubicación óptima dependiendo de las condiciones de la red. Como resultado, el servicio ofrece latencia baja consulta para los usuarios finales, así como actualización de baja latencia para sus necesidades de administración de registros de DNS.

Rentable: Amazon ruta 53 pasa sobre los beneficios de escala de AWS a usted. Usted sólo paga por gestión de dominios a través del servicio y el número de consultas que el servicio de respuestas para cada uno de sus dominios, a un bajo costo y sin compromisos de uso mínimo ni cargos por adelantado.

Seguro: Mediante la integración amazónica ruta 53 con AWS identidad y acceso gestión (IAM), puede otorgar credenciales únicas y gestionar los permisos de cada usuario dentro de su cuenta AWS y especificar quién tiene acceso a qué partes del servicio Amazon ruta 53.

Flexible: Amazon ruta 53 ofrece Weighted Round-Robin (WRR), también conocido como equilibrio de carga de DNS. Esto le permite asignar pesos a sus registros de DNS que especifican qué porción de su tráfico se enruta a diversos extremos.

