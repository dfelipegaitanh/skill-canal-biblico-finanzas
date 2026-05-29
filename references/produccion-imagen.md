# Producción — Imagen, Animación y Edición

## PREREQUISITO ABSOLUTO

> ⛔ No se genera ningún prompt de imagen sin tener el guión final con timestamps. Sin timestamps, no hay prompts.

**Frecuencia de imágenes:**
- **Micro-Short** (15–20s): máximo 5–6 imágenes totales (1 cada 3 segundos)
- **Short estándar** (50–60s): 1 imagen cada 3–4 segundos
- **Video largo** (5–20 min): 1 imagen cada 8–10 segundos

**Flujo correcto:**
```
1. Guión con timestamps ✓
2. Contar bloques → calcular número exacto de imágenes ✓
3. Preguntar estilo (A o B) ✓
4. Generar prompts uno por uno en orden ✓
```

Si el usuario pide prompts sin el guión con timestamps, responder:
> *"Para generar los prompts necesito el guión final con timestamps. ¿Me lo compartes?"*

---

## Estilos disponibles — preguntar siempre antes de generar

> "¿En qué estilo quieres las imágenes?
> **A) Estilo "Codex" (Manuscrito Da Vinci)** — personajes cómic latinoamericano, trazos de tinta gruesa, fondo beige texturizado (default). Contra-señal a la basura 3D.
> **B) Kurzgesagt bíblico** — 2D flat, azul noche + dorado, personajes latinos"

Solo se puede elegir A o B. No se generan prompts en ningún otro estilo.

---

## ESTILO A — Estilo "Codex" (Manuscrito Da Vinci)

**Paleta:**
| Uso | Hex |
|-----|-----|
| Fondo principal | `#E8D5B0` |
| Personajes | `#1A1A1A` |
| Acento cálido | `#C4956A` |

**3 elementos obligatorios en cada personaje:**

**1. Micro-expresiones y Ojos Expresivos** — `large round head, expressive cartoon eyes (white circles with black pupils) and thick bold black eyebrows showing [EMOCIÓN]`
- Cejas inclinadas hacia el centro, boca curvada hacia abajo = preocupación / culpa intensa
- Cejas arqueadas altas, ojos abiertos = sorpresa / revelación
- Cejas rectas, mirada firme = calma / autoridad / seriedad

**2. Silueta monigote con túnica** — `stick-figure character with thick black ink stroke arms and legs, torso wearing a simple flowing ancient tunic or shirt with stylized folds and volume`

**3. Personajes Bíblicos (Regla Excepcional):** Si el guión pide un personaje bíblico (Salomón, José, Jesús), SIGUEN SIENDO "stick-figures" (sin rasgos faciales realistas), pero se distinguen agregando *props* de poder o vestuario. Ej: `a stick-figure character representing King Solomon wearing a worn golden crown and royal ancient robes`. NUNCA dibujar caras humanas.

**3. Fondos texturizados y definidos** — `background features architectural details drawn in dark, slightly thinner hand-drawn sketchy outlines, with pencil-sketch textures, stone cracks, and wood grain`

---

**Reglas de Oro del Delineado e Iluminación (¡CRÍTICO para evitar líneas digitales delgadas!):**

> ⛔ **PROHIBICIÓN DURA DE LÍNEAS VECTORIALES:** Prohibido usar "clean line art" o "smooth lines".
> **Prompt Obligatorio de Delineado/Sombra:** `thick bold hand-drawn black ink outlines, coarse textured warm beige paper background (#E8D5B0) with visible organic fiber flecks, soft charcoal shading and warm gradients for rich volumetric depth`.

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

*   **Modo Normal (Beige Cálido):** Para bloques de calma, enseñanza o aplicación LATAM. Fondo beige con textura gruesa de papel y luz cálida difusa.
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
stick-figure character with thick black ink stroke arms and legs, large round head, expressive cartoon eyes with pupils and thick bold black eyebrows showing [EMOCIÓN],
wearing a simple ancient [flowing tunic / plain shirt] with stylized folds,
— midground: [objeto secundario o figura de contexto en trazos medianos de tinta],
— background: [ELEMENTO CONTEXTUAL] drawn in dark, slightly thinner hand-drawn sketchy outlines, with pencil-sketch textures, stone cracks, and wood grain,
felt-tip pen ink illustration style, premium hand-drawn comic book aesthetic,
coarse textured warm beige paper background (#E8D5B0) with visible organic fiber flecks and sand grain texture,
thick bold hand-drawn black ink outlines with subtle organic imperfections and slightly rough edges,
soft charcoal shading and warm gradients for rich volumetric depth,
color accent rule: [ELEMENTO PRINCIPAL DE IMPACTO] in [COLOR + HEX] — main accent,
[ELEMENTO DE CONTRASTE SECUNDARIO] in [COLOR + HEX] — secondary accent,
everything else in bold black ink outlines on textured warm beige,
no text
```

**Ejemplo de Prompt real (Estilo A):**
> *A stick-figure character kneeling in distress, holding an empty small leather pouch with both hands, thick black ink stroke arms and legs, large round head, expressive cartoon eyes with pupils and thick bold black eyebrows showing intense guilt and worry, wearing a simple flowing ancient tunic with stylized folds, — midground: a simple rustic wooden table drawn in sketchy outlines, — background: an ancient stone temple wall with visible cracks and rough stone textures drawn in slightly thinner sketchy ink outlines, felt-tip pen ink illustration style, premium hand-drawn comic book aesthetic, coarse textured warm beige paper background (#E8D5B0) with visible organic fiber flecks and sand grain texture, thick bold hand-drawn black ink outlines with subtle organic imperfections and slightly rough edges, soft charcoal shading and warm gradients for rich volumetric depth, color accent rule: empty leather pouch in dark brown (#C4956A) — main accent, everything else in black ink outlines on textured warm beige, no text*

---

Frame Hook — solo para la primera imagen del Short:
```
A stick-figure character with wide alarmed eyes and body recoiling backward in shock, one hand pressing against chest in disbelief, the other hand gripping [OBJETO BÍBLICO-FINANCIERO: ancient scroll / gold coin / iron chains] tightly, thick black ink stroke arms and legs, large round head, expressive cartoon eyes with pupils wide open and thick bold black eyebrows shot up high showing intense shock and disturbed revelation, mouth slightly open, wearing a simple ancient tunic with stylized folds,
— midground: [ELEMENTO DE CONTEXTO: stone ledge with scrolls / rustic wooden table / iron gate],
— background: dark ancient stone walls with visible cracks and deep dramatic shadows, oppressive enclosed space with no sky visible,
single oil lamp casting amber side light, high-contrast chiaroscuro lighting,
felt-tip pen ink illustration style, premium hand-drawn comic book aesthetic,
coarse textured warm beige paper background (#E8D5B0) with visible organic fiber flecks and sand grain texture,
thick bold hand-drawn black ink outlines with subtle organic imperfections,
soft charcoal shading and warm gradients for rich volumetric depth,
color accent rule: [OBJETO PRINCIPAL] in golden yellow (#C9A84C) — main accent,
dramatic amber oil lamp light (#E67E22) — secondary accent,
everything else in bold black ink outlines on textured warm beige,
massive bold red text that says "[TEXTO DE CHOQUE: ERROR / DEUDA]" dominating the center,
all elements within the 20%–80% vertical safe zone
```

**Reglas de Oro del Primer Frame (Visual Hook — Detener el Scroll):**

> ⛔ **GRAFICAR LA ASFIXIA (Mostrar el Dolor, NO la Cura):** Esta es la única imagen de todo el video donde NUNCA se ilustra la mayordomía bíblica ni la solución. El Visual Hook (0-3s) DEBE mostrar angustia financiera cruda. Para todas las imágenes posteriores del interior del video, sí se ilustra la sabiduría de Dios.

> 📊 *Patrón comprobado en analíticas: Short con primer frame optimizado = 1,145 vistas vs 226 vistas (5x de rendimiento). El primer frame detiene el scroll, no el audio.*

*   **Regla 1 — Shock corporal, NUNCA reposo:** El personaje debe mostrar reacción física violenta: retroceder, agarrarse el pecho, soltar algo, inclinarse hacia atrás. NUNCA parado recto, sonriendo, caminando tranquilo ni con las manos a los lados. Prompt obligatorio: `body recoiling backward in shock, eyebrows shot up in alarm, mouth slightly open, one hand pressing against chest`.
*   **Regla 2 — Fondo CERRADO y oscuro (Nunca exterior abierto):** Muros de piedra, cueva, habitación con una sola antorcha. NUNCA desierto, cielo visible, paisaje abierto ni exterior soleado. Prompt obligatorio: `dark enclosed stone walls, oppressive space, no sky, no open landscape, no horizon line`.
*   **Regla 3 — Zona Segura Vertical (20%–80%):** La UI de YouTube tapa el 20% inferior. Todo elemento relevante (cara, objeto clave) debe estar en la zona central de la pantalla.
*   **Regla 4 — Texto de ruptura en CapCut (No descriptivo):** Por regla general, el texto no describe el video, golpea una contradicción o herida (ej: `JESÚS LO CONDENÓ` o `ORASTE AÑOS Y SIGUES IGUAL`). Nunca colocar una referencia vacía (ej. "Proverbios 22"). El texto se aplica en CapCut, **excepto en la primerísima imagen del video** donde el texto de choque SÍ va embebido directamente en el prompt de DALL-E (ver "Regla de ORO de Texto: La Excepción del Primer Segundo" más abajo).
*   **Regla 5 — Color de Ruptura en el texto (solo CapCut):** La palabra más perturbadora del texto superpuesto debe ir en un color de ruptura que rompa el patrón visual del feed: rosa intenso (`#FF2D78`), rojo vivo (`#FF3333`) o naranja neón (`#FF6B00`). El resto del texto va en blanco o negro bold. Este color NUNCA va dentro del prompt de DALL-E, solo en la edición de CapCut.

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
Middle Eastern biblical setting, Latin Mediterranean skin tones,
expressive characters with detailed surrounding environment,
Kurzgesagt-inspired style meets biblical manuscript art,
high contrast, storytelling mood, no text
```

> **NOTA SOBRE EL COLOR (ESTILO B):** Aunque este estilo usa una paleta distinta, **aplica la misma regla de minimalismo de color**. El dorado y ocre deben reservarse para elementos simbólicos o luz, no para bañar toda la escena.

**Ejemplo de Prompt real (Estilo B):**
> *A young merchant counting silver coins on a dark wooden table in a busy marketplace under warm torchlight, — midground: clay jars, fabrics, and baskets of grain, — background: sandstone arches and palm trees under a deep navy night sky, 2D flat illustration, warm cinematic lighting, rich layered scene with foreground midground and background depth, deep navy and ochre color palette, golden accents, Middle Eastern biblical setting, Latin Mediterranean skin tones, expressive characters with detailed surrounding environment, Kurzgesagt-inspired style meets biblical manuscript art, high contrast, storytelling mood, no text*

---

## Tabla de prompts — formato de entrega obligatorio

Entregar SIEMPRE en una sola tabla unificada — una fila por imagen, sin excepciones:

| Bloque | Prompt imagen (DALL-E 3) | Prompt video (Kling/Runway) | Prioridad Video | Animación CapCut | Texto en pantalla | Prioridad Texto |
|--------|--------------------------|-----------------------------|--------------|------------------|-------------------|-----------------|
| **00:00–00:03** | (prompt completo de fondo según estilo A o B elegido) | N/A (Solo texto inicial) | OPCIONAL | Entrada: Zoom rápido / Salida: Fade | PARA DEUDORES | IDEAL (Visual Hook) |
| **00:03–00:06** | (prompt completo con personaje) | Fast push-in camera, character violently recoils backward dropping the scroll, heavy dust floating in the air, dramatic flickering amber light | RECOMENDADO | Entrada: Flash Blur / Salida: Wipe-L | ¿Llevas años en quiebra? | RECOMENDADO |
| **00:06–00:10** | (prompt completo de crisis) | Shaky handheld camera, heavy red chains forcefully wrapping around the figure, dust particles violently swirling | RECOMENDADO | Entrada: Shaky Lens / Salida: Wipe-Down | La deuda te atrapa | OPCIONAL |

### ⛔ REGLA DE ORO DE TEXTO: LA EXCEPCIÓN DEL PRIMER SEGUNDO
Por regla general, las imágenes generadas por DALL-E 3 deben venir **totalmente limpias de texto** (incluyendo la directiva `no text` al final del prompt) porque la IA suele tener faltas de ortografía en español. El texto normal se superpone en CapCut.

**LA ÚNICA EXCEPCIÓN:** La primerísima imagen del video (Bloque 00:00–00:03) **SÍ DEBE LLEVAR TEXTO**. El prompt de DALL-E para esta primera imagen debe incluir explícitamente la orden de integrar el "Primer Segundo de Choque" gigante y en rojo directamente en la ilustración (ej. "huge bold red text that says 'ERROR' dominating the center"). Para todas las demás imágenes del video, aplica la regla de `no text`.

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

| Tipo de escena | Entrada (IN) | Salida (OUT) | Combo |
|---------------|-------------|-------------|-------|
| Hook / impacto emocional | Flash Blur | Dark Wipe-L | Flash Shot |
| Enseñanza / revelación | Fade In | Dark Wipe-L | Swing Slide |
| Crisis / decisión | Forceful Pull | Dark Wipe-Up | Dynamic Shake |
| Transformación / esperanza | Slide Up | Vision Shrink | Bounce Up |
| Deuda / trampa | Shaky Lens | Dark Wipe-Down | Jelly Resistance |
| Familia / empatía | Fade-In Wipe | Vision Shrink | Bouncy Pan |
| Cierre / CTA (Interruptor de Velocidad) | Forceful Pull | Dark Wipe-Up | Dynamic Shake |
| Giro / revelación dramática | Flash Flip-In | Slice Shrink | Grid Spin |
| Tensión acumulada | Wavy Wash-Up | Dark Wipe-Up | Wave Amplification |

## Fuentes de recursos

| Recurso | Uso |
|---------|-----|
| MixKit | SFX y efectos de transición — gratuito, arsenal principal |
| Coverr | Videos cinemáticos en bucle para fondos (opcional) |
