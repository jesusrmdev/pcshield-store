# PcShield Store - JRM

Aplicación web para la gestión de incidencias de soporte técnico de una tienda online de informática, desarrollada como proyecto práctico del módulo de **Fundamentos de Inteligencia Artificial Generativa (FIAG)** de 2.º curso del ciclo formativo de Desarrollo de Aplicaciones Web (DAW).

La aplicación permite gestionar tickets de soporte, consultar estadísticas y aplicar mecanismos de protección de datos personales mediante anonimización y detección de posibles intentos de Prompt Injection.

## Características principales

- **Dashboard interactivo:** visualización de indicadores KPI y estadísticas generales de las incidencias.
- **Gestión de tickets:** creación, consulta, resolución y eliminación de incidencias.
- **Búsqueda y filtrado:** localización de tickets mediante palabras clave y categorías.
- **Protección de datos personales:** detección y anonimización de DNI/NIE, números de tarjetas bancarias y direcciones IPv4.
- **Protección frente a XSS:** detección y bloqueo de contenido HTML y JavaScript potencialmente peligroso.
- **Detección de Prompt Injection:** identificación de instrucciones sospechosas y bloqueo del envío cuando se detectan.
- **Laboratorio de Pruebas RGPD:** ejecución de pruebas controladas con datos ficticios y escenarios de seguridad.

## Tecnologías utilizadas

- HTML5: estructura de la aplicación.
- TailwindCSS: diseño y estilos de la interfaz.
- JavaScript Vanilla: lógica y funcionalidades interactivas.
- localStorage: almacenamiento local y persistencia de los datos en el navegador.
- JSON: datos iniciales utilizados para cargar las incidencias.

## Herramientas y metodología de desarrollo

Durante el desarrollo se han utilizado herramientas y técnicas de inteligencia artificial generativa para planificar, construir y mejorar la aplicación:

- **OpenCode:** asistente de desarrollo mediante instrucciones estructuradas.
- **Prompt Engineering:** diseño de instrucciones para procesar, anonimizar y clasificar información.
- **Comandos personalizados:** automatización de tareas mediante instrucciones reutilizables.
- **Skills:** incorporación de instrucciones especializadas para diseño web y protección de datos.
- **OpenSpec:** definición de propuestas, requisitos funcionales y tareas de desarrollo.
- **Prompt Chaining:** división de la construcción de la aplicación en diferentes etapas.
- **Auditoría y reflexión:** análisis del código, identificación de problemas y aplicación de mejoras.
- **Git y GitHub:** control de versiones y alojamiento del código fuente.
- **Netlify:** despliegue de la aplicación web.

## Instalación y ejecución

La aplicación está desarrollada con tecnologías web que se ejecutan directamente en el navegador. No requiere un proceso de compilación ni la instalación de dependencias mediante npm para su ejecución básica.

1. Clonar el repositorio o descargar el proyecto.
2. Abrir la carpeta `01-taller-helpdesk` en Visual Studio Code.
3. Abrir el archivo `index.html` utilizando Live Server.
4. Acceder a la dirección local proporcionada por Live Server desde el navegador.

## Almacenamiento de datos

La aplicación utiliza `localStorage` para guardar los cambios realizados en los tickets y mantenerlos después de recargar la página.

Los datos iniciales se encuentran en `datos_tickets.json`. No se utiliza una base de datos remota, por lo que la información almacenada depende del navegador y del dispositivo desde el que se accede.

## Arquitectura y documentación del proyecto

El proyecto incluye archivos de código fuente y documentación técnica para organizar el desarrollo asistido por inteligencia artificial:

- `index.html`: estructura principal de la interfaz.
- `app.js`: lógica de la aplicación y gestión de incidencias.
- `datos_tickets.json`: datos iniciales de los tickets.
- `AGENTS.md`: contexto técnico y reglas de desarrollo para el agente.
- `.opencode/commands/`: comandos personalizados de OpenCode.
- `.agents/skills/`: Skills utilizadas durante el desarrollo.
- `openspec/`: propuestas, especificaciones y tareas de las funcionalidades.

## Aplicación desplegada

La aplicación está publicada en Netlify y se puede consultar desde el siguiente enlace:

**[Acceder a PcShield Store - JRM](https://sparkly-dodol-373c21.netlify.app)**

## Contexto académico

Este proyecto se ha desarrollado en el marco del taller UT2, *Construcción de una aplicación web con Ingeniería de Prompts, Skills y OpenSpec*, correspondiente al módulo de Fundamentos de Inteligencia Artificial Generativa de 2.º DAW.

**Autor:** Jesús Rodríguez Marín  
**Centro educativo:** IES Alcántara  
**Curso académico:** 2026/2027

El proyecto tiene su origen en una actividad académica y documenta la aplicación práctica de técnicas de ingeniería de prompts y desarrollo asistido por inteligencia artificial generativa.

## Limitaciones actuales

- Los datos se almacenan localmente en el navegador mediante `localStorage`.
- No existe una base de datos remota ni sincronización entre dispositivos.
- No se ha integrado un servicio externo de inteligencia artificial en tiempo real.

---

**PcShield Store - JRM** · Proyecto desarrollado con HTML5, TailwindCSS y JavaScript Vanilla.