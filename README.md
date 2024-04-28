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
Para crear esta aplicación desde cero siguiendo el Secure Software Development Lifecycle (S-SDLC), se deberían seguir estos pasos:

### 1. Recopilación de Requisitos
Definir los Requisitos de la Aplicación:
- Identificar y documentar las funcionalidades básicas, como agregar, eliminar y marcar tareas.
- Establecer requisitos de rendimiento, seguridad y usabilidad.
Análisis de Riesgos:
- Identificar posibles amenazas y vulnerabilidades en la aplicación.
- Realizar análisis de riesgos y establecer estrategias para mitigarlos.
  
### 2. Diseño del Sistema
Diseño de la Arquitectura:
- Establecer la estructura de directorios, modelos de datos y rutas.
- Definir la arquitectura de la aplicación, incluyendo el patrón MVC (Modelo-Vista-Controlador) u otro diseño adecuado.
Medidas de Seguridad:
- Implementar autenticación y autorización para controlar el acceso a las funcionalidades.
- Encriptar datos sensibles y establecer medidas de protección contra ataques como XSS y CSRF.

### 3. Implementación
Configuración del Entorno de Desarrollo:
- Instalar y configurar Node.js y Express.js para el desarrollo de la aplicación.
- Configurar la base de datos, según las necesidades del proyecto.
Desarrollo de Funcionalidades:
- Escribir scripts y controladores para las operaciones CRUD (Crear, Leer, Actualizar, Eliminar) de las tareas.
- Implementar lógica de negocio para validar y procesar las tareas según los requisitos.
Seguridad en la Implementación:
- Aplicar buenas prácticas de programación segura, como la validación de entrada de datos y la prevención de inyecciones SQL.
- Implementar manejo adecuado de sesiones y tokens para la autenticación.

### 4. Pruebas
Pruebas Unitarias:
- Desarrollar pruebas unitarias para cada función y componente de la aplicación.
- Verificar que cada función se comporte como se espera y maneje casos de borde.
Pruebas de Integración:
- Ejecutar pruebas de integración para garantizar que los diferentes componentes funcionen correctamente juntos.
- Verificar la comunicación entre las capas de la aplicación, como las rutas y la capa de persistencia.
Pruebas de Seguridad:
- Realizar análisis estático de código para identificar posibles vulnerabilidades.
- Ejecutar pruebas de penetración y análisis de vulnerabilidades para identificar y corregir posibles brechas de seguridad.

### 5. Despliegue
Configuración del Entorno de Producción:
- Configurar un entorno de producción seguro utilizando HTTPS y certificados SSL para proteger la comunicación.
- Establecer medidas de seguridad adicionales, como cortafuegos y reglas de acceso.
Despliegue de la Aplicación:
- Empaquetar la aplicación en contenedores Docker para facilitar el despliegue y la portabilidad.
- Utilizar Docker Compose para gestionar y orquestar los contenedores en el entorno de producción.

### 6. Mantenimiento
Gestión de Versiones y Actualizaciones:
- Mantener un control de versiones adecuado utilizando herramientas como Git para gestionar el código fuente.
- Aplicar actualizaciones de seguridad y correcciones de errores de manera regular.
Monitorización y Registro:
- Implementar herramientas de monitoreo para supervisar el rendimiento y la disponibilidad de la aplicación en producción.
- Configurar registros para registrar eventos y alertas de posibles problemas o actividades sospechosas.
