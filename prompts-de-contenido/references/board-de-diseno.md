# Social media board de opciones (elegir el diseño mirando)

Antes de producir piezas con texto, la persona elige su **sistema de diseño** viendo cómo se aplica, no
leyendo nombres de fuentes. Para eso la skill entrega **3 prompts de social media board**, uno por opción:
cada uno genera una grilla de posts de Instagram con la misma paleta, la misma tipografía y el mismo
recurso gráfico, aplicados a distintos tipos de post. Ejemplo del formato: `assets/referencias/texto/`
**txt-022** (feed rojo y crema: titulares en máquina de escribir y serif condensada, palabras clave
encerradas en un círculo a mano, objetos de color héroe, tarjetas tipo nota).

## Cuándo se entrega

- **Piezas, carruseles y campañas con texto**, también en la ruta express: reemplaza al prompt de muestra
  tipográfica. Va al inicio, antes de los prompts de las piezas.
- **En campañas**, cada dirección creativa trae su board: el board **es** la vista previa de la dirección
  (paleta, letra, recurso, tono de foto y layouts juntos).
- **No en la ruta de marca antes del logo aprobado.** Ahí el orden lo manda `estudio-de-marca.md` (el
  moodboard del paso 5 sigue siendo el molde 01 del playbook, con el logo como `@imagen 1`).
- Si la pieza no lleva texto, no hace falta: alcanza con la dirección y su moodboard.

## Cómo se arman las 3 opciones

Las 3 deben ser **sistemas distintos**, no la misma idea con otro color: cambian al menos la paleta, la
pareja tipográfica y el recurso gráfico. Salen de las referencias de la persona, del repositorio
(`assets/referencias/indice.md`, sobre todo `texto/` y el nicho) y de la marca real si existe (orden de
`tipografia.md`). Antes de los prompts, presenta cada opción en 4 líneas:

1. **Nombre** de la opción y la sensación que transmite.
2. **Paleta por roles** con HEX: fondo · texto · acento · color héroe (reservado al producto).
3. **Tipografía:** titular + texto, con el nombre real para Canva.
4. **Recurso gráfico** que se repite (círculo a mano, píldoras, tarjeta de nota, subrayado, sticker…) y de
   qué referencias sale.

Marca tu recomendación. Después dile: "Genera los 3 boards, elige 1, 2 o 3 (o combina, por ejemplo la
paleta de la 1 con las letras de la 3) y seguimos con las piezas". El board elegido queda como el sistema
bloqueado de la serie.

## Molde del prompt (uno por opción)

```
Create a professional social media design board, 2:3 vertical (1200x1800), presenting a cohesive Instagram feed design system for "[MARCA]", [una línea: qué es la marca y su personalidad]. This is OPTION [N] — "[NOMBRE DE LA OPCIÓN]".

BOARD LAYOUT:
A clean grid of 12 Instagram post mockups, 4 rows x 3 columns, each post 4:5, separated by thin even [#HEX] gutters on a [#HEX] background. Along the top, a slim header strip with the text "OPCIÓN [N]" and, next to it, [5] round color swatches in a row, each labeled with its HEX code in a tiny monospaced font.

DESIGN SYSTEM — IDENTICAL IN ALL 12 POSTS:
Palette: background [#HEX] and [#HEX], text [#HEX], accent [#HEX], hero color [#HEX] used only on the product and on one key object per post. No other colors.
Headline typeface: [estilo exacto: e.g. condensed high-contrast serif, uppercase, tight tracking].
Secondary typeface: [estilo exacto: e.g. typewriter monospace, small caps].
Recurring graphic device: [e.g. one key word per headline circled with a loose hand-drawn ellipse in the accent color].
Photography style: [luz, grade y tipo de foto: e.g. warm flash editorial, cropped hands and objects, soft film grain].

THE 12 POSTS (each a different layout of the same system):
1. Cover: big headline "[TITULAR 1]" over [fondo o foto].
2. Product hero: the product from @imagen 1 as the protagonist, [escena], small label "[TEXTO CORTO]".
3. Statement: only typography, "[FRASE]".
4. Educational list: headline "[TITULAR]" with 4 numbered pill labels.
5. Lifestyle photo: [escena con persona o manos], tiny caption.
6. Object concept: [objeto de color héroe] with headline "[TITULAR]".
7. Note card: a phone-notes style card over a photo, title "[TITULAR]".
8. Benefit or data: "[BENEFICIO O DATO REAL]".
9. Quote: "[CITA O FRASE DE MARCA]".
10. Behind the scenes: [escena del negocio].
11. Product detail macro: close-up of @imagen 1 [detalle].
12. Call to action: "[CTA]" with a button-shaped label.

PRODUCT ACCURACY: Use the product from @imagen 1 exactly as provided in posts 2 and 11 (and wherever it appears): same shape, colors, logo and label. Do not redesign it or invent other products of the brand.

[Bloque SPANISH TEXT — EXACT RENDERING de `corrector-espanol.md` con los titulares deletreados.]
Only the headlines must be readable; small body copy may be rendered as fine, neat placeholder lines. NO handles or brand names other than "[MARCA]". NO other brand logos. NO watermarks. Consistent margins and alignment in every post. Photoreal photos, crisp typography.
```
📎 Adjunta en tu generador: @imagen 1 = foto del producto (si hay producto). Si no hay producto, quita las
líneas del producto y escribe: "Sin adjuntos — este prompt es solo texto".

## Reglas

- **Textos reales, no relleno:** los titulares del board son copys propuestos para la marca (ángulo,
  fórmula, anti-cliché de `copywriting.md`), en español con tildes y Ñ. Máximo 6–8 palabras por titular.
- **Handle:** solo si la persona lo dio; si no, no aparece ninguno (nada de "@YOURHANDLE").
- **Honestidad:** el generador aproxima letras y detalles en 12 posts pequeños; sirve para elegir el
  sistema, no como piezas finales. Las fuentes exactas se aplican en Canva con el nombre real.
- **Después de elegir:** paleta, tipografía, recurso y estilo de foto del board elegido se copian
  idénticos en todos los prompts de la serie (consistencia de familia).
