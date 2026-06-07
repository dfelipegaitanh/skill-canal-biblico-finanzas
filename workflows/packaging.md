# Empaque, Títulos y Miniaturas (Packaging)

**Propósito:** Este módulo rige la creación conceptual de las miniaturas y la redacción de títulos. En este canal, la miniatura no es "clickbait"; es la portada de un manual antiguo que contiene un secreto.

---

## 1. La Regla del Enigma Técnico
La miniatura nunca debe explicar o resumir el video (eso mata la curiosidad). Debe mostrar un "enigma" o una fricción técnica irresoluble a simple vista.
*Ejemplo:* Si el video es sobre el Rey Salomón y la deuda, la miniatura no es Salomón sonriendo; es una corona rota sobre un contrato o personajes agobiados.

## 2. Los 3 Pilares de la Miniatura (Actualizado)

### Pilar 1: El Foco (Flexibilidad Total)
*   La IA tiene flexibilidad para decidir si la miniatura se centra en **Objetos Metafóricos** (ej. un cofre vacío, un reloj de arena) o en **Personajes** expresando emociones financieras (estrés, liberación).
*   **Regla Estricta de Personajes:** Si usas personajes, no pueden ser humanos realistas. Deben seguir el `[CHARACTER_RULE]` de *stick-figures* (Máximo 3 personajes por imagen).

### Pilar 2: Color de Ruptura (Semántica Obligatoria)
*   El 90% de la miniatura debe tener la estética *Codex* (Sepia/Grabado cálido).
*   El elemento clave (el enigma, el dolor o la solución) debe brillar usando UNO de los Colores Semánticos (Ver `visual_style.md`: **Rojo** para deuda, **Dorado** para riqueza, **Verde** para liberación).
*   **Prohibido:** Neones estridentes o magenta genérico.

### Pilar 3: Regla de Cero Texto Incrustado (CRITICAL)
*   **Prohibición Absoluta:** La IA NO puede redactar promts de imágenes exigiendo palabras escritas (Ej: *Prohibido usar "massive bold text that says 'SECRETO'"*).
*   La única excepción permitida para indicar texto ambiental en la imagen es añadir la frase: `"optional environmental text in Spanish only"`.
*   *(Nota: El texto final para la miniatura será agregado por el editor humano en Canva o Photoshop después).*

---

## 3. Redacción de Títulos (Disonancia Bíblica)
El título NO es descriptivo. Es un secuestro de atención que genera una crisis cognitiva.

### Reglas Fundamentales
*   **Power Words (OBLIGATORIO):** Cada título debe contener al menos una (código, sistema, decodificar, condenó, 3.000 años).
*   **El "Tú" Directo y el Dolor:** Usa segunda persona ("Tu", "Tus", "Te").
*   **Personaje Bíblico:** Va en las primeras 5 palabras. Nunca enterrado al final.
*   **Longitud:** Shorts → máximo 40 caracteres. Largo → máximo 60 caracteres. Cero hashtags.
*   **Keywords long-tail:** Van al extremo izquierdo del título.

### Formatos del Título
Genera opciones de títulos utilizando las siguientes estructuras, priorizando siempre la que genere mayor disonancia:
1.  **Formato A (Pregunta):** `[Interrogativa] + [Personaje Bíblico] + [Dolor directo al "Tú"]` *(Ej: "¿Por qué Jesús condenó tu ahorro?")*
2.  **Formato B (Afirmación):** `[Keyword long-tail] + [Personaje] + [Consecuencia para el "Tú"]` *(Ej: "Jesús condenó al prudente. Y tú eres él.")*

### SEIS (6) OPCIONES DE TÍTULO
Genera siempre 6 versiones. Ordénalas por nivel de viralidad descendente. El orden lo dicta la intensidad de la disonancia, no la gramática.

| Opción | Formato (P/A) | Título (Disonancia Bíblica) | Por qué funciona | Viralidad |
|--------|---------------|-----------------------------|------------------|-----------|
| 1 | [P o A] | [Título] | Justificación breve | 🔥🔥🔥🔥🔥 |
| 2 | [P o A] | [Título] | Justificación breve | 🔥🔥🔥🔥 |
| 3 | [P o A] | [Título] | Justificación breve | 🔥🔥🔥 |
| 4 | [P o A] | [Título] | Justificación breve | 🔥🔥 |
| 5 | [P o A] | [Título] | Justificación breve | 🔥 |
| 6 | [P o A] | [Título] | Justificación breve | 🧊 |
*(P = Pregunta / A = Afirmación Disruptiva)*

> ⛔ **ERRORES QUE INVALIDAN EL TÍTULO AUTOMÁTICAMENTE:**
> *   **Informativo/Descriptivo:** *"El sistema financiero de José en la Biblia"*
> *   **Clickbait sin dolor:** *"El secreto que nadie te contó"*
> *   **Ausencia de Power Word:** *"¿Por qué Moisés manejaba bien el dinero?"*
> *   **Personaje enterrado:** *"¿Cómo manejar tu dinero según José?"*
> *   **Largo excedido:** Más de 40 caracteres en Shorts.
> *   **Hashtags:** `#finanzas #biblia`

---

## 4. El Comentario Fijado (La Ruptura Extendida)
El comentario fijo no es un "gracias por ver". Es la última bala de retención. Debe contener:
1.  **La Ruptura Extendida:** Una frase que profundiza la disonancia del video.
2.  **El Comando de Mapeo:**
    *   **Videos Largos:** SIEMPRE pide comentario ("Comenta tu país 👇 — estoy mapeando dónde está la trinchera.")
    *   **Shorts:** PROHIBIDO pedir "comenta tu país". Usa un CTA de Share.
3.  **El Puente de Autoridad:** Un link al siguiente video.

---

## 5. Formato de Salida Obligatorio (Empaque Completo)
Cuando el usuario pida empaquetar, entrega este bloque:

**1. METADATOS Y SEO**
*   **Descripción Corta:** [150-200 caracteres]
*   **Hashtags / Etiquetas:** [Bloque continuo separado por comas]

**2. MINIATURA (SUGERENCIAS Y PROMPT)**
*   🧠 **Concepto Visual:** [Descripción de la composición]
*   🖼️ **Prompt Visual (DALL-E/Midjourney):** [Prompt en inglés, aplicando la regla de Cero Texto, Máximo 3 Personajes y Color Semántico]
*   ✍️ **Sugerencia de Texto para el Editor:** [1-3 palabras impactantes que el humano debería añadir sobre la imagen final]

**3. TÍTULOS (Las 6 Opciones)**
*   [Tabla con las 6 opciones ordenadas por viralidad]

**4. COMENTARIO FIJADO**
*   [Texto listo para copiar y pegar]
