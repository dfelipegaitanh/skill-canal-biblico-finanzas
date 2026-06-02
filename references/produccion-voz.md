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
- Cómo suena el narrador (urgente, intenso, ágil — amigo que te advierte de un peligro inminente)
- El arco emocional bloque por bloque (manteniendo siempre alta energía y tensión)
- Las pausas críticas explícitas — enfocarse en la pausa obligatoria de 1 segundo
- Qué NO debe hacer la voz (PROHIBIDO hablar lento, relajado, calmado o como un locutor de meditación)

**TEXT**
El guión completo en español, de corrido, con etiquetas de emoción intercaladas. Sin títulos de bloque, sin separadores. Solo el texto que se narra.

---

### Etiquetas de emoción para el campo TEXT

| Etiqueta | Cuándo usarla |
|----------|---------------|
| `[somber]` | Momentos graves, peso emocional, diagnóstico duro |
| `[urgent]` | Ritmo rápido, advertencia inminente, no hay tiempo |
| `[warm]` | Empatía, conexión, "te entiendo" |
| `[intense]` | Fuerza sin gritar, confrontación directa |
| `[emphatic]` | El golpe clave, la frase que más importa |
| `[sharp]` | Cortante, directo al punto, revelación cruda |
| `[fast]` | Velocidad máxima, avalancha de datos técnicos |

#### Pausas

Usar `,` o `.` para marcar micropausas de respiración naturales.
NO usar la etiqueta `[pause]`, ni `...` ni ningun otro recurso para marcar pausas.

**Identidad del Narrador y Configuración de Voz:**
- **El Tono Exacto:** Hombre, voz medio-grave. Tono según SKILL.md (Confrontacional-empático). **NO es un predicador, NO es un coach motivacional.** El tono es de autoridad técnica pero empático.
- **Velocidad:** **Fast-Pace estricto (110–115% de velocidad natural).** Ritmo ágil, urgente y fluido. No hay tiempo para respirar, el espectador debe sentir que la revelación lo asfixia hasta la pausa.
- **Shorts:** Duración estricta de **15–20 segundos** para Micro-Shorts (presupuesto **50–60 palabras**) o **50–60 segundos** para Shorts estándar (presupuesto **máximo 150 palabras**). 
- **Videos largos:** Duración de 5–20 minutos. **OBLIGATORIO FRAGMENTAR:** Para evitar que la IA de voz colapse por exceso de texto, el guion largo DEBE entregarse dividido en bloques lógicos (ej. agrupando 2 o 3 Pilares por bloque). Cada bloque debe entregarse como un prompt de voz independiente con su propia estructura completa.

### Formato de entrega

```text
[BLOQUE 1 - Pilares 1 al 3] (Solo necesario si es video largo)

SCENE
[Descripción cinematográfica en inglés del arco visual completo.]

SAMPLE CONTEXT
[Descripción del viewer, narrador con tono urgente, arco emocional con alta energía,
las pausas críticas y la instrucción explícita: "urgent delivery, fast-paced pacing, no slow meditation".]

TEXT
[Guión completo en español con etiquetas de emoción. De corrido. Sin separadores.]

---
*(Si es un video largo, repetir esta estructura exacta para el BLOQUE 2, BLOQUE 3, etc.)*
```

---

## Prompt de música de fondo

> ⚠️ Generar DESPUÉS de tener el guión cuadrado. Sin el guión no se sabe el arco emocional.

### Identidad sonora del canal

**Estilo base:** Acústico cálido — guitarra española o clásica como instrumento principal, piano suave o cuerdas de fondo opcionales.

**Regla absoluta: siempre instrumental.** La música NUNCA tiene voces, coros ni samples vocales. Quedan excluidos los beats de hip-hop/trap, la electrónica prominente, la percusión fuerte, los tempos rápidos (+100 BPM) y los ritmos tristes, pesados o dramáticos. La instrumentación debe ser armoniosa, dejando a la voz del narrador como el único elemento vocal del video.  La música debe ser tensa e incómoda UNICAMENTE al inicio del video.

---

### Arco global por tipo de video

| Tipo de video | Dynamic arc |
|--------------|-------------|
| Short de impacto emocional | starts with sharp uncomfortable tension, quickly drops to calm, brief resolution at the end |
| Short de revelación bíblica | starts with uncomfortable tension, quickly transitions to calm, subtle crescendo in the middle, soft resolution |
| Video largo de enseñanza | starts with uncomfortable tension, transitions to calm and warm, maintains steady low energy, gentle fade out |
| Video largo con giro dramático | starts with sharp uncomfortable tension, drops to minimal in the middle, subtle crescendo before close, clean resolution |
| Video de esperanza / transformación | starts with uncomfortable tension, quickly transitions to contemplative, gradually becomes warmer and brighter |

### Mood por bloque interno (videos largos)
*(Los nombres de los pilares están definidos en `guion-reglas-largo.md`)*

| Pilar del guion | Mood musical |
|-----------------|--------------|
| 1. El Contraste de Avatares (Intro) | Tensión contenida — nota sostenida o arpeggio lento |
| 2. El Secreto Mal Interpretado | Peso emocional — tempo lento, acordes menores |
| 3. Micro-CTA Algoritmo (Temprano) | Disrupción breve — subida rítmica corta |
| 4. El Arquitecto Bíblico | Autoridad — crescendo progresivo de intensidad |
| 5. Contexto Histórico / Secular | Documental — cuerdas amplias, tempo estable |
| 6. La Aritmética Brutal a 10 Años | Tensión matemática — crescendo con peso |
| 7. La Escalera de Acción Práctica | Esperanza activa — acordes mayores, tempo estable |
| 8. El Principio del Descanso (Shabbat) | Calma reflexiva — guitarra suave, tempo íntimo |
| 9. El Plan de Acción a 7 Días | Urgencia controlada — ritmo firme |
| 10. La Oración de Activación (Cierre) | Resolución — nota final limpia, fade out natural |

---

### Prompt base de música

```text
Acoustic instrumental music for a Spanish-language YouTube channel
about biblical principles and personal finance for Latin American Christians aged 28–45.

Mood: starts tense and uncomfortable for the first 5 seconds, then strictly transitions into [INSERTAR: contemplative / hopeful / warm / reflective] and remains highly harmonious
Tempo: slow to mid — between 55 and 75 BPM
Instruments: classical or Spanish acoustic guitar as the main instrument,
optionally supported by soft piano or gentle strings in the background.
Exclusions: strictly no vocals or choirs of any kind, no hip-hop/trap beats,
no electronic elements, no heavy percussion or drums, 
no sad, heavy, or dramatic rhythms AFTER the first 5 seconds.
Texture: intimate, warm, and highly harmonious (after initial tension) — like a private conversation, not a concert
Dynamic arc: [INSERTAR desde tabla de arco global]
Style references: background music in documentaries about spirituality or personal growth,
clean mix, no reverb excess, suitable to play under a narrator's voice at 15–20% volume
```
