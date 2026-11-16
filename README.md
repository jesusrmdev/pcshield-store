# Taller UT2: Construcción de una App Web con Ingeniería de Prompts, Skills y OpenSpec

**PcShield Store - JRM**

## Índice de contenidos

- **1.** Introducción y objetivo del taller
- **2.** Requisitos previos y entregables
  - 2.1. Requisitos previos
  - 2.2. Entregables exigidos
- **3.** Regla 0: personalización obligatoria del proyecto
  - 3.1. Adaptación temática
  - 3.2. Nombre definitivo e identidad del proyecto
  - 3.3. Personalización de los archivos
- **4.** Fase 1. Preparación del proyecto y el mapa para la IA (AGENTS)
  - 4.1. Paso 1.1. Estructura de carpetas del proyecto
  - 4.2. Paso 1.2. Archivo AGENTS.md (contexto raíz del proyecto)
- **5.** Fase 2. Laboratorio de prompts en OpenCode
  - 5.1. Paso 2.1. Archivo bandeja_entrada_sucia.txt
  - 5.2. Paso 2.2. Técnicas de Prompt Engineering como comando
  - 5.3. Modificación del alumno 1
- **6.** Fase 3. Equipamos OpenCode con Skills
  - 6.1. Paso 3.1. Instalación de una Skill oficial de diseño web
  - 6.2. Paso 3.2. Creación de la Skill personalizada de calidad y escudo RGPD
  - 6.3. Modificación del alumno 2
- **7.** Fase 4. Construcción de la aplicación web con OpenSpec y Prompt Chaining
  - 7.1. Paso 4.1. Inicialización de OpenSpec
  - 7.2. Paso 4.2. Documentos proposal, spec y tasks
  - 7.3. Paso 4.3. Ejecución del Prompt Chaining
- **8.** Fase 5. Auditoría y mejora con Chain-of-Thought (CoT) y patrón Reflexión
  - 8.1. Auditoría del funcionamiento y seguridad
  - 8.2. Autocrítica, mejoras aplicadas y verificación posterior
- **9.** Fase 6. Funcionalidad individual con OpenSpec y despliegue web
  - 9.1. Paso 6.1. Especificación de la funcionalidad individual
  - 9.2. Paso 6.2. Subida a GitHub y publicación de la aplicación
- **10.** Pruebas finales y verificación de entregables
  - 10.1. Comprobaciones técnicas
  - 10.2. Pruebas funcionales del dashboard
  - 10.3. Pruebas del Laboratorio de Pruebas RGPD
  - 10.4. Verificación del gráfico y del despliegue
  - 10.5. Verificación de entregables
- **11.** Incidencias y soluciones aplicadas
  - 11.1. Advertencias durante la validación de OpenSpec
  - 11.2. Acceso restringido a la aplicación en Netlify
- **12.** Conclusiones
- **13.** Enlaces y referencias
  - 13.1. Repositorio GitHub
  - 13.2. Aplicación desplegada
  - 13.3. Documentación y herramientas consultadas
- **14.** Reto extra (opcional)

## 1. Introducción y objetivo del taller

El presente trabajo corresponde al Taller UT2: Construcción de una App Web con Ingeniería de Prompts, Skills y OpenSpec, perteneciente al módulo profesional optativo de Fundamentos de Inteligencia Artificial Generativa (FIAG), de 2.º curso del ciclo formativo de Grado Superior en Desarrollo de Aplicaciones Web (DAW), durante el curso académico 2026/2027.

El objetivo principal del taller ha sido construir una aplicación web funcional mediante el uso de herramientas de inteligencia artificial generativa, aplicando técnicas de Ingeniería de Prompts y metodologías de especificación y desarrollo asistido. El proyecto se ha desarrollado evitando el denominado Vibe Coding, basado en solicitar código sin una planificación previa. En su lugar, se ha seguido un flujo de trabajo estructurado, utilizando archivos de contexto, comandos personalizados, Skills y especificaciones formales.

Para ello, se han utilizado las siguientes herramientas y técnicas:

- OpenCode: asistente de terminal empleado para dirigir las tareas de desarrollo mediante instrucciones y comandos personalizados.
- Ingeniería de Prompts: diseño de instrucciones estructuradas para procesar información, clasificar incidencias y aplicar medidas de seguridad.
- Comandos personalizados: creación de comandos reutilizables mediante archivos Markdown dentro de .opencode/commands/.
- Skills: incorporación de instrucciones reutilizables para orientar a la inteligencia artificial en tareas de diseño web y protección de datos.
- OpenSpec: definición formal de las funcionalidades mediante documentos de propuesta, especificación y planificación de tareas.
- Prompt Chaining: división del proceso de construcción de la aplicación en diferentes etapas encadenadas.
- Auditoría y reflexión: revisión del código para identificar problemas de seguridad y usabilidad y aplicar mejoras.
- Git y GitHub: control de versiones y alojamiento del código fuente.
- Netlify: publicación de la aplicación para permitir su acceso desde Internet.

Como resultado del trabajo se ha desarrollado PcShield Store - JRM, una aplicación web destinada a la gestión de incidencias y pedidos de una tienda online de informática. La aplicación incorpora un dashboard interactivo, protección de datos personales, detección de intentos de Prompt Injection, filtros, estadísticas y un laboratorio de pruebas RGPD.

El proceso ha finalizado con la publicación de la aplicación en Netlify y la comprobación de su acceso público.

## 2. Requisitos previos y entregables

### 2.1. Requisitos previos

Para realizar el taller se han utilizado las herramientas de desarrollo indicadas en el guión oficial:

- Visual Studio Code: editor de código utilizado para trabajar con los archivos y carpetas del proyecto.
- Git: sistema de control de versiones utilizado para registrar los cambios y sincronizar el proyecto con GitHub.
- Node.js: entorno de ejecución de JavaScript necesario para utilizar las herramientas del ecosistema Node.
- npm y npx: herramientas utilizadas para gestionar paquetes y ejecutar utilidades del proyecto.
- OpenCode: asistente de terminal utilizado para ejecutar comandos personalizados, aplicar Skills y desarrollar la aplicación mediante instrucciones estructuradas.

Durante el desarrollo se ha comprobado el funcionamiento de estas herramientas mediante su utilización práctica:

- Se ha trabajado con el proyecto desde Visual Studio Code.
- Se han ejecutado operaciones Git para consultar el estado del repositorio, preparar cambios, crear commits y realizar el envío a GitHub.
- Se ha utilizado Node.js mediante el comando node --check app.js para comprobar la sintaxis de JavaScript.
- Se ha utilizado npx para ejecutar OpenSpec y validar las especificaciones.
- Se ha utilizado OpenCode para procesar los datos iniciales, construir la aplicación, realizar auditorías e implementar la funcionalidad individual.

No se ha registrado en esta memoria la versión exacta instalada de Node.js ni de npm.

### 2.2. Entregables exigidos

El guión del taller establece tres entregables principales:

#### 1. Repositorio privado en GitHub

Se ha utilizado el repositorio privado daw2-fiag, dentro de la siguiente ruta: ut2-prompt-engineering/01-taller-helpdesk/

En esta carpeta se encuentra el proyecto PcShield Store - JRM, con sus archivos de configuración, datos, comandos personalizados, Skills, especificaciones OpenSpec y código fuente.

#### 2. Aplicación web desplegada

La aplicación se ha publicado mediante Netlify y se ha configurado con visibilidad pública para permitir que el profesor pueda acceder a ella directamente desde el navegador. Dirección de acceso:

https://sparkly-dodol-373c21.netlify.app

#### 3. Memoria técnica en PDF

Se ha elaborado esta memoria técnica para documentar el desarrollo del taller, incluyendo las operaciones realizadas, las modificaciones individuales, las pruebas ejecutadas, las incidencias, las soluciones aplicadas y las capturas de pantalla correspondientes a las diferentes fases. La memoria ha sido entregada en formato PDF a través del Aula Virtual.

## 3. Regla 0: personalización obligatoria del proyecto

### 3.1. Adaptación temática

Mi primer apellido es Rodríguez, cuya inicial se encuentra dentro del grupo de apellidos comprendidos entre la O y la Z. Por tanto, según las instrucciones del taller, corresponde desarrollar un panel de soporte técnico y pedidos de una tienda online de informática.

### 3.2. Nombre definitivo e identidad del proyecto

El nombre seleccionado para la aplicación es:

**PcShield Store - JRM**

Las iniciales JRM corresponden a las iniciales de mi nombre y apellidos. La temática elegida representa una tienda online de informática que necesita gestionar incidencias técnicas y pedidos, manteniendo la protección de los datos personales de sus usuarios. Esta identidad se ha aplicado al proyecto y a la interfaz de la aplicación.

### 3.3. Personalización de los archivos

La personalización exigida se ha trasladado a los elementos principales del proyecto:

- AGENTS.md: se ha establecido el contexto y la identidad del proyecto PcShield Store - JRM.
- proposal.md: se ha definido la propuesta de desarrollo de acuerdo con la temática de soporte técnico y pedidos de una tienda de informática.
- index.html: se ha incorporado el nombre PcShield Store - JRM como título e identidad visual de la aplicación.
- bandeja_entrada_sucia.txt: el primer mensaje de entrada incluye mi nombre y primer apellido como remitente, tal como exige el guion.

De esta manera, se ha respetado la regla de personalización obligatoria y se ha mantenido una identidad coherente entre los documentos de planificación, los datos de entrada y la aplicación web final.

## 4. Fase 1. Preparación del proyecto y el mapa para la IA (AGENTS)

### 4.1. Paso 1.1. Estructura de carpetas del proyecto

Se creó la estructura inicial del proyecto UT2 dentro del repositorio privado daw2-fiag mediante el comando mkdir -p ut2-prompt-engineering/01-taller-helpdesk. Este comando permitió crear la carpeta principal ut2-prompt-engineering y, dentro de ella, la subcarpeta 01-taller-helpdesk, destinada a contener los archivos y recursos necesarios para desarrollar la aplicación web PcShield Store - JRM. Posteriormente, se ejecutó el comando find ut2-prompt-engineering -maxdepth 2 -type d para comprobar que ambas carpetas se habían creado correctamente.

El resultado confirmó que la estructura inicial coincide con la ruta establecida en el guion del taller.

![Figura 1. Creación y verificación de la estructura inicial de carpetas del proyecto UT2 en el repositorio daw2-fiag.](./img/img_01.png)

*Figura 1. Creación y verificación de la estructura inicial de carpetas del proyecto UT2 en el repositorio daw2-fiag.*

![Imagen de página 7](./img/img_02.png)

### 4.2. Paso 1.2. Archivo AGENTS.md (contexto raíz del proyecto)

Se creó el archivo AGENTS.md dentro de la carpeta ut2-prompt-engineering/01-taller-helpdesk/ para establecer el contexto técnico y las instrucciones que deberá seguir OpenCode durante el desarrollo de la aplicación PcShield Store - JRM. En el documento se definió la descripción general del proyecto, orientado a la gestión de incidencias de soporte técnico y pedidos de una tienda online de informática, así como el stack tecnológico obligatorio: HTML5, TailwindCSS, JavaScript Vanilla y almacenamiento de datos mediante localStorage, con carga inicial desde datos_tickets.json. Además, se incorporaron cuatro reglas de código para el agente, relacionadas con el uso del español, la prevención de vulnerabilidades XSS, la claridad del código y el control de lectura automatizada del enunciado. De este modo, el archivo proporciona a OpenCode una referencia con las características y restricciones que deberá respetar al trabajar en el proyecto.

![Figura 2. Creación y configuración del archivo AGENTS.md con el contexto técnico y las reglas de desarrollo de PcShield Store - JRM.](./img/img_03.png)

*Figura 2. Creación y configuración del archivo AGENTS.md con el contexto técnico y las reglas de desarrollo de PcShield Store - JRM.*

## 5. Fase 2. Laboratorio de prompts en OpenCode

### 5.1. Paso 2.1. Archivo bandeja_entrada_sucia.txt

Se creó el archivo bandeja_entrada_sucia.txt dentro de la carpeta ut2-prompt-engineering/01-taller-helpdesk/, incorporando los ocho mensajes sin procesar establecidos en el guion del taller. Estos mensajes representan diferentes situaciones relacionadas con incidencias informáticas y contienen ejemplos de información personal sensible (PII), como documentos de identidad, teléfonos, contraseñas, datos bancarios y direcciones IP, además de un intento de Prompt Injection y una consulta ajena al ámbito informático. También se realizaron las personalizaciones obligatorias: el primer mensaje incluye el nombre y primer apellido del alumno como remitente, mientras que el octavo plantea una incidencia relacionada con PcShield Store - JRM e incorpora una dirección IP privada y una contraseña en texto plano. Este archivo servirá como entrada para el posterior proceso de limpieza, anonimización y clasificación mediante OpenCode.

![Figura 3. Archivo bandeja_entrada_sucia.txt con los ocho mensajes de entrada y las personalizaciones requeridas para PcShield Store - JRM.](./img/img_04.png)

*Figura 3. Archivo bandeja_entrada_sucia.txt con los ocho mensajes de entrada y las personalizaciones requeridas para PcShield Store - JRM.*

### 5.2. Paso 2.2. Técnicas de Prompt Engineering como comando

Se creó el comando personalizado limpiar-y-clasificar.md dentro de la ruta .opencode/commands/ del proyecto PcShield Store - JRM. Este archivo define un prompt estructurado para procesar los mensajes de entrada mediante técnicas de Prompt Engineering. Se estableció el rol del agente, las reglas de anonimización de datos personales (PII), las instrucciones de seguridad frente a intentos de Prompt Injection y los criterios para clasificar las incidencias. Además, se incorporaron ejemplos Few-Shot para orientar el formato y el comportamiento esperado, así como una estructura de salida JSON y la variable $ARGUMENTS de OpenCode para recibir el archivo que se debe procesar. El objetivo es automatizar la limpieza, anonimización y clasificación de los mensajes, generando el archivo datos_tickets.json.

![Figura 4. Configuración del comando personalizado limpiar-y-clasificar.md con las instrucciones y técnicas de Prompt Engineering para PcShield Store - JRM.](./img/img_05.png)

*Figura 4. Configuración del comando personalizado limpiar-y-clasificar.md con las instrucciones y técnicas de Prompt Engineering para PcShield Store - JRM.*

Se inició OpenCode desde la terminal integrada de Visual Studio Code, situándose en la carpeta ut2-prompt-engineering/01-taller-helpdesk/ del repositorio daw2-fiag. La herramienta se abrió correctamente y mostró su interfaz inicial, confirmando que está disponible para trabajar sobre el proyecto PcShield Store - JRM. Esta herramienta se utilizará para ejecutar el comando personalizado de limpieza y clasificación de mensajes definido previamente.

![Figura 5. Inicio de OpenCode desde la carpeta del proyecto PcShield Store - JRM en Visual Studio Code.](./img/img_06.png)

*Figura 5. Inicio de OpenCode desde la carpeta del proyecto PcShield Store - JRM en Visual Studio Code.*

Se accedió al menú de conexión de proveedores de OpenCode mediante el comando /connect. La herramienta mostró diferentes proveedores de modelos de inteligencia artificial, entre ellos OpenCode, OpenAI, GitHub Copilot, Anthropic y Google. Se seleccionó como opción inicial OpenCode (Recommended), con el objetivo de configurar el proveedor integrado y disponer de un modelo de IA para ejecutar los comandos personalizados del proyecto.

![Figura 6. Menú de selección de proveedores de inteligencia artificial disponibles en OpenCode.](./img/img_07.png)

*Figura 6. Menú de selección de proveedores de inteligencia artificial disponibles en OpenCode.*

Tras seleccionar el proveedor OpenCode (Recommended), se regresó a la pantalla principal de la herramienta. En la interfaz aparece seleccionado el modelo Big Pickle OpenCode en el modo Build, que se utilizará para procesar las instrucciones del proyecto PcShield Store - JRM y ejecutar el comando personalizado de Prompt Engineering.

![Figura 7. Pantalla principal de OpenCode con el modelo Big Pickle OpenCode seleccionado.](./img/img_08.png)

*Figura 7. Pantalla principal de OpenCode con el modelo Big Pickle OpenCode seleccionado.*

Se ejecutó el comando personalizado /limpiar-y-clasificar @bandeja_entrada_sucia.txt desde OpenCode utilizando el modelo Big Pickle OpenCode. El agente procesó los ocho mensajes del archivo de entrada y generó automáticamente datos_tickets.json en la carpeta principal del proyecto. Durante el procesamiento, se identificó y bloqueó un mensaje que contenía un intento de Prompt Injection y se rechazó otro por estar fuera del ámbito de las incidencias informáticas. Asimismo, se sustituyeron los datos personales detectados por los marcadores de anonimización definidos en las instrucciones. Finalmente, OpenCode ejecutó una comprobación mediante python3 -m json.tool, que confirmó que el archivo generado tenía una estructura JSON válida.

![Figura 8. Ejecución del comando limpiar-y-clasificar y generación de datos_tickets.json con ocho mensajes procesados y formato JSON validado.](./img/img_09.png)

*Figura 8. Ejecución del comando limpiar-y-clasificar y generación de datos_tickets.json con ocho mensajes procesados y formato JSON validado.*

### 5.3. Modificación del alumno 1

Se actualizó el comando personalizado limpiar-y-clasificar.md para ampliar sus capacidades de anonimización y clasificación. Se incorporó la detección de matrículas de vehículos e IBAN, utilizando los marcadores [MATRICULA_OCULTA] e [IBAN_OCULTO]. Además, se añadió el campo obligatorio tiempo_estimado_minutos a la estructura de salida JSON, con una estimación entera para las incidencias válidas y valor cero para los mensajes rechazados o bloqueados. También se reforzaron las instrucciones de clasificación para evitar asignar categorías informáticas a mensajes ajenos al ámbito del proyecto.

![Figura 9. Modificación del comando limpiar-y-clasificar.md para incorporar la anonimización de matrículas e IBAN y el cálculo del tiempo estimado de resolución.](./img/img_10.png)

*Figura 9. Modificación del comando limpiar-y-clasificar.md para incorporar la anonimización de matrículas e IBAN y el cálculo del tiempo estimado de resolución.*

## 6. Fase 3. Equipamos OpenCode con Skills

### 6.1. Paso 3.1. Instalación de una Skill oficial de diseño web

Se instaló la Skill oficial web-design-guidelines, procedente del repositorio vercel-labs/agent-skills, utilizando la herramienta npx skills. Para ello, se ejecutó el comando npx skills add vercel-labs/agent-skills --skill web-design-guidelines -a opencode -y desde la carpeta principal del proyecto. El instalador localizó las habilidades disponibles en el repositorio, seleccionó la solicitada y completó su instalación para OpenCode. La Skill quedó almacenada en la ruta .agents/skills/web-design-guidelines/ del proyecto. El resultado confirmó que se había instalado una habilidad y que la evaluación de seguridad no había detectado alertas.

![Figura 10. Instalación de la Skill oficial web-design-guidelines para OpenCode mediante npx skills.](./img/img_11.png)

*Figura 10. Instalación de la Skill oficial web-design-guidelines para OpenCode mediante npx skills.*

Una vez completada la instalación, se ejecutó el comando npx skills list para verificar las habilidades disponibles en el proyecto. El resultado mostró web-design-guidelines dentro del apartado Project Skills, junto con su ruta de instalación en .agents/skills/web-design-guidelines/. También se comprobó que OpenCode figura entre los agentes compatibles y que el origen de la habilidad corresponde al repositorio vercel-labs/agent-skills. De esta manera, se verificó que la instalación se había realizado correctamente.

![Figura 11. Verificación de la Skill web-design-guidelines mediante el comando npx skills list.](./img/img_12.png)

*Figura 11. Verificación de la Skill web-design-guidelines mediante el comando npx skills list.*

### 6.2. Paso 3.2. Creación de la Skill personalizada de calidad y escudo RGPD

Se inicializó una nueva Skill personalizada mediante el comando npx skills init escudo-rgpd-js, ejecutado desde la carpeta principal del proyecto. La herramienta generó correctamente el directorio escudo-rgpd-js y creó en su interior el archivo SKILL.md, que servirá como documento principal para definir las instrucciones de la habilidad. El instalador indicó que los siguientes pasos consisten en editar dicho archivo y completar el nombre y la descripción en su cabecera. Esta Skill se utilizará para establecer criterios propios de calidad del código JavaScript y protección de datos en la aplicación PcShield Store - JRM.

![Figura 12. Inicialización de la Skill personalizada escudo-rgpd-js y creación del archivo SKILL.md.](./img/img_13.png)

*Figura 12. Inicialización de la Skill personalizada escudo-rgpd-js y creación del archivo SKILL.md.*

### 6.3. Modificación del alumno 2

Como modificación individual del alumno 2, se amplió la Skill personalizada escudo-rgpd-js incorporando una cuarta regla de protección de datos. Esta modificación establece que la función JavaScript sanitizarTextoPII(texto) también debe detectar las direcciones IPv4 presentes en el texto introducido por el usuario y sustituirlas automáticamente por el marcador [IP_OCULTA]. De esta manera, la habilidad amplía sus criterios de anonimización para incluir direcciones IP, además de los DNI/NIE y los números de tarjetas bancarias contemplados inicialmente. Finalmente, se guardaron los cambios en el archivo SKILL.md.

![Figura 13. Incorporación de la cuarta regla de anonimización de direcciones IPv4 en la Skill personalizada escudo-rgpd-js.](./img/img_14.png)

*Figura 13. Incorporación de la cuarta regla de anonimización de direcciones IPv4 en la Skill personalizada escudo-rgpd-js.*

![Imagen de página 17](./img/img_15.png)

## 7. Fase 4. Construcción de la aplicación web con OpenSpec y Prompt Chaining

### 7.1. Paso 4.1. Inicialización de OpenSpec

Se inicializó el framework OpenSpec en el proyecto PcShield Store - JRM mediante el comando npx @fission-ai/openspec@latest init. Durante el asistente de configuración se seleccionó OpenCode como herramienta de desarrollo, siguiendo las indicaciones del guion. El proceso finalizó correctamente y generó la estructura necesaria para trabajar con especificaciones. También se creó el archivo de configuración openspec/config.yaml, utilizando el esquema spec-driven, y se incorporaron seis Skills en el directorio .agents/skills/. La salida de la terminal confirmó que la configuración de OpenSpec para OpenCode se había completado satisfactoriamente.

![Figura 14. Inicialización y configuración de OpenSpec para trabajar con OpenCode en el proyecto PcShield Store - JRM.](./img/img_16.png)

*Figura 14. Inicialización y configuración de OpenSpec para trabajar con OpenCode en el proyecto PcShield Store - JRM.*

### 7.2. Paso 4.2. Documentos proposal, spec y tasks

Se redactó el documento proposal.md dentro de openspec/changes/mvp-dashboard/ para definir la propuesta inicial de la aplicación PcShield Store - JRM mediante OpenSpec. El documento se organizó en dos apartados. En el primero, «Por qué (Objetivo)», se describió la necesidad de disponer de un panel web para que el equipo de soporte técnico consulte incidencias y pedidos, filtre tickets, modifique sus estados y registre nuevas incidencias con protección de datos personales. En el segundo, «Qué se construye (Alcance)», se estableció el desarrollo de una aplicación SPA utilizando HTML5, TailwindCSS y JavaScript Vanilla, con los archivos index.html y app.js, y persistencia de datos mediante localStorage.

![Figura 15. Documento proposal.md con la propuesta y el alcance de la aplicación PcShield Store - JRM.](./img/img_17.png)

*Figura 15. Documento proposal.md con la propuesta y el alcance de la aplicación PcShield Store - JRM.*

Se elaboró el documento spec.md dentro de openspec/changes/mvp-dashboard/specs/interfaz-web/ para definir los requisitos funcionales de la aplicación PcShield Store - JRM. La especificación se estructuró mediante tres requisitos principales: un panel superior de estadísticas (KPIs), un listado de tickets con filtros y buscador, y un formulario con protección RGPD en tiempo real. Para cada requisito se definieron escenarios utilizando la estructura WHEN/THEN, describiendo las condiciones que deben producirse y el comportamiento esperado de la aplicación. Además, se completó el escenario de creación de tickets con datos sensibles, incorporando la anonimización de DNI, números de tarjetas bancarias y direcciones IPv4 mediante sus correspondientes marcadores.

También se especificó el bloqueo del envío del formulario ante intentos de Prompt Injection.

![Figura 16. Documento spec.md con los requisitos funcionales y escenarios de la aplicación PcShield Store - JRM.](./img/img_18.png)

*Figura 16. Documento spec.md con los requisitos funcionales y escenarios de la aplicación PcShield Store - JRM.*

Se creó el documento tasks.md dentro de openspec/changes/mvp-dashboard/ para establecer el plan de construcción de la aplicación PcShield Store - JRM mediante la técnica Prompt Chaining. El documento divide el desarrollo en tres eslabones secuenciales. El primero contempla la creación de index.html con TailwindCSS, incluyendo la cabecera, las cuatro tarjetas KPI, los filtros, el listado de tickets y el formulario con vista previa RGPD. El segundo establece la creación de app.js, encargado de cargar los datos iniciales de datos_tickets.json, gestionar su persistencia en localStorage, representar las incidencias y aplicar los filtros y cambios de estado. El tercer eslabón define la integración de la Skill personalizada escudo-rgpd-js, incorporando la anonimización de DNI/NIE, tarjetas bancarias y direcciones IPv4, la vista previa protegida en tiempo real y el bloqueo de intentos de Prompt Injection. Cada tarea se representó mediante una casilla de verificación para controlar su ejecución.

![Figura 17. Documento tasks.md con el plan de construcción de PcShield Store - JRM dividido en tres eslabones mediante Prompt Chaining.](./img/img_19.png)

*Figura 17. Documento tasks.md con el plan de construcción de PcShield Store - JRM dividido en tres eslabones mediante Prompt Chaining.*

Una vez creados los tres documentos de OpenSpec, se ejecutó el comando npx @fission-ai/openspec@latest validate para comprobar la validez de la especificación del proyecto PcShield Store - JRM. Durante el proceso se seleccionó la opción «All (changes + specs)», que permite validar conjuntamente los cambios y las especificaciones. OpenSpec reconoció correctamente el cambio mvp-dashboard y finalizó la comprobación con un resultado de un elemento validado, cero errores y tres advertencias. Estas advertencias recomendaban utilizar los términos normativos SHALL o MUST en los requisitos de spec.md.

Aunque no impidieron superar la validación, se decidió conservar la redacción actual y continuar con el desarrollo.

![Figura 18. Validación de la especificación mvp-dashboard mediante OpenSpec, con cero errores y tres advertencias.](./img/img_20.png)

*Figura 18. Validación de la especificación mvp-dashboard mediante OpenSpec, con cero errores y tres advertencias.*

Después de validar la especificación, se ejecutó el comando npx @fission-ai/openspec@latest view para visualizar el estado del proyecto mediante el panel de OpenSpec. La herramienta reconoció el cambio activo mvp-dashboard y mostró que utiliza el esquema de trabajo spec-driven. También presentó el estado de los documentos y el progreso de las tareas, indicando que había un cambio en curso, ninguno completado y cero de las tres tareas ejecutadas (0 %). Esta comprobación permitió verificar que OpenSpec reconoce el plan de trabajo y que la implementación todavía está pendiente de comenzar.

![Figura 19. Panel de OpenSpec con el estado del cambio mvp-dashboard y el progreso inicial de las tareas.](./img/img_21.png)

*Figura 19. Panel de OpenSpec con el estado del cambio mvp-dashboard y el progreso inicial de las tareas.*

### 7.3. Paso 4.3. Ejecución del Prompt Chaining

Se ejecutó el primer eslabón de la técnica Prompt Chaining mediante OpenCode, siguiendo las instrucciones definidas en openspec/changes/mvp-dashboard/tasks.md. Para ello, se proporcionó al agente el contexto técnico de AGENTS.md, la especificación funcional spec.md y la Skill oficial web-design-guidelines. OpenCode generó el archivo index.html de PcShield Store - JRM, incorporando la cabecera, las cuatro tarjetas KPI, la barra de filtros y búsqueda, el contenedor de incidencias y el formulario de creación de tickets con vista previa RGPD y alerta de Prompt Injection. La interfaz se desarrolló utilizando HTML5 semántico y TailwindCSS mediante CDN, incluyendo características de accesibilidad y adaptación a los modos claro y oscuro. Finalmente, OpenCode marcó como completada la primera tarea en tasks.md, sin implementar todavía la lógica JavaScript ni las funciones de anonimización, reservadas para los siguientes eslabones.

![Figura 20. Ejecución del primer eslabón de Prompt Chaining y finalización de la estructura HTML de PcShield Store - JRM mediante OpenCode.](./img/img_22.png)

*Figura 20. Ejecución del primer eslabón de Prompt Chaining y finalización de la estructura HTML de PcShield Store - JRM mediante OpenCode.*

Se ejecutó el segundo eslabón de la técnica Prompt Chaining mediante OpenCode para desarrollar el motor de datos y las funcionalidades interactivas de PcShield Store - JRM. El agente creó el archivo app.js, tomando como referencia la estructura de index.html y los datos de datos_tickets.json. La implementación incorpora la carga inicial de incidencias, un conjunto de datos de respaldo para permitir la apertura directa mediante el protocolo file://, la persistencia en localStorage y la representación dinámica de las tarjetas de tickets. También se implementaron los filtros por categoría, la búsqueda en tiempo real, la posibilidad de marcar incidencias como resueltas y la actualización de las cuatro tarjetas KPI.

Además, se modificó index.html para incorporar el archivo JavaScript mediante el atributo defer. OpenCode informó de la comprobación sintáctica con node --check y de pruebas del DOM con jsdom. Finalmente, marcó el segundo eslabón como completado en tasks.md, dejando para el siguiente paso las funciones de anonimización y protección frente a Prompt Injection.

![Figura 21. Ejecución del segundo eslabón de Prompt Chaining y desarrollo del motor de datos y filtros JavaScript de PcShield Store - JRM.](./img/img_23.png)

*Figura 21. Ejecución del segundo eslabón de Prompt Chaining y desarrollo del motor de datos y filtros JavaScript de PcShield Store - JRM.*

Se ejecutó el tercer y último eslabón de la técnica Prompt Chaining mediante OpenCode, integrando en app.js las instrucciones de la Skill personalizada escudo-rgpd-js. Se implementó la función sanitizarTextoPII(), encargada de detectar y anonimizar DNI/NIE, números de tarjetas bancarias de 16 dígitos y direcciones IPv4, sustituyéndolos por sus correspondientes marcadores de protección. También se incorporó una vista previa RGPD en tiempo real, actualizada mediante el evento input, y un detector de Prompt Injection que muestra una alerta visual roja e impide el envío del formulario cuando identifica frases sospechosas. Además, se modificó index.html para gestionar la visualización de la alerta y asociarla al campo de descripción. Se mantuvo la compatibilidad con las funcionalidades desarrolladas en los eslabones anteriores y se estableció que los datos introducidos se almacenen previamente anonimizados en localStorage. OpenCode informó de la realización de comprobaciones sintácticas con node --check y pruebas del DOM con jsdom.

Finalmente, marcó el tercer eslabón como completado en tasks.md.

![Figura 22. Ejecución del tercer eslabón de Prompt Chaining e integración de la Skill personalizada Escudo RGPD en PcShield Store - JRM.](./img/img_24.png)

*Figura 22. Ejecución del tercer eslabón de Prompt Chaining e integración de la Skill personalizada Escudo RGPD en PcShield Store - JRM.*

Una vez completados los tres eslabones del Prompt Chaining, se abrió el archivo index.html mediante Live Server para comprobar visualmente la aplicación PcShield Store - JRM en el navegador. La interfaz se cargó correctamente y mostró la cabecera con la identificación del proyecto, las cuatro tarjetas de indicadores KPI, el buscador, los filtros por categoría y la bandeja de incidencias con diez tickets. También se comprobó visualmente la presencia del formulario para registrar nuevas incidencias y del indicador que informa de que el Escudo RGPD está activo. Esta primera revisión permitió verificar que la estructura visual generada durante los tres eslabones se integra correctamente y que los principales componentes de la aplicación aparecen en pantalla. Las pruebas funcionales específicas de filtros, resolución de tickets, anonimización y bloqueo de Prompt Injection quedan pendientes.

![Figura 23. Vista general de la aplicación web PcShield Store - JRM ejecutada en el navegador mediante Live Server.](./img/img_25.png)

*Figura 23. Vista general de la aplicación web PcShield Store - JRM ejecutada en el navegador mediante Live Server.*

Se realizó una prueba funcional del filtro por categoría de la aplicación PcShield Store - JRM. Para ello, se seleccionó una categoría distinta de «Todas» en el selector de filtros y se comprobó que el listado se actualizaba mostrando únicamente los tickets pertenecientes a la categoría seleccionada. El resultado confirmó que el filtrado funciona correctamente y permite localizar los tickets según su clasificación.

![Figura 24.1 Verificación del funcionamiento del filtro de tickets por categoría en PcShield Store - JRM.](./img/img_26.png)

*Figura 24.1 Verificación del funcionamiento del filtro de tickets por categoría en PcShield Store - JRM.*

![Figura 24.2 Verificación del funcionamiento del filtro de tickets por categoría en PcShield Store - JRM.](./img/img_27.png)

*Figura 24.2 Verificación del funcionamiento del filtro de tickets por categoría en PcShield Store - JRM.*

![Figura 24.3 Verificación del funcionamiento del filtro de tickets por categoría en PcShield Store - JRM.](./img/img_28.png)

*Figura 24.3 Verificación del funcionamiento del filtro de tickets por categoría en PcShield Store - JRM.*

![Figura 24.4 Verificación del funcionamiento del filtro de tickets por categoría en PcShield Store - JRM.](./img/img_29.png)

*Figura 24.4 Verificación del funcionamiento del filtro de tickets por categoría en PcShield Store - JRM.*

![Figura 24.5 Verificación del funcionamiento del filtro de tickets por categoría en PcShield Store - JRM.](./img/img_30.png)

*Figura 24.5 Verificación del funcionamiento del filtro de tickets por categoría en PcShield Store - JRM.*

![Figura 24.6 Verificación del funcionamiento del filtro de tickets por categoría en PcShield Store - JRM.](./img/img_31.png)

*Figura 24.6 Verificación del funcionamiento del filtro de tickets por categoría en PcShield Store - JRM.*

Se realizó una prueba funcional del buscador de tickets de la aplicación PcShield Store - JRM. Para comprobar su funcionamiento, se introdujo una palabra clave presente en el asunto o en el contenido de uno de los tickets. Se verificó que el listado se actualizaba mostrando únicamente los registros que coincidían con el término introducido. El resultado confirmó que el buscador permite localizar tickets mediante palabras clave y funciona correctamente.

![Figura 25. Verificación del funcionamiento del buscador de tickets mediante palabras clave en PcShield Store - JRM.](./img/img_32.png)

*Figura 25. Verificación del funcionamiento del buscador de tickets mediante palabras clave en PcShield Store - JRM.*

Se realizó una prueba funcional del sistema de resolución de tickets de PcShield Store - JRM. Para ello, se seleccionó un ticket que se encontraba pendiente y se pulsó el botón «RESUELTO» asociado a dicho registro. Se comprobó que el estado del ticket cambiaba correctamente y que los indicadores KPI se actualizaban para reflejar la nueva situación. El resultado confirmó el funcionamiento de la resolución de tickets y la actualización dinámica de los contadores.

![Figura 26. Verificación de la resolución de un ticket y de la actualización dinámica de los indicadores KPI.](./img/img_33.png)

*Figura 26. Verificación de la resolución de un ticket y de la actualización dinámica de los indicadores KPI.*

![Figura 26. Verificación de la resolución de un ticket y de la actualización dinámica de los indicadores KPI.](./img/img_34.png)

*Figura 26. Verificación de la resolución de un ticket y de la actualización dinámica de los indicadores KPI.*

Se realizó una prueba funcional del mecanismo de anonimización de datos personales del escudo RGPD de PcShield Store - JRM. Para ello, se introdujo un DNI ficticio (12345678Z) en el campo de descripción de la incidencia del formulario de creación de tickets. Se comprobó que la vista previa RGPD detectaba el patrón correspondiente al DNI y sustituía el dato por su etiqueta de anonimización. La prueba se realizó sin guardar ni crear un nuevo ticket, verificando así el funcionamiento de la protección de datos en tiempo real.

![Figura 27. Verificación de la detección y anonimización de un DNI ficticio mediante el escudo RGPD.](./img/img_35.png)

*Figura 27. Verificación de la detección y anonimización de un DNI ficticio mediante el escudo RGPD.*

Se realizó una prueba funcional para comprobar la detección y anonimización de números de tarjetas bancarias mediante el escudo RGPD de PcShield Store - JRM. Para ello, se introdujo el número de tarjeta de prueba 4111111111111111 en el campo de descripción del formulario. Se comprobó que la vista previa RGPD detectaba el patrón correspondiente y ocultaba el número mediante su etiqueta de anonimización. La prueba se llevó a cabo sin guardar ni crear un nuevo ticket.

![Figura 28. Verificación de la detección y anonimización de un número de tarjeta bancaria de prueba mediante el escudo RGPD.](./img/img_36.png)

*Figura 28. Verificación de la detección y anonimización de un número de tarjeta bancaria de prueba mediante el escudo RGPD.*

Se realizó una prueba funcional para comprobar la detección y anonimización de direcciones IPv4 mediante el escudo RGPD de PcShield Store - JRM. Para ello, se introdujo la dirección IP ficticia 192.168.1.100 en el campo de descripción del formulario de creación de tickets. Se comprobó que la vista previa RGPD identificaba el patrón correspondiente a una dirección IPv4 y sustituía el dato por su etiqueta de anonimización. La prueba se realizó sin guardar ni crear un nuevo ticket.

![Figura 29. Verificación de la detección y anonimización de una dirección IPv4 ficticia mediante el escudo RGPD.](./img/img_37.png)

*Figura 29. Verificación de la detección y anonimización de una dirección IPv4 ficticia mediante el escudo RGPD.*

Se realizó una prueba funcional del mecanismo de detección de Prompt Injection integrado en el escudo RGPD de PcShield Store - JRM. Para ello, se introdujo en el campo de descripción del formulario un texto con instrucciones maliciosas que intentaba modificar el comportamiento de la aplicación y acceder a información privada. Se comprobó que el sistema detectaba el contenido, mostraba una alerta visual roja y bloqueaba su procesamiento. La prueba se llevó a cabo sin guardar ni crear un nuevo ticket.

![Figura 30. Verificación de la detección y bloqueo de instrucciones maliciosas mediante el mecanismo de protección contra Prompt Injection.](./img/img_38.png)

*Figura 30. Verificación de la detección y bloqueo de instrucciones maliciosas mediante el mecanismo de protección contra Prompt Injection.*

## 8. Fase 5. Auditoría y mejora con Chain-of-Thought (CoT) y patrón Reflexión

### 8.1. Auditoría del funcionamiento y seguridad

Se creó el segundo comando personalizado de OpenCode, denominado reflexionar-calidad.md, dentro de la carpeta .opencode/commands/ del proyecto PcShield Store - JRM. Este comando está diseñado para auditar el código de la aplicación mediante el patrón Reflexión y la técnica Chain-of-Thought (CoT), estructurando el análisis en tres fases: evaluación del comportamiento de la aplicación ante distintos escenarios, autocrítica para identificar tres posibles puntos débiles y refactorización para aplicar las mejoras correspondientes en los archivos index.html y app.js.

![Figura 31. Creación del comando personalizado reflexionar-calidad.md para la auditoría y mejora del código mediante el patrón Reflexión y CoT.](./img/img_39.png)

*Figura 31. Creación del comando personalizado reflexionar-calidad.md para la auditoría y mejora del código mediante el patrón Reflexión y CoT.*

Se inició OpenCode desde el directorio del proyecto PcShield Store - JRM para ejecutar el comando personalizado reflexionar-calidad.md. Antes de comenzar la auditoría, se comprobó que OpenCode estaba configurado en modo Plan y utilizando el modelo Big Pickle. En la captura se muestra el contenido del comando, que establece un proceso de revisión dividido en tres fases: análisis del comportamiento de la aplicación mediante Chain-of-Thought (CoT), autocrítica para identificar tres puntos débiles y propuesta de refactorización para mejorar el código sin perder las funcionalidades existentes.

![Figura 32. Inicio de la auditoría de calidad del proyecto PcShield Store - JRM con OpenCode en modo Plan mediante el comando reflexionar-calidad.](./img/img_40.png)

*Figura 32. Inicio de la auditoría de calidad del proyecto PcShield Store - JRM con OpenCode en modo Plan mediante el comando reflexionar-calidad.*

Se ejecutó el comando personalizado /reflexionar-calidad en OpenCode, utilizando el modelo Big Pickle y el modo Plan, para realizar una auditoría del código de PcShield Store - JRM. Durante la primera fase del patrón Reflexión, la herramienta analizó el comportamiento de la aplicación ante tres situaciones: el filtrado de una categoría sin tickets, la introducción de etiquetas HTML potencialmente peligrosas mediante el formulario y la persistencia de los cambios después de recargar la página. El análisis examinó las funciones implicadas y sus correspondientes ubicaciones en app.js, identificando aspectos relacionados con la usabilidad, la seguridad frente a ataques XSS y la persistencia de los datos.

![Figura 33. Análisis del comportamiento de PcShield Store - JRM durante la primera fase de la auditoría con el patrón Reflexión y Chain-of-Thought (CoT).](./img/img_41.png)

*Figura 33. Análisis del comportamiento de PcShield Store - JRM durante la primera fase de la auditoría con el patrón Reflexión y Chain-of-Thought (CoT).*

### 8.2. Autocrítica, mejoras aplicadas y verificación posterior

Se completó la segunda fase del patrón Reflexión mediante la autocrítica del código de PcShield Store - JRM. OpenCode identificó tres puntos débiles relacionados con la usabilidad del filtrado, la seguridad frente a contenido HTML potencialmente peligroso y la gestión de los datos almacenados. Para cada problema se especificaron el archivo y la zona afectados, los riesgos o consecuencias y las mejoras propuestas. Entre las soluciones planteadas destacan incorporar una opción para quitar filtros, detectar y bloquear patrones HTML peligrosos, añadir la eliminación de tickets, volver a sanear los datos durante su carga y notificar los errores de persistencia.

![Figura 34. Tabla de autocrítica con los tres puntos débiles detectados y las mejoras propuestas durante la auditoría de PcShield Store - JRM.](./img/img_42.png)

*Figura 34. Tabla de autocrítica con los tres puntos débiles detectados y las mejoras propuestas durante la auditoría de PcShield Store - JRM.*

Una vez identificados los tres puntos débiles durante la auditoría, se cambió OpenCode del modo Plan al modo Build para ejecutar la tercera fase del patrón Reflexión. Se proporcionaron instrucciones para aplicar directamente las mejoras propuestas en los archivos index.html y app.js. La refactorización contempla la mejora del estado vacío y la eliminación de filtros, el refuerzo de la protección frente a contenido HTML y JavaScript potencialmente peligroso, y la incorporación de funcionalidades de eliminación de tickets, saneamiento de datos durante la carga y notificación de errores de persistencia. También se indicó que debían conservarse las funcionalidades existentes y comprobar la sintaxis y las pruebas disponibles.

![Figura 35. Ejecución de la fase de refactorización y mejora del código de PcShield Store - JRM mediante OpenCode en modo Build.](./img/img_43.png)

*Figura 35. Ejecución de la fase de refactorización y mejora del código de PcShield Store - JRM mediante OpenCode en modo Build.*

Se completó la tercera fase del patrón Reflexión mediante la refactorización de la aplicación PcShield Store - JRM con OpenCode en modo Build. Se implementaron las tres mejoras identificadas durante la autocrítica: optimización del estado vacío y los filtros, refuerzo de la protección frente a contenido HTML y JavaScript potencialmente peligroso, y mejora de la gestión de datos mediante la eliminación de tickets, el saneamiento durante la carga y la notificación de errores de persistencia. Posteriormente, se realizaron comprobaciones de sintaxis JavaScript, validación del HTML y revisión de diferencias. También se ejecutó una batería temporal de pruebas funcionales con Chrome Headless y CDP, obteniendo 44 comprobaciones superadas. Una primera ejecución detectó un problema en la prueba de resolución, que fue corregido antes de completar satisfactoriamente la segunda ejecución.

![Figura 36. Resultado de la refactorización de PcShield Store - JRM y verificación de las mejoras mediante 44 comprobaciones funcionales superadas.](./img/img_44.png)

*Figura 36. Resultado de la refactorización de PcShield Store - JRM y verificación de las mejoras mediante 44 comprobaciones funcionales superadas.*

Se realizó una prueba funcional de la mejora del estado vacío de PcShield Store - JRM. Para ello, se introdujo en el buscador un término que no coincidía con ningún ticket, comprobando que el listado mostraba cero resultados. La aplicación presentó un mensaje informativo indicando el criterio de búsqueda activo y mostró el botón «Quitar filtros» para facilitar la recuperación del listado. El resultado confirmó que la nueva gestión del estado vacío proporciona información contextual y una acción directa para restablecer los criterios de filtrado.

![Figura 37. Verificación del nuevo estado vacío y del botón «Quitar filtros» ante una búsqueda sin resultados.](./img/img_45.png)

*Figura 37. Verificación del nuevo estado vacío y del botón «Quitar filtros» ante una búsqueda sin resultados.*

Se comprobó el funcionamiento del botón «Quitar filtros» después de realizar una búsqueda sin resultados. Al pulsarlo, la aplicación eliminó el texto introducido en el buscador, restableció la categoría «Todas» y recuperó el listado completo de los diez tickets. También desapareció el mensaje de estado vacío. La prueba confirmó que los criterios de búsqueda y filtrado se restablecen correctamente sin necesidad de recargar la página.

![Figura 38. Restablecimiento de los filtros y recuperación del listado completo de tickets.](./img/img_46.png)

*Figura 38. Restablecimiento de los filtros y recuperación del listado completo de tickets.*

Se comprobó el mecanismo de protección frente a la introducción de código HTML y JavaScript potencialmente peligroso en el formulario de creación de tickets. Para realizar la prueba, se introdujo la expresión `<script>alert(1)</script>` en el campo de descripción de la incidencia. La aplicación detectó la etiqueta script y mostró el aviso «Envío bloqueado por seguridad», indicando que el contenido debía eliminarse antes de permitir la creación del ticket.

La vista previa protegida mostró el contenido como texto, sin ejecutar el código introducido. El resultado confirmó el funcionamiento del control de seguridad implementado.

![Figura 39. Detección y bloqueo de código JavaScript potencialmente peligroso en el formulario de creación de tickets.](./img/img_47.png)

*Figura 39. Detección y bloqueo de código JavaScript potencialmente peligroso en el formulario de creación de tickets.*

Se verificó la funcionalidad de eliminación de tickets incorporada durante la fase de refactorización. Tras aceptar el mensaje de confirmación para eliminar el ticket número 10, este desapareció de la bandeja y el contador se actualizó de diez a nueve tickets. Los demás registros permanecieron disponibles. El resultado confirmó que la eliminación se ejecuta correctamente y que la interfaz actualiza el número de tickets tras la operación.

![Figura 40. Verificación de la eliminación del ticket número 10 y actualización del contador de registros.](./img/img_48.png)

*Figura 40. Verificación de la eliminación del ticket número 10 y actualización del contador de registros.*

![Figura 40. Verificación de la eliminación del ticket número 10 y actualización del contador de registros.](./img/img_49.png)

*Figura 40. Verificación de la eliminación del ticket número 10 y actualización del contador de registros.*

Se realizó una prueba funcional de creación de tickets para comprobar que las modificaciones de seguridad no habían afectado al funcionamiento habitual del formulario. Se introdujo una incidencia de prueba con la descripción «El ordenador de recepción no arranca correctamente» y se completó el envío. La aplicación creó correctamente el ticket número 10, lo incorporó a la bandeja con prioridad media y estado pendiente, y actualizó el contador de nueve a diez registros. El resultado confirmó que la creación de nuevos tickets continúa funcionando correctamente tras la refactorización.

![Figura 41. Creación correcta de un nuevo ticket y actualización de la bandeja a diez registros.](./img/img_50.png)

*Figura 41. Creación correcta de un nuevo ticket y actualización de la bandeja a diez registros.*

Se comprobó el funcionamiento de la acción de resolución de tickets después de aplicar las mejoras de la fase de auditoría. Al pulsar «Marcar resuelto» en el ticket número 10, su estado cambió correctamente de «Pendiente» a «Resuelto», reflejándose visualmente mediante el indicador verde. Además, el botón de resolución quedó deshabilitado para impedir que la operación se ejecute nuevamente sobre un ticket ya resuelto. El contador permaneció en diez registros.

![Figura 42. Verificación del cambio de estado de un ticket a «Resuelto» tras aplicar la refactorización.](./img/img_51.png)

*Figura 42. Verificación del cambio de estado de un ticket a «Resuelto» tras aplicar la refactorización.*

Tras ejecutar el comando de auditoría /reflexionar-calidad en OpenCode, se aplicaron las mejoras identificadas durante el análisis y la autocrítica del código. Se optimizó el estado vacío de la bandeja, incorporando información contextual y la opción de restablecer los filtros. También se reforzó la seguridad mediante la detección y el bloqueo de etiquetas HTML y JavaScript potencialmente peligrosas, manteniendo el uso de textContent para representar los datos. En la gestión de información se incorporó la eliminación de tickets con confirmación, el re-saneamiento de los datos recuperados desde localStorage y avisos visibles y accesibles ante errores de persistencia. Finalmente, OpenCode ejecutó 44 comprobaciones funcionales, todas superadas, incluyendo pruebas de filtros, seguridad, creación, resolución, eliminación y persistencia de datos.

![Figura 43. Informe final de OpenCode con las mejoras de auditoría implementadas y las 44 comprobaciones funcionales superadas.](./img/img_52.png)

*Figura 43. Informe final de OpenCode con las mejoras de auditoría implementadas y las 44 comprobaciones funcionales superadas.*

## 9. Fase 6. Funcionalidad individual con OpenSpec y despliegue web

### 9.1. Paso 6.1. Especificación de la funcionalidad individual

Se creó el archivo proposal.md dentro de la carpeta openspec/changes/mi-mejora/ para definir la propuesta de la funcionalidad individual del proyecto PcShield Store - JRM. El documento establece como objetivo incorporar un «Laboratorio de Pruebas RGPD» que permita ejecutar pruebas controladas con datos personales ficticios y ataques de Prompt Injection.

También define la incorporación de botones para generar las pruebas, la visualización de sus resultados y un gráfico de barras desarrollado con HTML y CSS para representar las incidencias por categoría. Por último, se especifica el impacto técnico previsto en los archivos index.html y app.js, así como la necesidad de conservar las funcionalidades existentes.

![Figura 44. Archivo proposal.md con la propuesta de la funcionalidad individual «Laboratorio de Pruebas RGPD» mediante OpenSpec.](./img/img_53.png)

*Figura 44. Archivo proposal.md con la propuesta de la funcionalidad individual «Laboratorio de Pruebas RGPD» mediante OpenSpec.*

Se creó el archivo spec.md dentro de la carpeta openspec/changes/mi-mejora/specs/nueva-funcion/ para establecer los requisitos funcionales de la nueva sección «Laboratorio de Pruebas RGPD». El documento define los escenarios de acceso al laboratorio, ejecución de pruebas con DNIs, tarjetas bancarias e IPs ficticias, detección de ataques de Prompt Injection y visualización de resultados. También especifica la incorporación de un gráfico de barras para representar las incidencias por categoría y establece que la nueva funcionalidad debe mantener intactas las características existentes de PcShield Store - JRM.

![Figura 45. Archivo spec.md con los requisitos funcionales y escenarios de la nueva funcionalidad individual.](./img/img_54.png)

*Figura 45. Archivo spec.md con los requisitos funcionales y escenarios de la nueva funcionalidad individual.*

Se creó el archivo tasks.md dentro de la carpeta openspec/changes/mi-mejora/ para organizar el proceso de implementación de la funcionalidad individual mediante OpenSpec. El documento divide el trabajo en cuatro tareas: construcción de la interfaz del laboratorio, implementación del simulador de seguridad, creación del gráfico de incidencias e integración y comprobación de las funcionalidades existentes. Las tareas se registraron mediante casillas de verificación para facilitar el seguimiento del progreso durante el desarrollo.

![Figura 46. Archivo tasks.md con la planificación de las tareas para implementar el Laboratorio de Pruebas RGPD.](./img/img_55.png)

*Figura 46. Archivo tasks.md con la planificación de las tareas para implementar el Laboratorio de Pruebas RGPD.*

Se ejecutó el comando npx @fission-ai/openspec@latest validate mi-mejora desde la carpeta raíz del proyecto para validar los documentos de la nueva funcionalidad individual. OpenSpec confirmó que el cambio «mi-mejora» es válido y no detectó errores de validación. El resultado mostró seis advertencias relacionadas con la recomendación de utilizar los términos SHALL o MUST en los requisitos, conforme a las buenas prácticas RFC 2119 para especificaciones en inglés. Estas advertencias no impidieron la validación correcta del cambio.

![Figura 47. Validación correcta del cambio mi-mejora mediante OpenSpec, con seis advertencias informativas.](./img/img_56.png)

*Figura 47. Validación correcta del cambio mi-mejora mediante OpenSpec, con seis advertencias informativas.*

Se inició la implementación de la funcionalidad individual «Laboratorio de Pruebas RGPD» mediante OpenCode, utilizando el modo Build y el modelo Big Pickle. Para ello, se proporcionaron al asistente los documentos de OpenSpec (proposal.md, spec.md y tasks.md), junto con el archivo AGENTS.md, para que desarrollara la nueva funcionalidad siguiendo los requisitos y las tareas definidos. El prompt establece la incorporación de una sección de pruebas de seguridad, la reutilización de los mecanismos existentes de protección RGPD, la creación de un gráfico de barras por categorías y la conservación de las funcionalidades actuales. También se solicitaron comprobaciones técnicas y funcionales, sin realizar ningún commit ni push.

![Figura 48. Ejecución del prompt de implementación del Laboratorio de Pruebas RGPD en OpenCode mediante el modo Build.](./img/img_57.png)

*Figura 48. Ejecución del prompt de implementación del Laboratorio de Pruebas RGPD en OpenCode mediante el modo Build.*

OpenCode finalizó la implementación de la funcionalidad individual «Laboratorio de Pruebas RGPD» siguiendo los requisitos definidos en los documentos de OpenSpec. Se modificaron los archivos index.html y app.js para incorporar una nueva sección con pruebas de detección y anonimización de DNIs, tarjetas bancarias e IPv4 ficticias, así como una prueba de detección de ataques de Prompt Injection. También se incorporó una representación visual de los resultados y un gráfico dinámico de barras con las incidencias agrupadas por categoría. Las cuatro tareas de implementación quedaron marcadas como completadas en tasks.md. Las comprobaciones técnicas finalizaron correctamente y se superaron 33 pruebas funcionales con DOM simulado. No se realizó ningún commit ni push. Quedó pendiente la comprobación visual de la aplicación en un navegador real.

![Figura 49. Informe final de OpenCode con la implementación del Laboratorio de Pruebas RGPD y las 33 comprobaciones funcionales superadas.](./img/img_58.png)

*Figura 49. Informe final de OpenCode con la implementación del Laboratorio de Pruebas RGPD y las 33 comprobaciones funcionales superadas.*

Se realizó la primera comprobación visual de la nueva sección «Laboratorio de Pruebas RGPD» mediante el navegador y Live Server. La interfaz muestra los cuatro botones destinados a ejecutar pruebas de seguridad con datos ficticios: DNI, tarjeta bancaria, dirección IPv4 y Prompt Injection. También incorpora el botón «Ejecutar todas las pruebas» y un área para presentar los resultados del procesamiento. En la parte derecha se visualiza un gráfico de barras desarrollado con HTML y CSS que representa la distribución de los tickets registrados por categoría. La nueva sección conserva la identidad visual de PcShield Store - JRM y se integra en el diseño de la aplicación.

![Figura 50. Visualización del Laboratorio de Pruebas RGPD integrado en el panel PcShield Store - JRM.](./img/img_59.png)

*Figura 50. Visualización del Laboratorio de Pruebas RGPD integrado en el panel PcShield Store - JRM.*

Se realizó la primera prueba individual del Laboratorio de Pruebas RGPD utilizando el botón «DNI ficticio». La aplicación procesó un texto de prueba que contenía el DNI ficticio 12345678Z mediante los mecanismos de detección y anonimización existentes. El Escudo RGPD identificó correctamente el documento de identidad y lo sustituyó por el marcador [DNI_OCULTO], conservando el resto del contenido del mensaje. El resultado confirmó el funcionamiento de la detección y protección de datos personales desde el nuevo laboratorio.

![Figura 51. Prueba de detección y anonimización de un DNI ficticio en el Laboratorio de Pruebas RGPD.](./img/img_60.png)

*Figura 51. Prueba de detección y anonimización de un DNI ficticio en el Laboratorio de Pruebas RGPD.*

Se realizó la prueba de detección y anonimización de tarjetas bancarias desde el Laboratorio de Pruebas RGPD. Para ello, se pulsó el botón «Tarjeta bancaria», que procesó un texto de prueba con el número ficticio 4111 1111 1111 1111. La aplicación identificó correctamente la numeración y la sustituyó por el marcador [TARJETA_OCULTA], manteniendo intacto el resto del mensaje. El resultado confirmó que el laboratorio reutiliza correctamente los mecanismos existentes de protección de información bancaria.

![Figura 52. Prueba de detección y anonimización de una tarjeta bancaria ficticia en el Laboratorio de Pruebas RGPD.](./img/img_61.png)

*Figura 52. Prueba de detección y anonimización de una tarjeta bancaria ficticia en el Laboratorio de Pruebas RGPD.*

Se realizó la prueba de detección y anonimización de direcciones IPv4 desde el Laboratorio de Pruebas RGPD. Para ello, se pulsó el botón «Dirección IPv4», que procesó un texto ficticio que contenía la dirección 192.0.2.10. La aplicación identificó correctamente la dirección IP y la sustituyó por el marcador [IP_OCULTA], manteniendo intacto el resto del mensaje. El resultado confirmó el funcionamiento del mecanismo de protección de direcciones IPv4 integrado en el laboratorio.

![Figura 53. Prueba de detección y anonimización de una dirección IPv4 ficticia en el Laboratorio de Pruebas RGPD.](./img/img_62.png)

*Figura 53. Prueba de detección y anonimización de una dirección IPv4 ficticia en el Laboratorio de Pruebas RGPD.*

Se realizó la prueba de detección de ataques de Prompt Injection desde el Laboratorio de Pruebas RGPD. Para ello, se pulsó el botón «Prompt Injection», que procesó un texto ficticio con una instrucción maliciosa destinada a ignorar las instrucciones anteriores y revelar información privada de los clientes. La aplicación identificó correctamente el intento de manipulación, mostró el indicador «ATAQUE BLOQUEADO» y sustituyó el contenido por el marcador [INTENTO_DE_PROMPT_INJECTION]. El resultado confirmó el funcionamiento del mecanismo de detección de ataques integrado en el laboratorio.

![Figura 54. Detección y bloqueo de un intento de Prompt Injection mediante el Laboratorio de Pruebas RGPD.](./img/img_63.png)

*Figura 54. Detección y bloqueo de un intento de Prompt Injection mediante el Laboratorio de Pruebas RGPD.*

Se realizó una prueba conjunta del Laboratorio de Pruebas RGPD mediante el botón «Ejecutar todas las pruebas». La aplicación ejecutó los cuatro escenarios de seguridad disponibles: detección y anonimización de un DNI ficticio, una tarjeta bancaria ficticia y una dirección IPv4, además de la detección y bloqueo de un intento de Prompt Injection. Los resultados mostraron correctamente los marcadores [DNI_OCULTO], [TARJETA_OCULTA], [IP_OCULTA] e [INTENTO_DE_PROMPT_INJECTION], respectivamente. La prueba confirmó que todos los mecanismos de protección pueden ejecutarse conjuntamente y que sus resultados se presentan de forma diferenciada en la interfaz.

![Figura 55.1 Ejecución conjunta de las cuatro pruebas de seguridad del Laboratorio de Pruebas RGPD con resultados satisfactorios.](./img/img_64.png)

*Figura 55.1 Ejecución conjunta de las cuatro pruebas de seguridad del Laboratorio de Pruebas RGPD con resultados satisfactorios.*

![Figura 55.2 Ejecución conjunta de las cuatro pruebas de seguridad del Laboratorio de Pruebas RGPD con resultados satisfactorios.](./img/img_65.png)

*Figura 55.2 Ejecución conjunta de las cuatro pruebas de seguridad del Laboratorio de Pruebas RGPD con resultados satisfactorios.*

Se comprobó la representación gráfica de las incidencias por categoría incorporada al Laboratorio de Pruebas RGPD. El gráfico de barras, desarrollado mediante HTML y CSS, muestra la distribución de los diez tickets registrados en la aplicación: dos incidencias de Redes, dos de Hardware, dos de Software, tres de Facturación y una de Seguridad. Cada categoría dispone de una barra visual diferenciada y un contador numérico. El resultado confirmó que la aplicación presenta correctamente la distribución de incidencias utilizando los datos registrados en la bandeja.

![Figura 56. Gráfico de barras con la distribución de las diez incidencias registradas por categoría.](./img/img_66.png)

*Figura 56. Gráfico de barras con la distribución de las diez incidencias registradas por categoría.*

Se inició la prueba de actualización dinámica del gráfico de incidencias eliminando un ticket de la categoría Redes. Al pulsar el botón «Eliminar» del ticket número 1, la aplicación mostró un cuadro de confirmación que identificaba el registro que se iba a eliminar y advertía de que la acción no se podía deshacer. Esta comprobación permitió verificar que la eliminación requiere una confirmación explícita del usuario.

![Figura 57. Cuadro de confirmación previo a la eliminación del ticket número 1 para comprobar la actualización del gráfico de incidencias.](./img/img_67.png)

*Figura 57. Cuadro de confirmación previo a la eliminación del ticket número 1 para comprobar la actualización del gráfico de incidencias.*

Tras confirmar la eliminación del ticket número 1, se comprobó la actualización automática del gráfico «Incidencias por categoría». El contador de Redes pasó de dos a una incidencia, mientras que las demás categorías conservaron sus cantidades. El resultado confirmó que el gráfico obtiene los datos actualizados de la bandeja y modifica su representación visual cuando se elimina un ticket.

![Imagen de página 59](./img/img_68.png)

![Figura 58. Actualización dinámica del gráfico de incidencias tras eliminar un ticket de la categoría Redes.](./img/img_69.png)

*Figura 58. Actualización dinámica del gráfico de incidencias tras eliminar un ticket de la categoría Redes.*

### 9.2. Paso 6.2. Subida a GitHub y publicación de la aplicación

Se ha realizado el despliegue de la aplicación PcShield Store - JRM mediante Netlify Drop. La plataforma ha procesado los archivos del proyecto y ha generado una dirección web para acceder a la aplicación. La vista previa confirma que el panel de soporte técnico se ha publicado correctamente.

![Figura 59.1 Publicación de PcShield Store - JRM mediante Netlify Drop.](./img/img_70.png)

*Figura 59.1 Publicación de PcShield Store - JRM mediante Netlify Drop.*

![Figura 59.2 Publicación de PcShield Store - JRM mediante Netlify Drop.](./img/img_71.png)

*Figura 59.2 Publicación de PcShield Store - JRM mediante Netlify Drop.*

Se ha verificado el acceso público a la aplicación desplegada en Netlify mediante una ventana de navegación privada. La aplicación PcShield Store - JRM carga correctamente sin necesidad de iniciar sesión, por lo que el enlace puede compartirse con terceros para su evaluación.

![Figura 60.1. Configuración de la visibilidad del proyecto PcShield Store - JRM en Netlify.](./img/img_72.png)

*Figura 60.1. Configuración de la visibilidad del proyecto PcShield Store - JRM en Netlify.*

*Figura 60.2. Verificación de que la visibilidad de producción y de las vistas previas está establecida como pública en Netlify.*

## 10. Pruebas finales y verificación de entregables

Una vez finalizado el desarrollo de PcShield Store - JRM, se han realizado diferentes pruebas para comprobar el funcionamiento de la aplicación, las medidas de protección RGPD, la detección de ataques y la persistencia de los datos. Las pruebas se han dividido entre comprobaciones técnicas, pruebas funcionales manuales y verificaciones del despliegue.

### 10.1. Comprobaciones técnicas

- Sintaxis de JavaScript: se ejecutó node --check app.js. Resultado esperado: ausencia de errores sintácticos. Resultado obtenido: comprobación correcta.
- Integridad de los cambios: se ejecutó git diff --check. Resultado esperado: ausencia de errores de formato en los cambios. Resultado obtenido: sin errores.
- Estructura HTML: se realizó una comprobación del análisis del documento HTML. Resultado esperado: ausencia de errores de análisis. Resultado obtenido: sin errores detectados.
- Pruebas automatizadas: OpenCode informó de 44 comprobaciones superadas durante la auditoría de calidad y de 33 pruebas funcionales superadas durante la implementación de la mejora individual. Evidencias: figuras 43 y 49.

### 10.2. Pruebas funcionales del dashboard

- Búsqueda sin resultados: se introdujo un criterio de búsqueda que no coincidía con ningún ticket. Resultado esperado: mostrar un estado vacío contextual. Resultado obtenido: comportamiento correcto. Evidencia: figura 37.
- Limpieza de filtros: se utilizó la opción para limpiar los filtros. Resultado esperado: recuperar la visualización de los tickets. Resultado obtenido: comportamiento correcto. Evidencia: figura 38.
- Bloqueo de código malicioso: se introdujo una etiqueta `<script>` para comprobar la protección frente a contenido HTML/JavaScript peligroso. Resultado esperado: impedir su ejecución. Resultado obtenido: el contenido peligroso fue neutralizado. Evidencia: figura 39.
- Eliminación de tickets: se eliminó un ticket y se recargó la página. Resultado esperado: mantener la eliminación después de la recarga. Resultado obtenido: eliminación persistente. Evidencia: figura 40.
- Creación de tickets: se creó una nueva incidencia y se recargó la página. Resultado esperado: conservar el nuevo ticket. Resultado obtenido: persistencia correcta. Evidencia: figura 41.
- Resolución de tickets: se marcó una incidencia como resuelta y se recargó la página. Resultado esperado: conservar el nuevo estado. Resultado obtenido: persistencia correcta. Evidencia: figura 42.

### 10.3. Pruebas del Laboratorio de Pruebas RGPD

- Detección de DNI: se introdujo el DNI ficticio 12345678Z. Resultado esperado: sustituirlo por [DNI_OCULTO]. Resultado obtenido: dato anonimizado correctamente. Evidencia: figura 51.
- Detección de tarjeta bancaria: se introdujo el número de tarjeta de prueba 4111 1111 1111 1111. Resultado esperado: sustituirlo por [TARJETA_OCULTA]. Resultado obtenido: dato ocultado correctamente. Evidencia: figura 52.
- Detección de dirección IPv4: se introdujo la dirección 192.0.2.10. Resultado esperado: sustituirla por [IP_OCULTA]. Resultado obtenido: dirección ocultada correctamente. Evidencia: figura 53.
- Detección de Prompt Injection: se introdujo un mensaje que intentaba que el sistema ignorase sus instrucciones anteriores. Resultado esperado: detectar y bloquear el intento. Resultado obtenido: ataque bloqueado y sustituido por [INTENTO_DE_PROMPT_INJECTION]. Evidencia: figura 54.
- Ejecución conjunta de pruebas: se ejecutaron los cuatro escenarios desde el botón de pruebas completas. Resultado esperado: obtener un resultado satisfactorio en cada escenario. Resultado obtenido: las cuatro pruebas finalizaron correctamente. Evidencia: figura 55.

### 10.4. Verificación del gráfico y del despliegue

- Representación gráfica inicial: se comprobó la visualización de las incidencias por categorías. Resultado esperado: mostrar las cantidades correspondientes a cada categoría. Resultado obtenido: gráfico generado correctamente. Evidencia: figura 56.
- Actualización del gráfico: se eliminó un ticket de la categoría Redes. Resultado esperado: reducir el contador de esa categoría. Resultado obtenido: el contador pasó de 2 a 1. Evidencias: figuras 57 y 58.
- Persistencia tras recargar: se recargó la aplicación después de las pruebas. Resultado esperado: mantener el funcionamiento del dashboard y del laboratorio. Resultado obtenido: funcionamiento correcto.
- Publicación en Netlify: se desplegó la aplicación y se configuró la visibilidad pública. Resultado esperado: permitir el acceso mediante una URL sin autenticación. Resultado obtenido: acceso público comprobado desde una ventana de incógnito. Evidencia: figura 60.

### 10.5. Verificación de entregables

- Proyecto alojado en el repositorio privado de GitHub daw2-fiag.
- Código fuente de PcShield Store - JRM incluido en la carpeta correspondiente al taller.
- Documentación OpenSpec de la funcionalidad individual incorporada al proyecto.
- Aplicación publicada en Netlify y accesible públicamente.
- Capturas de pantalla incorporadas a la memoria técnica.

Las pruebas descritas corresponden a comprobaciones realizadas durante el desarrollo, la auditoría y la publicación de la aplicación.

## 11. Incidencias y soluciones aplicadas

Durante el desarrollo y la publicación se identificaron algunas situaciones que requirieron ajustes.

### 11.1. Advertencias durante la validación de OpenSpec

- Incidencia: al validar el cambio mi-mejora mediante OpenSpec aparecieron seis advertencias.
- Causa identificada: las advertencias indicaban que las especificaciones en inglés suelen utilizar los términos SHALL o MUST para expresar requisitos obligatorios. Los requisitos del proyecto estaban redactados en español.
- Solución aplicada: se revisó el resultado de la validación y se comprobó que el cambio era válido, aunque mantenía las advertencias.
- Comprobación posterior: OpenSpec indicó que el cambio mi-mejora era válido y permitió continuar con la implementación.

### 11.2. Acceso restringido a la aplicación en Netlify

- Incidencia: después del primer despliegue, Netlify indicaba que el sitio solamente era visible para los miembros del equipo.
- Causa identificada: la visibilidad del proyecto estaba configurada como privada.
- Solución aplicada: se accedió a la configuración de visibilidad del proyecto y se seleccionó la opción Public.
- Comprobación posterior: Netlify mostró la visibilidad de producción y de las vistas previas como pública. Posteriormente se abrió la aplicación desde una ventana de incógnito y se comprobó que no solicitaba identificación.

## 12. Conclusiones

La realización de este taller ha permitido conocer y aplicar un flujo de desarrollo web dirigido mediante herramientas de inteligencia artificial generativa. Uno de los principales aprendizajes ha sido comprender que el desarrollo asistido por IA requiere planificación, contexto y especificaciones claras. El uso de AGENTS.md permitió establecer las instrucciones y características técnicas del proyecto, mientras que los comandos personalizados de OpenCode facilitaron la automatización de tareas de procesamiento y clasificación de información.

También se ha trabajado con Skills para incorporar instrucciones reutilizables, especialmente relacionadas con el diseño web y la protección de datos personales. La creación de la Skill propia escudo-rgpd-js permitió definir reglas de anonimización de información sensible y detección de intentos de Prompt Injection.

Mediante OpenSpec se aprendió a estructurar una funcionalidad a partir de una propuesta, una especificación y un plan de tareas. Posteriormente, el uso de Prompt Chaining permitió dividir la construcción de la aplicación en diferentes etapas, facilitando su implementación y revisión. La auditoría y las mejoras posteriores permitieron reforzar aspectos de seguridad, usabilidad y persistencia de datos. Además, la incorporación del Laboratorio de Pruebas RGPD supuso una ampliación individual del proyecto, con escenarios controlados para comprobar la anonimización de datos y el bloqueo de ataques.

Finalmente, la publicación mediante Netlify permitió desplegar la aplicación en Internet y comprobar su acceso público. Como resultado, se ha obtenido PcShield Store - JRM, una aplicación web funcional para la gestión de incidencias de una tienda de informática, con mecanismos de protección de datos, detección de ataques, filtros, estadísticas y un laboratorio de pruebas de seguridad.

## 13. Enlaces y referencias

### 13.1. Repositorio GitHub

Repositorio del proyecto:

https://github.com/2416082-debug/daw2-fiag/tree/main/ut2-prompt-engineering

El repositorio contiene el proyecto del taller, incluyendo los archivos de configuración, comandos personalizados, Skills, especificaciones OpenSpec y código fuente de la aplicación.

### 13.2. Aplicación desplegada

PcShield Store - JRM:

https://sparkly-dodol-373c21.netlify.app

Aplicación publicada mediante Netlify y configurada con visibilidad pública.

### 13.3. Documentación y herramientas consultadas

- Material del taller: Taller UT2: Construcción de una App Web con Ingeniería de Prompts, Skills y OpenSpec. Módulo de Fundamentos de Inteligencia Artificial Generativa, IES Alcántara, curso 2026/2027.
- OpenCode: herramienta utilizada para ejecutar comandos personalizados y dirigir la implementación asistida por IA.
- skills.sh: plataforma utilizada para consultar e instalar Skills reutilizables.
- OpenSpec: herramienta utilizada para definir y validar las especificaciones de las funcionalidades.
- Git y GitHub: herramientas utilizadas para el control de versiones y el alojamiento del código fuente.
- Netlify: plataforma utilizada para publicar la aplicación web.

## 14. Reto extra (opcional)

El reto extra propuesto en el taller contempla la posibilidad de ampliar la aplicación mediante una conexión con inteligencia artificial en vivo o una base de datos en la nube. En este proyecto no se ha realizado ninguna de esas dos ampliaciones. La aplicación se ha desarrollado utilizando JavaScript y almacenamiento local mediante localStorage, sin integrar un servicio externo de inteligencia artificial ni una base de datos remota.

Por tanto, este apartado queda sin implementar y no se presentan pruebas ni evidencias de funcionalidades correspondientes al reto extra.
