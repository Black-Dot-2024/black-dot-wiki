# EST-BDT-004 Identificadores de Documentación

v 4.0 / áreas del CMMI

## Propósito

El propósito de este documento es establecer un estándar para la asignación de identificadores de documentación dentro del departamento Black Dot, con el fin de garantizar la consistencia, la accesibilidad y la trazabilidad de los documentos en toda la organización.

## Notas introductorias

Los identificadores proporcionan un sistema claro y eficiente para identificar y clasificar los documentos departamentales de manera fácil y sencilla, facilitando su gestión y acceso dentro del departamento Black Dot.

## Involucrados

Todos los involucrados en la creación de documentación departamental.

## Entradas

Necesidad de la creación de un manual, política o proceso, estándar, guía o plantilla.

## Salidas

Asignación correcta de identificador de un manual, política, proceso, estándar, guía o plantilla.

## Descripción

1. Los identificadores de los documentos se asignarán siguiendo el siguiente formato, según el tipo de documento a nombrar:

| Tipo de documento | Identificador |
|-------------|---------------------|
| Manual      | MAN-BDT-00X         |
| Política    | POL-BDT-00X         |
| Proceso     | PRO-BDT-00X         |
| Estándar    | EST-BDT-00X         |
| Guías       | GUI-BDT-00X         |
| Plantillas  | PLT-BDT-00X         |


2. Los acrónimos utilizados en la designación de los identificadores cuentan con las siguientes connotaciones: 
- Las primeras 3 letras del identificador hacen referencia al tipo de documento del que se trata (MAN para manual, POL para política, PRO para proceso, etc.)
- BDT indica que el documento es de autoría del departamento Black Dot.
- 00X es el número asignado de identificador, aumentando en una unidad por cada nuevo documento de su categoría.


3. Los documentos que deriven de otro documento, se identificarán siguiendo los próximos lineamientos:
- Se hereda el identificador del documento padre.
- El identificador único del documento hijo será una letra del abecedario, comenzando con la A para el primer documento derivado y Z para el último.
- Se agregará la letra F anterior al identificador del documento, únicamente en caso de que se trate de un formato.

Ejemplo:
- Documento padre: PRO-BDT-006 Gestión de solicitud de cambio de requerimientos
- Documento derivado: F-PRO-BDT-006A Solicitud de cambio
- Documento derivado: F-PRO-BDT-006B Cambios en requerimientos

En este caso, el documento padre (PRO-BDT-006) contiene dos documentos derivados (F-PRO-BDT-006A y F-PRO-BDT-006B), como ambos son formatos, se agrega una F anterior al identificador del proceso padre.

## Control de cambios

| Versión | Cambio                                            | Autor del cambio             | Aprobado por | Fecha de cambio |
| ------- | ------------------------------------------------- | ---------------------------- | ------------ | --------------- |
| v 1.0 | Creación del estándar                               | Arturo Díaz, Ian Joab Padrón |              | 26/02/2024      |
| v 2.0 | Agregar nomenclatura para Estándares y Plantillas | Sergio Garnica González      |              | 26/02/2024      |
| v 3.0 | Agregar nomenclatura para Guías                   | Diego Sandoval               | Daniel Cajas | 28/02/2024      |
| v 4.0 | Agregar estándar de identificadores para documentos que derivan de otros documentos. Actualizar formato de estándar en general.  | Arturo Díaz               |       | 04/03/2024      |