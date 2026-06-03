# Skill: Código Bíblico del Dinero (V2)

Bienvenido a la versión 2 (V2) de la Skill del canal **Código Bíblico del Dinero**. 

NO DEFINITIVA Y SOLO PARA PRUEBAS**

En esta versión, hemos transicionado de un enfoque monolítico a una **arquitectura completamente modular**. Esto permite que el modelo cargue únicamente el contexto necesario según la tarea solicitada, optimizando el rendimiento, reduciendo el consumo de tokens y mejorando la precisión en las respuestas.

## Arquitectura Modular

La skill se divide en las siguientes áreas de responsabilidad:

### Orquestador Principal
- `SKILL.md`: Es el punto de entrada de la skill. Contiene la descripción de alto nivel y las reglas de enrutamiento (qué módulo cargar dependiendo de lo que pida el usuario).

### 1. Identidad (`/identity`)
Todo lo relacionado con la esencia del canal, quiénes somos y a quién le hablamos.
- `identity/brand.md`: Nombre, propuesta de valor y nicho.
- `identity/audience.md`: Perfil del cristiano latinoamericano (avatar), vocabulario clave y horarios.
- `identity/manifesto.md`: Manifiesto de la Mayordomía, tono confrontacional-empático y disonancia bíblica.

### 2. Guías de Estilo (`/guidelines`)
Reglas estéticas y de comunicación que rigen la creación de contenido.
- `guidelines/tone_and_voice.md`: Instrucciones sobre el tono, qué decir y qué evitar estrictamente (no somos predicadores, no somos coaches motivacionales).
- `guidelines/visual_style.md`: Detalles del estilo visual "Codex" (Manuscrito Da Vinci), paleta de colores y formato de los personajes (stick-figure).

### 3. Flujos de Trabajo y Producción (`/workflows`)
Módulos especializados por cada etapa del embudo de producción (reemplaza y expande la antigua carpeta `references`).
- `workflows/scripting_rules.md`: Reglas fundamentales obligatorias para cualquier tipo de guion.
- `workflows/script_long.md`: Estructura y reglas para guiones largos.
- `workflows/script_shorts.md`: Estructura y reglas para formato Short.
- `workflows/script_audit.md`: Criterios para revisar, auditar y mejorar guiones existentes.
- `workflows/packaging.md`: Creación de títulos, miniaturas (el "empaque") y metadatos SEO.
- `workflows/visuals_and_prompts.md`: Prompts de generación de imagen y directrices de animación visual.
- `workflows/audio_and_voice.md`: Guías para generación de voz, locución y música.
- `workflows/threads.md`: Creación de hilos (threads) para redes sociales.

### 4. Interacción Básica (`/interaction`)
- `interaction/onboarding.md`: Módulo de carga por defecto para cuando el usuario hace contacto inicial o no da suficiente contexto.

## ¿Cómo usar esta Skill?

Cuando se inicie una interacción:
1. Revisa el requerimiento del usuario.
2. Si el requerimiento es ambiguo o falta contexto, carga `interaction/onboarding.md`.
3. Si el requerimiento es específico, carga **solo** el archivo pertinente de la carpeta `/workflows/` junto con las guías de `/identity/` o `/guidelines/` que correspondan.

**Regla de Oro:** NUNCA cargues todos los módulos al mismo tiempo. Selecciona únicamente la combinación de módulos que resuelva la tarea en curso.
