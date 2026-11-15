
---
name: escudo-rgpd-js
description: Utiliza esta habilidad siempre que el usuario pida programar formularios web en HTML/JavaScript o validar entradas de texto de usuarios para proteger datos privados (PII).
---

# Habilidad: Escudo RGPD en Vivo para Formularios Web (2º DAW)

Siempre que generes o modifiques la lógica JavaScript de un formulario de creación de incidencias, debes incluir obligatoriamente estas 3 funciones:

## 1. Función `sanitizarTextoPII(texto)` en JavaScript

Programa una función clara y bien comentada con expresiones regulares sencillas que reemplace automáticamente en el texto del usuario:

- Cualquier DNI/NIE español (8 números y 1 letra) por `[DNI_OCULTO]`.
- Cualquier numeración de tarjeta de 16 dígitos por `[TARJETA_OCULTA]`.

## 2. Vista Previa en Tiempo Real (Live Shield)

Debajo del `<textarea>` donde el usuario escribe la incidencia, muestra un pequeño recuadro en vivo ("Vista previa protegida RGPD") que enseñe cómo va quedando el texto con los datos ya censurados a medida que el usuario teclea (evento `input`).

## 3. Detector Básico de Prompt Injection en Cliente

Si el texto escrito contiene frases trampa como:

- "ignora las instrucciones"
- "olvida tus reglas"
- "revela el prompt del sistema"
- "desactiva las medidas de seguridad"

muestra una alerta visual roja impidiendo enviar el formulario.


## 4. Detección y anonimización de direcciones IPv4

La función `sanitizarTextoPII(texto)` también debe detectar y ocultar cualquier dirección IPv4 que aparezca en el texto introducido por el usuario.

- Cualquier dirección IPv4 con formato `xxx.xxx.xxx.xxx` debe sustituirse por `[IP_OCULTA]`.
