# Onboarding — Flujo guiado para sesiones sin contexto

Activa este flujo cuando el usuario llegue con frases vagas como "ayúdame con el canal", "dame ideas", o sin especificar qué necesita.

## Paso 1 — Identificar qué quiere hacer

> "Perfecto, estoy listo. ¿Por dónde arrancamos hoy?"
> - 🎬 Crear un guión de video largo
> - 📱 Crear un Short (Micro-Short o estándar)
> - 🖼️ Crear Títulos y Miniaturas (Empaque)
> - 🎨 Prompts de imagen o voz
> - 🔍 Revisar o auditar un guión existente
> - 🔄 Resucitar un Short estancado (<100 vistas)

## Paso 2 — Según lo que elija, hacer la pregunta específica que falta

**Si elige GUIÓN (video largo):**
→ "¿Cuál es el tema o la idea del video?"
→ "¿Duración objetivo?" (opciones: 8 min / 12 min / 15 min)
→ Cargar `guion-clean.md` y ejecutar

**Si elige SHORT:**
→ "¿Cuál es el tema o el gancho central?"
→ Cargar `guion-clean.md` (sección Shorts) y ejecutar

**Si elige EMPAQUE (Títulos y Miniaturas):**
→ "¿De qué trata el video para el cual haremos el empaque?"
→ Cargar `produccion-empaque.md` y ejecutar

**Si elige PROMPTS:**
→ "¿Tienes el guión con timestamps listo?"
→ Si sí: "¿Necesitas prompts de imagen o de voz?"
  → Imagen: preguntar estilo A o B, luego cargar `produccion-imagen.md`
  → Voz: cargar `produccion-voz.md`
→ Si no: "Necesito el guión con timestamps primero. ¿Lo tienes o arrancamos por ahí?"

**Si elige AUDITAR un guión:**
→ "¿El guión es para Short o para video largo?"
→ "Compárteme el guión completo o el link del video publicado."
→ Cargar `auditoria-guion.md` y ejecutar el protocolo completo (Pasos 0 al 7).

**Si elige RESUCITAR SHORT:**
→ "¿Cuál es el tema del Short que tiene menos de 100 vistas en sus primeras 48 horas?"
→ Cargar `produccion-empaque.md` y generar un nuevo empaque (Título con Disonancia Bíblica + Miniatura Asfixia) para resubirlo.

## Paso 3 — Siempre cerrar con acción concreta

Nunca terminar una respuesta sin proponer el siguiente paso.
Ejemplo: "¿Seguimos con el guión o prefieres pasar a los prompts de voz e imagen?"

---

## Flujo de Producción Maestro

Este es el pipeline general para crear un video o Short desde cero hasta la publicación.

1. **Frecuencia Máxima:** 1 Short al día. (No asfixiar el algoritmo).
2. **Guión:** Ver `guion-clean.md` (Micro-Short para canales en fase de crecimiento, Short estándar o video largo según contexto).
3. **Audio (Voz y Música):** Ver `produccion-voz.md`.
4. **Imágenes:** Generar con DALL-E 3 (según estilo y frecuencia detallados en `produccion-imagen.md`).
5. **Empaque (Título, Descripción, Tags y Miniatura):** Ver `produccion-empaque.md`. (Obligatorio aplicar Disonancia Bíblica en Shorts).
6. **Animación:** Kling/Runway (recomendado) o efectos en CapCut.
7. **Edición:** Regla de los 3 segundos sin corte. Orden: Voz → Imágenes → SFX → Música → Texto.
8. **Autenticidad:** B-roll demostrativo (Scholar, noticias, capturas).
