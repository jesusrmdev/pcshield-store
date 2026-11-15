
# Propuesta: Laboratorio de Pruebas RGPD

## Por qué (Objetivo)

Necesitamos ampliar PcShield Store - JRM con un entorno de pruebas que permita comprobar visualmente el funcionamiento de los mecanismos de protección de datos personales y detección de ataques implementados en la aplicación.

Esta funcionalidad permitirá realizar pruebas controladas de seguridad sin tener que introducir manualmente los datos de prueba en el formulario de creación de tickets.

## Qué se construye (Alcance)

Se incorporará una nueva sección denominada "Laboratorio de Pruebas RGPD" que incluirá:

- Botones para generar pruebas con DNIs, números de tarjetas bancarias y direcciones IPv4 ficticias.
- Pruebas de detección de ataques de Prompt Injection.
- Visualización del resultado de cada prueba, indicando si el contenido ha sido detectado y anonimizado o bloqueado.
- Un gráfico de barras desarrollado con HTML y CSS que represente el número de incidencias por categoría.

## Impacto técnico

- Modificación de `index.html` para incorporar la nueva sección y sus componentes visuales.
- Modificación de `app.js` para gestionar las pruebas y representar sus resultados.
- Reutilización de las funciones de protección RGPD existentes siempre que sea posible.
- Mantenimiento de las funcionalidades actuales de la aplicación.

## Resultado esperado

El usuario podrá ejecutar pruebas de seguridad desde el propio panel, comprobar visualmente los mecanismos de protección RGPD y consultar una representación gráfica de las incidencias clasificadas por categoría.
