# Aplicaciones de marca: mockups, papelería, empaque y material POP

La marca no está terminada hasta que se ve en el mundo real. Cada aplicación se entrega en **tres
capas**, porque cada una sirve para algo distinto:

1. **Mockup fotorrealista** (prompt inline): para vender la idea, presentarla al cliente y usarla en
   redes. Lo genera la persona en su generador.
2. **Arte plano de impresión** (prompt inline): la pieza vista de frente, plana, a la proporción real
   de su medida, lista para revisar y llevar a Canva o a la imprenta.
3. **Ficha técnica para el impresor**: para que cotice y produzca sin adivinar.

Entrada típica: marca ya definida, con **logo aprobado y ficha de marca** (paso 3 de
`estudio-de-marca.md`, o la marca que trae la persona con su ficha armada). **Si no hay logo aprobado y
ficha, no hagas empaques ni mockups:** primero los pasos 1–3. Nunca inventes un logo provisional para
"mostrar cómo quedaría".

**Reglas fijas de todos los prompts de este archivo:**
- `@imagen 1` = **logo aprobado, versión limpia**, siempre, con su línea 📎 (`ficha-de-marca.md`).
- La **ficha (BRAND LOCK) pegada completa**, justo después de las imágenes de referencia.
- Los textos en español con el bloque de `corrector-espanol.md` (tildes, Ñ, mayúsculas acentuadas,
  unidades) y dentro del **límite de líneas** de cada pieza.
- Formato del empaque, personaje y datos de producto: **los de la ficha, idénticos**.

## Empaques (paso 7 de la ruta de marca)

Molde adaptado del 07 del playbook (REGLA #2). Orden obligatorio, con aprobación entre cada uno:

1. **Frente de UNA referencia** (la principal). Se aprueba.
2. **Reverso o etiqueta técnica** de esa referencia, si lleva datos técnicos. Se aprueba.
3. **Las demás referencias**, una por prompt, usando el empaque aprobado como referencia de forma y
   diseño: cambian **solo** lo que la ficha dice que cambia (color de esa referencia, nombre y datos).
4. **Línea completa** en una sola foto, con los empaques aprobados como referencias.
5. Opcional: empaque secundario (caja, manga, tag), arte plano de impresión y ficha técnica (pasos 3 y 4
   de este archivo).

**Frente — una referencia:**

```
Create a hyperrealistic 4:5 vertical (1080x1350) premium packaging hero photograph of the "[BRAND NAME]" [product], reference "[REFERENCE NAME]", as seen in a high-end [category] brand launch campaign. Every detail must look like a real, unretouched professional photograph of real printed packaging.
REFERENCE IMAGES — MANDATORY:
@imagen 1 is the EXACT approved logo: reproduce its letterforms, proportions, spelling, accents, device and colors exactly on the package, adapted only to the printing technique ([hot foil / printed ink / deboss]). Do not redraw, restyle or replace it. Do not copy its background.
[@imagen 2 is the EXACT approved character: print it on the package exactly as it is. Never redraw or change it.]
[@imagen N is the EXACT real product ([beans / cookies / bottle]): reproduce it exactly where it appears.]
[BRAND LOCK pegado completo, tal cual]
PACKAGING STRUCTURE — FROM THE BRAND LOCK, DO NOT CHANGE:
[Formato exacto de la ficha: type, size, finish, closure, valve, window, label position].
FRONT DESIGN — REFERENCE "[REFERENCE NAME]":
- Package color: [color #HEX of this reference, from the BRAND LOCK].
- [Position]: the logo from @imagen 1, about [X]% of the width.
- [Position]: [character or illustration, if any, from @imagen 2].
- [Position]: the reference name "[REFERENCE NAME]".
- [Position]: "[ORIGIN]".
- [Position]: "[NOTES]".
- Bottom: "[WEIGHT]".
SPANISH TEXT — EXACT RENDERING — MANDATORY:
Render ONLY the texts listed below, in Spanish, exactly as written between quotes, character by character. Keep every accent mark and the Ñ, also on uppercase letters. Do not translate, do not drop or move accents, do not add any other word, letter, number or symbol.
- Logo: "[BRAND NAME]" (exactly as in @imagen 1)
- Reference name: "[REFERENCE NAME]"
- Origin: "[ORIGIN]" ([L-E-T-T-E-R-S], with [a tilde over the N / the accent over the …], if it has one)
- Notes: "[NOTES]"
- Weight: "[WEIGHT]"
No other text on the front. Maximum five lines of text on the front.
COMPOSITION:
[Camera angle and placement], [surface and background from the approved mood board], [real product or ingredients beside the package].
MATERIAL HYPERREALISM — MANDATORY:
[Material phrases of the package from the block list below], natural crinkles and folds, seams and seals, the logo adapted to its printing technique, crisp printing with correct ink density.
NO CGI render look. NO flat digital mockup. NO perfectly smooth package.
CAMERA AND LIGHTING:
Shot on a Hasselblad X2D 100C with an XCD 90mm lens, ISO 64, f/11, 1/250s, [angle]. [Light scheme of the approved mood board], 8K ultra-high resolution, 16-bit color depth, tack-sharp on the package, true-to-life colors.
NO different packaging format. NO different or provisional logo. NO changed product data. NO data from another reference. NO misspelled words. NO missing accents. NO extra text. NO barcodes on the front. NO other logos. NO watermarks.
4:5 vertical, 1080x1350.
```
📎 Adjunta en tu generador: @imagen 1 = logo aprobado (versión limpia) · [@imagen 2 = personaje aprobado] · [@imagen N = foto real del producto]

**Reverso o etiqueta técnica (máximo 6 líneas):** mismo molde, con la cámara de frente al reverso y este
bloque de textos en lugar del frontal. Cada dato sale de la ficha, de **esa** referencia:

```
BACK LABEL — REFERENCE "[REFERENCE NAME]":
A clean label on the back of the same package, [label color #HEX], six short lines aligned [left], in the BRAND LOCK typography:
- "ORIGEN: [ORIGIN]"
- "VARIEDAD: [VARIETY]"
- "ALTITUD: [ALTITUDE]" (for example "ALTITUD: 1.900 msnm" — "msnm" in lowercase, exactly)
- "PROCESO: [PROCESS]"
- "NOTAS: [NOTES]"
- "[WEIGHT]"
SPANISH TEXT — EXACT RENDERING — MANDATORY: render ONLY these six lines, character by character, keeping every accent and Ñ. No other text.
```

**Las demás referencias:** el mismo prompt del frente, con dos cambios:
- Agrega a REFERENCE IMAGES: "@imagen [X] is the APPROVED package of reference "[REFERENCE 1]". Reproduce
  its exact structure, layout, logo position, typography and finish. Change ONLY the package color, the
  reference name and the reference data listed below."
- FRONT DESIGN y SPANISH TEXT con los datos de **esta** referencia, copiados de la ficha.

📎 Adjunta en tu generador: @imagen 1 = logo aprobado · [@imagen 2 = personaje] · @imagen [X] = empaque aprobado de la referencia 1

**Línea completa:** una foto con todas las referencias de pie, una al lado de otra. Cada empaque aprobado
va como su propia `@imagen` ("Place each approved package exactly as it is; do not regenerate or alter
it"), y el bloque de textos lista solo los textos que ya están en ellos.

## Paso 1 — Elegir 6–10 aplicaciones (no todas)

Pregunta tipo de negocio y canales, y ofrece este menú con botones (multi-selección). Marca tu
recomendación según dónde vive la marca.

| Tipo de negocio | Aplicaciones que más impacto tienen |
| --- | --- |
| Restaurante / café / panadería | Carta y porta-menú, hablador de mesa, vaso y manga, bolsa y sticker de cierre, delantal y gorra, aviso de fachada o caja de luz, vinilo de vitrina, tarjeta de fidelización |
| Tienda / producto físico / retail | Etiqueta y colgante (tag), empaque y caja, papel de seda y cinta, bolsa, rompetráfico y cenefa, exhibidor de mostrador, wobbler, vinilo de vitrina |
| Belleza / estética / peluquería | Tarjeta de cita, carta de servicios, etiquetas de frasco, bolsa, señalética interna, vinilo de espejo, uniforme, kit de bienvenida |
| Salud / consultorio | Papelería (receta, sobre, carpeta), tarjeta, señalética, aviso de fachada, uniforme bordado, roll-up de sala de espera |
| Servicios / marca personal / consultora | Tarjeta, firma de correo, presentación comercial, kit de bienvenida, cuaderno y merch, backing para fotos o lives, roll-up para charlas |
| Mascotas | Empaque, sticker, bandana, tarjeta de adopción o regalo, exhibidor de mostrador, bolsa |
| Eventos / ferias / emprendimiento en bazares | Pendón o roll-up, mantel de mesa, backing, exhibidor de mostrador, stickers, tarjeta, bolsa |
| E-commerce sin local | Caja de envío, cinta adhesiva, papel de seda, tarjeta de agradecimiento con QR, sticker de cierre, inserto |

## Glosario de material POP (como se dice aquí → qué es)

Medidas **de referencia** del mercado: cada imprenta tiene sus formatos; confírmalas antes del arte final.

| Pieza | Qué es | Medida de referencia | Material habitual |
| --- | --- | --- | --- |
| Hablador de mesa / de estante | Tarjeta de pie o en porta-hablador con promo o mensaje | 10×15 cm, 10×20 cm | Propalcote 300 g, cartón, PVC o acrílico |
| Rompetráfico / stopper | Pieza perpendicular al estante que frena la mirada | 10×15 a 15×20 cm | PVC 1–2 mm, cartón |
| Wobbler | Pieza pequeña que se mueve sobre una tira flexible | 8–12 cm | Cartón o PVC + tira plástica |
| Dangler / colgante | Pieza que cuelga del techo, doble cara | 30×40 a 50×70 cm | Cartón, PVC, foam |
| Cenefa | Franja en el borde del estante | Largo del estante × 5–10 cm | Cartón, PVC |
| Exhibidor de mostrador | Display pequeño que sostiene el producto en caja | A medida del producto | Cartón microcorrugado, acrílico, MDF |
| Exhibidor de piso / isla | Estructura de piso con producto | A medida | Cartón corrugado, MDF, metal |
| Pendón | Lona impresa con tubos o cuerda | 60×160, 80×180, 100×200 cm | Lona banner |
| Roll-up / araña | Estructura enrollable portátil | 80×200, 85×200 cm | Lona o PET en estructura de aluminio |
| Backing | Fondo grande para eventos y fotos | 2×2 a 3×2,4 m | Lona en estructura |
| Vinilo de vitrina | Adhesivo para vidrio, de corte o impreso | A medida | Vinilo de corte, vinilo impreso o microperforado |
| Aviso de fachada | Letrero exterior | A medida | Acrílico, caja de luz, letras corpóreas, neón LED flex |
| Carta / menú | Carta de productos o servicios | Carta 21,6×27,9 o media carta | Propalcote, cartón, acrílico, madera |
| Volante | Pieza de mano | Media carta 14×21,6 cm o 10×15 cm | Propalcote 150 g |
| Tarjeta de presentación | — | 9×5 cm (Colombia), 8,5×5,5 cm | Cartulina 300–350 g |
| Sticker / etiqueta | Troquelado o en rollo | A medida | Vinilo, papel adhesivo, kraft adhesivo |
| Empaque | Bolsa, doypack, caja, manga, tag | A medida | Kraft, propalcote, cartón, plástico flexible |
| Textil | Delantal, camiseta, gorra, bandana, bolsa de tela | — | Bordado o estampado (serigrafía, DTF, vinilo textil) |

## Paso 2 — Mockup fotorrealista (prompt inline)

**Molde (REGLA #2): no inventes la estructura; adapta los prompts del playbook.**
- Papelería y logo en objetos → molde **02B** (flat-lay de aplicaciones).
- Empaques → sección "Empaques" de este archivo (adaptada del molde **07**); caja o empaque secundario →
  molde **08**.
- Redes en celular → molde **09**.
- Material POP y espacios → molde **08** (pieza hero en escena) con un bloque de ENTORNO.

Conserva los bloques del playbook con sus nombres: REFERENCE IMAGES — MANDATORY · BRAND LOCK · [PIECE]
DESIGN · COMPOSITION · SPANISH TEXT — EXACT RENDERING — MANDATORY (reemplaza al antiguo TEXT ACCURACY) ·
MATERIAL HYPERREALISM — MANDATORY · CAMERA AND LIGHTING · cierre de NO… y formato. Siempre con
`@imagen 1` = logo aprobado y la línea 📎 de qué adjuntar.

**Lo que hace que un mockup se vea real (y no "pegado"):**
- El logo se **adapta a la técnica de cada material**, nunca se pega plano: tinta absorbida en kraft,
  relieve en cartón, bordado con hilo, vinilo con borde troquelado, luz que sale de la caja de luz.
- Cada pieza tiene **física**: grosor, bordes, cómo se apoya, cómo cuelga, qué sombra proyecta.
- La luz del mockup coincide con la del lugar (luz de vitrina, de techo de local, de ventana).
- Escala real: un hablador mide lo que una mano; un roll-up lo que una persona.

**Bloques de material (frases para MATERIAL HYPERREALISM):**
- Propalcote / cartulina: *crisp die-cut edges, visible board thickness, matte or satin laminate sheen.*
- Kraft: *visible paper fibers, slightly irregular edges, ink absorbed into the paper, matte.*
- Cartón corrugado: *visible flute layers on the cut edges, slight wear on the corners.*
- Acrílico: *clear cast acrylic with polished edges, soft reflections and faint micro-scratches.*
- Lona / roll-up: *matte vinyl banner with subtle weave texture, slight tension waves near the edges, aluminum base.*
- Vinilo de vitrina: *cut vinyl lettering on glass with real reflections of the street, slight edge lift catching light.*
- Caja de luz / neón LED flex: *even internal glow with subtle hotspots, light spill on the wall, visible mounting hardware.*
- Bordado: *raised satin-stitch embroidery with individual thread sheen and slight fabric puckering.*
- Acabados: *selective gloss UV spot on the logo · hot-foil stamping with metallic reflections · blind deboss with soft shadows inside the letters.*

**Ejemplo de molde POP en escena (adaptado de 08; rellena lo que está entre corchetes):**

```
Create a hyperrealistic 4:5 vertical (1080x1350) point-of-sale photograph for "[BRAND]", showing its branded counter materials inside a real [business type], as seen in a premium retail branding presentation. Every detail must look like a real, unretouched professional photograph of real printed materials.
REFERENCE IMAGES — MANDATORY:
@imagen 1 is the EXACT approved logo: reproduce its letterforms, proportions, spelling, accents and colors exactly on every piece. The logo reads exactly "[BRAND]". Do not redraw or reinterpret it. Do not copy its background.
@imagen 2 is the EXACT approved product: [exact description]. Do not change its shape, colors or label.
[BRAND LOCK pegado completo, tal cual]
POINT-OF-SALE PIECES:
- TABLE TENT: a [10x15 cm] [material] table tent standing on the counter, [background color #HEX], the logo at the top and the text "[TEXT]" in [font style], [color #HEX].
- WOBBLER: a [10 cm] round die-cut wobbler in [color #HEX] attached to the shelf edge with a clear flexible strip, with the text "[TEXT]".
- [Other piece]: [design].
ENVIRONMENT:
[Counter material, wall, props, depth], a softly blurred [business] interior in the background in the brand palette: [HEX list]. No other brands visible.
COMPOSITION:
[Camera position], the table tent in the foreground right, the product beside it, the wobbler on the shelf edge in the mid-ground. Real scale: the table tent is the size of a hand.
SPANISH TEXT — EXACT RENDERING — MANDATORY:
Render ONLY the texts listed below, in Spanish, exactly as written between quotes, character by character. Keep every accent mark and the Ñ, also on uppercase letters. Do not translate, do not drop or move accents, do not add any other word, letter or symbol.
- Table tent: "[TEXT 1]"
- Wobbler: "[TEXT 2]"
No other text anywhere, except the logo. Maximum two lines of text per piece.
MATERIAL HYPERREALISM — MANDATORY:
[Material blocks of each piece], the logo adapted to each printing technique, real thickness, edges and contact shadows on the counter.
NO CGI render look. NO flat digital mockup. NO pasted-on logo.
CAMERA AND LIGHTING:
Shot on a Hasselblad X2D 100C with an XCD 55mm lens, ISO 100, f/5.6, 1/125s, [angle]. [Light that matches the space: warm ceiling spots / window daylight], with a soft fill, 8K ultra-high resolution, 16-bit color depth, tack-sharp on the pieces, true-to-life colors.
NO misspelled words. NO missing accents. NO extra text. NO other logos. NO different logo. NO watermarks. NO distorted product.
4:5 vertical, 1080x1350.
```
📎 Adjunta en tu generador: @imagen 1 = logo aprobado, limpio · @imagen 2 = foto del producto

### En su propio local (la opción que más vende)

Si la persona trae una foto real de su mostrador, vitrina o fachada, úsala como `@imagen` de ESPACIO:

```
@imagen 3 is the EXACT real space: keep its architecture, furniture, materials, perspective and lighting exactly as they are. Only ADD the branded pieces described below, integrated with correct perspective, scale, contact shadows and reflections. Do not redecorate, recolor or remove anything from the space.
```

Avísale que el resultado es una simulación para decidir y vender, no una medición: el arte final se
hace a medida real.

### Sets de presentación (tipo estudio)

| Set | Qué muestra | Formato | Molde |
| --- | --- | --- | --- |
| Papelería | Tarjeta, hoja membretada, sobre, sticker, sello, tag | 4:5 o 16:9 flat-lay | 02B |
| Punto de venta | Mostrador con hablador, wobbler, exhibidor, producto | 4:5 | 08 + entorno |
| Fachada y vitrina | Aviso, vinilo de vitrina, horario, puerta | 4:5 o 16:9 | 08 + entorno |
| Línea de empaque | Bolsas, cajas, etiquetas por variante | 4:5 | 07 |
| Unboxing / e-commerce | Caja de envío abierta, papel de seda, tarjeta, sticker | 4:5 o 1:1 cenital | 08 |
| Feria / evento | Mesa con mantel, pendón o roll-up, exhibidor, stickers | 16:9 | 08 + entorno |
| Textil y merch | Delantal, camiseta, gorra, bolsa de tela | 4:5 | 02B |
| Digital | Perfil, historias, destacados en celular | 4:5 | 09 |

## Paso 3 — Arte plano de impresión (prompt)

El mockup vende la idea; el arte plano es el diseño de la pieza en sí, de frente y sin escena, para
revisar textos y llevarlo a producción. Calcula la **proporción real** desde la medida (10×15 cm → 2:3,
roll-up 85×200 cm → aprox. 9:21, tarjeta 9×5 cm → 9:5) y úsala en el prompt.

```
Create a flat, front-facing print-ready graphic design of a [PIECE, e.g. table tent] for "[BRAND]", exact aspect ratio [W:H] (it will be printed at [W×H cm]). Pure flat design filling the whole frame edge to edge: no mockup, no photo, no perspective, no shadows, no background scene.
REFERENCE IMAGE — MANDATORY:
@imagen 1 is the EXACT approved logo: reproduce it identically, with its spelling and accents; do not redraw it.
[BRAND LOCK pegado completo, tal cual]
DESIGN:
Background [#HEX]. Logo at [position], about [X]% of the width. Headline "[TEXT]" in [letterform description], [#HEX], [position]. Secondary text "[TEXT]" in [style], [#HEX]. [Brand device / pattern / mother shape and where]. Keep all text and the logo at least 5% away from every edge (safety margin).
COLOR PALETTE:
Only the BRAND LOCK colors. No other colors.
SPANISH TEXT — EXACT RENDERING — MANDATORY:
Render ONLY the texts listed below, in Spanish, exactly as written between quotes, character by character. Keep every accent mark and the Ñ, also on uppercase letters. Do not translate, do not drop or move accents, do not add any other word, letter or symbol.
- Headline: "[TEXT 1]"
- Secondary: "[TEXT 2]"
No other text anywhere, except the logo.
NO mockup. NO perspective. NO shadows. NO misspelled words. NO missing accents. NO extra text. NO other logos. NO watermarks.
[W:H], highest resolution available.
```
📎 Adjunta en tu generador: @imagen 1 = logo limpio aprobado

Luego dile en una línea cómo terminarlo: llevar la imagen a Canva a la medida exacta y exportar en PDF
para impresión (o pasarla al diseñador de la imprenta). Antes de imprimir, revisa cada texto letra por
letra (tildes, Ñ, unidades) con `corrector-espanol.md`; si algo salió mal, usa su prompt de corrección o
corrígelo en Canva **escrito correctamente**. Los textos muy pequeños (menos de ~7 pt) y los precios
quedan más seguros puestos en Canva (`modo-texto.md`).

**Reglas de impresión (dilas en el arte y en la ficha):**
- Modo de color **CMYK**; los HEX de pantalla cambian al imprimir: pedir prueba de color.
- Resolución **300 ppp** a tamaño real (gran formato como pendón o backing: 100–150 ppp a tamaño real).
- **Sangrado** de 3 mm por lado (algunas imprentas piden 5 mm) y **margen de seguridad** de 3–5 mm
  sin textos importantes.
- Texto mínimo legible ~7 pt; textos negros en 100 % K; fondos negros grandes en negro enriquecido.
- Troqueles en una capa o color directo aparte; fuentes convertidas a curvas; exportar PDF de alta
  calidad (PDF/X-1a si la imprenta lo pide).

## Paso 4 — Ficha técnica para el impresor

Una tabla por pieza, lista para mandar a cotizar:

| Pieza | Medida final | Sangrado | Material / gramaje | Tintas | Acabado | Troquel | Cantidad | Archivo |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Hablador de mesa | 10×15 cm | 3 mm | Propalcote 300 g | 4×4 | Laminado mate | Pie plegable | 50 | PDF CMYK |

Tintas: 4×0 = color por un lado, 4×4 = color por ambos lados, 1×0 = una tinta.
Acabados frecuentes: laminado mate o brillante, UV selectivo, hot stamping (foil), relieve o bajo
relieve, barniz, troquel.

## Orden de entrega

0. Empaques primero, si es la ruta de marca (sección "Empaques", paso 7). El resto de aplicaciones es
   opcional, después del paso 7.
1. Menú de aplicaciones → la persona elige 6–10.
2. Por cada aplicación (o set): mockup (prompt inline + 📎) → espera aprobación.
3. Arte plano de impresión (prompt) y cómo terminarlo en Canva o en la imprenta.
4. Ficha técnica de todo el paquete en una sola tabla.
5. Las aplicaciones aprobadas entran como bloques del tablero de identidad (prompt de ensamble en
   `tablero-identidad.md`) y como lámina "Aplicaciones" en el brand board.
