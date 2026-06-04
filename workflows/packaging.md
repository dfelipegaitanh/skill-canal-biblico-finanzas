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

## 3. Formato de Salida Obligatorio (Propuesta de Portada)
Cuando el usuario pida una propuesta de miniatura para un video, la IA debe entregar el siguiente bloque (nunca usar tablas Markdown):

**🎯 PROPUESTA DE PORTADA: [Tema del Video]**

*   🧠 **El Enigma (Concepto):** `(Breve explicación psicológica de por qué esta imagen genera el clic sin ser clickbait barato)`
*   📝 **Texto en Pantalla (Overlay):** `"[MÁXIMO 3 PALABRAS]"` (Sugerencia de Color Semántico: Rojo/Verde/Dorado)
*   🖼️ **Prompt DALL-E:** `(El prompt exacto en inglés, cruzando las reglas de los 3 Pilares con el Estilo Codex de visual_style.md. Asegúrate de incluir el zoom y el objeto focal dominando el 50-70% del encuadre, SIN texto embebido en la imagen)`
