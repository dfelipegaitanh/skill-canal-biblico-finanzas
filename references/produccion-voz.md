# Producción — Voz y Música

## Sistema de generación de voz — Google AI Studio

El output se entrega en **un solo bloque con 3 campos**. El usuario lo copia completo y lo pega directamente.

---

### Los 3 campos del bloque único

**SCENE**
Describe en inglés el arco visual completo del video — todas las escenas en orden, de corrido. Qué aparece en pantalla, qué texto aparece superpuesto, qué hace cada personaje, cómo evoluciona el mood visual de inicio a fin. Extenso y cinematográfico. El arco visual siempre sigue al guión, no lo contradice.

**SAMPLE CONTEXT**
Describe en inglés al viewer, el arco emocional del video completo, el tono del narrador y las pausas críticas. Incluye:
- Quién es el viewer (edad, situación emocional, qué carga)
- Cómo suena el narrador (no predicador, no coach — amigo que sabe algo)
- El arco emocional bloque por bloque
- Las pausas críticas explícitas — qué frases deben respirar y por qué
- Qué NO debe hacer la voz

**TEXT**
El guión completo en español, de corrido, con etiquetas de emoción intercaladas. Sin títulos de bloque, sin separadores. Solo el texto que se narra.

---

### Etiquetas de emoción para el campo TEXT

| Etiqueta | Cuándo usarla |
|----------|---------------|
| `[somber]` | Momentos graves, peso emocional, diagnóstico duro |
| `[calm]` | Explicaciones, transiciones, credibilidad |
| `[warm]` | Empatía, conexión, "te entiendo" |
| `[serious]` | Afirmaciones directas, condenas bíblicas |
| `[emphatic]` | El golpe clave, la frase que más importa |
| `[soft]` | Íntimo, casi susurro, reflexión profunda |
| `[measured]` | Cada palabra pesa, ritmo deliberado |

#### Pausas

Usar `,` o `.` para marcar micropausas de respiración naturales.
NO usar la etiqueta `[pause]`, ni `...` ni ningun otro recurso para marcar pausas.

**Identidad del Narrador y Configuración de Voz:**
- **El Tono Exacto:** Hombre, voz medio-grave. Tono según SKILL.md (Confrontacional-empático). **NO es un predicador, NO es un coach motivacional.** El tono es de autoridad técnica pero empático.
- **Velocidad:** Ritmo deliberado, 85–90% de la velocidad natural de habla humano (pausado, con peso). Las palabras clave deben tener peso.
- **Shorts:** Duración estricta de **15–20 segundos** para Micro-Shorts (presupuesto **50–60 palabras**) o **50–60 segundos** para Shorts estándar (presupuesto **máximo 150 palabras**). 
- **Videos largos:** Duración de 5–20 minutos.

### Formato de entrega

```
SCENE
[Descripción cinematográfica en inglés del arco visual completo.]

SAMPLE CONTEXT
[Descripción del viewer, el narrador, el arco emocional bloque por bloque,
las pausas críticas con sus frases exactas, y lo que la voz NO debe hacer.]

TEXT
[Guión completo en español con etiquetas de emoción. De corrido. Sin separadores.]
```

---

## Prompt de música de fondo

> ⚠️ Generar DESPUÉS de tener el guión cuadrado. Sin el guión no se sabe el arco emocional.

### Identidad sonora del canal

**Estilo base:** Acústico cálido — guitarra española o clásica como instrumento principal, piano suave o cuerdas de fondo opcionales.

**Regla absoluta: siempre instrumental.** La música NUNCA tiene voces, coros ni samples vocales. Quedan excluidos los beats de hip-hop/trap, la electrónica prominente, la percusión fuerte, los tempos rápidos (+100 BPM) y los ritmos tristes, pesados o dramáticos. La instrumentación debe ser armoniosa, dejando a la voz del narrador como el único elemento vocal del video.

---

### Arco global por tipo de video

| Tipo de video | Dynamic arc |
|--------------|-------------|
| Short de impacto emocional | starts with tension, brief resolution at the end |
| Short de revelación bíblica | starts calm, subtle crescendo in the middle, soft resolution |
| Video largo de enseñanza | starts calm and warm, maintains steady low energy, gentle fade out |
| Video largo con giro dramático | starts with mild tension, drops to minimal in the middle, subtle crescendo before close, clean resolution |
| Video de esperanza / transformación | starts contemplative, gradually becomes warmer and brighter, ends with hopeful resolution |

### Mood por bloque interno (videos largos)
*(Nota: Los nombres de los pilares están definidos en guion-reglas-largo.md)*

| Pilar del guion | Mood musical |
|-----------------|--------------|
| 1. El Gancho de Herida | Tensión contenida — nota sostenida o arpeggio lento |
| 2. La Autopsia Bíblica | Peso emocional — tempo lento, acordes menores |
| 3. Micro-CTA de Algoritmo | Disrupción — subida rítmica breve |
| 4. Aritmética Brutal | Autoridad y crescendo — subida progresiva de intensidad |
| 5. El Puente Emocional | Empatía — acordes mayores suaves, tempo íntimo |
| 6. Escalera de Acción | Esperanza activa — acordes mayores, tempo estable |
| 7. CTA de Trascendencia | Resolución — nota final limpia, fade out natural |

---

### Prompt base de música

```
Acoustic instrumental music for a Spanish-language YouTube channel
about biblical principles and personal finance for Latin American Christians aged 28–45.

Mood: [INSERTAR: contemplative / hopeful / tense / warm / reflective] — must remain harmonious
Tempo: slow to mid — between 55 and 75 BPM
Instruments: classical or Spanish acoustic guitar as the main instrument,
optionally supported by soft piano or gentle strings in the background.
Exclusions: strictly no vocals or choirs of any kind, no hip-hop/trap beats,
no electronic elements, no heavy percussion or drums, 
no sad, heavy, or dramatic rhythms.
Texture: intimate, warm, and highly harmonious — like a private conversation, not a concert
Dynamic arc: [INSERTAR desde tabla de arco global]
Style references: background music in documentaries about spirituality or personal growth,
clean mix, no reverb excess, suitable to play under a narrator's voice at 15–20% volume
```

