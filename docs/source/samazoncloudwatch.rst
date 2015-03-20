===================
Amazon CloudWatch
===================

sinopsis
-------------

Amazon CloudWatch es un servicio de monitoreo por AWS nube los recursos y las aplicaciones que se ejecuta en AWS. Puede utilizar Amazon CloudWatch para recoger y seguimiento de métricas, recolectar y controlar los archivos de registro y establecer alarmas. Amazon CloudWatch puede monitorear los recursos AWS como instancias de EC2 de Amazon, Amazon DynamoDB mesas y Amazon RDS DB instancias, así como indicadores personalizados generados por las aplicaciones y servicios y cualquier sus aplicaciones generan los archivos de registro. Puede utilizar Amazon CloudWatch ganar visibilidad de todo el sistema de salud operacional, performance de las aplicaciones y utilización de los recursos. Puede utilizar estos conocimientos para reaccionar y mantener tu aplicación funcionando sin problemas.


comando Ayuda
----------------------

Este comando ayuda a determinar el uso de Amazon CloudWatch. El usuario llegará a saber acerca del manera/formato diferente para ejecutar este módulo. Este comando guía al usuario final para conocer el propósito de este comando. A continuación dado son el comando y la captura de pantalla del mismo.

.. code-block:: bash

 kevell@corp:/# ptconfigure AWSCloudWatch help

 ******************************


  This command allows you to install a few GC recommended Standard Tools
  for productivity in your system.  The kinds of tools we found ourselves
  installing on every box we have, client or server. These include curl,
  vim, drush and zip.

  AWSCloudWatch, aws-cloud-watch, aws-cloudwatch

        - install
        Installs AWSCloudWatch. Note, you'll also need Java installed
        as it is a prerequisite for AWSCloudWatch
        example: ptconfigure aws-cloudwatch install

 ------------------------------
 End Help
 ******************************

instalación
----------------

Si el usuario necesita instalar el módulo de Amazon CloudWatch en máquina, la continuación dado comando se ejecutará el proceso de instalación.


.. code-block:: bash
        
        ptconfigure aws-cloudwatch install

.. code-block:: bash 

	

beneficios
--------------

Monitor Amazon EC2: Ver métricas para utilización de CPU, transferencia de datos y actividad de uso de disco de instancias de Amazon EC2 (supervisión básica) sin cargo adicional. Por un cargo adicional, CloudWatch proporciona monitoreo detallado para instancias de EC2 con mayor resolución y agregación de métricas. No necesita instalar ningún software adicional.


Otros recursos AWS monitor: Monitor métricas en Amazon DynamoDB mesas, volúmenes Amazon EBS, Amazon RDS DB instancias, Amazon MapReduce elástico los flujos de trabajo, elástico balanceadores de carga, colas Amazon SQS, Amazon SNS temas y más sin costo adicional. No necesita instalar ningún software adicional.


Monitor personalizado métricas: Presentar métricas costumbre generada por sus propias aplicaciones mediante una simple solicitud de API y tenerlos vigilados por Amazon CloudWatch. Puede enviar y almacenar las métricas que son importantes para el funcionamiento de la aplicación para ayudarle a solucionar problemas y detectar tendencias.


Monitor y tienda de registros: puede utilizar CloudWatch registros para supervisar y solucionar problemas de sus sistemas y aplicaciones que utilizan su sistema existente, aplicación y los archivos de registro personalizado. Puede enviar su sistema existente, la aplicación y los archivos de registro personalizado CloudWatch troncos y monitorear estos registros en casi en tiempo real. Esto puede ayudarle a entender mejor y operar sus sistemas y aplicaciones, y puede almacenar los registros usando almacenamiento altamente durable y de bajo costo para el acceso posterior.


Sistema de alarmas: Configurar alarmas en cualquiera de sus métricas para enviarle notificaciones o tomar otras acciones automatizadas. Por ejemplo, cuando una métrica específica de Amazon EC2 cruza el umbral de alarma, podremos Auto escala dinámicamente agregue o quite instancias de EC2 o enviarle una notificación.


Ver gráficas y estadísticas: ver gráficos y estadísticas para cualquiera de sus mediciones en el salpicadero de Amazon CloudWatch y obtener una visión rápida de todas sus alarmas y supervisar los recursos AWS en un solo lugar.

