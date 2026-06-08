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

**Estructura de 3 planos (Obligatoria para evitar personajes flotando en el vacío):**
- **Foreground (Plano cercano):** Personaje principal + objeto central de la escena (monedas, Biblia, cadenas).
- **Midground (Plano medio):** Mobiliario, escalones, personas de soporte, puertas que dan contexto.
- **Background (Plano lejano):** Ambiente completo que ubica la escena — nunca vacío o beige liso.

**Biblioteca de Fondos (Backgrounds) recomendados por Contexto:**

| Contexto de Escena | Elementos de Background Obligatorios (DALL-E 3) |
|---------------------|-----------------------------------------------|
| **Interior Bíblico** | Stone walls with cracks, arched doorway with curtain, clay oil lamps, wooden shelves |
| **Exterior Bíblico** | Dusty hills winding dirt road, city gates on horizon, olive trees, overcast sky |
| **Interior Moderno LATAM** | Modest kitchen shelves, handwritten calendar on wall, small window showing neighborhood |
| **Escena de Deuda / Trampa** | Locked iron gates, enclosed stone walls closing in, papers on floor, well-lit indoor environment |
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
STRICTLY NO TEXT, NO WORDS, NO LETTERS IN THE IMAGE
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

**IMAGEN HOOK (Stop Stack)** — solo para la primera imagen del Short (gancho, primeros 3-4 segundos):
```text
Dynamic extreme close-up with forced perspective, an intense visual break happening right behind a massive red text. [CHARACTER_RULE], gripping or holding a [OBJETO BÍBLICO-FINANCIERO: ancient scroll / golden coin / iron chain / among others] tensely near the chest, thick black ink stroke arms, subtle action lines emphasizing tension without violence,
— midground: out-of-focus fragments of the broken object flying toward the viewer,
— background: ancient stone walls with visible cracks, well-lit enclosed indoor space with no sky visible, NO dark environment, completely eliminating deep dark shadows,
bright and warm ambient lighting, multiple oil lamps casting bright amber light across the entire scene,
[STYLE_RULE],
color accent rule: [OBJETO PRINCIPAL] fragments in golden yellow (#C9A84C) — main accent,
bright ambient amber light (#E67E22) — secondary accent,
massive bold distressed red text that says "[TEXTO DE CHOQUE: ERROR / MENTIRA]" positioned dead center, with the character clearly visible behind the text,
all elements within the 20%–80% vertical safe zone
```

**Reglas OBLIGATORIAS del Visual Hook (Stop Stack — Detener el Scroll):**

> ⛔ **GRAFICAR LA ASFIXIA (Mostrar el dolor, NO la cura):** El *Visual Hook* (0-3s) DEBE transmitir angustia financiera cruda. NUNCA ilustres la solución en este primer frame.

*   **Regla 1 — Texto en imágenes (Excepción):** Esta es la **ÚNICA** imagen que lleva texto integrado desde el prompt. Para las demás, es **OBLIGATORIO** añadir el texto en CapCut.
    *   **Primer frame (00:00–00:03):** El texto de impacto va **OBLIGATORIAMENTE** en el prompt  (`massive bold red text that says "[TEXTO]" positioned dead center`).
*   **Regla 2 — El quiebre visual (Stop Stack):** NUNCA uses un personaje estático y aburrido. Debe haber un encuadre dinámico (extreme close-up), pero **SIN ser agresivo ni violento**. El personaje debe sostener la tensión desde atrás del texto, manteniendo neutralidad en su expresión.
*   **Regla 3 — Fondo cerrado y visible (Sin oscuridad extrema):** NUNCA muestres desiertos, cielos ni exteriores soleados. El fondo debe verse, no puede ser una mancha negra. El prompt debe incluir OBLIGATORIAMENTE: `No dark environment, enclosed stone walls, oppressive space, no sky, no open landscape, no horizon line`.
*   **Regla 4 — Texto en Color Semántico en el centro absoluto:** El texto va en el centro (usar el color correspondiente de la tabla semántica). La acción de tensión ocurre *detrás* del texto, asegurándose de que el personaje permanezca visible.
*   **Regla 5 — Zona segura vertical (20%–80%):** La interfaz de YouTube oculta el 20% inferior de la pantalla.

---

### 🟢 TERCER PROMPT BASE: El Cierre / Llamado a la Acción (CTA)
Este prompt se usa EXCLUSIVAMENTE para la última imagen del video. Perspectiva Forzada, rompe la cuarta pared.

```text
Dynamic mid-shot from a low angle, stick-figure character leaning forward breaking the fourth wall. [CHARACTER_RULE] but with intense piercing stare directly at the viewer with furrowed eyebrows showing extreme conviction, one arm extended straight toward the camera with forced perspective making the open palm appear huge in the foreground,
— midground: a massive glowing [OBJETO BÍBLICO-FINANCIERO: golden coin / heavy iron key / sealed scroll] floating above the oversized open palm, casting a warm amber light on the character's face,
— background: ancient stone walls with visible cracks, well-lit enclosed indoor space, NO dark environment,
[STYLE_RULE],
color accent rule: floating object in golden yellow (#C9A84C) — main accent,
intense warm amber wash (#E67E22) illuminating the face and palm — secondary accent,
all elements within the 20%–80% vertical safe zone
```

---

**Checklist de Validación Visual (Validar CADA imagen antes de entregar):**
* [ ] ¿El personaje muestra tensión física (retrocede, agarra el pecho, ojos desorbitados)? *(NO neutral ni sonriente)*
* [ ] ¿El fondo es cerrado pero bien iluminado (paredes, interior, sin cielo)? *(NO desierto, campo, exterior)*
* [ ] ¿El personaje sostiene o interactúa con un objeto bíblico-financiero? *(NO brazos a los lados)*
* [ ] ¿La cara y el objeto están en el 20%–80% vertical de la pantalla?
* [ ] ¿El texto de CapCut confronta con una paradoja (no describe el video)?
* [ ] ¿La palabra clave del texto va en Color Semántico según la tabla?

---

### 🎬 MATRIZ DE AUTORIDAD VISUAL (Animación vs Estática)
Las IA de video (Sora, Kling, Runway) tienden a suavizar la estética cruda del grabado. Para mantener la autoridad del "Código", aplica estrictamente la regla del 90/10:

1. **90% Ken Burns (Estático):** La base del formato. La imagen de DALL-E se mantiene estática, y el movimiento se logra con zooms o paneos lentísimos en CapCut.
2. **10% Animación Técnica:** Se usa SOLO para demostrar la mecánica de un sistema (ej. el flujo de capital, o gráficos llenándose). 
   - **Prohibición Absoluta:** NUNCA animes personajes caminando, hablando o haciendo movimientos bruscos.
3. **Semántica de Ruptura (El Flujo):** En las animaciones técnicas (10%), el personaje y el fondo permanecen estáticos (sepia). Lo único que se mueve es el activo/dato, usando el **Color Semántico** correspondiente de la tabla (ej. Rojo para deuda, Dorado para acumulación).
