===========================================================
Identificación de *Entities*, *Value Objects* y *Services*
===========================================================

Esta sección contiene la clasificación de los elementos del modelo de dominio como *entities*, *value objects* o *services* de acuerdo con la filosofía de diseño *domain-driven design* [Evans2003]_.

.. Attention:: Por cuestiones de brevedad, y para hacer este proyecto más fácilmente comprensible, esta sección sólo contiene la clasificación de las entidades que aparecen en los diagramas ``Vehículos``, ``Reparaciones`` y ``Órdenes de Trabajo``  del modelo de dominio.

Entities
=========

  Aseguradora

  Departamento

  Empleado

  Material
    Los tipos de materiales que se utilizarán para las reparaciones son un tipo de elemento con identidad clara, cuya existencia se debe monitorizar a lo largo del ciclo de vida de la aplicación. Existen búsquedas, por ejemplo, para elaborar presupuestos, o definir servicios, que harán búsquedas de materiales concretos.

  Modelo

  OrdenTrabajo

  Persona
    Son elementos con identidad clara, que pueden ser utilizados para realizar búsquedas que sirvan de punto de entrada al sistema, y cuyos cambios a lo largo de su ciclo de vida nos interesa trazar con claridad. Por ejemplo, nos interesa saber el númeo de facturas abonadas por una determianda persona.

  Propietario

  Recepción

  Servicio

  Siniestro

  Usuario

  Vehiculo

Descartados
------------

  * Calendario
  * Cheque
  * Cuenta Corriente
  * Documento
  * Factura
  * Log
  * Pago
  * Semana laboral
  * Tarjeta (entity)

Value Objects
==============

  Categoría Profesional

  Datos Bancarios

  Dirección

  Estado Orden de Trabajo

  Estado Presupuesto

  Fabricante

  Gasto de Material

  Gasto de Servicio Realizado

  Marca

  Material para Servicio

  País

  Presupuesto

  Provincia

  Tipo de Combustible

  Tipo de Vía

Services
=========

.. [Evans2003]  Eric Evans. *Domain-Driven Design* Addison-Wesley, 2003.
