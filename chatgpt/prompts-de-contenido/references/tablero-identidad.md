# Tablero de identidad (paso 6 de la ruta de marca)

Es la pieza que presenta la identidad completa de un vistazo: sistema de logo, monograma, paleta con
significado, tipografía, palabras clave y aplicaciones fotorrealistas. Es lo que más impacta en una
presentación a cliente, en un portafolio y como contenido de redes.

## Cuándo se usa

- **Paso 6 de la ruta de marca** (`estudio-de-marca.md`): después del moodboard aprobado (paso 5) y
  antes de los empaques (paso 7).
- **Marca existente (entrada C):** la persona trae su logo; primero se arma su ficha
  (`ficha-de-marca.md`) y después el tablero.

> ⛔ **Nunca antes del logo aprobado.** Este tablero no inventa, no explora ni "propone" un logo: solo
> **aplica** el logo aprobado (`@imagen 1`) y la ficha. No existe versión express con logo provisional.

> Los layouts A, B y C y la anatomía de abajo son **ejemplos de estructura**, no un estilo. Si la persona
> trajo referencias de tableros o brand boards (paso 4), el layout y el estilo salen de ellas
> (`ingenieria-inversa.md`); A, B o C se ofrecen solo si no las trae.

## Anatomía de un tablero que se ve de estudio

- **Grilla editorial** de bloques rectangulares de distintos tamaños, unidos sin espacios o con
  separaciones finas; un bloque héroe dominante.
- **Etiquetas de sección** numeradas en mono pequeño y mayúsculas, con una regla fina.
- **Ritmo plano/foto:** bloques planos (logo, paleta, tipografía, palabras clave) alternados con
  bloques fotográficos (aplicaciones) que comparten **la misma luz**: la del moodboard aprobado.
- **Paleta:** solo la de la ficha, por roles; cada muestra con su nombre y su HEX.
- **Un dispositivo gráfico** repetido en logo, monograma, afiche y stickers.
- **Franja de pie** con el tagline aprobado.

## Tres layouts (elige uno con la persona, con botones)

**A · Showcase (2:1 o 16:9).** Fila 1: bloque héroe del logo sobre oscuro (≈50 % del ancho) + 4
bloques de color en 2×2 con el logo en cada fondo de la paleta. Fila 2: columna estrecha de íconos de
app + 4 aplicaciones fotográficas. Mucho impacto, poca información.

**B · Sistema creativo (4:3).** Cabecera fina "[MARCA] · SISTEMA DE IDENTIDAD · [AÑO]". Fila 1: héroe
grande + logo claro y oscuro apilados + bloque de monograma con íconos. Fila 2 (01–04): tipografía ·
tagline · paleta · palabras clave. Fila 3: 4–5 aplicaciones.

**C · Guía numerada (4:3).** Fila 1 (01–04): logo principal · logo secundario · versión de color ·
monograma. Fila 2 (05–06): paleta con nombre y HEX · tipografía con alfabeto de muestra.
Fila 3 (07–10): cuatro aplicaciones. Pie: franja con tagline. Es el más completo y el más útil como
mini manual.

## Cómo evitar los errores del "one-shot"

Los tableros generados de una vez suelen fallar en lo mismo: letras sueltas o de más, el logo cambia de
bloque a bloque, monogramas distintos, tildes perdidas, ® y ™ mezclados y microtexto ilegible. Se evita así:

1. **Logo aprobado como `@imagen 1`**, más la hoja del sistema de logo y el moodboard aprobado como
   referencias. El tablero solo los **aplica**.
2. **Ficha pegada completa** (BRAND LOCK): colores, tipografía, personaje y textos salen de ahí.
3. **Lista cerrada de textos**, máximo 25 cadenas (sin contar códigos HEX ni nombres de fuentes), todas en español correcto **con tildes y Ñ** y el
   bloque de `corrector-espanol.md`. Si hacen falta más, sobra información.
4. **Mapa de grilla explícito:** cada bloque con su fila, su ancho aproximado y su contenido.
5. **Una sola luz** en los bloques fotográficos: la del moodboard aprobado.
6. **Sin empaque inventado:** el empaque se diseña en el paso 7. Si se quiere en el tablero, se rearma
   el tablero después del paso 7 con el empaque aprobado (prompt de ensamble).
7. **Mayor resolución** del generador. Si un texto sale mal, se corrige con el prompt de corrección,
   sin regenerar todo.

## Prompt maestro — layout C (adáptalo; para A o B cambia solo el bloque LAYOUT)

```
Create a professional brand identity presentation board, 4:3 horizontal (2048x1536), for "[BRAND NAME]", a [one-line brand description]. It must look like a premium design studio's brand guidelines page: an editorial grid of rectangular blocks joined edge to edge, mixing flat graphic blocks and hyperrealistic photographic application blocks, all clearly belonging to one coherent identity.
REFERENCE IMAGES — MANDATORY:
@imagen 1 is the EXACT approved logo: reproduce its letterforms, proportions, spelling, accents, device and colors exactly in every block. Do not redraw, reinterpret or replace it. Do not copy its background.
[@imagen 2 is the EXACT approved character — only if the brand has one; copy it, never redraw it.]
@imagen [N] is the approved logo system sheet: use it ONLY for the secondary version, the color versions and the monogram, reproduced exactly. Do not copy its layout or labels.
@imagen [N+1] is the approved mood board: use it ONLY for the light, color grading and material mood of the photographic blocks. Do not copy its tiles.
[BRAND LOCK pegado completo, tal cual]
LAYOUT (three rows, every block with a tiny monospaced uppercase label and number in its top-left corner, followed by a thin hairline rule):
ROW 1 — "01. LOGO PRINCIPAL": large block (40% width), the primary logo in [color #HEX] on [dark #HEX]. "02. LOGO SECUNDARIO": block (35%), the secondary version in [color #HEX] on [light #HEX]. Right column (25%) split in two: "03. VERSIÓN DE COLOR" with the logo on [accent #HEX]; "04. MONOGRAMA" with two rounded-square app icons, one [#HEX] and one [#HEX].
ROW 2 — "05. PALETA": half width, the palette swatches from the BRAND LOCK in a row, each with its HEX code and its color name below. "06. TIPOGRAFÍA": half width, the headline typeface name "[FONT NAME]" set in that typeface with its alphabet including Á É Í Ó Ú Ñ, the body typeface "[FONT NAME]" with its alphabet, and a sample: "[SHORT HEADLINE]".
ROW 3 — four equal photographic blocks: "07. AFICHE": a printed poster with the headline "[POSTER HEADLINE]" and the logo, [material and setting]. "08. BOLSA DE TELA": a natural canvas tote bag with the logo screen-printed, [setting]. "09. STICKERS": die-cut vinyl stickers of the logo and the monogram on [surface]. "10. TARJETA": two thick business cards, one [dark #HEX] and one [light #HEX], with the logo and "[WEBSITE OR @HANDLE]".
FOOTER: one thin full-width band in [accent #HEX] with "[BRAND NAME]" and the tagline "[TAGLINE]".
CONSISTENCY — MANDATORY:
The logo, monogram, device and palette are identical in every block and identical to the references. No color outside the BRAND LOCK. The monogram is the same in every icon.
SPANISH TEXT — EXACT RENDERING — MANDATORY:
Render ONLY the texts listed below, in Spanish, exactly as written between quotes, character by character. Keep every accent mark and the Ñ, also on uppercase letters. Do not translate, do not drop or move accents, do not add any other word, letter or symbol.
- Block labels: "01. LOGO PRINCIPAL", "02. LOGO SECUNDARIO", "03. VERSIÓN DE COLOR" (with the accent over the O), "04. MONOGRAMA", "05. PALETA", "06. TIPOGRAFÍA" (with the accent over the I), "07. AFICHE", "08. BOLSA DE TELA", "09. STICKERS", "10. TARJETA"
- Brand: "[BRAND NAME]", "[DESCRIPTOR]"
- Tagline: "[TAGLINE]"
- Poster headline: "[POSTER HEADLINE]"
- Card: "[WEBSITE OR @HANDLE]"
- The HEX codes and color names from the BRAND LOCK, and the two font names.
No other text anywhere in the image.
FLAT BLOCKS:
Clean vector-style graphic design, crisp edges, flat solid colors, generous margins, precise alignment to the grid.
PHOTOGRAPHIC BLOCKS — HYPERREALISM:
Real unretouched professional photographs, all with the same light as the approved mood board: [light scheme]. Visible paper fibers on the poster, canvas weave and printed ink on the tote, glossy die-cut edges on the stickers, thick cotton card stock with crisp edges. Shot on a Hasselblad X2D 100C, XCD 55mm, f/5.6, 8K detail, true-to-life colors.
NO provisional or different logo. NO misspelled words. NO missing accents. NO extra text. NO stray characters. NO other logos or brands. NO inconsistent logo versions. NO gradients on flat blocks. NO CGI look on photographic blocks. NO watermarks.
4:3 horizontal, 2048x1536.
```
📎 Adjunta en tu generador: @imagen 1 = logo aprobado (versión limpia) · [@imagen 2 = personaje aprobado, si hay] · @imagen [N] = hoja del sistema de logo · @imagen [N+1] = moodboard aprobado

**Prompt de ensamble (cuando ya hay aplicaciones aprobadas, por ejemplo después del paso 7):** usa el
mismo prompt maestro y cambia:
- REFERENCE IMAGES: agrega "@imagen [X] is the approved [package / poster / stickers / business cards].
  Place each approved image inside its block exactly as it is, only cropped to fit; do not regenerate,
  restyle or alter them."
- ROW 3: en lugar de describir cada foto, "Block 07 = @imagen [X] · Block 08 = @imagen [Y]…". Si un bloque
  pasa a mostrar el empaque, cambia también su etiqueta (por ejemplo "08. EMPAQUE") en la lista de textos.
📎 Adjunta: @imagen 1 = logo aprobado · las demás en el orden que diga el prompt.

**Prompt de corrección de texto:** el de `corrector-espanol.md` (sección 6), indicando el bloque:
"in the block "[BLOCK LABEL]", change ONLY the text…".

**Adaptaciones por layout:** para A (2:1, 2048x1024) usa la fila de colorways y la columna de íconos en
lugar de paleta y tipografía; para B (4:3) agrega la cabecera "[MARCA] · SISTEMA DE IDENTIDAD · [AÑO]" y
la fila de tipografía, tagline, paleta y palabras clave. En los dos, la lista cerrada de textos cambia
con las etiquetas del layout.

**Servicios sin producto físico** (consultoras, marcas personales): cambia afiche y bolsa de tela por
presentación, firma de correo, perfil en celular o cuaderno.

**Generadores:** los que mejor manejan texto y composiciones densas son ChatGPT (imagen), Gemini (Nano
Banana Pro) e Ideogram. Pide la mayor resolución disponible y revisa la ortografía bloque por bloque.
