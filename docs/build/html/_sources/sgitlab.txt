==========
Git lab
==========

sinopsis
------------

GitLab es una increíblemente poderosa plataforma de colaboración de código fuente abierto, gerente repositorio git, seguimiento de incidencias y revisor código. Se integra con los gestores de incidencias, servicios de integración continua y tiene compatibilidad con Active Directory fenomenal. Se instala redis servidor y funciones de la biblioteca también. Esta es manejable en Ubuntu y CentOS.

comando Ayuda
----------------------

Comando de Ayuda incluye una extensa, sistema de ayuda basado en la consola, que recuerda a las páginas de manual en Ubuntu. Los temas de ayuda incluyen ayuda para la instalación de las dependencias y bibliotecas Redis servidor. Fácil de escribir los comandos sin argumentos.

.. code-block:: bash

		ptconfigure gitlab help

Las siguientes capturas de pantalla explica sus funciones claramente.

.. code-block:: bash

 kevell@corp:/# ptconfigure gitlab help
 ******************************


  This command allows you to install a full Git Lab installation on to a server
  The dependencies for GitLab are also installed.

  GitLab, gitlab, git-lab

        - install
        Installs the latest version of GitLab on a system
        example: ptconfigure gitlab install

 ------------------------------
 End Help
 ******************************

instalación
---------------------

    La instalación incluye la provisión de o conexión a los servicios necesarios para hacer que el equipo instalado listo para funcionar. Es un proceso de revelado a instalar el módulo de laboratorio git bajo ptconfigure sólo por el uso de la orden dada a continuación,

.. code-block:: bash

		ptconfigure gitlab install

Después de vitalizar el comando se catequizar entrada.

La entrada del usuario como si automáticamente se instalará gitlab con la comprobación del sistema. La siguiente captura de pantalla demuestra.

Opciones
------------

.. cssclass:: table-bordered

 +--------------------------+--------------------------------------------+-------------+-----------------------------------------+
 | Parámetros               | Parámetro Alternativa                      | Opciones    | Comentarios                             |
 +==========================+============================================+=============+=========================================+
 |Install gitlab?(Y/N)      | En lugar de utilizar gitlab podemos        | Y(Yes)      | Se instalará git y un conjunto de       |
 |                          | utilizar Gitlab, gitlab, git-lab           |             | gitlab común bajo ptconfigure.          |
 +--------------------------+--------------------------------------------+-------------+-----------------------------------------+
 |Install gitlab?(Y/N)      | En lugar de utilizar gitlab podemos        | N(No)       | La salida de sistema de la instalación  |
 |                          | utilizar Gitlab, gitlab, git-lab|          |             |                                         | 
 +--------------------------+--------------------------------------------+-------------+-----------------------------------------+


Beneficios
--------------

* Gitlab rastrea el contenido en lugar de los archivos
* Las ramas son de peso ligero, y la fusión es un proceso sencillo
* Permite un proceso de desarrollo fuera de línea más aerodinámica
* Los repositorios son de menor tamaño y se almacenan en un único directorio .git
* Permite operaciones de almacenamiento intermedio avanzados, y el uso de esconder cuando se trabaja a través de secciones problemáticos.
* Desarrollado para sistemas Ubuntu, sin embargo existe el apoyo comunitario a otras distribuciones como Arch, CentOS, Fedora o Gentoo
* Requiere una versión y componentes incluidos para operar
