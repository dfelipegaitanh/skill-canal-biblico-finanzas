# Código Bíblico del Dinero (Sistema Operativo V2)

Bienvenido a la versión 2 (V2) definitiva de la Skill operativa del canal **Código Bíblico del Dinero**. 

En esta versión, hemos transicionado de un enfoque monolítico a una **arquitectura de producción modular de alto rendimiento**. El sistema opera bajo estrictas reglas de autoridad visual, disonancia bíblica y fricción selectiva.

## Arquitectura Modular (El Motor)

La inteligencia de producción se divide en las siguientes áreas de responsabilidad:

### Orquestador Principal
*   `SKILL.md`: El cerebro de la operación. Contiene la filosofía del canal (El "Tono de la Trinchera") y las tablas de enrutamiento que dictan qué módulos cargar dependiendo de lo que pida el usuario.

### 1. Guías Base (`/guidelines`)
Reglas estéticas inquebrantables.
*   `guidelines/tone_and_voice.md`: Instrucciones sobre el tono, qué decir y qué evitar. Prohibida la motivación barata o el tono de predicador.
*   `guidelines/visual_style.md`: La **Matriz de Autoridad Visual**. Reglas del estilo "Codex", la paleta de colores semánticos (Rojo, Dorado, Verde, Azul, Naranja) y la estricta limitación de animación (Regla del 90/10).

### 2. Flujos de Trabajo y Producción (`/workflows`)
Cada etapa de producción tiene su propio manual técnico:
*   **Guiones:**
    *   `workflows/scripting_rules.md`: Reglas base inquebrantables (ej. un solo espectador, cero plurales).
    *   `workflows/script_long.md`: Arquitectura de **7 Pilares** para videos largos y puntuación de texto semántico ("Pulsar").
    *   `workflows/script_shorts.md`: Estructura estricta para formato Short, con CTA enfocado en "Shares" y restricción de animaciones a solo 2 segundos.
    *   `workflows/script_audit.md`: Criterios técnicos para auditar y elevar la retención de los guiones.
*   **Visuales y Audio:**
    *   `workflows/visuals_and_prompts.md`: Traducción de guiones aprobados a Tarjetas de Producción. Genera prompts para DALL-E, Textos Semánticos y parámetros de movimiento (CapCut/Video AI) de forma condicional.
    *   `workflows/audio_and_voice.md`: Estructura de 3 campos para Google AI Studio y diseño de prompts de música acústica con "Dynamic Arc".
*   **Empaque y Distribución:**
    *   `workflows/packaging.md`: Ingeniería de Títulos con **Disonancia Bíblica**, generación de propuestas de miniatura (El Enigma Técnico) y arquitectura SEO (Etiquetas de 3 niveles).
    *   `workflows/threads.md`: Distribución de alto impacto en texto mediante la estrategia de **Fricción Selectiva** de 3 Posts.

### 3. Interacción Básica (`/interaction`)
*   `interaction/onboarding.md`: Módulo de carga por defecto para recibir al usuario y auditar su petición inicial.

---

## Protocolo de Operación de la IA
**Regla de Oro:** La IA NUNCA carga todos los módulos al mismo tiempo. Opera leyendo `SKILL.md` y ruteando la petición exclusivamente a los manuales necesarios para no contaminar el contexto (ej. Si pides un guion, no carga las reglas de empaque).
