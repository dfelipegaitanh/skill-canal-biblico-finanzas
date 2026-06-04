# Empaque, Títulos y Miniaturas (Packaging)

**Propósito:** Este módulo rige la creación visual de las miniaturas y la redacción de títulos. En este canal, la miniatura no es "clickbait"; es la portada de un manual antiguo que contiene un secreto.

## 1. La Regla del Enigma Técnico
La miniatura nunca debe explicar o resumir el video (eso mata la curiosidad). Debe mostrar un "enigma" o una fricción técnica irresoluble a simple vista.
*Ejemplo:* Si el video es sobre el Rey Salomón y la deuda, la miniatura no es Salomón sonriendo; es una corona rota sobre un contrato, con un sello rojo.

## 2. Los 3 Pilares de la Miniatura de Autoridad
La IA debe estructurar sus propuestas visuales respetando estos pilares:

### Pilar 1: El Ancla (Punto Focal)
*   Debe ser un **objeto icónico** del grabado (ej: una balanza, una bolsa de monedas, un sello, una cadena, un rollo sagrado).
*   Debe ocupar el 50-70% del encuadre.
*   **Prohibición Absoluta:** Cero rostros genéricos expresivos o de youtubers gritando. Si hay presencia humana, deben ser las manos interactuando con el objeto.

### Pilar 2: Color de Ruptura (Semántica)
*   El 90% de la miniatura debe ser Sepia/Grabado.
*   El elemento clave (el enigma o el dolor) debe brillar usando UNO de los colores de la Tabla Semántica definida en `guidelines/visual_style.md` (ej. **Rojo** para deuda/trampa, **Dorado** para riqueza/sistema).
*   **Prohibición Absoluta:** Prohibido usar "magenta genérico" o neones estridentes tipo gaming/clickbait.

### Pilar 3: La Tipografía (El Código)
*   **Límite Estricto:** Máximo 3 palabras.
*   **Formato:** Sans-serif, pesada, contorno grueso. Debe ser legible en 160px (pantalla de celular).
*   **Prohibición Absoluta:** Nunca repetir el título del video en la imagen. El texto de la miniatura complementa el título.

---

## 3. Redacción de Títulos (Disonancia Bíblica)
El título NO es descriptivo, es un secuestro de atención.
*   **Formato Pregunta (OBLIGATORIO):** Absolutamente TODOS los títulos deben formularse como una pregunta. DEBEN empezar con una palabra interrogativa (¿Por qué...?, ¿Cómo...?, ¿Qué...?, ¿De qué...?, ¿Dónde...?, ¿Cuándo...?). Prohibidos los títulos afirmativos.
*   **Personaje Bíblico Inmediato:** El personaje bíblico debe ir justo después de la palabra interrogativa para no perder el enganche (ej. "¿Por qué Jesús condenó tu ahorro?").
*   **El "Tú" Directo y el Dolor:** Usa la segunda persona ("Tu", "Tus", "Te"). El título debe implicar que el espectador está perdiendo algo AHORA.
*   **Power Words:** Debe contener una Power Word (código, sistema, decodificar, condenó, 3.000 años).
*   **Longitud:** Máximo 40 caracteres para Shorts (porque YouTube lo corta). Máximo 60 para largos. Cero hashtags.

### **SEIS (6) OPCIONES DE TÍTULOS (Ordenadas por Viralidad)**
> ⚠️ **NOTA:** La siguiente tabla es solo un ejemplo de formato. El orden de las palabras interrogativas (Por qué, Cómo, Qué, etc.) NO es estricto ni secuencial. La IA debe evaluar cuál título tiene mayor potencial de disonancia y ordenarlos puramente por su Nivel de Viralidad, independientemente de con qué palabra empiecen.

| Opción | Título (Disonancia Bíblica) | Explicación del porqué | Viralidad |
|--------|-----------------------------|------------------------|-----------|
| 1 | [Ej. ¿Qué...? / ¿Cómo...?] | Breve justificación... | 🔥🔥🔥🔥🔥 |
| 2 | [Ej. ¿Por qué...?] | Breve justificación... | 🔥🔥🔥🔥 |
| 3 | [Ej. ¿Dónde...?] | Breve justificación... | 🔥🔥🔥 |
| 4 | [Ej. ¿De qué...?] | Breve justificación... | 🔥🔥 |
| 5 | [Ej. ¿Cuándo...?] | Breve justificación... | 🔥 |
| 6 | [Ej. ¿Qué...?] | Breve justificación... | 🧊 |

---

## 4. Formato de Salida Obligatorio (Empaque Completo)
Cuando el usuario pida empaquetar un video, la IA debe entregar el siguiente bloque:

**METADATOS Y SEO**
*   **Descripción Corta:** [150-200 caracteres enfocados en el dolor y la disonancia]
*   **Hashtags:** `#Keyword1 #Keyword2 #Keyword3`
*   **Etiquetas Categorizadas:**
    *   *Específicas:* [3-4 tags del tema]
    *   *Nicho:* [3-4 tags del sector]
    *   *Amplias:* [2-3 tags generales]
*   **Bloque de Etiquetas (Copy-Paste):** `[Todas las etiquetas anteriores separadas por comas en un solo bloque continuo]`

**MINIATURA Y PROMPT (DALL-E)**
*   🧠 **Concepto Visual (El Enigma):** `(Breve descripción de la imagen que grafique la asfixia o el enigma basado en la Opción 1 de los Títulos)`
*   📝 **Texto en Pantalla (Overlay):** `"[MÁXIMO 3 PALABRAS EN ROJO O DORADO]"`
*   🖼️ **Prompt DALL-E:** `(El prompt exacto en inglés para generar el concepto visual, cruzando los 3 Pilares con el Estilo Codex. Asegúrate de incluir el objeto focal dominando el 50-70% del encuadre, SIN texto embebido en la imagen)`
