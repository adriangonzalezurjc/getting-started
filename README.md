# Aplicación "To-Do"

## Definición de la Aplicación
La aplicación "To-Do" es un gestor de tareas simple que permite a los usuarios crear, editar, marcar como completadas y eliminar tareas de su lista personal. Está desarrollada utilizando Node.js para el backend y Express.js como framework web, con una interfaz de usuario interactiva construida con HTML, CSS y JavaScript.

## Cómo Ejecutar la Aplicación
Para ejecutar la aplicación utilizando Docker Compose, sigue estos pasos:

### 1. Clonar el Repositorio
git clone https://github.com/adriangonzalezurjc/getting-started.git
cd app

### 2. Construir y Ejecutar la Aplicación
Ejecutar el siguiente comando para construir y ejecutar la aplicación:
docker-compose up

Esto construirá la imagen de la aplicación y lanzará el contenedor. Una vez que la aplicación esté en funcionamiento, se puede acceder a ella desde el navegador en http://localhost:8000


## Consideraciones de Seguridad
Durante el diseño de la aplicación, se han tenido en cuenta diversas consideraciones de seguridad para proteger los datos de los usuarios y garantizar un funcionamiento seguro. Algunas de estas consideraciones incluyen:

- Validación de entrada de datos para prevenir ataques de inyección.
- Uso de tokens JWT para autenticación y autorización.
- Configuración de encabezados de seguridad en Express.js para protección contra ataques XSS y CSRF.
- Encriptación de contraseñas almacenadas en la base de datos.
- Implementación de medidas de protección contra vulnerabilidades comunes.


## Paso a Paso para Crear la Aplicación (S-SDLC)
Para crear el proyecto del Juice Shop desplegado en Docker siguiendo el Secure Software Development Lifecycle (S-SDLC), se deben seguir los siguientes pasos:

### 1. Recopilación de Requisitos

Definición de los Requisitos de la Aplicación:
- Identificar y documentar las funcionalidades esenciales de la aplicación, incluyendo la gestión de usuarios, la visualización de productos y el proceso de compra.
- Establecer requisitos de rendimiento, seguridad y usabilidad para garantizar una experiencia óptima para el usuario.

Análisis de Riesgos:
- Identificar posibles amenazas y vulnerabilidades asociadas con la aplicación.
- Realizar un análisis de riesgos exhaustivo y desarrollar estrategias para mitigarlos.

### 2.  Diseño del Sistema

Diseño de la Arquitectura:
- Establecer la estructura de directorios, modelos de datos y rutas necesarias para la aplicación.
- Definir la arquitectura de la aplicación, incluyendo la elección de un patrón de diseño apropiado como MVC.

Medidas de Seguridad:
- Implementar mecanismos de autenticación y autorización para controlar el acceso a las funcionalidades sensibles.
- Encriptar datos sensibles y aplicar medidas de protección contra vulnerabilidades comunes como XSS y CSRF.

### 3. Implementación

Configuración del Entorno de Desarrollo:
- Instalar y configurar las herramientas necesarias, como Node.js, Express.js y la base de datos correspondiente.
- Configurar el entorno de desarrollo para facilitar el desarrollo y la depuración de la aplicación.

Desarrollo de Funcionalidades:
- Escribir código para implementar las funcionalidades requeridas, como la gestión de usuarios, la navegación por el catálogo de productos y la finalización de pedidos.
- Implementar controles de validación y manejo de errores para garantizar la integridad y seguridad de los datos.

Seguridad en la Implementación:
-Aplicar prácticas de programación segura, como la sanitización de entradas y la prevención de vulnerabilidades de inyección.

### 4. Pruebas

Pruebas Unitarias:
- Desarrollar pruebas unitarias para cada componente de la aplicación, verificando su funcionamiento individual.
- Garantizar que todas las funciones cumplan con los requisitos y manejen adecuadamente casos límite.

Pruebas de Integración:
- Realizar pruebas de integración para asegurar la interoperabilidad entre los diferentes módulos de la aplicación.
- Verificar que la comunicación entre el front-end y el back-end funcione correctamente.

Pruebas de Seguridad:
- Ejecutar pruebas de seguridad, como análisis estático de código y pruebas de penetración, para identificar y corregir posibles vulnerabilidades.

### 5. Despliegue

Configuración del Entorno de Producción:

- Configurar un entorno de producción seguro, utilizando protocolos de comunicación cifrados como HTTPS y certificados SSL.
- Implementar medidas de seguridad adicionales, como firewalls y restricciones de acceso.

Despliegue de la Aplicación:
- Empaquetar la aplicación en contenedores Docker para facilitar su despliegue y escalabilidad.
- Utilizar herramientas como Docker Compose para gestionar y orquestar los contenedores en el entorno de producción.

### 6. Mantenimiento

Gestión de Versiones y Actualizaciones:
- Mantener un control de versiones utilizando sistemas de control de versiones como Git.
- Aplicar actualizaciones y correcciones de seguridad de manera regular para mantener la aplicación protegida contra las últimas amenazas.

Monitorización y Registro:
- Implementar sistemas de monitorización para supervisar el rendimiento y la disponibilidad de la aplicación en tiempo real.
- Configurar registros detallados para registrar eventos y alertas, facilitando la detección temprana de problemas y actividades sospechosas.

