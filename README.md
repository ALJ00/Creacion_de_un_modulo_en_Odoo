# Manual de creación de un módulo de Odoo con Python

Odoo utiliza una arquitectura basada en Cliente/Servidor en la que en la parte de cliente atúan los navegadores web y el 
servidor la propia tecnología de Odoo.

La lógica de negocio se realiza toda en el lado del servidor aunque se pueden agragar al cliente características compatibles.

Prácticamente todo el trabajo se ejecuta por lína de comandos propios de Odoo por lo que se partíría de invocar el comando 
***`odoo-bin`*** .

### Construcción de un módulo

Odoo basa su estructura de trabajo en módulos los cuales pueden tener una lógica de negocio propia o tenerla vinculada a 
a otro. Por lo tanto Odoo comienza en los módulos y acaban el los módulos.

### Composición de un módulo

Un módulo de Odoo se podría decir que se compone de tres elementos principales:

* Objectos de negocio

    Se declaran como clases en Python.
    
* Archivos de datos:
    
    Archivos XML o CSV que declaran metadatos (vistas o informes), datos de configuración (parametrización de módulos) y 
    datos de demostración.
    
* Controladores web

    Sun función es manejar las solicitudes de navegadores web, datos web, archivos css o javascript.
    
### Estructura de un módulo

Se puede decir que un módulo es una estructura de archivos interrelacionados entre sí y se declara mediante un archivo 
manifiesto. También es un paquete ***`_init_.py`*** que contiene instrucciones importables para varios archivos Python del 
módulo.

Para instanciar un módulo simplemente habría que tener en cuenta el archivo ***`nombredelmodulo.py`*** .

### Modelo Objeto-Relación

Un componente clave de Odoo es la capa ORM. Esta capa evita tener que escribir la mayoría de los SQL a mano y 
proporciona servicios de extensibilidad y seguridad.

### Archivos de datos

Odoo es un sistema altamente impulsado por datos. Aunque el comportamiento se personaliza utilizando el código Python.

### Acciones y menús.

Las acciones y los menús son registros regulares en la base de datos, generalmente declarados a través de archivos de datos. 







