# Producción — Títulos, Miniaturas y Metadatos (El Empaque)

Skill para creación de títulos, miniaturas y metadatos.

> ⛔ **REGLA DE CONFIANZA DEL CABALLO DE TROYA:** Para que la estrategia funcione, el espectador no debe sentirse engañado al hacer clic, sino iluminado al ver el contenido.

---

## 1. La Arquitectura del Título (El Vehículo)

El título no es un resumen teológico del video. Es el agravio personal o la queja financiera que le sirve de vehículo al espectador para entrar.

- **Fórmula de Disonancia Bíblica (NUEVA REGLA MAESTRA):** Las palabras como *"Jesús", "Biblia", "Dios"* ESTÁN PERMITIDAS EXCLUSIVAMENTE si se usan para romper una creencia establecida y generar shock (ej. "Jesús condenó al hombre prudente").
- **Disonancia Específica (Stop Stack):** Aplica la Regla de Disonancia Específica de `guion-clean.md` (JAMÁS atacar conceptos abstractos, DEBE atacar acciones físicas del espectador).
- **La Regla de Oro (Prioridad Izquierda):** *El shock va primero, la explicación va después.* La Disonancia Bíblica o la Power Word DEBEN estar en la extrema izquierda del título (las primeras 3 palabras). Si lo pones al final, la interfaz lo cortará.
- **Ataque al Dolor y "Stakes" (Urgencia):** El título debe implicar que el espectador está perdiendo algo AHORA. (Ej. "Por qué tu ahorro se está pudriendo" > "Cómo ahorrar").
- **El "Tú" Directo:** Usa la segunda persona obligatoriamente ("Tu", "Tus", "Te"). El canal es un diálogo confrontacional.
- **Power Words (OBLIGATORIO):** TODO título debe contener al menos una Power Word de nuestra matriz (código, sistema, condenó, decodificar, 3.000 años).
- **Frases Muertas (BLACKLIST):** PROHIBIDO usar frases quemadas ("La respuesta te sorprenderá", "El secreto de...").
- **Hashtags:** NUNCA usar hashtags (#) en el título. Desperdician espacio valioso y van en la descripción.
- **Regla de Longitud (40 Caracteres para Shorts):** En Shorts, el gancho principal y la disonancia DEBEN estar en los primeros 35-40 caracteres, porque YouTube corta el resto o lo tapa. Para videos largos, máximo 50-60 caracteres.

### Análisis de Referencias (Antes vs Después)

Para entender la diferencia entre un título "religioso" genérico y uno optimizado para CTR, usa esta matriz:

| Título Religioso (PROHIBIDO) | Título Optimizado | Razón del Cambio |
|-----------------------------|-------------------|------------------|
| "¿Oras por dinero pero sigues igual?" | "La razón por la que tus oraciones no pagan tus deudas" | **Story-led:** Cambia una pregunta abstracta por un síntoma externo específico y doloroso. |
| "¿Dios quiere que seas pobre? La respuesta te sorprenderá" | "Jesús condenó al hombre prudente" | **Disonancia Bíblica:** Usa a Jesús para romper el cerebro ("condenó la prudencia"), no para dar un sermón predecible. Elimina la frase muerta. |
| "¿Por qué le vendieron sus hermanos?" | "Cómo detectar la envidia antes de que destruya tu negocio" | **News-jacking:** Empaqueta un relato bíblico como un manual de supervivencia empresarial moderna. |

---

## 2. La Arquitectura de la Miniatura (El Empaque Visual)

La miniatura no repite el título; **amplifica su emoción**.

- **Identidad Innegociable:** Todas las miniaturas deben ejecutarse estrictamente bajo el **Estilo "Codex" (Manuscrito Da Vinci)**. Personajes stick-figure, trazos de tinta negra gruesa e intensa, montados siempre sobre un fondo beige texturizado (`#E8D5B0`).
- **Graficar la Asfixia (Mostrar el Dolor, NO la Cura):** La imagen JAMÁS debe mostrar elementos religiosos. Debe ilustrar visualmente el estrés, la deuda, o la trampa del sistema actual.
- **Regla de No-Repetición (Título vs. Miniatura):** La miniatura genera la *Emoción*, el título da el *Contexto*. Queda estrictamente prohibido que el texto de la imagen y el título digan lo mismo.
  - *Ejemplo correcto:* Miniatura: Imagen de un bolsillo roto + Texto "Vaciado". Título: "El sistema que drena tus ahorros sin que te des cuenta (3,000 años)".
- **Texto de Impacto:** Máximo 2 a 4 palabras gigantes que amplifiquen el sentimiento, NUNCA que lo repitan.

### Prompt Base para DALL-E (Miniaturas 16:9)

```text
A highly legible YouTube thumbnail in a 16:9 aspect ratio.
Style: Da Vinci manuscript "Codex" fused with Latin American comic style.
Color Palette: Textured warm beige background (#E8D5B0), thick and intense black ink outlines, single spot color (amber or gold) for emphasis.
Scene: [Describe the Pain/Asphyxia. E.g. A stick-figure character holding a broken hourglass dropping gold coins].
Typography: The text "[Insert 2-4 Impact Words]" in massive, bold, distressed red or black letters taking up at least 30% of the space on the left or right side for extreme readability on mobile devices.
Rule: Zero religious symbols. Zero 3D renders. 100% hand-drawn ink aesthetic.
```

> 📌 **Reglas de delineado, color semántico, modos de iluminación y estructura de planos** del Estilo Codex están en `produccion-imagen.md`. Si necesitas un prompt más elaborado o con iluminación de tensión (Modo Contraste Alto), consultar ese archivo.

---

## 3. Arquitectura de Metadatos y Algoritmo

No desperdicies los metadatos del video. Son herramientas críticas para el algoritmo.

- **Descripción (Los Primeros 150-200 Caracteres):** Es la parte visible antes de que el usuario tenga que presionar "Mostrar más". Aquí DEBE ir tu palabra clave principal y un gancho fuerte que refuerce el agravio del título.
- **Hashtags (En Descripción):** Máximo 3 hashtags estratégicos al final de la descripción.
- **Sistema de Etiquetas (Tags) de 3 Niveles:** La IA siempre debe generar:
  1.  **Específicas del video (3-4):** tema exacto (ej. "parábola de los talentos", "inflación").
  2.  **Específicas del nicho (3-4):** sector (ej. "finanzas personales", "educación financiera bíblica").
  3.  **Amplias (2-3):** genéricas (ej. "shorts", "viral", "dinero").
- **Protocolo de Resurrección (Shorts):** Si un Short no pasa de las 100 vistas en sus primeros dos días (48h), el algoritmo no lo captó. Se debe borrar, cambiar el título (manteniendo la Disonancia Bíblica), y resubir otro día.

---

## Formato de Entrega y Checklist de Empaque

Cuando el usuario pida empaquetar un video, SIEMPRE debes entregar tu respuesta en este formato:

1.  **Tres (3) opciones completas de Empaque** en formato de tabla. Cada opción debe incluir:
    *   **Título del video** (Aplicando Disonancia Bíblica, Power Words, sin hashtags, y Máx 40 caracteres para Shorts o 60 para largos).
    *   **Texto de Impacto** para la miniatura (2 a 4 palabras gigantes).
    *   **Concepto visual** breve de la miniatura (Graficar la asfixia).

2.  **Bloque de Metadatos:**
    *   Un párrafo de 150-200 caracteres con la palabra clave y el gancho fuerte.
    *   3 Hashtags estratégicos.
    *   Etiquetas en los 3 niveles requeridos.

3.  **Prompt de DALL-E:** Después de que el usuario elija su opción favorita, genera el prompt en inglés usando el **Prompt Base para DALL-E (Miniaturas 16:9)**.

**Checklist Final (Validar antes de sugerir opciones):**
*   [ ] ¿La Disonancia Bíblica o Power Word está en las primeras 3 palabras (Prioridad Izquierda)?
*   [ ] ¿El título implica "Urgencia o Pérdida" e incluye el "Tú" directo?
*   [ ] ¿El título NO contiene hashtags ni Frases Muertas?
*   [ ] ¿El gancho de Shorts está en los primeros 35-40 caracteres?
*   [ ] ¿La miniatura y el título NO repiten la misma frase (Emoción vs Contexto)?
*   [ ] ¿Las miniaturas omiten la solución bíblica y muestran solo la "Asfixia"?
*   [ ] ¿La descripción usa lenguaje de calle y dolor real en lugar de "jerga bancaria fría"?
*   [ ] ¿El empaque total (título + miniatura) supera el Filtro de WhatsApp (es altamente compartible)?
*   [ ] ¿Se generaron las etiquetas en 3 niveles (Específicas, Nicho, Amplias)?
