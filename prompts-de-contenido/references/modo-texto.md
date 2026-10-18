# Modo de texto — ¿los títulos van en la imagen o aparte?

Decisión que se pregunta **justo antes de generar los prompts** (y se confirma de pasada si ya quedó
claro). Define cómo se maneja el texto visible de la pieza. Es importante porque los generadores de
imagen pueden dañar el texto, sobre todo los precios y los textos pequeños. En los tres modos el texto
se escribe en **español correcto, con tildes, Ñ y mayúsculas acentuadas** (`corrector-espanol.md`):
nunca se quitan las tildes para "evitar errores".

## ⚠️ Importante: los COPYS siempre los propone la skill

El modo de texto decide **dónde va** el texto, **no si lo escribes**. En los tres modos, **tú siempre
sugieres los copys** como copywriter: titular gancho, bajada y CTA, apoyados en el nicho/tendencia y en
la promesa del producto. Si la persona solo dio el **precio** (o nada), **tú propones el resto del
texto** y se lo presentas para que apruebe o ajuste — nunca la dejes inventando los títulos. La persona
aporta datos duros (precio, promo, claim propio si lo tiene); el copy que vende lo pones tú.

## Las 3 opciones (ofrécelas tal cual)

**A · Prompts SIN texto (lo más seguro para precios y textos pequeños).**
La imagen se genera **limpia** (sin títulos), y entregas aparte una **hoja de texto lista para Canva**:
qué dice cada texto (ya pasado por el corrector), en qué fuente (combo de `tipografia.md`),
tamaño/jerarquía, color (HEX de la paleta) y posición sugerida. La persona pega los textos en Canva y
quedan perfectos, consistentes y con los precios bien escritos. Es lo más confiable.

**B · Prompts CON texto en la imagen.**
El prompt le pide al generador que **incluya el texto** en el lugar indicado, en español correcto, con
el bloque **SPANISH TEXT — EXACT RENDERING** de `corrector-espanol.md` (cada texto entre comillas, con
tildes y Ñ, deletreo de las palabras con tilde, precio dígito por dígito, "NO misspelled words. NO
missing accents. NO extra text.") y dentro del **límite de líneas** de la pieza. Es el modo de las piezas
de marca (logo, tablero, empaques). Advierte con honestidad que el generador puede fallar en alguna
letra: se revisa letra por letra y se corrige con el prompt de corrección, no quitando tildes. **Actúa como
diseñador gráfico profesional** al dirigir la composición del texto (ver `diseno-tipografico.md`):
jerarquía, ubicación, alineación, aire y relación con el producto.

**C · Que Claude arme la pieza final (overlay).**
Claude compone la pieza final **como diseñador gráfico profesional**: la imagen generada como fondo + el
texto encima con las fuentes exactas, maquetado con jerarquía, grid y buen gusto (carga `artifact-design`
y `frontend-design`; ver `diseno-tipografico.md`). Es un diseño/artifact HTML que la persona exporta.
Honestidad: **no hay conector directo a Canva**, así que Claude no maneja Canva por dentro; hace el
montaje él mismo (overlay) o entrega la hoja de texto de la opción A. Requiere que la persona comparta la
imagen ya generada.

## Regla

- Pregunta esto una vez, antes de generar; aplica la misma decisión a toda la campaña para que sea
  consistente.
- Por defecto, si la persona no decide y la pieza lleva **precio o textos pequeños**, usa **A** (sin
  texto + hoja Canva). En la ruta de marca (logo, tablero, empaques) el texto va en la imagen (**B**),
  con el corrector.
- En **A**, entrega SIEMPRE la hoja de texto: por cada pieza → textos exactos + fuente + color HEX +
  posición. Es lo que convierte "imagen limpia" en "pieza lista para montar en minutos".
- En **B**, los prompts llevan el texto dentro con el bloque SPANISH TEXT — EXACT RENDERING.
- Los generadores con mejor render de texto (ChatGPT imagen, Gemini Nano Banana Pro, Ideogram) manejan
  bien textos cortos en español; aun así, nunca garantices precios perfectos y revisa siempre letra por
  letra.
