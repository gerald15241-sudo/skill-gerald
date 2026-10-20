# Ficha de marca bloqueada (BRAND LOCK)

La ficha es el **candado de la marca**. Se genera **en el momento en que la persona aprueba la hoja del
sistema de logo** (paso 3 de la ruta de marca, `estudio-de-marca.md`) y desde ahí se pega **idéntica,
palabra por palabra**, en todos los prompts siguientes: moodboard, tablero de identidad, empaques,
mockups, POP, piezas y correcciones.

Existe porque, sin ella, cada prompt vuelve a describir la marca a su manera y el generador cambia
cosas entre piezas: el origen, el formato de la bolsa, el personaje de la ilustración o la forma del
logo. La ficha evita eso: **una sola fuente de verdad, copiada tal cual**.

## Reglas

1. **Cuándo nace:** al aprobar la hoja del sistema de logo. Nunca antes: sin logo aprobado no hay
   ficha, y sin ficha no hay moodboard, tablero ni empaques.
2. **Nada se inventa.** Cada campo sale de algo aprobado o dicho por la persona. Si falta un dato
   (formato del empaque, altitud, proceso, notas…), **pregúntalo antes de cerrar la ficha**, con
   botones cuando se pueda. Si la persona no lo sabe o no aplica, el campo dice `NOT USED` y ese dato
   **no aparece en ninguna imagen**. Nunca rellenes con un dato "probable".
3. **Se pega igual en todos los prompts.** Mismo texto, mismo orden, sin resumirla, traducirla ni
   "mejorarla". Va justo después del bloque de imágenes de referencia de cada prompt.
4. **El logo aprobado siempre se adjunta.** Todo prompt posterior al paso 3 lleva
   `@imagen 1 = logo aprobado, versión limpia` y su línea 📎. Sin excepción.
5. **Solo cambia si la persona lo pide.** Si quiere ajustar algo (un color, un dato, el formato), se
   emite la ficha completa en una **versión nueva** (v2, v3…), se dice qué cambió y desde ahí se usa
   solo la nueva. Nunca se edita "un poquito" dentro de un prompt suelto.
6. **Lo que no está en la ficha no existe.** Si un prompt necesita un texto, un color o un dato que no
   está en la ficha, primero se agrega a la ficha (con aprobación) y después se usa.

## Orden fijo de imágenes en la ruta de marca

Para que no haya confusión entre prompts, las imágenes se adjuntan siempre en este orden:

- `@imagen 1` = **logo aprobado, versión limpia** (ronda 3 de `logos-profesionales.md`). Siempre.
- `@imagen 2` = **personaje o ilustración aprobada**, solo si la marca tiene uno y ya fue aprobado.
- Las siguientes = lo propio de cada prompt (hoja del sistema de logo, moodboard aprobado, foto del
  producto, foto del local…), en el orden que diga ese prompt.

Si la marca no tiene personaje, las imágenes propias del prompt empiezan en `@imagen 2`.

## Personaje e ilustración (el candado que más se rompe)

- Si la marca lleva ilustración o personaje, su **estilo** (técnica, trazo, nivel de detalle, colores)
  y su **descripción exacta** (qué es, rasgos, pose base, ropa o accesorios, proporciones) van en la
  ficha desde la v1, aunque todavía no exista la imagen.
- La primera vez que el personaje aparece aprobado en una imagen (normalmente en el moodboard del
  paso 5), se emite la ficha v2 con esa imagen como `@imagen 2` fija. Desde ahí, el personaje **se
  copia de la imagen, nunca se redibuja** por descripción.
- Prohibido en todos los prompts: cambiar su especie, edad, rasgos, ropa, colores o estilo de trazo.

## Formato del empaque

Se define **antes de cerrar la ficha** si la marca tiene producto físico: tipo (doypack con fuelle,
bolsa de fondo plano, caja, lata, frasco…), tamaño o peso, acabado (mate, brillante, kraft), cierre,
válvula, ventana y dónde va la etiqueta. Una vez en la ficha, **todas las piezas usan ese mismo
formato**. Las variedades cambian solo lo que la ficha dice que cambia (color de la bolsa, nombre y
datos de la variedad).

## Plantilla de la ficha (en inglés; los textos visibles en español, con tildes y Ñ)

Entrégala en el chat en un bloque de código, después de un resumen de 3–4 líneas en español para la
persona. Rellena cada corchete; lo que no aplique queda `NOT USED`.

```
BRAND LOCK — "[BRAND NAME]" — v[N] — COPY EXACTLY, DO NOT ALTER
Apply every item below exactly as written. Do not reinterpret, simplify, translate or improve it.

BRAND NAME: "[BRAND NAME]", spelled [L-E-T-T-E-R-S] ([N] letters). Descriptor: "[DESCRIPTOR or NOT USED]".

LOGO: @imagen 1 is the EXACT approved logo. [Architecture: wordmark / monogram + wordmark / emblem…]. [Exact letterform description: weight, width, contrast, case, tracking]. [Device or symbol: exact description]. Colors: [#HEX] on [#HEX]. Reproduce it identically on every piece, adapted only to the printing technique of each material. Never redraw, restyle, recolor outside the palette or invent a provisional logo.

COLORS (only these, by role):
- Background: [NAME] [#HEX]
- Typography: [NAME] [#HEX]
- Accent: [NAME] [#HEX]
- Hero (product only): [NAME] [#HEX]
- [Extra role]: [NAME] [#HEX]
No other colors anywhere.

TYPOGRAPHY: headlines in [letterform description, in the style of FREE FONT]; body text in [description, in the style of FREE FONT]; small labels in [description, in the style of FREE FONT].

ILLUSTRATION STYLE: [technique, line weight, level of detail, colors from the palette — or NOT USED].
CHARACTER: [exact description: what it is, features, base pose, clothing/accessories, proportions — or NOT USED]. [From v2: @imagen 2 is the EXACT approved character; copy it, never redraw it.] Never change its species, features, clothing, colors or line style.

PACKAGING FORMAT: [type], [size/weight], [finish], [closure], [valve], [window], label on [position]. The same format on every piece and every variety. [What changes per variety: e.g. bag color only].

FIXED PRODUCT DATA (texts appear exactly as written, only on the pieces that need them):
- REF 1 "[VARIETY NAME]": origin "[ORIGIN]" · variety "[VARIETY]" · altitude "[ALTITUDE]" · process "[PROCESS]" · notes "[NOTES]" · weight "[WEIGHT]" · bag color [#HEX]
- REF 2 "[VARIETY NAME]": origin "[…]" · variety "[…]" · altitude "[…]" · process "[…]" · notes "[…]" · weight "[…]" · bag color [#HEX]
Never mix data between references. Never change a value.

APPROVED SPANISH TEXTS (the only texts allowed in images): "[TEXT 1]", "[TEXT 2]", "[TEXT 3]"…

NEVER: a different or provisional logo, colors outside the palette, a different packaging format, a different character, changed product data, missing accents or Ñ, extra text.
```

Los campos de FIXED PRODUCT DATA se adaptan al producto (café: origen, variedad, altitud, proceso,
notas; galletas: sabor, ingredientes, peso; cosmética: activo, tipo de piel, contenido). Lo que no
cambia es la regla: **cada dato se escribe una vez en la ficha y se copia igual siempre**.

Ejemplo de cómo se ven los datos de una referencia de café (ilustrativo, no es un valor por defecto):

```
- REF 1 "GEISHA": origin "NARIÑO, COLOMBIA" · variety "GEISHA" · altitude "2.100 msnm" · process "LAVADO" · notes "JAZMÍN, DURAZNO, MIEL" · weight "250 g" · bag color #2F4A3A
```

## Cómo se usa dentro de cada prompt

```
REFERENCE IMAGES — MANDATORY:
@imagen 1 is the EXACT approved logo […].
[@imagen 2 …]

[BRAND LOCK pegado completo, tal cual]

[Resto del prompt: escena, composición, SPANISH TEXT — EXACT RENDERING, materiales, cámara, NO…]
```
📎 Adjunta en tu generador: @imagen 1 = logo aprobado (versión limpia) · [las demás]

El bloque de texto en español de cada prompt (`corrector-espanol.md`) **solo puede usar textos que
estén en APPROVED SPANISH TEXTS o en FIXED PRODUCT DATA**, escritos carácter por carácter igual.

## Revisión antes de entregar cualquier prompt de marca

- ¿Lleva el BRAND LOCK completo, en su última versión, sin cambios?
- ¿`@imagen 1` es el logo aprobado y está en la línea 📎?
- ¿Cada dato de producto coincide carácter por carácter con la ficha y con la referencia correcta?
- ¿El formato del empaque y el personaje son los de la ficha?
- ¿Algún texto, color o dato no está en la ficha? Si sí, para y pídele aprobación para agregarlo.
