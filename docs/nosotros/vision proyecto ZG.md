# Visión del Proyecto Zeitgeist

# Necesidad

Mejorar la trazabilidad y continuidad de las actividades de los proyectos de la empresa y facilitar la comunicación de éstos entre los departamentos legal y contable.

# Misión

Sistema centralizado de gestión de proyectos que les permita atender de manera continua las actividades de un proyecto y eliminar horas perdidas por olvido de ellas.

# Objetivos

- Facilitar la gestión de un proyecto de dos a un lugar.
- Informar periódicamente el estado de un proyecto a sus participantes.

- Aumentar la cantidad de proyectos semestrales que acepta la empresa en al menos 1.
- Reducir la cantidad de actividades olvidadas relacionadas a un proyecto en un 30%.

# Alcance y restricciones 

Consultar, agregar, borrar y modificar proyectos de la empresa y sus actividades (lineales y periódicas) en el área legal y contable. Notificar a los participantes de dichas actividades acerca de cambios y fechas de entrega.

# Entregables

- Código fuente
- Manual de usuario
- Manual de despliegue
- Perfil de desarrollador
- Descripción general del sistema

# Ciclo de vida del proyecto

| Comienzo                                          | Ejecución                                         | Transición                                |
| :-------:                                         | :--------:                                        | :----------:                              |
| Consolidar el departamento                        | Realizar prueba temprana de arquitectura          | Garantizar la disponibilidad del producto |
| Alinearse a la visión del cliente                 | Abordar las necesidades cambiantes del cliente    | Desplegar la solución                     |
| Definir el alcance                                | Producir una solución potencialmente consumible   |                                           |
| Identificar estrategia de arquitectura            | Mejorar la calidad                                |                                           |
| Planificar las entregas                           | Acelerar la entrega de valor                      |                                           |
| Desarrollar estrategia de pruebas                 |                                                   |                                           |
| Establecer una visión compartida con el cliente   |                                                   |                                           |
| Asegurar financiamiento del proyecto              |                                                   |                                           |

A lo largo de todo el ciclo de vida, las siguientes actividades deben verse reflejadas de forma continua
* Desarrollar las habilidades del equipo
* Transformar nuestro WoW
* Manejar trabajo entrante
* Organización del equipo
* Coordinar actividades
* Aprovechar y mejorar la infraestructura existente
* Monitorear métricas 
* Evaluación de resultados
* Manejar el riesgo

# Iteraciones del proyecto 

## Comienzo
Se realizarán dos iteraciones.

**1ra iteración**: Se crea la primera versión de los lineamientos departamentales y se validan. <br/>
**2da iteración**: Se modifican los lineamientos de acuerdo a la reatroalimentación para consolidarlos.

####    Hitos asociados:
- Inicio del proyecto
- Validación de la visión con el cliente

## Construcción
Se realizarán al menos tres iteraciones, una por cada versión para que sea validada antes de pasar a la fase de transición.

####    Hitos asociados:
- Prueba de arquitectura
- Viabilidad del proyecto

## Transición
Se realizarán tres iteraciones, una por cada versión entregada.

####    Hitos asociados:
- MVP
- MBI 1
- MBI 2

# Stakeholders

| Categoría          | Encargado |
| -------------------|-----------|
| Customer or Client | ZeitGeist |
| Project Core Team  | Black Dot |
| Program Manager    | Olimpia Garcia y Daniel Fuentes |
| Product Owner      | Ricardo Fernandez |
| Team Lead          | Rodrigo Terán Hernández |
| Architecture Owner | Carlos Salguero |
| Project Team Member | Diego Perdomo, Armando Rosas Balderas, Sebastian Flores, Sergio Garnica, Daniel Hurtado, Frida Bailleres, Denisse Dominguez, Ian Padrón, Yuna Chung ., Arturo Díaz y Ramona Nájera |

# Hitos del Proyecto

| | Descripción | Fecha |
|-|-------------|-------|
| Inicio del proyecto | Primer día del proyecto | 13/02/2024 |
| Validación de visión con el cliente | Validación de este documento | 01/03/2024 |
| Prueba de la arquitectura | | | 
| Validación del proyecto | | |
| MVP | Primera entrega del proyecto | 10/05/2024 |
| MBI 1.0 | | 24/05/2024 |
| MBI 2.0 | | 07/06/2024 |
| Fin del proyecto | Último día del proyecto | 14/06/2024 | 

# Arquitectura 

## Arquitectura seleccionada

### Frontend 🌐

- <u>[**React**](https://reactjs.org/) </u> ⚛️: Biblioteca de JavaScript para construir interfaces de usuario. Utilizada para gestionar el estado y las interacciones en la aplicación web.
- <u>[**TypeScript**](https://www.typescriptlang.org/) </u>📘: Superset de JavaScript que añade tipado estático, mejorando la calidad del código y la productividad.
- <u>[**Tailwind CSS**](https://tailwindcss.com/) </u> 🎨: Framework de CSS para diseñar componentes de interfaz de usuario con estilos predefinidos y utilidades personalizables.

### Backend 🔧

- <u>[**Node.js**](https://nodejs.org/) </u> 🟢: Entorno de ejecución para JavaScript en el servidor, maneja las solicitudes HTTP y la lógica de negocio.
- <u>[**Express.js**](https://expressjs.com/) </u> 🚀: Framework para Node.js que facilita la creación de servidores web y la definición de rutas de API.
- <u>[**Prisma**](https://www.prisma.io/)  </u> 🗃️: Herramienta ORM para modelar y gestionar la base de datos, simplificando las interacciones con PostgreSQL.
- <u>[**PostgreSQL**](https://www.postgresql.org/)  </u>🐘: Sistema de gestión de bases de datos relacional, utilizado para almacenar los datos de la aplicación.
- <u>[**Mocha**](https://mochajs.org/) </u> & <u> [**Chai**](https://www.chaijs.com/) </u>☕🍵: Herramientas para realizar pruebas unitarias y de integración en el backend.

## Justificación de arquitectura

| Aspecto | Opción seleccionada | Alternativa 1 | Alternativa 2 | Razón de la selección |
|---------|---------------------|---------------|---------------|-----------------------|
| Backend | NodeJS con Express  | Django y python | Flask y python | Node.js con Express es altamente eficiente para operaciones I/O no bloqueantes, lo que es crucial para un ERP que maneja múltiples solicitudes simultáneas. Django y Flask son robustos, pero Node.js supera en rendimiento para aplicaciones en tiempo real y de alta concurrencia. | 
| ORM | Prisma | SQLAlchemy | Django ORM | Prisma ofrece una integración perfecta con TypeScript y una experiencia de desarrollo más moderna y segura, con funciones avanzadas como la migración automática de esquemas. SQLAlchemy y Django ORM son poderosos, pero Prisma proporciona una experiencia más fluida con TypeScript. |
| Frontend | ReactJS con Material-UI | Angular con Angular Material | Vue.JS con Vuetify | ReactJS ofrece una curva de aprendizaje más suave y una mayor flexibilidad en comparación con Angular, lo que permite un desarrollo más rápido y eficiente. Material-UI proporciona un conjunto de componentes de diseño coherente y personalizable que se integra bien con ReactJS. Angular y Vue.js son potentes, pero ReactJS ofrece mayor agilidad en el desarrollo.|
| Lenguaje de Programación | TypeScript | Python | JavaScript | TypeScript ofrece ventajas significativas en términos de seguridad de tipos y detección de errores en tiempo de compilación, lo que reduce los errores en tiempo de ejecución en aplicaciones complejas como un ERP. Python y JavaScript son versátiles, pero carecen de la seguridad de tipos de TypeScript. |

## Presupuestos de Despliegue

En esta propuesta, presentamos una estimación de costos para los servicios de infraestructura que se utilizarán en el proyecto. 

| Propuesta | Descripción de Servicios | Costo Total Mensual (MXN) |
|-----------|--------------------------|---------------------------|
| Básico AWS | Servicios gratuitos limitados para alojar la aplicación y almacenar documentos. | $5 |
| Intermedio AWS | Servicios básicos para alojar y gestionar la aplicación, con almacenamiento para documentos y archivos  | $216.39 |
| Avanzado AWS | Servicios mejorados para un mejor rendimiento y capacidad de almacenamiento. | $315 |
| Alternativa Google | Alternativa gratuita con servicios de Google para alojar y gestionar la aplicación, con límites de uso. | $0 |

# Riesgos 

```
Falta por agregar 
```
