UC001 - Recepcionar Vehículo
==============================

:Fuente: Gerente del Taller
:Actor Primario: Trabajador del Taller
:Actores Sec.: ---
:Descripción: 
:Objetivo: Reparar Vehículo
:Ev. Activación: Se selecciona la opción registrar vehículo al intentar recepcionar el mismo.
:Precondición: No existe ningún vehículo previo en el sistema con la misma matrícula que se intenta registrar.
:Garantía Éxito: El vehículo queda incorporado a la base de datos.
:Garantía Mín.: El sistema permanece en el mismo estado que al inicio del caso de uso y el usuario queda informado de las razones por las que no se pudo completar el caso de uso.
:Escenario:

 1. El sistema muestra al usuario el formulario `Registrar Vehículo`.
 2. El usuario completa y envía el formulario.
 3. El sistema certifica que los datos son correctos y están completos.
 4. El sistema certifica que no existe ningún vehículo con el mismo número de matrícula previamente registrado.
 5. El sistema incorpora el vehículo en el sistema de persistencia.
 6. El sistema notifica al usuario que el vehículo se ha incorporado al sistema, mostrando los datos del mismo.

:Extensiones:

  1. Hay algún problema de conexión con la base de datos y no se puede cargar correctamente el formulario.
  2. La red no está operativa.

    1. El sistema notifica del error al usuario.
    2. El usuario confirma haber leído el mensaje.
    3. El sistema vuelve al punto desde donde se originó el caso de uso.

  3. Algún dato del formulario es incorrecto.

    1. El sistema resalta en el formulario los campos incorrectos, proporcionando una explicación de por qué son incorrectos.
    2. El sistema regresa al punto 2 del escenario principal.

  3. Falta algún dato obligatorio.

    1. El sistema resalta en el formulario los campos obligatorios no completados, indicando que estos campos deben ser propocionados.
    2. El sistema regresa al punto 2 del escenario principal.

  4. Existe un vehículo con la misma matrícula dentro del sistema.

    1. El sistema notifica del error al usuario.
    2. El usuario confirma haber leído el mensaje.
    3. El sistema vuelve al punto 2 del escenario principal.

  5. El sistema de persistencia falla o no está disponible.

    1. El sistema notifica del error al usuario.
    2. El usuario confirma haber leído el mensaje.
    3. El sistema vuelve al punto desde donde se originó el caso de uso.

  8. El usuario selecciona la opción `Cancelar Alta`.

    1. El sistema vuelve al punto desde donde se originó el caso de uso.

:Comentarios:

  TODO: Añadir restricciones que deben cumplir los datos de entrada.

.. TODO: Añadir aquí el diseño del formulario como imagen.
