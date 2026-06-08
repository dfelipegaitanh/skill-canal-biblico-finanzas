# Guía de Estilo Visual (Exclusivo para formato LONG)

Esta guía establece el estándar visual "Premium Biblical Editorial" para los videos en formato largo (15-30 minutos). El objetivo es mantener una consistencia visual inquebrantable a escala masiva sin fatigar al espectador, controlando estrictamente la continuidad, la cámara y limitando la inventiva de la IA.

## Flujo de Trabajo Obligatorio (Lógica de Generación)

Antes de ensamblar el prompt visual, es **OBLIGATORIO** aplicar la capa lógica de clasificación y traducción para evitar desviaciones.

### Pasos:
1. **Analizar** el texto del guion correspondiente a la escena.
2. **Clasificar** la escena en una de las 5 categorías oficiales.
3. **Traducir** los conceptos abstractos usando la tabla autorizada y seleccionar un objeto de la biblioteca oficial.
4. **Construir** el prompt visual rellenando los templates.

### Las 5 Categorías Narrativas

| Categoría | Uso Principal | Emoción / Atmósfera | Elementos Frecuentes |
| :--- | :--- | :--- | :--- |
| **PARABLE** | Historias y enseñanzas figurativas | Reflexión, curiosidad, asombro | Maestro enseñando, uno o dos oyentes, objeto simbólico principal. |
| **TEACHING** | Explicaciones bíblicas directas | Sabiduría, convicción, calma | Pergaminos, actitud de instrucción, luz cálida. |
| **MONEY** | Dinero, riqueza, ahorro material | Interés, atención, responsabilidad | Monedas, balanzas, bolsas, cofres. |
| **WARNING** | Errores, deudas, codicia, peligro | Preocupación, cautela, arrepentimiento | Bolsas cerradas, contratos rotos. La tensión visual se logra por la postura y arreglo de los objetos, manteniendo la iluminación consistente. |
| **STEWARDSHIP**| Administración responsable, inversión | Humildad, responsabilidad, gratitud | Monedas organizadas, siembra, balanzas. |

### Biblioteca Oficial de Objetos (APPROVED OBJECT LIBRARY)
Para evitar que la IA invente elementos extraños, el foco narrativo (`MAIN FINANCIAL OR PARABLE OBJECT`) debe extraerse estrictamente de esta lista:
* gold coin
* small coin stack
* money pouch
* balance scale
* ancient scroll
* clay jar
* grain sack
* storage chest
* seed bag
* oil lamp
* key

### Regla de Conceptos Abstractos (ABSTRACT CONCEPT RULE)
Cuando el guion hable de conceptos abstractos, conviértelos en una metáfora visual bíblica sencilla antes de insertarlos en el prompt:
* discipline → organized coin stacks
* debt → heavy money pouch / torn contract
* greed → overflowing coin bag
* wisdom → open scroll
* patience → seed bag
* stewardship → balanced scale
* trust → open hand receiving coin

---

## Reglas de Construcción (Los Bloques)

Estos bloques deben ser insertados exactamente como están escritos en el generador de imágenes.

### 1. Personajes y Continuidad
**[CHARACTER_RULE_BIBLICAL_EDITORIAL]**
```text
Character rule: 1 to 3 biblical-era characters interacting naturally within a teaching, financial, or parable-based scene.
Characters use simplified adult proportions with elegant silhouettes and subtle facial features.
Faces are stylized and illustrative rather than realistic:
small expressive eyes,
subtle eyebrows,
minimal facial detail,
no skin pores,
no hyper-realistic anatomy,
no exaggerated cartoon features,
no oversized mascot eyes.
Characters wear simple ancient biblical robes, shawls, sandals, belts, or modest period-appropriate garments.
The primary biblical teacher, storyteller, merchant, steward, king, servant, farmer, debtor, lender, or listener must remain the clear focal point of the image.
Supporting characters are visually secondary and may only reinforce the narrative being explained.
Maximum 3 characters.
Never depict crowds.
Never create complex social scenes.
Character emotions should remain subtle, mature, and readable:
wisdom, reflection, curiosity, concern, conviction, gratitude, regret, responsibility, humility.
Avoid comedy expressions, exaggerated reactions, slapstick poses, childish gestures, or mascot behavior.
```

**[VISUAL_CONTINUITY_RULE]**
```text
VISUAL CONTINUITY RULE:
The same recurring biblical teacher should maintain a consistent visual identity throughout the entire video.
Maintain consistent:
- facial structure
- hairstyle
- beard style
- robe design
- silhouette
- body proportions
- age appearance
Avoid generating a different-looking teacher between scenes.
The viewer should immediately recognize the same teacher across the entire video.
```

### 2. Estilo
**[STYLE_RULE_BIBLICAL_EDITORIAL]**
```text
Premium biblical finance editorial illustration for adult audiences.
Digital watercolor illustration.
Refined ink sketch linework.
Thin elegant outlines.
Subtle watercolor textures.
Minimalist visual storytelling.
Sophisticated educational publishing aesthetic.
Inspired by high-end illustrated books, financial editorials, biblical teaching materials, and premium educational media.
Muted color palette.
Desaturated earth tones.
Warm ivory fabrics.
Aged gold accents.
Soft olive greens.
Terracotta browns.
Dusty blue-gray shadows.
No bright saturated colors.
No neon colors.
No cartoon palettes.
No childish appearance.
Soft natural lighting.
Gentle shadows.
Balanced contrast.
WARNING scenes should increase visual tension through posture, composition, and object arrangement rather than darkness. Maintain the same visual style and lighting consistency.
Extremely clean composition.
Large negative space.
No visual clutter.
No visual noise.
No text.
No letters.
No captions.
No logos.
No watermarks.
```

### 3. Cámara, Composición y Variación
**[CAMERA_RULE]**
```text
CAMERA RULE:
Prefer medium shots and medium-close shots.
Avoid extreme closeups.
Avoid wide cinematic establishing shots.
The characters should remain clearly visible and readable on mobile screens.
```

**[COMPOSITION_RULE_BIBLICAL_EDITORIAL]**
```text
Composition rule:
The main character occupies approximately 60% to 70% of visual attention.
The narrative teaching object occupies approximately 15% to 20% of visual attention.
Supporting characters occupy approximately 10% to 15% of visual attention.
Environmental context occupies approximately 5% to 10% of visual attention.
The viewer's eye must immediately identify:
1. Main teacher or protagonist.
2. Financial or symbolic teaching object.
3. Listener or secondary character.
4. Minimal contextual environment.
Every image must communicate a single idea.
Only one central narrative concept per image.
Avoid multiple competing focal points.
Avoid visual complexity.
Maintain generous negative space around subjects.
```

**[VARIATION_RULE]**
```text
VARIATION RULE:
Alternate between:
teacher explaining
teacher listening
teacher presenting object
teacher walking with listener
teacher showing object
teacher receiving object
teacher observing object
while maintaining overall style consistency.
```

### 4. Entorno
**[ENVIRONMENT_RULE_BIBLICAL_EDITORIAL]**
```text
Environment rule:
The environment is suggested rather than illustrated.
Include only 1 or 2 subtle contextual elements when relevant:
small stone wall section,
simple wooden beam,
market basket,
clay jar,
ancient doorway,
small table,
storage chest,
grain sack,
faint architectural silhouette.
Environmental elements must never compete with the characters.
No detailed cities, no complex architecture, no large temples, no landscapes, no mountains, no forests, no large crowds, no dramatic skies, no highly detailed scenery.
The scene should feel intimate, focused, and instructional.
```

### 5. Regla Exclusiva CTA
**[CTA_VISUAL_RULE]**
```text
CTA VISUAL RULE:
The character occupies approximately 80% of the frame.
Eye contact with the viewer is mandatory.
Background complexity reduced to near zero.
The teaching object is larger than normal scenes.
Slightly stronger contrast than standard scenes.
```

---

## Templates Generadores

### TEMPLATE PRINCIPAL
Se usa para el 99% de las escenas del video. Este template unifica todas las reglas de consistencia para prevenir fatiga visual a gran escala.

```text
[SCENE ACTION OR PARABLE MOMENT]

[CHARACTER_RULE_BIBLICAL_EDITORIAL]
[VISUAL_CONTINUITY_RULE]

— narrative focus: [MAIN FINANCIAL OR PARABLE OBJECT FROM APPROVED LIBRARY]

— supporting narrative element: [OPTIONAL SECONDARY OBJECT OR LISTENER REACTION]

— environmental suggestion: [OPTIONAL MINIMAL CONTEXTUAL ELEMENT]

[CAMERA_RULE]
[VARIATION_RULE]
[COMPOSITION_RULE_BIBLICAL_EDITORIAL]
[ENVIRONMENT_RULE_BIBLICAL_EDITORIAL]
[STYLE_RULE_BIBLICAL_EDITORIAL]
```

### TEMPLATE CTA
Exclusivo para la llamada a la acción (Cierre del video). Rompe la cuarta pared para indicar al espectador que el video está concluyendo.

```text
A biblical teacher directly addressing the viewer with calm authority and conviction.

[CHARACTER_RULE_BIBLICAL_EDITORIAL]
[VISUAL_CONTINUITY_RULE]

The teacher is positioned slightly forward and looking directly into the viewer's eyes.
One hand is gently extended toward the audience as if inviting reflection or action.

— narrative focus: a single [gold coin / ancient scroll / clay jar / balance scale] positioned naturally near the extended hand.

— supporting narrative element: subtle warm light illuminating the teaching object.

— environmental suggestion: faint stone wall or simple interior architectural cue.

[CTA_VISUAL_RULE]
[ENVIRONMENT_RULE_BIBLICAL_EDITORIAL]
[STYLE_RULE_BIBLICAL_EDITORIAL]
```
