# Producción — Títulos, Miniaturas y Metadatos (El Empaque)

Skill para creación de títulos, miniaturas y metadatos.

> ⛔ **REGLA DE CONFIANZA DEL CABALLO DE TROYA:** Para que la estrategia funcione, el espectador no debe sentirse engañado al hacer clic, sino iluminado al ver el contenido.

---

## 1. La Arquitectura del Título (El Vehículo)


- **La Fórmula Maestra (3 Bloques):** `[Personaje Bíblico / Concepto de Shock] | [Keyword Long-Tail Secular] | [Power Word]`.
    * **Bloque 1 (Izquierda):** El "gancho de autoridad". Debe ser la disonancia cognitiva o el personaje bíblico que rompe creencias. Es el ancla de CTR.
    * **Bloque 2 (Centro):** El dolor secular (lo que el usuario busca). Aquí metemos el SEO.
    * **Bloque 3 (Derecha):** El Power Word o indicador de urgencia.
- **Reglas de Hierro:**
    * **Prioridad absoluta:** El shock/personaje SIEMPRE va primero (izquierda). Si el keyword no cabe sin sacrificar el gancho, el keyword se mueve a la segunda parte o se sacrifica. CTR > SEO.
    * **Longitud:** 50-60 caracteres máximo.
    * **Prohibido:** Hashtags, frases de clickbait barato (ej: "No creerás lo que pasó"), jerga motivacional ("sueños", "bendición").
    * **Disonancia:** Usar términos religiosos SÓLO para atacar, no para predicar (ej: "Jesús condenó al prudente").
    * **Carácter especial:** Usar siempre `|` para separar bloques.

### Análisis de Referencias (Antes vs Después)

Para entender la diferencia entre un título "religioso" genérico y uno optimizado para CTR, usa esta matriz:

| Intención | Título Anterior (Prohibido) | Nuevo Título (SOP) |
|-----------|-----------------------------|--------------------|
| Deuda | Cómo salir de deudas rápido | Salomón \| Cómo pagar deudas hoy \| Sistema |
| Inflación | La Biblia y la economía | Jesús \| Sobrevive a la inflación \| Código |
| Ahorro | ¿Es malo ahorrar dinero? | El Siervo Malo \| Por qué tu ahorro es pérdida \| 3,000 años |

---

## 2. La Arquitectura de la Miniatura (El Empaque Visual)

La miniatura no repite el título; **amplifica su emoción**.

- **Identidad Innegociable:** Todas las miniaturas deben ejecutarse estrictamente bajo el **Estilo "Codex" (Manuscrito Da Vinci)**. Personajes stick-figure, trazos de tinta negra gruesa e intensa, montados siempre sobre un fondo beige texturizado (`#E8D5B0`).
- **Graficar la Asfixia (Mostrar el Dolor, NO la Cura):** La imagen JAMÁS debe mostrar elementos religiosos. Debe ilustrar visualmente el estrés, la deuda, o la trampa del sistema actual.
- **Regla de No-Repetición (Título vs. Miniatura):** La miniatura genera la *Emoción*, el título da el *Contexto*. Queda estrictamente prohibido que el texto de la imagen y el título digan lo mismo.
  - *Ejemplo correcto:* Miniatura: Imagen de un bolsillo roto + Texto "Vaciado". Título: "El sistema que drena tus ahorros sin que te des cuenta (3,000 años)".
- **Texto de Impacto (Priorizar Trauma):** Máximo 2 a 4 palabras gigantes que ataquen la identidad o herencia del espectador (ej. \"NO HEREDASTE POBREZA\", \"ESTÁS PROGRAMADO\"). NUNCA repetir el título.

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
  3.  **Amplias de Nicho (Long-Tails) (2-3):** PROHIBIDO usar buzzwords inútiles como "shorts", "viral" o "dinero". Usa frases amplias pero ancladas a la temática (ej. "educación financiera cristiana", "biblia y dinero", "prosperidad biblica").
- **Protocolo de Resurrección (Shorts):** Si un Short no pasa de las 100 vistas en sus primeros dos días (48h), el algoritmo no lo captó. Se debe borrar, cambiar el título (manteniendo la Disonancia Bíblica), y resubir otro día.

---

## Formato de Entrega y Checklist de Empaque

Cuando el usuario pida empaquetar un video, SIEMPRE debes entregar tu respuesta en este formato y orden estricto:

1.  **Definir el Término de Búsqueda (SEO):** Antes de generar opciones, la IA debe declarar explícitamente cuál es el dolor secular que la gente está buscando en YouTube en relación al video (ej. *"Término Objetivo SEO: Cómo ganarle a la inflación"*).

2.  **Cinco (5) opciones completas de Empaque** en formato de tabla. Cada opción debe incluir:
    *   **Título del video (Híbrido)** (Aplicando la Fórmula Maestra de 3 bloques: `[Personaje Bíblico] | [Keyword SEO] | [Power Word]`).
    *   **Texto de Impacto** para la miniatura (2 a 4 palabras gigantes).
    *   **Concepto visual** breve de la miniatura (Graficar la asfixia).

3.  **Bloque de Metadatos:**
    *   Un párrafo de 150-200 caracteres con la palabra clave y el gancho fuerte.
    *   3 Hashtags estratégicos.
    *   Etiquetas en los 3 niveles requeridos.

3.  **Prompt de DALL-E:** Después de que el usuario elija su opción favorita, genera el prompt en inglés usando el **Prompt Base para DALL-E (Miniaturas 16:9)**.

**Checklist Final (Validar antes de sugerir opciones):**
*   [ ] ¿El título empieza con una figura bíblica o una declaración que rompe creencias?
*   [ ] ¿Incluye un Power Word obligatorio (Código, Sistema, Bolsillo vacío, 3,000 años, Decodificar)?
*   [ ] ¿El dolor secular está incluido para captar tráfico de búsqueda (SEO)?
*   [ ] ¿Cumple los 50-60 caracteres?
*   [ ] ¿Sustituiste el separador por `|` entre bloques?
*   [ ] ¿La miniatura y el título NO repiten la misma frase (Emoción vs Contexto)?
*   [ ] ¿Las miniaturas omiten la solución bíblica y muestran solo la "Asfixia"?
*   [ ] ¿La descripción usa lenguaje de calle (sin jerga financiera de banco) y dolor real?
*   [ ] ¿El empaque total (título + miniatura) supera el Filtro de WhatsApp (es altamente compartible)?
*   [ ] ¿Se generaron las etiquetas en 3 niveles (Específicas, Nicho, Amplias)?
