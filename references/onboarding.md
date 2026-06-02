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
> - 🧵 Crear un Hilo de Threads para promocionar un video
> - 📊 Diagnosticar métricas de un video publicado

## Paso 2 — Según lo que elija, hacer la pregunta específica que falta

**Si elige GUIÓN (video largo):**
→ "¿Cuál es el tema o la idea del video?"
→ "¿Duración objetivo?" (opciones: 8 min / 12 min / 15 min)
→ Seguir el protocolo de `guion-reglas-obligatorias.md` + `guion-reglas-largo.md` y ejecutar

**Si elige SHORT:**
→ "¿Cuál es el tema o el gancho central?"
→ Seguir el protocolo de `guion-reglas-obligatorias.md` + `guion-reglas-shorts.md` y ejecutar

**Si no dice qué tipo de video:**
→ Asumir el formato de SHORT, por defecto

**Si elige EMPAQUE (Títulos y Miniaturas):**
→ "¿De qué trata el video para el cual haremos el empaque?"
→ Seguir el protocolo de `produccion-empaque.md` y ejecutar

**Si elige PROMPTS:**
→ "¿Tienes el guión con timestamps listo?"
→ Si sí: "¿Necesitas prompts de imagen o de voz?"
  → Voz: seguir el protocolo de `produccion-voz.md`
  → Imagen: seguir el protocolo de `produccion-imagen.md` (Estilo Codex)
→ Si no: "Necesito el guión con timestamps primero. ¿Lo tienes o arrancamos por ahí?" (Mientras el guion no tenga timestamps, no se pueden generar prompts de imagen)

**Si elige AUDITAR un guión:**
→ "¿El guión es para Short o para video largo?"
→ "Compárteme el guión completo o el link del video publicado."
→ Seguir el protocolo de `auditoria-guion.md` completo (Pasos 0 al 5).

**Si elige DIAGNOSTICAR métricas:**
→ "Pásame el CTR, Retención y vistas del video."
→ Seguir el protocolo de `auditoria-guion.md` Paso 4 (Auditoría Analítica).

**Si elige RESUCITAR SHORT:**
→ "¿Cuál es el tema del Short que tiene menos de 100 vistas en sus primeras 48 horas?"
→ Seguir el protocolo de `produccion-empaque.md` y generar un nuevo empaque (Título con Disonancia Bíblica + Miniatura Asfixia) para resubirlo.

**Si elige THREADS:**
→ "Pásame el tema principal del video o el guión que quieres promocionar."
→ Seguir el protocolo de `produccion-threads.md` y generar el Hilo de 3 posts (Conflicto + Ruptura + Invitación).

## Paso 3 — Siempre cerrar con acción concreta

Nunca terminar una respuesta sin proponer el siguiente paso lógico de producción.

---

## Flujo de Producción Maestro

Este es el pipeline general para crear un video o Short desde cero hasta la publicación.

1. **Tema:** Definir tema y enfoque (ver `onboarding.md`).
2. **Guión:** Cargar `guion-reglas-obligatorias.md` y sumar `guion-reglas-shorts.md` o `guion-reglas-largo.md` según el formato.
3. **Imágenes:** Ver `produccion-imagen.md`.
4. **Audio (Voz y Música):** Ver `produccion-voz.md`.
5. **Empaque (Título, Descripción, Tags y Miniatura):** Ver `produccion-empaque.md`. (Obligatorio aplicar Disonancia Bíblica en Shorts).
6. **Threads:** Ver `produccion-threads.md`.
