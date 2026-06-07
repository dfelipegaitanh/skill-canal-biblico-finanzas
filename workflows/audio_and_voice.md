# Producción — Voz y Música

**Propósito:** Este módulo rige la generación del prompt para clonación/generación de voz en Google AI Studio y el diseño sonoro del video.

## 1. Identidad del Narrador
*   **Tono:** Hombre, voz medio-grave. Tono de *Estratega de Trinchera* (Confrontacional-empático). **NO es un predicador, NO es un coach motivacional.**
*   **Velocidad:** **Fast-Pace estricto (110–115%).** Ágil, urgente. No hay tiempo para respirar, el espectador debe sentir que la revelación lo asfixia hasta la pausa quirúrgica.
*   **Pausas Quirúrgicas:** Usar comas o puntos. Prohibido usar etiquetas explícitas como `[pause]` para forzar pausas en el generador, usar puntuación natural.

## 2. Sistema de Generación de Voz (Google AI Studio)
La IA debe entregar su respuesta dentro de un bloque de código (`text`) con 3 campos (`SCENE`, `SAMPLE CONTEXT`, `TEXT`). 
*   **Para Shorts:** Se entrega todo en **un solo bloque continuo** (de corrido).
*   **Para Videos Largos:** Se debe entregar **bloque por bloque** (separado por cada Pilar), repitiendo la estructura de los 3 campos para cada bloque.

**Formato de Salida de Voz:**
```text
[BLOQUE / PILAR #] (Solo si es video largo)

SCENE
[Descripción en inglés del arco visual completo. Qué aparece en pantalla, qué hace el personaje. El arco visual siempre sigue al guion, no lo contradice.]

SAMPLE CONTEXT
[Descripción en inglés del viewer y del tono. Ej: "Urgent delivery, fast-paced pacing, no slow meditation". Describir las pausas críticas.]

TEXT
[Guion en español intercalado con etiquetas de emoción. Si es Short: texto completo de corrido. Si es Largo: solo el texto correspondiente a este bloque/pilar.]
```
*(Si es un video largo, repetir esta estructura SCENE/CONTEXT/TEXT para el siguiente bloque/pilar dentro del mismo código `text`)*

### Etiquetas de Emoción para el campo TEXT:
*   `[somber]` Momentos graves, peso emocional.
*   `[urgent]` Ritmo rápido, advertencia inminente.
*   `[warm]` Empatía, conexión.
*   `[intense]` Fuerza sin gritar, confrontación.
*   `[emphatic]` El golpe clave.
*   `[sharp]` Cortante, revelación cruda.
*   `[fast]` Avalancha de datos técnicos.

---

## 3. Diseño Sonoro y Música
La música justifica la inmersión estática de los planos Macro.
*   **Estilo base:** Acústico cálido (guitarra española o clásica). Piano o cuerdas de fondo opcionales.
*   **Prohibición Absoluta:** Cero voces, cero coros. Cero hip-hop, trap, electrónica o percusión pesada. La música NUNCA compite con la voz.
*   **Arco Dinámico (Dynamic Arc):** Inicia SIEMPRE con tensión incómoda los primeros 5 segundos (El Gancho/Dolor) y luego transiciona a algo armonioso/contemplativo.

### Formato de Salida de Música
Cuando el usuario pida música, entrega este prompt para herramientas de generación musical (ej. Suno/Udio/Suno):
```text
Acoustic instrumental music for a Spanish-language YouTube channel about biblical principles and personal finance.
Mood: starts tense and uncomfortable for the first 5 seconds, then strictly transitions into [uplifting/optimistic/bright] and remains highly energetic and harmonious.
Tempo: mid to fast (90-115 BPM).
Instruments: upbeat classical or Spanish acoustic guitar as the main instrument.
Exclusions: strictly no vocals or choirs, no hip-hop/trap beats, no electronic elements, no heavy percussion, absolutely no sad, melancholic, or somber melodies.
Texture: bright, dynamic, and inspiring — driving momentum and clarity.
```
