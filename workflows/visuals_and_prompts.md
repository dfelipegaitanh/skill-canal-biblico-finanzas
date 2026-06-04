# Motor de Prompts Visuales

**Propósito:** Este módulo rige la traducción del guion aprobado a Prompts de imagen masivos (DALL-E).

## 1. Condición de Disparo (Bloqueo de Seguridad)
La IA tiene **PROHIBIDO** generar prompts de imágenes si el usuario no ha proporcionado el guion definitivo **con los timestamps exactos** (las marcas de tiempo) o si el usuario no lo pide explícitamente.
- Si el usuario pide generar imágenes pero no provee el texto con los timestamps, la IA debe responder: *"Alerta de Sistema: No puedo inventar tiempos. Por favor, provéeme el guion aprobado con sus respectivos timestamps para poder generar los prompts exactos."*

## 2. Traducción de Intenciones
Cuando la IA genera prompts, debe tomar las *Intenciones Visuales* del guion (Macro Pilar, Micro Flujo, Punch Impacto) y fusionarlas con las reglas estéticas de `guidelines/visual_style.md` (Estilo Codex, Stick-figure, Tinta negra, Texturas, Elemento Magenta) para generar un prompt perfecto en inglés.

## 3. Formato de Entrega Obligatorio
Entregar SIEMPRE la respuesta en dos partes, sin excepciones. Queda estrictamente PROHIBIDO usar tablas de Markdown, ya que comprimen el texto. No incluyas recomendaciones de CapCut ni de animación, SOLO el prompt para DALL-E.

**PARTE 1: Las Tarjetas de Producción**
Presenta cada bloque de imagen como una tarjeta vertical y fácil de leer.

**🎬 BLOQUE [00:00 – 00:03]**
*   🖼️ **DALL-E:** `(Prompt visual completo en inglés, siguiendo el Estilo Codex)` [OBLIGATORIO]

**🎬 BLOQUE [00:03 – 00:06]**
*   🖼️ **DALL-E:** `(Prompt visual completo en inglés, siguiendo el Estilo Codex)` [OBLIGATORIO]

*(Repetir para todos los bloques requeridos...)*

**PARTE 2: El Bloque Raw para Batch (Copy-Paste)**
Justo debajo de las tarjetas, entrega un único bloque de código (`text`) que contenga ÚNICAMENTE los prompts de imagen, uno por línea. Sin viñetas, sin números, sin timestamps. Esto es para que el usuario pueda copiar todo el bloque y pegarlo en su herramienta de batch-generation.

```text
(Prompt completo de la imagen 1)
(Prompt completo de la imagen 2)
(Prompt completo de la imagen 3)
```
