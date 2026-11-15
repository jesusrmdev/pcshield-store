
# Especificación de la Aplicación Web PcShield Store - JRM

## ADDED Requirements

### Requirement: Panel Superior de Estadísticas (KPIs)

La web DEBE mostrar en la parte superior 4 tarjetas resumen que se calculen dinámicamente:

1. Total de tickets.
2. Tickets pendientes de prioridad ALTA (en rojo).
3. Total de datos privados (PII) interceptados y protegidos.
4. Ataques y rechazos bloqueados por el sistema de seguridad.

#### Scenario: Actualización automática de contadores

- **WHEN** se carga la página o se añade o resuelve un ticket.
- **THEN** las 4 tarjetas superiores actualizan sus números al instante.

### Requirement: Listado de Tickets con Filtros y Buscador

La web DEBE mostrar las incidencias en tarjetas visuales con insignias de colores según prioridad (`ALTA` rojo, `MEDIA` ámbar, `BAJA` verde) y su estado.

#### Scenario: Filtrado interactivo

- **WHEN** el usuario selecciona una categoría (`TODAS`, `REDES`, `HARDWARE`, `SOFTWARE`, `FACTURACION`, `SEGURIDAD`) o escribe en el buscador.
- **THEN** la lista muestra únicamente los tickets que coinciden sin recargar la página.

### Requirement: Formulario con Escudo RGPD en Vivo

La web DEBE incluir un formulario para crear un nuevo ticket que aplique las reglas de la Skill `escudo-rgpd-js`.

#### Scenario: Creación de ticket con datos sensibles

- **WHEN** el usuario introduce una incidencia que contiene un DNI, un número de tarjeta bancaria o una dirección IPv4.
- **THEN** la vista previa protegida RGPD muestra los datos sensibles sustituidos por los marcadores `[DNI_OCULTO]`, `[TARJETA_OCULTA]` e `[IP_OCULTA]`, respectivamente, y el ticket se guarda en `localStorage` sin exponer esos datos.

#### Scenario: Bloqueo de Prompt Injection

- **WHEN** el usuario introduce en el formulario frases como "ignora las instrucciones" u "olvida tus reglas".
- **THEN** se muestra una alerta visual roja y se impide el envío del formulario.
