# Motor de Prompts Visuales

**Propósito:** Este módulo rige la traducción del guion aprobado a Prompts de imagen masivos (OpenAI Images 2).

## 1. Condición de Disparo (Bloqueo de Seguridad)
La IA tiene **PROHIBIDO** generar prompts de imágenes si el usuario no ha proporcionado el guion definitivo **con los timestamps exactos** (las marcas de tiempo) o si el usuario no lo pide explícitamente.
- Si el usuario pide generar imágenes pero no provee el texto con los timestamps, la IA debe responder: *"Alerta de Sistema: No puedo inventar tiempos. Por favor, provéeme el guion aprobado con sus respectivos timestamps para poder generar los prompts exactos."*

## 2. Traducción de Intenciones
Cuando la IA genera prompts, debe tomar las *Intenciones Visuales* del guion (las directivas de `[Visual: ...]` del Keyframe Scripting) y fusionarlas con las reglas estéticas correspondientes:
- Para **SHORTS**: usar `guidelines/visual_style_shorts.md` (Estilo Codex, Stick-figure, Tinta negra, Texturas, Color Semántico).
- Para **LONGS**: usar `guidelines/visual_style_longs.md` (Premium Biblical Editorial, Personajes Universales, Traducción Conceptual).

## 3. Deducción de Formato y Pacing (REGLA DE HIERRO)
Antes de generar las Tarjetas, la IA DEBE analizar el timestamp final del guion provisto para deducir el formato:
*   **Si el guion total dura menos de 60 segundos:** ES UN SHORT.
*   **Si el guion total dura más de 60 segundos:** ES UN LARGO.

> [!IMPORTANT]
> **⏱️ BLINDAJE DE RITMO VISUAL DE RETENCIÓN (INAMOVIBLE):**
> La IA tiene prohibido agrupar grandes bloques de texto en una sola imagen. La Tabla de Edición DEBE fragmentar el texto rigurosamente respetando esta matemática:
> - **Para SHORTS:** Cada prompt visual abarca **EXACTAMENTE de 4 a 5 segundos** del guion hablado.
> - **Para LONGS:** Cada prompt visual abarca **EXACTAMENTE de 6 a 9 segundos** del guion hablado.

## 4. Formato de Entrega Obligatorio
Entregar SIEMPRE la respuesta en dos partes, sin excepciones. Queda estrictamente PROHIBIDO usar tablas de Markdown, ya que comprimen el texto.

**PARTE 1: Las Tarjetas de Producción**
Presenta cada bloque de imagen como una tarjeta vertical. Los campos de Video y Texto se llenan basados en la *Matriz de Autoridad Visual* (90% estático, 10% datos en movimiento) y la *Tabla de Colores Semánticos* (Rojo, Dorado, Verde, Azul, Naranja).

**🎬 BLOQUE 1 [00:00 – 00:03]**
*   🗣️ **Audio/Guion:** `"(Texto literal del guion que cubre este bloque)"` [OBLIGATORIO]
*   🖼️ **OpenAI Images 2:** `(Prompt visual completo en inglés, siguiendo la guía de estilo correspondiente)` [OBLIGATORIO]
*   ✨ **Movimiento (CapCut):** `(Instrucción de Ken Burns o Zoom lento)` [OBLIGATORIO para el 90% de las imágenes estáticas]
*   📝 **Texto (Pulsar):** `("Frase breve", Color Semántico Ej: Rojo/Dorado/Verde)` [SOLO si la frase marca el ritmo]

**🎬 BLOQUE 2 [00:03 – 00:06]**
*   🗣️ **Audio/Guion:** `"(Texto literal del guion que cubre este bloque)"` [OBLIGATORIO]
*   🖼️ **OpenAI Images 2:** `(Prompt visual completo en inglés, siguiendo la guía de estilo correspondiente)` [OBLIGATORIO]
*   ✨ **Movimiento (CapCut):** `(Instrucción de Ken Burns o Zoom lento)` [OBLIGATORIO]
*   📝 **Texto (Pulsar):** `("Frase breve", Color Semántico)` [SOLO SI APLICA]

*(Repetir para todos los bloques requeridos...)*

**PARTE 2: El Bloque Raw para Batch (Copy-Paste)**
Justo debajo de las tarjetas, entrega un único bloque de código (`text`) que contenga ÚNICAMENTE los prompts de imagen, uno por línea. Sin viñetas, sin números, sin timestamps. Esto es para que el usuario pueda copiar todo el bloque y pegarlo en su herramienta de batch-generation.

```text
(Prompt completo de la imagen 1)
(Prompt completo de la imagen 2)
(Prompt completo de la imagen 3)
```
