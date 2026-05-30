# Producción — Imagen, Animación y Edición

## ⛔ 1. EL BLOQUEO ABSOLUTO (TIMESTAMPS)
La IA tiene estrictamente **PROHIBIDO** generar un solo prompt de imagen si el usuario no ha entregado previamente el guion con los **timestamps exactos del audio editado**. Sin timestamps, responder: *"Para generar los prompts necesito el guión final con timestamps. ¿Me lo compartes?"*

### ⏱️ EL POLICÍA DE TIEMPOS (REGLA DE AUTO-DIVISIÓN)

- **SHORT (< 01:10s):** **NINGUNA IMAGEN** puede durar más de 3-4 segundos. Auto-dividir bloques largos (ej. 9s → 3 imágenes de 3s).
- **VIDEO LARGO (> 02:00s):** 1 imagen cada 8–10 segundos es aceptable.

**Flujo:**
```
1. Guión con timestamps ✓
2. Contar bloques → número exacto de imágenes ✓
3. Generar prompts en orden (Estilo A por defecto) ✓
```

---

## Estilos disponibles

> **Default:** Estilo A (Codex). Generar automáticamente en Estilo A, a menos que el usuario pida explícitamente el Estilo B (Kurzgesagt bíblico).

---

## ESTILO A — Estilo "Codex" (Manuscrito Da Vinci)

**Paleta:**
| Uso | Hex |
|-----|-----|
| Fondo principal | `#E8D5B0` |
| Personajes | `#1A1A1A` |
| Acento cálido | `#C4956A` |

**4 elementos obligatorios en cada personaje:**

**1. Micro-expresiones y Ojos Expresivos** — `large round unfilled white head with thick black outlines, expressive cartoon eyes (white circles with black pupils) and thick bold black eyebrows showing [EMOCIÓN]`
- Cejas inclinadas hacia el centro, boca curvada hacia abajo = preocupación / culpa intensa
- Cejas arqueadas altas, ojos abiertos = sorpresa / revelación
- Cejas rectas, mirada firme = calma / autoridad / seriedad

**2. Silueta monigote con túnica** — `stick-figure character with thick black ink stroke arms and legs, torso wearing a simple flowing ancient tunic or shirt with stylized folds and volume`

> **Variaciones de la Cabeza del Personaje:**
> *   **PREDETERMINADO (Cabeza Blanca):** Usar siempre por defecto. Prompt: `large round unfilled white head with thick black outlines`.
> *   **OPCIONAL (Cabeza Negra Sólida):** Usar SOLO si el usuario pide explícitamente "el monigote negro" o "cabeza negra". Prompt: `large round solid black head`.

**3. Personajes Bíblicos (Regla Excepcional):** Si el guión pide un personaje bíblico (Salomón, José, Jesús), SIGUEN SIENDO "stick-figures" (sin rasgos faciales realistas), pero se distinguen agregando *props* de poder o vestuario. Ej: `a stick-figure character representing King Solomon wearing a worn golden crown and royal ancient robes`. NUNCA dibujar caras humanas.

**4. Fondos texturizados y definidos** — `background features architectural details drawn in dark, slightly thinner hand-drawn sketchy outlines, with pencil-sketch textures, stone cracks, and wood grain`

---

**Reglas de Oro del Delineado e Iluminación (¡CRÍTICO para evitar líneas digitales delgadas!):**

> ⛔ **PROHIBICIÓN DURA DE LÍNEAS VECTORIALES Y RUIDO:** Prohibido usar "clean line art" aburrido, pero también **PROHIBIDO** el ruido de textura (fibras, granos de arena, lápiz rasposo) porque arruina la animación de video en Kling/Runway (efecto boiling).
> **Prompt Obligatorio de Delineado/Sombra:** `thick bold hand-drawn black ink outlines with clean crisp solid edges, smooth solid warm beige background (#E8D5B0) completely free of paper grain or noise, flat cel-shading and smooth digital color wash for rich volumetric depth`.

---

**Reglas de Oro para el Acento de Color (¡CRÍTICO para evitar exceso de color!):**

> ⛔ **REGLA DE MINIMALISMO DE COLOR:** Los colores semánticos son SOLO para objetos pequeños de impacto (monedas, pergaminos, cadenas). NUNCA colorear áreas grandes, fondos, luz ambiental, ropa o paredes (todo esto va en outline negro o beige cálido natural).

**Colores semánticos corregidos y sus límites:**

| Color | Hex | Significado Narrativo | Cuándo Usarlo (LÍMITES ESTRICTOS) |
|-------|-----|----------------------|-----------------------------------|
| **Rojo** | `#C0392B` | Deuda, peligro, trampa, error | Solo en símbolos pequeños: un candado, un contrato abusivo, unas cadenas de esclavo, una X roja. *Nunca en fondos ni ropa.* |
| **Verde** | `#27AE60` | Bendición, salida, camino correcto | Solo en símbolos pequeños: una línea de camino que guía, un checkmark (✓), un brote de planta, una flecha de salida. *Nunca en luz ambiental, puertas ni ventanas.* |
| **Dorado** | `#C9A84C` | Dinero, talentos, lo sagrado | Solo en objetos: monedas de oro, el rollo/scroll sagrado abierto, una balanza de justicia. *Nunca en paredes ni cielos.* |
| **Azul** | `#2980B9` | Lo divino, revelación espiritual | Solo en destellos espirituales sutiles (como una línea de luz celestial o un halo). *Nunca en ropa ni agua de fondo.* |
| **Naranja** | `#E67E22` | Urgencia activa, transformación, calor | Solo en fuentes de luz viva y real: la llama de una antorcha, una lámpara de aceite, rayos de sol sutiles rompiendo nubes. *Usar para toda la luz ambiental en lugar de verde/azul.* |

---

**Modos de Iluminación por Bloque Narrativo:**

*   **Modo Normal (Beige Cálido):** Para bloques de calma, enseñanza o aplicación LATAM. Fondo beige cálido sólido y limpio, luz cálida difusa. Sin grano ni textura de papel.
*   **Modo Contraste Alto (Fondo Oscuro - Tensión):** Para bloques de Gancho, Deuda o Crisis. Forzar a DALL-E a usar sombras dramáticas: `dark rustic stone backgrounds with deep atmospheric shadows, soft focal amber light from oil lamps illuminating the main figure, creating a high-contrast printed comic book look`.

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
| **Escena de Deuda / Trampa** | Locked iron gates, dark oppressive stone walls closing in, crumple papers on floor |
| **Atmósfera Emocional** | Storm clouds (crisis), golden rays breaking through (hope), heavy dark sky (guilt) |

**Prompt base (sustituir campos en MAYÚSCULAS):**
```
[DESCRIPCIÓN DEL PERSONAJE Y ACCIÓN EN EL PRIMER PLANO],
stick-figure character with thick black ink stroke arms and legs, large round unfilled white head with thick black outlines, expressive cartoon eyes with pupils and thick bold black eyebrows showing [EMOCIÓN],
wearing a simple ancient [flowing tunic / plain shirt] with stylized folds,
— midground: [objeto secundario o figura de contexto en trazos medianos de tinta],
— background: [ELEMENTO CONTEXTUAL] drawn in dark, slightly thinner hand-drawn sketchy outlines, with pencil-sketch textures, stone cracks, and wood grain,
premium hand-drawn comic book aesthetic with clean precision,
smooth solid warm beige background (#E8D5B0) completely free of paper grain or noise,
thick bold hand-drawn black ink outlines with clean, crisp and solid edges,
flat cel-shading and smooth digital color wash for rich volumetric depth,
color accent rule: [ELEMENTO PRINCIPAL DE IMPACTO] in [COLOR + HEX] — main accent,
[ELEMENTO DE CONTRASTE SECUNDARIO] in [COLOR + HEX] — secondary accent,
everything else in crisp black ink outlines on smooth warm beige,
strictly no high-frequency noise, no pencil sketch marks, no dust particles, optimized for video animation,
optional environmental text in Spanish only
```

**Ejemplo de Prompt real (Estilo A):**
> *A stick-figure character kneeling in distress, holding an empty small leather pouch with both hands, thick black ink stroke arms and legs, large round unfilled white head with thick black outlines, expressive cartoon eyes with pupils and thick bold black eyebrows showing intense guilt and worry, wearing a simple flowing ancient tunic with stylized folds, — midground: a simple rustic wooden table drawn in sketchy outlines, — background: an ancient stone temple wall with deep shadows drawn in crisp outlines, premium hand-drawn comic book aesthetic with clean precision, smooth solid warm beige background (#E8D5B0) completely free of paper grain or noise, thick bold hand-drawn black ink outlines with clean, crisp and solid edges, flat cel-shading and smooth digital color wash for rich volumetric depth, color accent rule: empty leather pouch in dark brown (#C4956A) — main accent, everything else in crisp black ink outlines on smooth warm beige, strictly no high-frequency noise, optimized for video animation, optional environmental text in Spanish only*

---

Frame Hook (Stop Stack) — solo para la primera imagen del Short:
```text
Dynamic extreme close-up with forced perspective, an intense visual break happening right behind a massive red text, stick-figure character with large round unfilled white head with thick black outlines, hands violently smashing or breaking a [OBJETO BÍBLICO-FINANCIERO: ancient scroll / golden coin / iron chain] directly toward the camera, thick black ink stroke arms, action lines emphasizing the sudden violent motion,
— midground: out-of-focus fragments of the broken object flying toward the viewer,
— background: dark ancient stone walls with visible cracks and deep dramatic shadows, oppressive enclosed space with no sky visible,
single harsh spotlight or oil lamp casting dramatic amber side light, extreme high-contrast chiaroscuro lighting,
premium hand-drawn comic book aesthetic with clean precision,
thick bold hand-drawn black ink outlines with clean, crisp and solid edges,
flat cel-shading and smooth digital color wash for rich volumetric depth,
color accent rule: [OBJETO PRINCIPAL] fragments in golden yellow (#C9A84C) — main accent,
dramatic amber light (#E67E22) — secondary accent,
everything else in crisp black ink outlines on deep shadows,
massive bold distressed red text that says "[TEXTO DE CHOQUE: ERROR / MENTIRA]" positioned dead center, with the violent physical action happening around and behind the text to force the viewer's eye to the absolute center,
strictly no high-frequency noise, no pencil sketch marks, optimized for video animation,
optional environmental text in Spanish only,
all elements within the 20%–80% vertical safe zone
```

**Reglas de Oro del Primer Frame (Visual Hook — Detener el Scroll):**

> ⛔ **GRAFICAR LA ASFIXIA (Mostrar el Dolor, NO la Cura):** El Visual Hook (0-3s) DEBE mostrar angustia financiera cruda. NUNCA ilustrar la solución en el primer frame.

*   **Regla 1 — El Quiebre Visual (Stop Stack):** NUNCA un personaje parado reaccionando. Debe ser un zoom violento, un ángulo contrapicado, o un objeto rompiéndose violentamente en primer plano (Perspectiva forzada).
*   **Regla 2 — Fondo CERRADO y oscuro:** NUNCA desierto, cielo visible ni exterior soleado. Prompt obligatorio: `dark enclosed stone walls, oppressive space, no sky, no open landscape, no horizon line`.
*   **Regla 3 — Texto rojo en el centro absoluto:** La acción violenta ocurre *detrás o alrededor* del texto para forzar un solo punto focal.
*   **Regla 4 — Zona Segura Vertical (20%–80%):** La UI de YouTube tapa el 20% inferior.
*   **Regla 5 — Texto en CapCut vs Texto en DALL-E:**
    - **Primer frame (00:00–00:03):** El texto de choque va embebido directamente en el prompt de DALL-E (`massive bold red text that says "[TEXTO]" positioned dead center`).
    - **Resto del video:** El texto va superpuesto en CapCut. Debe golpear una contradicción, nunca describir el video. La palabra más perturbadora va en color de ruptura: rosa (`#FF2D78`), rojo (`#FF3333`) o naranja neón (`#FF6B00`). Este color NUNCA va dentro del prompt de DALL-E.

---

### 🟢 TERCER PROMPT BASE: El Cierre / Llamado a la Acción (CTA)
Este prompt se usa EXCLUSIVAMENTE para la última imagen del video (el clímax y comando final). Usa Perspectiva Forzada, luces dramáticas y rompe la cuarta pared para obligar al usuario a tomar acción.

```text
Dynamic mid-shot from a low angle, stick-figure character leaning forward breaking the fourth wall, large round unfilled white head with thick black outlines, intense piercing stare directly at the viewer with furrowed thick bold black eyebrows showing extreme conviction, one arm extended straight toward the camera with forced perspective making the open palm appear huge in the foreground, thick black ink stroke arms, wearing a simple plain shirt with stylized folds,
— midground: a massive glowing [OBJETO BÍBLICO-FINANCIERO: golden coin / heavy iron key / sealed scroll] floating just millimeters above the oversized open palm, casting a warm amber light on the character's face,
— background: dark ancient stone walls with deep heavy shadows, completely out of focus to force all attention on the glowing object and the character's intense eyes,
premium hand-drawn comic book aesthetic with clean precision,
thick bold hand-drawn black ink outlines with clean crisp and solid edges,
flat cel-shading but with high-contrast dramatic chiaroscuro lighting,
color accent rule: floating object in golden yellow (#C9A84C) — main accent,
intense warm amber wash (#E67E22) illuminating the face and palm — secondary accent,
everything else in crisp black ink outlines on deep shadows,
strictly no high-frequency noise, no pencil sketch marks, no dust particles, optimized for video animation,
optional environmental text in Spanish only,
all elements within the 20%–80% vertical safe zone
```

---
> ⛔ **ANTI-LISTA: Frames que SIEMPRE rinden mal (rechazar y regenerar si aparecen):**
>
> | Señal de frame muerto | Por qué falla | Ejemplo real de bajo rendimiento |
> |----------------------|---------------|----------------------------------|
> | Personaje sonriendo o neutral | No hay tensión = no hay razón para detenerse | Figura parada en desierto con sonrisa (226 vistas) |
> | Exterior abierto (desierto, campo, cielo) | Se pierde en el feed, sin contraste visual | Paisaje soleado con personaje pequeño al centro |
> | Personaje de pie con brazos a los lados | Parece ilustración de libro infantil, no urgencia | Figura estática sin interacción con ningún objeto |
> | Sin objeto bíblico-financiero en manos | No hay anclaje visual = la mirada del espectador no sabe a dónde ir | Solo personaje sin contexto de lo que descubrió |

**Checklist rápido para el Primer Frame (Validar antes de entregar):**
* [ ] ¿El personaje muestra shock físico (retrocede, se agarra el pecho, ojos desorbitados)?
* [ ] ¿El fondo es cerrado, oscuro y con alto contraste (muros, cueva, sin cielo)?
* [ ] ¿El personaje sostiene o interactúa con un objeto bíblico-financiero?
* [ ] ¿La cara y el objeto están en el 20%–80% vertical de la pantalla?
* [ ] ¿El texto de CapCut confronta con una paradoja (no describe el video)?
* [ ] ¿La palabra clave del texto va en color de ruptura (rosa/rojo/naranja)?


---

## ESTILO B — Kurzgesagt bíblico

**Paleta:**
| Uso | Hex |
|-----|-----|
| Fondo principal | `#0D1B2A` |
| Acento principal | `#C9A84C` |
| Acento secundario | `#E8A020` |

**Prompt base:**
```
[DESCRIPCIÓN DE LA ESCENA],
— midground: [elementos secundarios de contexto],
— background: [ambiente con al menos 2 elementos específicos],
2D flat illustration, warm cinematic lighting,
rich layered scene with foreground midground and background depth,
deep navy and ochre color palette, golden accents,
Middle Eastern biblical setting, expressive characters with detailed surrounding environment,
Kurzgesagt-inspired style meets biblical manuscript art,
high contrast, storytelling mood, no text
```

> **NOTA SOBRE EL COLOR (ESTILO B):** Aunque este estilo usa una paleta distinta, **aplica la misma regla de minimalismo de color**. El dorado y ocre deben reservarse para elementos simbólicos o luz, no para bañar toda la escena.

> **NOTA SOBRE EL PERSONAJE (ESTILO B):** Las **Variaciones de la Cabeza del Personaje** (cabeza blanca por defecto / cabeza negra opcional) aplican a ambos estilos. Si el usuario usa Estilo B, el personaje sigue siendo un stick-figure con `large round unfilled white head with thick black outlines` a menos que se indique lo contrario.

**Ejemplo de Prompt real (Estilo B):**
> *A young merchant counting silver coins on a dark wooden table in a busy marketplace under warm torchlight, — midground: clay jars, fabrics, and baskets of grain, — background: sandstone arches and palm trees under a deep navy night sky, 2D flat illustration, warm cinematic lighting, rich layered scene with foreground midground and background depth, deep navy and ochre color palette, golden accents, Middle Eastern biblical setting, expressive characters with detailed surrounding environment, Kurzgesagt-inspired style meets biblical manuscript art, high contrast, storytelling mood, no text*

---

## Formato de entrega obligatorio (Tarjetas de Producción + Bloque Raw)

Entregar SIEMPRE la respuesta en dos partes, sin excepciones. Queda estrictamente PROHIBIDO usar tablas de Markdown, ya que comprimen el texto.

**PARTE 1: Las Tarjetas de Producción**
Presenta cada bloque de imagen como una tarjeta vertical y fácil de leer.

**🎬 BLOQUE [00:00 – 00:03]**
*   🖼️ **DALL-E:** `(Prompt visual completo)`
*   🎥 **Kling/Runway:** `(Prompt de movimiento en inglés)` [OPCIONAL / RECOMENDADO]
*   ✨ **CapCut:** Entrada: Zoom rápido / Salida: Fade
*   📝 **Texto en Pantalla:** "PARA DEUDORES" [IDEAL / OPCIONAL]

**🎬 BLOQUE [00:03 – 00:06]**
*   🖼️ **DALL-E:** `(Prompt visual completo)`
*   🎥 **Kling/Runway:** `Fast push in camera, heavy dust...` [RECOMENDADO]
*   ✨ **CapCut:** Entrada: Flash Blur / Salida: Wipe-L
*   📝 **Texto en Pantalla:** "¿Llevas años?" [RECOMENDADO]

*(Repetir para todos los bloques...)*

**PARTE 2: El Bloque Raw para Batch (Copy-Paste)**
Justo debajo de la tabla, entrega un único bloque de código (`text`) que contenga ÚNICAMENTE los prompts de imagen de DALL-E, uno por línea. Sin viñetas, sin números, sin timestamps. Esto es para que el usuario pueda copiar todo el bloque y pegarlo en una extensión de Chrome para generar en masa.

```text
(Prompt completo de la imagen 1)
(Prompt completo de la imagen 2)
(Prompt completo de la imagen 3)
```

### ⛔ REGLA DE TEXTOS EN PANTALLA (Dos tipos — no confundir)

| Tipo | Qué es | Dónde va | Ejemplo |
|------|--------|----------|---------|
| **Texto Ambiental** | Decoración diegética (en pergaminos, paredes, carteles del fondo) | En el prompt de DALL-E con sufijo: `optional environmental text in Spanish only` | Texto en un calendario de fondo |
| **Texto de Choque** | Texto gigante rojo de impacto que domina la pantalla | SOLO en el primer frame (00:00–00:03), embebido en el prompt de DALL-E | `massive bold red text that says "ERROR" positioned dead center` |

Si DALL-E alucina demasiado texto ambiental, reemplazar el sufijo por `no text`.

### 🎬 REGLA DE ANIMACIÓN DE VIDEO: LAS 3 CAPAS DE MOVIMIENTO (KLING/RUNWAY)
Las IA de video (Kling, Runway) tienden a ser estáticas si no se les exige acción intensa. Para evitar videos congelados, el **Prompt video (Kling/Runway)** debe forzar obligatoriamente tres capas de movimiento dinámico simultáneo, siempre en inglés:
1. **Cámara (Cinematografía):** `fast push-in camera`, `shaky handheld camera`, `slow pan right`.
2. **Sujeto (Acción agresiva):** Verbos fuertes. No "raises head", sino `violently recoils backward`, `smashes hand on table`, `drops the coins`.
3. **Entorno (Partículas/Luz):** Obliga a la IA a procesar físicas. `heavy dust floating in the air`, `smoke billowing`, `dramatic flickering light`.

*Ejemplo perfecto:* `Fast push-in camera, character violently recoils backward dropping the scroll, heavy dust floating in the air, dramatic flickering amber light.`

**Prioridad Video (Columna 4):**
- **RECOMENDADO:** Hook / impacto inicial, Crisis / decisión, Deuda / trampa, Giro dramático, Tensión.
- **OPCIONAL:** Enseñanza / teoría, Transformación / esperanza, Familia / empatía, Cierre.

**Regla de sincronización guión → tabla de prompts (Shorts):**
> Cuando generes la tabla de prompts para Shorts, incluye la etiqueta `[PAUSA 1s]` y el prompt de animación de la cifra creciendo (ej. `number growing from 0 to 70, smooth count-up animation`) en la columna **Prompt video (Kling/Runway)**, tal como se exige en el bloque DECODIFICACIÓN del archivo de guiones. Si el guión marca `[PAUSA 1s — número crece en pantalla]`, la fila correspondiente en la tabla DEBE tener el prompt de animación que ejecuta ese efecto. Sin excepción.

---

## Tabla de animaciones CapCut por tipo de escena

| Tipo de escena | Entrada (IN) | Salida (OUT) |
|---------------|-------------|-------------|
| Hook / impacto emocional | Flash Blur | Dark Wipe-L |
| Enseñanza / revelación | Fade In | Dark Wipe-L |
| Crisis / decisión | Forceful Pull | Dark Wipe-Up |
| Transformación / esperanza | Slide Up | Vision Shrink |
| Deuda / trampa | Shaky Lens | Dark Wipe-Down |
| Familia / empatía | Fade-In Wipe | Vision Shrink |
| Cierre / CTA | Forceful Pull | Dark Wipe-Up |
| Giro / revelación dramática | Flash Flip-In | Slice Shrink |
| Tensión acumulada | Wavy Wash-Up | Dark Wipe-Up |

## Fuentes de recursos

| Recurso | Uso |
|---------|-----|
| MixKit | SFX y efectos de transición — gratuito, arsenal principal |
| Coverr | Videos cinemáticos en bucle para fondos (opcional) |
