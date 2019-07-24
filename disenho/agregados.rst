=============================
 Identificación de Agregados
=============================

Esta sección contiene el agrupamiento de los elementos del modelo de dominio en *aggregates*, más la identificación por cada *aggregate* de un *aggregate root*, de acuerdo con la filosofía de diseño *domain-driven design* [Evans2003]_.

.. Attention:: Por cuestiones de brevedad, y para hacer este proyecto más fácilmente comprensible, esta sección sólo contiene los agregados relacionados con los elementos de los diagramas ``Vehículos``, ``Reparaciones`` y ``Órdenes de Trabajo`` del modelo de dominio.

Agregado Vehículo
==================

  * Vehiculo
  * TipoCombustible

Agregado Modelo
================

  * Modelo
  * Marca

Agregado Propietario
=====================

  * Persona
  * Propietario
  * Catergoía Profesional
  * DatosBancarios
  * Dirección
  * País
  * Provincia
  * Tipo de Vía

Agregado Recepción
===================

  * Recepción
  * Siniestro

Agregado Aseguradora
=====================

  * Aseguradora

Agregado Presupuesto
=====================

  * Presupuesto
  * GastoServicio
  * GastoMaterial

Agregado Orden de Trabajo
==========================

  * Orden de Trabajo
  * Estado de Orden de Trabajo
  * Gasto de Material Realizado
  * Gasto de Servicio Realizado

Agregado Servicio
==================

 * Servicio
 * Gasto de Material por Servicio

Agregado Material
==================

  * Material
  * Fabricante

Agregado Empleado
==================

  * Empleado
  * No Laboral

Agregado Departamento
======================

  * Departamento
