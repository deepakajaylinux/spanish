==================
AWSCloudFormation
==================

sinopsis
-------------

AWS CloudFormation da los desarrolladores y los administradores de sistemas una manera fácil de crear y administrar una colección de recursos relacionados de la AWS, aprovisionamiento y actualizándolos en una manera ordenada y predecible.


Puede utilizar las plantillas de muestra de AWS CloudFormation o crear sus propias plantillas para describir los recursos de la AWS y dependencias asociadas o los parámetros de tiempo de ejecución, necesarios para ejecutar la aplicación. No necesitas saber el orden para el aprovisionamiento de servicios de AWS o las sutilezas de hacer trabajar a esas dependencias. CloudFormation se encarga de esto por usted. Después de que los recursos AWS se despliegan, puede modificar y actualizar de manera controlada y predecible, en efecto aplicar control de versiones para su infraestructura de AWS del mismo modo que hacer con su software.


Puede implementar y actualizar una plantilla y su asociado colección de recursos (llamado una pila) mediante el uso de la consola de administración de AWS, AWS Command Line Interface o API. CloudFormation está disponible sin costo adicional, y usted sólo paga por los recursos AWS necesarios para ejecutar sus aplicaciones.


comando Ayuda
----------------------

Este comando ayuda a determinar el uso de AWS CloudFormation. El usuario llegará a saber acerca del manera/formato diferente para ejecutar este módulo. Este comando guía al usuario final para conocer el propósito de este comando. A continuación dado son el comando y la captura de pantalla del mismo.


.. code-block:: bash

 kevell@corp:/# ptconfigure AWSCloudFormation help

 ******************************


  This command allows you to install a The AWS Cloud Formation Command
  Line Tools. This tool is provided by

  AWSCloudFormation, aws-cloud-formation, aws-cloudformation

        - install
        Installs AWSCloudFormation. Note, you'll also need Java installed
        as it is a prerequisite for AWSCloudFormation.
        example: ptconfigure aws-cloud-formation install

 ------------------------------
 End Help
 ******************************

instalación
----------------

Si el usuario necesita instalar el módulo AWSCloudFormation en la máquina, la continuación dado comando se ejecutará el proceso de instalación.


.. code-block:: bash
        
       ptconfigure aws-cloud-formation install

.. code-block:: bash 

 kevell@corp:/# ptconfigure aws-cloud-formation install

 Install AWSCloudFormation? (Y/N) 
 y
 *******************************
 *        Pharaoh Tools        *
 *         AWS CloudFn!        *
 *******************************
 Creating /tmp/ptconfigure-temp-script-17956189939.sh
 chmod 755 /tmp/ptconfigure-temp-script-17956189939.sh 2>/dev/null
 Changing /tmp/ptconfigure-temp-script-17956189939.sh Permissions
 Executing /tmp/ptconfigure-temp-script-17956189939.sh
 Cloning into 'aws-cloudformation'...
 remote: Counting objects: 64, done.
 remote: Total 64 (delta 0), reused 0 (delta 0), pack-reused 64
 Unpacking objects: 100% (64/64), done.
 Checking connectivity... done.
 mv: cannot move ‘/tmp/aws-cloudformation/bin’ to ‘/opt/aws-cloudformation/bin’: Directory not empty
 mv: cannot move ‘/tmp/aws-cloudformation/lib’ to ‘/opt/aws-cloudformation/lib’: Directory not empty
 Temp File /tmp/ptconfigure-temp-script-17956189939.sh Removed
 PHP Notice:  Undefined index: object in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BaseLinuxApp.php on line 279
 PHP Notice:  Undefined index: method in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BaseLinuxApp.php on line 279
 PHP Notice:  Undefined index: params in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BaseLinuxApp.php on line 279
 PHP Warning:  call_user_func_array() expects parameter 1 to be a valid callback, first array member is not a valid class name or object in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BaseLinuxApp.php on line 279
 PHP Notice:  Undefined index: object in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BaseLinuxApp.php on line 279
 PHP Notice:  Undefined index: method in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BaseLinuxApp.php on line 279
 PHP Notice:  Undefined index: params in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BaseLinuxApp.php on line 279
 PHP Warning:  call_user_func_array() expects parameter 1 to be a valid callback, first array member is not a valid class name or object in /opt/ptconfigure/ptconfigure/src/Modules/PtconfigureRequired/Model/BaseLinuxApp.php on line 279
 ... All done!
 *******************************
 Thanks for installing , visit www.pharaohtools.com for more
 ******************************


 Single App Installer:
 --------------------------------------------
 AWSCloudFormation: Success
 ------------------------------
 Installer Finished
 ******************************


parámetros alternativos
------------------------------       

Hay tres parámetros alternativos que pueden utilizarse en la línea de comandos.


AWSCloudFormation, aws-cloud-formation, aws-cloudformation 


beneficios
--------------

Soporta una amplia gama de recursos de AWS: AWS CloudFormation soporta una amplia gama de AWS recursos, permite generar una alta disponibilidad, confiable y escalable infraestructura AWS para sus necesidades de aplicación. AWS CloudFormation actualmente soporta los recursos en los siguientes servicios AWS:


Auto Scaling

Amazon CloudFront

AWS CloudWatch

Amazon DynamoDB

Amazon EC2

Amazon ElastiCache

AWS Elastic Beanstalk

AWS Elastic Load Balancing

AWS Identity and Access Management

Amazon RDS

Amazon Redshift

Amazon Route 53

Amazon S3

Amazon SimpleDB

Amazon SNS

Amazon SQS

Amazon VPC

Fácil de usar: CloudFormation hace que sea fácil de organizar y desplegar una colección de recursos AWS y permite describir cualquier dependencias o parámetros especiales para pasar en tiempo de ejecución. Puede utilizar una de las muchas plantillas de muestra CloudFormation--literales o como punto de partida.


No hay necesidad de reinventar la rueda: una plantilla puede usarse repetidamente para crear copias idénticas de la misma pila (o utilizar como base para iniciar una nueva pila). Puede capturar y controlar las variaciones de infraestructuras específicas para la región como Amazon EC2 AMIs, así como nombres de Amazon Elastic Block Store (EBS) y Amazon RDS instantánea.


Transparente y abierta: las plantillas son archivos de texto con formato JSON simple que pueden ser colocados bajo sus mecanismos de control de fuente normal, almacenados en lugares públicos o privados tales como Amazon S3 e intercambiados por correo electrónico. Con AWS CloudFormation, puede "abrir el capó," para ver exactamente qué recursos AWS conforman una pila. Puede mantener el control completo y tiene la capacidad de modificar cualquiera de los recursos AWS creados como parte de una pila.

Declarativo y Flexible: para crear la infraestructura que quieras, se enumeran qué recursos AWS, los valores de configuración y las interconexiones que necesita en una plantilla y luego deje que AWS CloudFormation hagan el resto con unos pocos clics en la consola de administración de AWS, un comando mediante el uso de la interfaz de línea de comandos AWS, o pide un solo mediante una llamada a las API. Usted no tendrá que recordar los detalles de cómo crear e interconectar los respectivos recursos AWS mediante su servicio APIs; AWS CloudFormation hace esto para usted. También no necesitas escribir una plantilla desde cero si empiezas con una de las muchas plantillas de muestra que vienen con AWS CloudFormation.


Personalizado via parámetros: puede utilizar parámetros para personalizar los aspectos de su plantilla en tiempo de ejecución cuando se construye la pila. Por ejemplo, puede pasar el RDS tamaño base de datos, EC2 instancia tipos, base de datos y números de Puerto de servidor web a AWS CloudFormation cuando se crea una pila. También puede usar una plantilla parametrizada para crear múltiples pilas que pueden diferir de forma controlada. Por ejemplo, su tipo de instancia de Amazon EC2, umbrales de alarma Amazon CloudWatch y Amazon RDS leer-réplica ajustes pueden diferir entre las regiones AWS si usted recibe más tráfico de clientes en los Estados Unidos que en Europa. Puede utilizar para ajustar la configuración de parámetros de plantilla y umbrales de cada región por separado y todavía estar seguro de que la aplicación esté desplegada sistemáticamente en todas las regiones.


Integración listo: Puede integrar AWS CloudFormation con las herramientas de desarrollo y gestión de su elección.


AWS CloudFormation publica eventos de progreso a través de Amazon Simple notificación servicio (SNS). Con el SNS, puede seguimiento pila creación y cancelación mediante correo electrónico y se integran con otros procesos mediante programación.


Sin recargo: AWS CloudFormation está disponible sin costo adicional. Usted será facturado solamente las tarifas normales para los recursos AWS que AWS CloudFormation crea y utiliza su aplicación.

