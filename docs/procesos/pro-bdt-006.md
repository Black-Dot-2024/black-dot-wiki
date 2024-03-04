# PRO-BDT-006 Gestión de solicitud de cambio de requerimientos

v 1.0.0 / REQM, RD

## Propósito

Manejar la solicitud para cambios, creación o deprecación de requerimientos posterior al acuerdo de requerimientos iniciales.

## Involucrados

Product Owner, Architecture Owner, Cliente

## Entradas

Se hace una solicitud escrita para cambios, creación o deprecación de requerimientos. [Plantilla](https://github.com/Black-Dot-2024/docs/wiki/PL%E2%80%90BDT%E2%80%90005-Plantilla-de-solicitud-de-cambio-de-requerimientos)

## Salidas

Requerimiento modificado, definido o deprecado, según corresponda.

## Descripción

| Fase        | Actividades                                                                                                                                                                                                                                                                                                                                                                          | Responsables       | Prácticas Asociadas al CMMI      |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------ | -------------------------------- |
| Análisis    | Recopilar detalles y razón del cambio                                                                                                                                                                                                                                                                                                                                                | PO                 | REQM SP1.1                       |
|             | Definir y registrar el cambio de necesidad y requerimientos en el registro de cambios                                                                                                                                                                                                                                                                                                | PO                 | REQM SP1.1, REQM SP1.3, RD SP1.1 |
|             | Determinar los Impactados por los cambios                                                                                                                                                                                                                                                                                                                                            | PO                 | REQM SP1.1, REQM SP1.2           |
| Evaluación  | Evaluar los cambios solicitados en base a los siguientes criterios: <ul><li>Aporta valora la solución</li> <li>Se alinea con los objetivos del proyecto</li> <li>No compromete el calendario del proyecto</li> <li> No conlleva un retrabajo no justificado de funcionalidades ya planeadas o implementadas</li> <li>Es realizable con las habilidades técnicas del equipo</li></ul> | PO, AO, impactados | REQM SP1.2                       |
| Decisión    | Decidir si aceptar o no los cambios, definir bajo que condiciones y justificación                                                                                                                                                                                                                                                                                                    | Impactados         | REQM SP1.2                       |
| Negociación | Comunicar al cliente la decisión, condiciones y justificación                                                                                                                                                                                                                                                                                                                        | PO                 |                                  |
|             | Cuando se llegue a un acuerdo se realizan los cambios, definiciones o deprecaciones de requerimientos necesarios de acuerdo a las condiciones dadas y se actualiza el registro de cambios con las conclusiones (Referenciar guía de definición de requerimientos)                                                                                                                    | PO                 | REQM SP1.3, RD SP1.1             |

## Control de cambios

| Versión | Cambio                 | Autor del cambio | Aprobado por | Fecha de cambio |
| ------- | ---------------------- | ---------------- | ------------ | --------------- |
| v 1.0 | Descripción del cambio | Daniel Cajas     | Uri Gopar    | 28/02/2024      |
