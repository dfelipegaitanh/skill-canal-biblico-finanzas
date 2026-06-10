# Guia de estilo para Shorts
Guia definitiva para las imagenes de Shorts

## Estilo "Codex" (Manuscrito Da Vinci)

> [!IMPORTANT]
> **⏱️ RITMO VISUAL:** Ver la regla de pacing canónico en `workflows/visuals_and_prompts.md`.
**Paleta:**
| Uso | Hex |
|-----|-----|
| Fondo principal | `#E8D5B0` |
| Personajes | `#1A1A1A` |
| Acento cálido | `#C4956A` |

**4 elementos obligatorios en cada personaje:**

**1. Micro-expresiones y Ojos Expresivos** — `large round unfilled white head with thick black outlines, expressive cartoon eyes (white circles with black pupils) and thick bold black eyebrows showing [EMOCIÓN]`
- Emociones clave: preocupación/culpa (cejas al centro, boca abajo), sorpresa/revelación (cejas altas, ojos abiertos), autoridad/seriedad (cejas rectas, mirada firme).

**2. Silueta monigote con túnica** — `stick-figure character with thick black ink stroke arms and legs, torso wearing a simple flowing ancient tunic or shirt with stylized folds and volume`

**3. Personajes Bíblicos (Regla Excepcional):** Si el guión pide un personaje bíblico (Salomón, José, Jesús), se distinguen agregando *props* de poder o vestuario. Ej: `a stick-figure character representing King Solomon wearing a worn golden crown and royal ancient robes`. NUNCA dibujar caras humanas.

**4. Fondos texturizados y definidos** — `background features architectural details drawn in dark, slightly thinner hand-drawn sketchy outlines, with pencil-sketch textures, stone cracks, and wood grain`

---

**Reglas de Oro del Delineado e Iluminación (¡CRÍTICO para evitar líneas digitales delgadas!):**

> ⛔ **PROHIBICIÓN DURA DE LÍNEAS VECTORIALES Y RUIDO:** Prohibido usar "clean line art" aburrido, pero también **PROHIBIDO** el ruido de textura (fibras, granos de arena, lápiz rasposo).
> **Prompt Obligatorio de Delineado/Sombra:** `thick bold hand-drawn black ink outlines with clean crisp solid edges, smooth solid warm beige background (#E8D5B0) completely free of paper grain or noise, flat cel-shading and smooth digital color wash for rich volumetric depth`.

---

**Reglas de Oro para el Acento de Color (¡CRÍTICO para evitar exceso de color!):**

> ⛔ **REGLA DE MINIMALISMO DE COLOR:** Los colores semánticos son SOLO para objetos pequeños de impacto (monedas, pergaminos, cadenas). NUNCA colorear áreas grandes, fondos, luz ambiental, ropa o paredes (todo esto va en outline negro o beige cálido natural).

**Colores semánticos corregidos y sus límites:**

| Color | Hex | Significado Narrativo | Cuándo Usarlo (LÍMITES ESTRICTOS) |
|-------|-----|----------------------|-----------------------------------|
| **Rojo** | `#C0392B` | Deuda, peligro, trampa, error, prohibicion | Solo en símbolos pequeños: un candado, un contrato abusivo, unas cadenas de esclavo, una X roja. *Nunca en fondos ni ropa.* |
| **Verde** | `#27AE60` | Bendición, salida, camino correcto | Solo en símbolos pequeños: una línea de camino que guía, un checkmark (✓), un brote de planta, una flecha de salida. *Nunca en luz ambiental, puertas ni ventanas.* |
| **Dorado** | `#C9A84C` | Dinero, talentos, lo sagrado | Solo en objetos: monedas de oro, el rollo/scroll sagrado abierto, una balanza de justicia. *Nunca en paredes ni cielos.* |
| **Azul** | `#2980B9` | Lo divino, revelación espiritual | Solo en destellos espirituales sutiles (como una línea de luz celestial o un halo). *Nunca en ropa ni agua de fondo.* |
| **Naranja** | `#E67E22` | Urgencia activa, transformación, calor | Solo en fuentes de luz viva y real: la llama de una antorcha, una lámpara de aceite, rayos de sol sutiles rompiendo nubes. *Usar para toda la luz ambiental en lugar de verde/azul.* |

---

**Modos de Iluminación por Bloque Narrativo:**

*   **Modo Normal (Beige Cálido):** Para bloques de calma, enseñanza o aplicación LATAM. Fondo beige cálido sólido y limpio, luz cálida difusa. Sin grano ni textura de papel.
*   **Modo Tensión Iluminada (Encierro sin Oscuridad):** Para bloques de Gancho, Deuda o Crisis. Forzar a la IA a crear ambientes opresivos pero bien iluminados: `well-lit enclosed indoor space with no sky visible, completely eliminating deep dark shadows, bright and warm ambient lighting from multiple oil lamps`.

---

## Reglas de Interpretación Narrativa

**[SHORTS_VISUAL_DECISION_RULE]**
```text
SHORTS VISUAL DECISION RULE:
The generator should first determine the dominant emotional objective of the scene before selecting background, props, composition, and symbolic elements.
Visual decisions should be driven by narrative impact rather than template repetition.
Priority order:
1. Emotional objective
2. Narrative meaning
3. Character action
4. Symbolic object
5. Environment

The environment exists to reinforce the emotional state of the scene.
The same emotional objective should not always generate the same environment.
```

**[ENVIRONMENT_FLEXIBILITY_RULE]**
```text
ENVIRONMENT FLEXIBILITY RULE:
Backgrounds are selected according to emotional pressure, narrative meaning, and visual clarity rather than fixed scene categories.
Possible environments may include:
* enclosed interior spaces
* modest family homes
* simple biblical courtyards
* market areas
* workshops
* storage rooms
* pathways
* city gates
* agricultural settings
* symbolic minimalist environments

The generator may choose any environment that strengthens the narrative while remaining consistent with the Codex visual world.
Avoid repetitive use of stone walls, locked gates, enclosed rooms, or identical backgrounds across consecutive scenes.
Visual freshness is preferred whenever narrative clarity is preserved.
```

**[SYMBOLIC_FREEDOM_RULE]**
```text
SYMBOLIC FREEDOM RULE:
Symbolic objects are tools, not requirements.
When communicating a concept, the generator may prioritize:
* character emotion
* character posture
* character action
* visual contrast
* object symbolism
* environmental symbolism

The strongest storytelling choice should always be selected.
A scene about debt does not require a debt object.
A scene about temptation does not require a temptation object.
A scene about scarcity does not require a scarcity object.
If the emotion is already clearly communicated through the character and composition, additional symbolic objects may be reduced or omitted.
Avoid object-driven storytelling when character-driven storytelling is stronger.
```

---

**Estructura de 3 planos (Preferred):**
Three-plane compositions are preferred but may be simplified when a stronger visual impact can be achieved through a cleaner composition.
- **Foreground (Plano cercano):** Personaje principal + objeto central de la escena (monedas, Biblia, cadenas).
- **Midground (Plano medio):** Mobiliario, escalones, personas de soporte, puertas que dan contexto.
- **Background (Plano lejano):** Ambiente completo que ubica la escena — nunca vacío o beige liso.

**Biblioteca de Fondos (Backgrounds) recomendados por Contexto:**

| Contexto de Escena | Recommended Background Elements (OpenAI Images 2) |
|---------------------|-----------------------------------------------|
| **Interior Bíblico** | Stone walls with cracks, arched doorway with curtain, clay oil lamps, wooden shelves |
| **Exterior Bíblico** | Dusty hills winding dirt road, city gates on horizon, olive trees, overcast sky |
| **Interior Moderno LATAM** | Modest kitchen shelves, handwritten calendar on wall, small window showing neighborhood |
| **Escena de Deuda / Trampa** | Locked iron gates, unfinished walls, broken carts, chaotic market, dry well, enclosed stone rooms, narrowing paths |
| **Atmósfera Emocional** | Storm clouds (crisis), golden rays breaking through (hope), heavy dark sky (guilt) |

### 🅰️ Bloques Reutilizables para SHORTS (Estilo Codex Intenso)
Se usa para videos cortos. Trazos gruesos, 1 personaje, alto contraste.

**[CHARACTER_RULE_SHORTS]**
```text
Character rule: STRICTLY NO realistic human faces, no noses, no detailed ears or skin. Character MUST be a single 2D stick-figure with a perfectly round unfilled white head with thick black outlines, expressive cartoon eyes with pupils and thick bold black eyebrows showing [EMOCIÓN] (but not so volatile). Hands MUST be simple outlined cartoon gloves (no realistic knuckles or nails), wearing a simple ancient [flowing tunic / plain shirt] with stylized folds.
```

**[STYLE_RULE_SHORTS]**
```text
premium hand-drawn comic book aesthetic with clean precision. STRICTLY NO 3D rendering, no CGI, no watercolor, no anime.
smooth solid warm beige background (#E8D5B0) completely free of paper grain or noise,
thick bold hand-drawn black ink outlines with clean, crisp and solid edges,
flat cel-shading and smooth digital color wash for rich volumetric depth,
everything else in crisp black ink outlines on fully visible, well-lit environments,
strictly no high-frequency noise, no pencil sketch marks, no dust particles, optimized for video animation,
STRICT ELEMENT LIMIT: Maximum of 3 to 4 narrative objects in the entire image to avoid visual clutter.
STRICTLY NO MASSIVE TEXT HEADINGS EXCEPT THE DESIGNATED HOOK FRAME. Optional environmental text organically integrated into the scene (e.g., words on a scroll, carved in stone) is allowed in Spanish only.
```



---

**Prompt base general para SHORTS (Sustituir campos):**
```text
[DESCRIPCIÓN DE LA ESCENA EN PRIMER PLANO]. [CHARACTER_RULE_SHORTS],
— midground: [objeto secundario o figura de contexto],
— background: [ELEMENTO CONTEXTUAL], NO dark environment, completely eliminating deep dark shadows,
[STYLE_RULE_SHORTS],
color accent rule: [ELEMENTO PRINCIPAL DE IMPACTO] in [COLOR + HEX] — main accent,
[ELEMENTO DE CONTRASTE SECUNDARIO] in [COLOR + HEX] — secondary accent
```

---

## SISTEMA DE HOOK FRAME (Clasificación Emocional y Reglas)

**[HOOK_TARGET_RULE]**
```text
HOOK TARGET RULE:
The Hook Frame should visualize the financial wound, tension, fear, mistake, temptation, contradiction, or painful question introduced by the first sentence.
Do not visualize the scripture.
Do not visualize the solution.
Do not visualize the conclusion.
Visualize the problem.
The scripture, lesson, revelation, and financial framework are revealed after the hook.
The first frame exists to make the viewer emotionally identify with the problem within the first 3 seconds.
```

**[HOOK_TEXT_RULE]**
```text
HOOK TEXT RULE:
The Hook Frame is the only image allowed to contain embedded text.
The text should reinforce the central wound, contradiction, tension, or financial problem introduced by the first sentence.
Text should normally contain 1 to 3 words.
Examples: DEUDA, CRISIS, MENTIRA, ERROR, TE ROBAN, CAPITAL QUIETO, MALA INVERSIÓN, DINERO MUERTO, FALSA FE, TE ENGAÑARON, SIGUES PERDIENDO.
Avoid using the same text repeatedly across multiple Shorts.
The text should amplify the hook rather than simply repeat the narration.
```

**[HOOK_FRAME_CORE_PRINCIPLE]**
```text
HOOK FRAME CORE PRINCIPLE:
The Hook Frame exists to interrupt scrolling and visually communicate the central tension of the first sentence.
The Hook Frame should represent the dominant emotion of the hook, not automatically default to fear, panic, debt, crisis, or danger.
The visual tension should match the narrative tension.
```

**[HOOK_EMOTION_CLASSIFICATION]**
```text
HOOK EMOTION CLASSIFICATION:
Before generating the Hook Frame, classify the hook into one of the following emotional categories:

TYPE A — CRISIS
Used for: debt, scams, financial mistakes, poverty, inflation, financial pressure, financial collapse, greed, temptation.
Visual characteristics: strong visual tension, red semantic accents allowed, compressed compositions, enclosed environments preferred, concern, urgency, caution.

TYPE B — REVELATION
Used for: hidden biblical principles, misunderstood scriptures, financial wisdom, unexpected truths, paradigm shifts.
Visual characteristics: curiosity, surprise, discovery, contrast, symbolic revelation. Avoid unnecessary fear elements.

TYPE C — OPPORTUNITY
Used for: multiplication, stewardship, diligence, wealth building, growth, long-term vision, discipline.
Visual characteristics: anticipation, conviction, possibility, progress, forward movement. Avoid crisis symbolism.
```

**[HOOK_ENVIRONMENT_RULE]**
```text
HOOK ENVIRONMENT RULE:
The environment should support the emotional objective rather than follow a single mandatory template.
Examples:
Crisis: enclosed rooms, pressure spaces, narrowing corridors, locked gates.
Revelation: teaching spaces, courtyards, symbolic light, scroll tables.
Opportunity: pathways, gates opening, fields, workshops, storage spaces, growth-oriented environments.
Visual variety is preferred. Avoid generating the same "locked gate and stone wall" environment for every crisis. A crisis can also happen in an empty field, a ruined vineyard, a chaotic market, a broken cart on a pathway, or a drying well.
```

**[HOOK_COMPOSITION_RULE]**
```text
HOOK COMPOSITION RULE:
The Hook Frame must remain dynamic.
However: Dynamic does not automatically mean aggressive.
Allowed: strong eye contact, visual contrast, symbolic tension, unusual perspective, object emphasis, narrative conflict.
Not required: flying debris, shattered objects, panic expressions, extreme distress, constant visual destruction. Use only when justified by the script.
```

**[HOOK_CHARACTER_RULE]**
```text
HOOK CHARACTER RULE:
The character should express the dominant emotional objective of the hook.
Possible emotions include: concern, urgency, caution, conviction, curiosity, surprise, realization, determination, responsibility, hope.
Avoid forcing extreme anxiety in every hook.
```

**[HOOK_OBJECT_RULE]**
```text
HOOK OBJECT RULE:
Objects are optional storytelling amplifiers.
The generator may prioritize: facial expression, gesture, posture, symbolic object, environmental metaphor.
The strongest storytelling solution should be selected.
The hook does not require a broken object, chain, scroll, or coin in every case.
```

---

**IMAGEN HOOK (Stop Stack)** — solo para la primera imagen del Short (gancho, primeros 3-4 segundos):
```text
Dynamic composition with forced perspective, an intense visual break happening right behind a massive [COLOR SEMÁNTICO SEGÚN TIPO] text. [CHARACTER_RULE_SHORTS] expressing [EMOTION ACCORDING TO CLASSIFICATION (A, B, C)], engaging in a [ACTION OR SYMBOLIC METAPHOR], thick black ink stroke arms, subtle action lines emphasizing narrative focus,
— midground: [SUPPORTING SECONDARY ELEMENT OR OBJECT],
— background: [ENVIRONMENT ACCORDING TO CLASSIFICATION (A, B, C)], NO dark environment, completely eliminating deep dark shadows,
bright and warm ambient lighting,
[STYLE_RULE_SHORTS],
color accent rule: [OBJETO PRINCIPAL O DESTAQUE] in [COLOR + HEX] — main accent,
massive bold distressed [COLOR SEMÁNTICO] text that says "[1 A 3 PALABRAS IMPACTANTES]" positioned dead center, with the character clearly visible behind the text,
all elements within the 20%–80% vertical safe zone
```

**Reglas OBLIGATORIAS del Visual Hook (Stop Stack — Detener el Scroll):**

> ⛔ **VISUALIZE THE CORE TENSION (Show the problem, question, conflict, revelation, temptation, or opportunity driving the hook. Do not prematurely show the final solution.)**

*   **Regla 1 — Texto en imágenes (Excepción):** Esta es la **ÚNICA** imagen que lleva texto integrado desde el prompt. Para las demás, es **OBLIGATORIO** añadir el texto en CapCut.
    *   **Primer frame (00:00–00:03):** El texto de impacto va **OBLIGATORIAMENTE** en el prompt  (`massive bold [color] text that says "[TEXTO]" positioned dead center`).
*   **Regla 2 — El quiebre visual (Stop Stack):** NUNCA uses un personaje estático y aburrido. Debe haber un encuadre dinámico, pero la agresividad debe ajustarse al Tipo de Emoción (A, B o C).
*   **Regla 3 — Fondo visible (Sin oscuridad extrema):** NUNCA muestres desiertos vacíos ni exteriores excesivamente soleados si no apoyan la tensión. El fondo debe verse, no puede ser una mancha negra.
*   **Regla 4 — Texto en Color Semántico en el centro absoluto:** El texto va en el centro (usar el color correspondiente de la tabla semántica). La acción de tensión ocurre *detrás* del texto, asegurándose de que el personaje permanezca visible.
*   **Regla 5 — Zona segura vertical (20%–80%):** La interfaz de YouTube oculta el 20% inferior de la pantalla.

---

### 🟢 TERCER PROMPT BASE: El Cierre / Llamado a la Acción (CTA)
Este prompt se usa EXCLUSIVAMENTE para la última imagen del video. Perspectiva Forzada, rompe la cuarta pared.

```text
Dynamic mid-shot from a low angle, stick-figure character leaning forward breaking the fourth wall. [CHARACTER_RULE_SHORTS] but with strong conviction appropriate to the lesson, one arm extended straight toward the camera with forced perspective making the open palm appear huge in the foreground,
— midground: a massive glowing [OBJETO BÍBLICO-FINANCIERO: golden coin / heavy iron key / sealed scroll] floating above the oversized open palm, casting a warm amber light on the character's face,
— background: ancient stone walls with visible cracks, well-lit enclosed indoor space, NO dark environment,
[STYLE_RULE_SHORTS],
color accent rule: floating object in golden yellow (#C9A84C) — main accent,
intense warm amber wash (#E67E22) illuminating the face and palm — secondary accent,
all elements within the 20%–80% vertical safe zone
```

---

**Checklist de Validación Visual (Validar CADA imagen antes de entregar):**
* [ ] Does the character clearly express the dominant emotion of the scene? (Possible emotions include: concern, urgency, curiosity, conviction, surprise, determination, hope, caution, responsibility. Avoid emotionally flat characters).
* [ ] Does the environment reinforce the emotional objective of the scene? Closed environments are preferred for debt, pressure, temptation, urgency, and crisis. Open environments may be used for freedom, growth, wisdom, stewardship, progress, hope, and long-term vision.
* [ ] Does the scene contain either a meaningful object, OR a meaningful action, OR a meaningful emotional situation? (Avoid static idle poses).
* [ ] ¿La cara y el objeto están en el 20%–80% vertical de la pantalla?
* [ ] ¿El texto de CapCut confronta con una paradoja (no describe el video)?
* [ ] ¿La palabra clave del texto va en Color Semántico según la tabla?

---

### 🎬 MATRIZ DE AUTORIDAD VISUAL (Animación vs Estática)
Las IA de video (Sora, Kling, Runway) tienden a suavizar la estética cruda del grabado. Para mantener la autoridad del "Código", aplica estrictamente la regla del 90/10:

1. **90% Ken Burns (Estático):** La base del formato. La imagen de OpenAI Images 2 se mantiene estática, y el movimiento se logra con zooms o paneos lentísimos en CapCut.
2. **10% Animación Técnica:** Se usa SOLO para demostrar la mecánica de un sistema (ej. el flujo de capital, o gráficos llenándose). 
   - **Prohibición Absoluta:** NUNCA animes personajes caminando, hablando o haciendo movimientos bruscos.
3. **Semántica de Ruptura (El Flujo):** En las animaciones técnicas (10%), el personaje y el fondo permanecen estáticos (sepia). Lo único que se mueve es el activo/dato, usando el **Color Semántico** correspondiente de la tabla (ej. Rojo para deuda, Dorado para acumulación).
