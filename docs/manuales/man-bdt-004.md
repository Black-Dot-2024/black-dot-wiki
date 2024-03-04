# MAN-BDT-004 Consideraciones para Diseñar un Requerimiento

v 1.0.0

## Propósito

Ayudar a los miembros del equipo a decidir la creación de un diagrama para describir un requisito.

## Notas introductorias

Los diagramas son importantes cuando se necesita aclarar la complejidad, visualizar interdependencias, comunicarse eficazmente, o documentar y mantener el sistema a lo largo del tiempo.

## Involucrados

Team members, AO, TL y PO

## Entradas

Requisito a nivel sistema.

## Salidas

Decisión sobre la necesidad de diseñar un diagrama.

## Procedimiento

Hacer un diagrama facilitará los siguientes aspectos:

1. Conocer la interdependencia de componentes
 - Debes ser capaz de visualizar como el requerimiento interactúa con los diferentes componentes del sistema (DB, Usuario, etc).

2. Comprender la descripción y funcionalidad del requerimiento
 - Identificar y entender su descripción. No eres capaz de explicarle a una persona cómo es que este requerimiento actúa en el sistema, ya sea backend o frontend.

3. El diagrama brinda valor a la documentación del proyecto
 - Existen varios requerimientos que llegan a ocupar el mismo diagrama, solo cambian algunos campos, por eso necesitas analizar si no existe un diagrama parecido. Si existen diagramas similares, entonces no aporta valor.

4. Existen interacciones o flujos complejos
 - Identificar si tu requisito implica la interacción con el usuario u otros componentes del sistema (como módulos, servicios y subsistemas).

5. Necesitas practicar
 - Es bueno realizar diagramas para entender las partes de como este requerimiento interactúa con el sistema.

6. Identificar procesos asíncronos o multihilos
 - Identificar si tu requisito incluye procesos asíncronos o multihilos.


## Control de cambios

| Versión | Cambio                 | Autor del cambio | Aprobado por | Fecha de cambio |
| ------- | ---------------------- | ---------------- | ------------ | --------------- |
| v 1.0.0 | Creación del manual    | Uri Gopar <br /> Mafer Moreno   | Ian Padrón <br /> Armando Rosas <br /> Ramona Nájera |02/03/2024|
