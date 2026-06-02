# Producción — Imagen, Animación y Edición

## ⛔ 1. EL BLOQUEO ABSOLUTO (TIMESTAMPS)
La IA tiene estrictamente **PROHIBIDO** generar un solo prompt de imagen si el usuario no ha entregado previamente el guion con los **timestamps exactos del audio editado**. Sin timestamps, responder: *"Para generar los prompts necesito el guión final con timestamps. ¿Me lo compartes?"*

### ⏱️ EL POLICÍA DE TIEMPOS (REGLA DE AUTO-DIVISIÓN)

- **EL GANCHO (Los primeros 0 a ~3s):** Queda ESTRICTAMENTE PROHIBIDO dividir el gancho en múltiples imágenes, sin importar si el audio tiene pausas de microsegundos o texto de impacto inicial (ej. 00:00 - 00:00,600). El Hook completo se cubre con UNA ÚNICA IMAGEN (Frame 0 — Hook visual).
- **SHORT (< 01:10s):** Después del gancho, **NINGUNA IMAGEN** puede durar más de 3-4 segundos. Auto-dividir bloques largos (ej. 9s → 3 imágenes de 3s).
- **VIDEO LARGO (> 02:00s):** Después del gancho, 1 imagen cada 8–10 segundos es aceptable.

**Flujo:**
```
1. Guión con timestamps ✓
2. Contar bloques → número exacto de imágenes ✓
3. Generar prompts en orden (Estilo A por defecto) ✓
```

---

## Estilo "Codex" (Manuscrito Da Vinci)

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

**IMPORTANTE REGLA DURA**
- El texto 'optional environmental text in Spanish only' en el promt es OBLIGATORIO para TODAS las imágenes.
- A EXCEPCIÓN DE LA PRIMERA IMAGEN HOOK, no generar **TEXTO** dentro de las imágenes. Para todos los demás bloques, el texto se añade en CapCut.

---

**IMAGEN HOOK (Stop Stack)** — solo para la primera imagen del Short (gancho, primeros 3-4 segundos):
```text
Dynamic extreme close-up with forced perspective, an intense visual break happening right behind a massive red text, stick-figure character with large round unfilled white head with thick black outlines, expressive cartoon eyes with pupils and thick bold black eyebrows showing [EMOCIÓN], hands violently smashing or breaking a [OBJETO BÍBLICO-FINANCIERO: ancient scroll / golden coin / iron chain] directly toward the camera, thick black ink stroke arms, action lines emphasizing the sudden violent motion,
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

**Reglas OBLIGATORIAS del Visual Hook (Stop Stack — Detener el Scroll):**

> ⛔ **GRAFICAR LA ASFIXIA (Mostrar el dolor, NO la cura):** El *Visual Hook* (0-3s) DEBE transmitir angustia financiera cruda. NUNCA ilustres la solución en este primer frame.

*   **Regla 1 — Texto en imágenes (Excepción):** Esta es la **ÚNICA** imagen que lleva texto integrado desde el prompt. Para las demás, es **OBLIGATORIO** añadir el texto en CapCut.
    *   **Primer frame (00:00–00:03):** El texto de impacto va **OBLIGATORIAMENTE** en el prompt  (`massive bold red text that says "[TEXTO]" positioned dead center`).
*   **Regla 2 — El quiebre visual (Stop Stack):** NUNCA uses un personaje estático reaccionando. Debe haber un zoom violento, un ángulo contrapicado o un objeto rompiéndose violentamente en primer plano (perspectiva forzada).
*   **Regla 3 — Fondo cerrado y oscuro:** NUNCA muestres desiertos, cielos ni exteriores soleados. El prompt debe incluir OBLIGATORIAMENTE: `dark enclosed stone walls, oppressive space, no sky, no open landscape, no horizon line`.
*   **Regla 4 — Texto rojo en el centro absoluto:** La acción violenta debe ocurrir *detrás o alrededor* del texto para forzar la atención en un solo punto focal.
*   **Regla 5 — Zona segura vertical (20%–80%):** La interfaz de YouTube oculta el 20% inferior de la pantalla.

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
> ⛔ **ANTI-LISTA: Frames que SIEMPRE rinden mal (rechazar y regenerar):**
>
> | Señal de frame muerto | Por qué falla |
> |----------------------|---------------|
> | Personaje sonriendo o neutral | No hay tensión = no detiene el scroll |
> | Exterior abierto (desierto, campo, cielo) | Se pierde en el feed, sin contraste |
> | Personaje de pie con brazos a los lados | Parece libro infantil, no urgencia |
> | Sin objeto bíblico-financiero en manos | No hay anclaje visual |

**Checklist rápido para la Primera Imagen (Hook Visual) (Validar antes de entregar):**
* [ ] ¿El personaje muestra shock físico (retrocede, se agarra el pecho, ojos desorbitados)?
* [ ] ¿El fondo es cerrado, oscuro y con alto contraste (paredes, cueva, sin cielo)?
* [ ] ¿El personaje sostiene o interactúa con un objeto bíblico-financiero?
* [ ] ¿La cara y el objeto están en el 20%–80% vertical de la pantalla?
* [ ] ¿El texto de CapCut confronta con una paradoja (no describe el video)?
* [ ] ¿La palabra clave del texto va en color de ruptura (rosa/rojo/naranja)?

---

## Formato de entrega obligatorio (Tarjetas de Producción + Bloque Raw)

Entregar SIEMPRE la respuesta en dos partes, sin excepciones. Queda estrictamente PROHIBIDO usar tablas de Markdown, ya que comprimen el texto.

**PARTE 1: Las Tarjetas de Producción**
Presenta cada bloque de imagen como una tarjeta vertical y fácil de leer.

**🎬 BLOQUE [00:00 – 00:03]**
*   🖼️ **DALL-E:** `(Prompt visual completo)`
*   🎥 **Kling/Runway:** `(Prompt de movimiento en inglés)` [OPCIONAL / RECOMENDADO]
*   ✨ **CapCut:** Entrada: Zoom rápido / Salida: Fade
*   📝 **Texto en Pantalla:** "PARA DEUDORES" (Fuente Blanca, palabra clave en Rojo `#FF3333` o Amarillo `#C9A84C`) [IDEAL / OPCIONAL]

**🎬 BLOQUE [00:03 – 00:06]**
*   🖼️ **DALL-E:** `(Prompt visual completo)`
*   🎥 **Kling/Runway:** `Fast push in camera, heavy dust...` [RECOMENDADO]
*   ✨ **CapCut:** Entrada: Flash Blur / Salida: Wipe-L
*   📝 **Texto en Pantalla:** "¿Llevas años?" (Fuente Blanca, palabra clave en Rojo `#FF3333` o Amarillo `#C9A84C`) [RECOMENDADO]

*(Repetir para todos los bloques...)*

**PARTE 2: El Bloque Raw para Batch (Copy-Paste)**
Justo debajo de la tabla, entrega un único bloque de código (`text`) que contenga ÚNICAMENTE los prompts de imagen , uno por línea. Sin viñetas, sin números, sin timestamps. Esto es para que el usuario pueda copiar todo el bloque y pegarlo en una extensión de Chrome para generar en masa.

```text
Create an image of (Prompt completo de la imagen 1)
Create an image of (Prompt completo de la imagen 2)
Create an image of (Prompt completo de la imagen 3)
```

### ⛔ REGLA DE TEXTOS EN PANTALLA (Dos tipos — no confundir)

| Tipo | Qué es | Dónde va | Ejemplo |
|------|--------|----------|---------|
| **Texto Ambiental** | Decoración diegética (en pergaminos, paredes, carteles del fondo) | En el prompt  con sufijo: `optional environmental text in Spanish only` | Texto en un calendario de fondo |
| **Texto de Choque** | Texto gigante rojo de impacto que domina la pantalla | SOLO en la primera imagen (Hook Visual) (00:00–00:03), embebido en el prompt  | `massive bold red text that says "[TEXTO]" positioned dead center` |

### 🎬 REGLA DE ANIMACIÓN DE VIDEO: LAS 3 CAPAS DE MOVIMIENTO
Las IA de video tienden a ser estáticas si no se les exige acción intensa. Para evitar videos congelados, el **Prompt video** debe forzar obligatoriamente tres capas de movimiento dinámico simultáneo, siempre en inglés:

1. **Cámara (Cinematografía):** `fast push-in camera`, `shaky handheld camera`, `slow pan right`.
2. **Sujeto (Acción agresiva):** Verbos fuertes. No "raises head", sino `violently recoils backward`, `smashes hand on table`, `drops the coins`.
3. **Entorno (Partículas/Luz):** Obliga a la IA a procesar físicas. `heavy dust floating in the air`, `smoke billowing`, `dramatic flickering light`.

> ⚠️ **REGLA PARA EL HOOK VISUAL (Conservación de Texto):** El texto de impacto ya fue generado en la primera imagen. Para evitar que la IA de video lo deforme o lo borre, NUNCA escribas la frase literal dentro del prompt de video. En su lugar, agrega la instrucción `text doesn't disappear in animation`.

*Ejemplo perfecto (Escena normal):* `Fast push-in camera, character violently recoils backward dropping the scroll, heavy dust floating in the air, dramatic flickering amber light`
*Ejemplo perfecto (Hook Visual con texto):* `Fast push-in camera, character violently recoils backward dropping the scroll, heavy dust floating in the air, dramatic flickering amber light, text doesn't disappear in animation`

**Prioridad de Animación de Video:**
- **RECOMENDADO:** Hook / impacto inicial, Crisis / decisión, Deuda / trampa, Giro dramático, Tensión.
- **OPCIONAL:** Enseñanza / teoría, Transformación / esperanza, Familia / empatía, Cierre.

**Regla de sincronización guión → tarjetas de producción (Shorts):**
> Cuando generes las tarjetas de producción para Shorts, incluye la etiqueta `[PAUSA 1s]` y el prompt de animación de la cifra creciendo (ej. `number growing from 0 to 70, smooth count-up animation`) en la sección **Kling/Runway**, tal como se exige en el bloque DECODIFICACIÓN del archivo de guiones. Si el guión marca `[PAUSA 1s — número crece en pantalla]`, la tarjeta correspondiente DEBE tener el prompt de animación que ejecuta ese efecto. Sin excepción.

---

## Directrices de Edición Pacing (CapCut)

Para evitar que una edición plana destruya la retención del video, exige siempre este pacing de "Frenar y Apilar":

1. **Frenado Visual (0.0s - 1.5s):** Edición rápida y cortes agresivos. No dejes que la imagen respire. La música debe ser tensa e incómoda. El texto en pantalla (generado en CapCut) debe aparecer **palabra por palabra** obligando al cerebro a leer ("Secuestro de la mente"). Siempre especifica el color de ruptura para la palabra clave (Rojo `#FF3333` o Amarillo Oro `#C9A84C`).
2. **Apilado Visual (1.5s - 5.0s):** Baja el ritmo ligeramente para que la autoridad técnica se asiente. Usa un zoom lento (15% zoom in) o un cambio drástico de color (ej. un tono magenta) para señalar que la información es crítica.
3. **Ruptura Visual (0:20 - 0:30):** Introduce un "swell" musical (subida repentina) y ejecuta un cambio drástico de plano (zoom 15% rápido o ruptura visual del personaje) para sacudir de nuevo al espectador y evitar el desgaste.

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
| MixKit | SFX y transiciones (gratuito) |
| Coverr | Videos cinemáticos en bucle para fondos (opcional) |
