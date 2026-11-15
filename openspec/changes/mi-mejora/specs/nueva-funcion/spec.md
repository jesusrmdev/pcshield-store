
# Especificación: Laboratorio de Pruebas RGPD

## ADDED Requirements

### Requirement: Acceso al Laboratorio de Pruebas RGPD

La aplicación DEBE incorporar una sección identificada como "Laboratorio de Pruebas RGPD", accesible desde la interfaz principal.

#### Scenario: Visualización del laboratorio

- **WHEN** el usuario accede a la sección del laboratorio
- **THEN** la aplicación muestra los controles disponibles para ejecutar las pruebas de seguridad.

### Requirement: Pruebas de detección y anonimización de datos personales

La aplicación DEBE proporcionar botones para generar textos de prueba con DNIs, números de tarjetas bancarias y direcciones IPv4 ficticias.

Los datos utilizados en las pruebas DEBEN ser exclusivamente ficticios.

#### Scenario: Detección de datos personales

- **WHEN** el usuario ejecuta una prueba de DNI, tarjeta bancaria o dirección IPv4
- **THEN** la aplicación procesa el texto mediante las funciones de protección RGPD existentes y muestra el resultado anonimizado.

### Requirement: Detección de ataques de Prompt Injection

La aplicación DEBE proporcionar una prueba específica para comprobar la detección de intentos de Prompt Injection.

#### Scenario: Bloqueo de Prompt Injection

- **WHEN** el usuario ejecuta una prueba con un texto que contiene instrucciones maliciosas
- **THEN** la aplicación utiliza el detector existente y muestra el resultado de la detección o bloqueo.

### Requirement: Visualización de resultados de las pruebas

La aplicación DEBE mostrar el resultado de cada prueba ejecutada, diferenciando entre datos detectados y anonimizados y ataques bloqueados.

#### Scenario: Presentación del resultado

- **WHEN** finaliza una prueba de seguridad
- **THEN** la aplicación muestra el texto original de prueba y el resultado de su procesamiento, sin almacenar datos personales reales.

### Requirement: Gráfico de incidencias por categoría

La aplicación DEBE incorporar un gráfico visual de barras, desarrollado mediante HTML y CSS, que represente el número de incidencias agrupadas por categoría.

#### Scenario: Representación de incidencias

- **WHEN** el usuario consulta el gráfico
- **THEN** la aplicación muestra barras diferenciadas por categoría y sus correspondientes cantidades.

### Requirement: Compatibilidad con las funcionalidades existentes

La incorporación del laboratorio NO DEBE alterar el funcionamiento de la bandeja de tickets, los filtros, el buscador, la creación, resolución y eliminación de incidencias ni los mecanismos de protección RGPD existentes.

#### Scenario: Conservación de funcionalidades

- **WHEN** el usuario utiliza la aplicación después de incorporar el laboratorio
- **THEN** las funcionalidades anteriores continúan funcionando correctamente.
