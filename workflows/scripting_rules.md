# Reglas de Escritura de Guiones (Partitura Audio-Visual)

**IMPORTANTE:** Olvida la prosa literaria tradicional. En este canal, el guion es una **partitura técnica** donde el audio y la imagen se sincronizan a nivel de keyframes. El guion dicta el movimiento.

## 1. La Regla de los 5 Segundos (El Reloj)
*   **Prohibido escribir párrafos.** Escribe en "bloques de respiración".
*   El audio es el reloj que marca el cambio. Si una frase o bloque de audio tarda más de 5 segundos en leerse en voz alta, estás **obligado** a cortarla y añadir un nuevo bloque `[Visual: ...]` para forzar un cambio de plano (zoom, paneo o corte).
*   Si la imagen se queda quieta por más de 5 segundos, la autoridad se evapora.

## 2. Keyframe Scripting (Formato Obligatorio)
La salida (output) del guion debe seguir estrictamente este formato de bloque y comando visual:

```
[Fase]: "Texto que se dirá en la locución. Frases contundentes."
[Visual: Comando de imagen exacto]
```

### Ejemplos de redacción:
✅ **Correcto (Rítmico y visual):**
`Hook: "¿Sigues pagando intereses? El sistema de 3.000 años no usaba bancos. Era capital directo."`
`[Visual: Plano fijo grabado sepia, personaje sosteniendo un contrato en magenta. Zoom lentísimo]`

❌ **Incorrecto (Prosa, mata la imagen):**
*"Mucha gente sigue pagando intereses mes a mes sin darse cuenta de que el sistema financiero bíblico no operaba bajo los principios..."*

## 3. Integración Visual Directa (Estilo Codex)
Los corchetes `[Visual: ...]` no deben ser descripciones vagas. Deben ser **comandos directos** que respeten nuestro estilo *Codex (Manuscrito Da Vinci)* para que funcionen como prompts casi listos.
*   **La paleta es la frontera:** Utiliza sepia/gris para representar el "pasado/ancestral/autoridad" y **Magenta** para el "presente/dolor/foco".
*   **Magenta como puntuación:** Usa el color magenta en el prompt visual exclusivamente para marcar un cambio técnico (ej: un contrato, una balanza, una moneda).
*   **Consistencia de trazo:** Incluso al mostrar tablas financieras modernas, el visual debe forzar la estética de grabado antiguo (`[Visual: Tabla contable estilo grabado antiguo...]`). Nunca elementos estilo Excel moderno.

## 4. Instrucción Suprema para la IA
Al escribir el guion, **no estás creando un texto, estás ejecutando un sistema de información**. Asegúrate de que el impacto de cada frase corta haga que el cambio de imagen propuesto se sienta absolutamente inevitable.
