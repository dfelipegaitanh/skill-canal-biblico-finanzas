# Protocolo de Auditoría de Guiones — Obligatorio al revisar un guión existente

> ⛔ **REGLA DURA:** Cuando el usuario pida revisar, auditar o mejorar un guión ya escrito (o ya grabado), NUNCA responder con un bloque de texto libre. Ejecutar este protocolo completo.

## Paso 0 — Bypass de Auditoría (Reescritura Directa)

> ⚠️ **BYPASS:** Si el usuario pide **exclusivamente** reescritura sin diagnóstico (ej. *"reescríbelo"*, *"ponlo más humano"*, *"sin tanta verborrea"*), la IA debe saltarse la evaluación paso a paso y pasar directamente a la solución. Si el usuario pide *"revisa"* o *"audita"*, ejecutar la auditoría completa (Pasos 1-5) Y entregar el guion corregido al final.

> ⛔ **REGLA DE REESCRITURA OBLIGATORIA:** Siempre que la IA proponga reescribir un bloque de texto o el guion completo (sea por Bypass o por Fix), DEBE cargar y aplicar estrictamente las reglas definidas en `references/guion-reglas-obligatorias.md`, más el módulo de formato correspondiente (`guion-reglas-shorts.md` o `guion-reglas-largo.md`).

En ese caso, la IA **DEBE ENTREGAR EXACTAMENTE DOS COSAS:**
1. **El Guion Completo Corregido:** Aplicando la regla de reescritura, el español neutral y eliminando la verborrea.
2. **Tabla de Cambios Quirúrgicos:** Inmediatamente después del guion, una tabla clara que documente qué cambió y por qué.

**Formato exigido para este atajo:**
[Guion en Markdown]

**Cambios Aplicados:**
| Qué se eliminó/cambió | Nueva versión | Por qué (Regla aplicada) |
|---|---|---|
| *(Frase original)* | *(Frase nueva)* | *(Ej. Síndrome del Púlpito / Filtro de WhatsApp)* |

## Paso 1 — Checkpoints de Supervivencia y Clasificación

Antes de llenar la tabla, verificar estas reglas de oro generales:
1. **Primer Segundo de Choque:** ¿El segundo 0 al 1 tiene texto gigante rojo (ej. ERROR, DEUDA) o imagen chocante? Si hay un arranque hablado pasivo → **Error Crítico**.
2. **Gancho Letal (Power Words en Shorts):** ¿El hook combina una palabra de *Síntoma* (deuda, cuenta en rojo, estancamiento) con una de *Autoridad* (Código, Sistema, 3.000 años)? Si falta alguna de las dos o no hay ninguna → **Error Crítico** (el algoritmo no clasificará el dolor ni la solución).
3. **Disonancia Bíblica vs. Caballo de Troya (Empaque):** Evaluar las 3 condiciones por separado:
   - 3a: ¿Las palabras religiosas en los primeros 3s generan shock/disonancia (ej. "Jesús condenó al hombre prudente")? → **CORRECTO**.
   - 3b: ¿Se usan de forma genérica que suena a sermón (ej. "Dios quiere prosperarte")? → **Error Crítico** (mata el CTR).
   - 3c: ¿El gancho NO usa disonancia y tampoco se ancla en un dolor secular masivo (deuda, bancos)? → **Error Crítico** (falta hook).
4. **Límite de Palabras (Shorts):** ¿El guión supera el presupuesto (60 para Micro-Short, 150 para estándar)? Si sí, durará más de la retención meta → **Error Crítico** (exigir recortes).
5. **PROHIBICIÓN TÉCNICA (Lenguaje de Calle):** ¿El guion usa jerga financiera de banco (ej. CDT, ETF, Inflación, Tasa de Interés, CAT) o términos complejos? Si es así → **Error Crítico INMEDIATO**. La IA DEBE reescribir la frase usando lenguaje 100% humano, visceral y de la calle (ej. cambiar "CDT al 5%" por "un lugar seguro que te pague intereses"). Si suena a profesor de economía, el guion fracasa.
6. **Diagnóstico del Síndrome del Púlpito:** ¿El narrador usa preguntas retóricas de iglesia abstractas, muletillas condescendientes ("Y mira...", "Aquí está el sistema"), o suena a un pastor regañando desde un altar en lugar de un amigo en el barro? Si es así → **Error Crítico** (exigir reescritura en español neutral, hiper-eficiente, directo y desde la frustración de las trincheras).
7. **Regla de la Sola Fuente:** ¿El guion cita un solo versículo/pasaje para exprimir su ingeniería, o salta disparando múltiples versículos de distintos libros como si fuera un sermón probatorio? Si usa más de una fuente bíblica principal → **Error Crítico** (borrar las secundarias y exprimir la principal).
8. **Bucle Parasocial (Personalidad y Vulnerabilidad):** ¿El guion expone la frustración/personalidad del creador hablando en primera persona ("Yo también fui al banco...", "Mi cuenta estaba en rojo") o usa datos crudos y específicos ("el banco te cobra casi el doble"), o es solo un relato distante de hechos? Si el guion es plano, no opina y no tiene vulnerabilidad → **Error Crítico** (no retendrá para un video #2).
9. **El Filtro de WhatsApp (Métrica Share):** ¿El CTA o el tono general del video provoca que el espectador quiera compartirlo? (Ej. "Mándale esto a tu amigo que sigue endeudado"). ¿Se siente como un video que enviarías a un familiar quebrado? Si el guion no es "compartible" o el CTA solo pide likes aburridos → **Error Crítico** (cambiar el CTA y el tono para fomentar el Share).
10. **Ingeniería Financiera vs. Escuela Dominical:** Si el guion menciona a un personaje bíblico, ¿lo trata como un "Ingeniero Financiero" (ej. José como creador del Fondo de Reserva) o relata un cuento bíblico tradicional ("Dios lo bendijo")? Si relata la historia como escuela dominical en lugar de traducir su perfil a Wall Street → **Error Crítico** (reescribir usando la Matriz de Ingenieros Financieros).

### Checkpoints de Empaque (si el usuario también proporcionó título/miniatura)
11. **Hashtags en el Título:** ¿El título tiene hashtags (#)? Si es así → **Error Crítico** (moverlos a la descripción).
12. **Power Words en el Título:** ¿El título contiene al menos 1 Power Word de la matriz? Si no → **Error Crítico**.
13. **Frases Muertas:** ¿El título usa una frase quemada ("La respuesta te sorprenderá", "No vas a creer")? Si es así → **Error Crítico**.

### Auditoría Estricta para Videos Largos (+3 minutos)
Si el guion a revisar es para un video largo, sumar estas verificaciones a la lista anterior:
14. **Micro-CTA Temprano (Pilar 3):** ¿El guion pide suscripción justo después del primer "mind-blow" (Pilar 2)? Si lo omite o lo pone demasiado tarde → **Error Crítico**.
15. **Aritmética Brutal (Pilar 6):** ¿Hay números reales y crudos (inflación, deuda, interés) o solo consejos genéricos? Si no hay cifras → **Error Crítico** por sonar a "motivación barata".
16. **Oración de Cierre (Pilar 10):** ¿El guion pide suscripción o like al final? Si lo hace → **Error Crítico**. El Pilar 10 es ÚNICAMENTE la oración de activación + redirección al siguiente video.

## Paso 2 — Herramientas de Reparación (Reglas de "Fixes")

Al momento de proponer la solución para un error, la IA debe aplicar obligatoriamente estas tres herramientas:

### 2.1. Regla "No Regrabar" (Priorizar Post-Producción)
> ⛔ **La primera solución siempre debe ser de post-producción.** Antes de sugerir cambiar el audio o regrabar, proponer arreglarlo con:
> 1. Texto superpuesto en CapCut (overlay desarmador, ejemplo tangible, promesa visual)
> 2. Corte visual o cambio de B-roll (sincronizar la imagen con la emoción del audio)
> 3. Animación en Kling/Runway (movimiento que refuerce la palabra clave)
>
> Solo sugerir regrabar audio si el problema es **estructural** (falta un bloque entero, el orden narrativo está roto, o hay un error teológico).

### 2.2. Regla del "Texto Desarmador" (Anti-Defensividad)
> Cuando el guión lanza una verdad incómoda o confrontacional (ej. "Piden mal", "Dios no te rescató"), el viewer cristiano puede ponerse a la defensiva y cerrar el video.
> **Fix obligatorio:** En la columna "Fix" de la auditoría, proponer un texto en pantalla que **desarme la defensividad** antes de que el espectador procese el juicio del audio.
> | Audio (Confronta) | Texto en pantalla (Desarma) |
> |---|---|
> | "Porque piden mal" | "No es tu culpa. Nadie te enseñó esto." |
> | "Llevas años y sigues igual" | "Y no eres el único." |

### 2.3. Regla Anti-Abstracción
> Si el audio del guión da un concepto abstracto o un mandato vago (ej. "define para qué vas a usar lo que pides"), la auditoría DEBE proponer un texto en pantalla con **3 ejemplos hiper-tangibles** que anclen el concepto inmediatamente.
> | Audio (Abstracto) | Texto en pantalla (Tangible) |
> |---|---|
> | "Escribe para qué usarías eso que pides" | "Ej: pago arriendo, deuda, negocio" |
> | "Invierte lo que Dios te da" | "Ej: curso, herramienta, inventario" |

## Paso 3 — Formato de entrega obligatorio (Tabla por Severidad)

Habiendo evaluado los Checkpoints (Paso 1) y usando las Herramientas de Reparación (Paso 2), entregar SIEMPRE la auditoría en una tabla con este formato exacto, ordenada de mayor a menor severidad:

| Severidad | Timestamp | Área | Problema | Fix (Aplicar Reglas del Paso 2) |
|-----------|-----------|------|----------|---------------------------------|
| **Crítico** | 00:00–00:05 | Hook | (Descripción del problema) | (Solución concreta: ej. Texto desarmador) |
| **Medio** | 00:25–00:29 | Pacing | (Descripción del problema) | (Solución concreta: ej. Corte de B-roll) |
| **Bajo** | 00:40–00:46 | CTA | (Descripción del problema) | (Solución concreta) |

**Definiciones de Severidad:**
- **Crítico:** Mata la retención o el Share. El viewer hace swipe/cierra el video en ese punto.
- **Medio:** Aburre o confunde por unos segundos. No mata pero debilita.
- **Bajo:** Se puede mejorar, pero el video funciona sin el fix.

## Paso 4 — Auditoría Analítica (Diagnóstico YouTube Studio)

Si el usuario proporciona métricas reales de un video publicado, DEBES diagnosticar la falla algorítmica. Si NO proporciona métricas, omitir este paso y pasar al Veredicto Final.
- **Alta Impresión + Bajo CTR:** El título o la miniatura fallaron. Recomendar un cambio urgente priorizando alto contraste visual y el **Gancho Bíblico (Personaje) a la izquierda** (CTR | SEO).
- **Alto CTR + Baja Retención inicial (caída brusca en primeros 30s):** Fuerte desconexión. La promesa del empaque (Caballo de Troya) no coincide con los primeros segundos del video, o la intro fue demasiado lenta. Hay que reempaquetar o cortar la intro desde el editor de YouTube.

## Paso 5 — Veredicto Final

Cerrar siempre la auditoría con un bloque de veredicto que incluya:
1. Qué funciona bien (no todo es negativo)
2. Cuántos fixes son de post-producción vs regrabar
3. Tiempo estimado de implementación en CapCut
4. Si los fixes pueden impactar significativamente la retención o las compartidas (Shares)
