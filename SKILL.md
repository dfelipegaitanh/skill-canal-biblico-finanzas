---
name: canal-biblico-finanzas
description: Skill especializado para construir y operar el canal de YouTube "Código Bíblico del Dinero". Úsalo siempre que el usuario hable de su canal de YouTube bíblico-financiero en español, pida guiones, prompts de imagen o voz, o cualquier tarea de producción del canal. Si el usuario NO da contexto suficiente, cargar onboarding.md.
---

# Canal Bíblico de Finanzas — Skill Master

## Identidad del canal

**Nombre:** Código Bíblico del Dinero | **Handle:** @CodigoBiblicoDelDinero

**Propuesta de valor:** El canal que decodifica el sistema financiero de la Biblia y lo aplica a la realidad económica latinoamericana — sin teología de prosperidad, sin promesas vacías.

**Nicho:** Canal largo en español sobre finanzas bíblicas animadas + Shorts diarios como palanca de crecimiento.

**Audiencia:** Cristiano latinoamericano 28–45 años, con fe genuina y bolsillo vacío. Busca el puente entre su fe y su realidad financiera. 80%+ celular, horario nocturno. Vocabulario clave: "el Señor proveerá", "declaro abundancia", "en el nombre de Jesús", "diezmo", "cosecha", "prosperidad".

**Tono:** Confrontacional-empático. Como un amigo que sabe algo que necesitas escuchar y te dice la verdad en la cara con frustración compartida. NO predicador, NO coach motivacional, NO profesor condescendiente, NO tecnicismos financieros, NO jerga bíblica.

**Principio maestro:** La gente no sigue contenido. Sigue cómo ese contenido los hace sentir. Crea para la emoción, edita para la retención.

**Manifiesto de la Mayordomía (El Interior):** Cero tolerancia hacia la teología de la prosperidad. El miedo es el pecado financiero original. Tratamos la Biblia como un manual de estrategia geopolítica y personal, no como cuentos de hadas. No vendemos milagros; vendemos una arquitectura mental.

**Estrategia Macro (Caballo de Troya y Disonancia Bíblica):** Empaque ataca dolor secular. Palabras religiosas PERMITIDAS EXCLUSIVAMENTE si rompen creencias y generan shock (ej. "Jesús condenó al prudente"). Prohibido el sermón genérico.

**Estilos visuales:**
- **A) Estilo "Codex" (Manuscrito Da Vinci)** (default) — 100% personajes stick-figure, trazos de tinta negra gruesa e intensa, fondo beige texturizado `#E8D5B0`. Contra-señal visual a la basura 3D genérica.
- **B) Kurzgesagt bíblico** — 2D flat, azul noche + dorado.

---

## Referencias — cuándo cargar cada una

| Tarea solicitada | Cargar (Máx. 1 módulo) |
|-----------------|-------------------------|
| Títulos, Miniaturas y Metadatos SEO (El Empaque) | `references/produccion-empaque.md` |
| Guiones nuevos, estructura narrativa, hooks, shorts o guión largo | `references/guion-reglas-obligatorias.md` (+ `references/guion-reglas-shorts.md` o `references/guion-reglas-largo.md`) |
| Revisar, auditar o mejorar un guión existente | `references/auditoria-guion.md` |
| Prompts de imagen, animación visual | `references/produccion-imagen.md` |
| Generación de voz, música, audio | `references/produccion-voz.md` |
| Threads | `references/produccion-threads.md` |
| Sin contexto claro, onboarding o primer contacto | `references/onboarding.md` |

**Regla:** Cargar SOLO la referencia que aplica (máximo 1 archivo a la vez). Nunca cargar todas.

---

## Comportamiento general y Protocolo de Fallback

- **Validación de Rutas e Incertidumbre:** Si el archivo modular no existe o la petición del usuario es ambigua/vaga, no intentar adivinar. Cargar *únicamente* `references/onboarding.md` como fallback y hacer UNA sola pregunta con opciones claras antes de continuar.
- **Para Guiones:** Siempre ejecutar el protocolo de arranque de `references/guion-clean.md` antes de redactar cualquier escena.
- **Ajuste de Género:** Por defecto, NO usar lenguaje inclusivo. **Excepción:** si el tema corresponde al segmento femenino, virar el lenguaje hacia el público femenino de forma directa. En caso de duda, usar el default masculino.
- **Algoritmo (Frecuencia y Calentamiento):** La frecuencia máxima de publicación es 1 Short al día. Antes de publicar, la cuenta debe "calentarse" consumiendo e interactuando en videos de finanzas para validar humanidad ante YouTube.
- **Cierre:** Siempre proponer el siguiente paso lógico de la producción del canal al finalizar.
