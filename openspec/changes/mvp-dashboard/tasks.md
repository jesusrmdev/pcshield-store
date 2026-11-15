
# Plan de Construcción Encadenado (Prompt Chaining)

- [x] **Eslabón 1 (Estructura HTML y Diseño):** Crear `index.html` con TailwindCSS incluyendo la cabecera de PcShield Store - JRM, las 4 tarjetas KPI, la barra de filtros y búsqueda, el contenedor de tickets y el modal o formulario de nuevo ticket con vista previa RGPD.

- [x] **Eslabón 2 (Motor de Datos y Filtros JS):** Crear `app.js` cargando los datos iniciales de `datos_tickets.json` en `localStorage`, renderizando las tarjetas de incidencias, implementando los filtros en vivo y el botón para marcar tickets como "RESUELTO".

- [x] **Eslabón 3 (Integración de la Skill Escudo RGPD):** Implementar en `app.js` las funciones definidas en la Skill `escudo-rgpd-js`: sanitización de datos personales mediante expresiones regulares (DNI/NIE, tarjetas bancarias y direcciones IPv4), vista previa protegida RGPD en tiempo real y bloqueo de intentos de Prompt Injection en el formulario.
