# Tipografía — sugerencia y combinación

La skill debe proponer tipografías y combinaciones profesionales, no dejarlas al azar. Esto aplica a
toda pieza con texto (posters, carruseles, promos, brand board).

## Realidad técnica (honestidad)

Los generadores de imagen **no cargan un archivo de fuente**: aproximan el estilo tipográfico a partir
de la *descripción*. Por eso en el prompt se describe el estilo con precisión (ej. "bold condensed
grotesque sans, uppercase, tight tracking, heavy weight") y, aparte, se le dice a la persona **qué
fuente real poner en Canva** para su edición final. Dos salidas:
1. Dentro del prompt: descripción del estilo tipográfico (para que la imagen generada se acerque).
2. Para la persona: el nombre de 1–2 fuentes reales (Canva/Google Fonts) para aplicar/editar después.

Recordatorio de render: los textos van en español correcto, **con tildes y Ñ**, cortos, deletreados
exactos y dentro del bloque SPANISH TEXT de `corrector-espanol.md`. Elige fuentes que tengan tildes y Ñ
(todas las de Google Fonts recomendadas aquí las tienen; confírmalo en Canva).

## Principios de combinación

- **Máximo 2 familias** por pieza: una para titulares (display), una para cuerpo/apoyo.
- **Contraste con intención:** serif display + sans limpia, o grotesca pesada + sans fina. Evita
  parear dos fuentes que compiten (dos display, dos geométricas casi iguales).
- **Jerarquía por peso y escala**, no por muchas fuentes: un solo display en 2–3 pesos rinde más.
- **El estilo tipográfico sigue el registro/nicho**, igual que la paleta (abajo).

## Orden para elegir la tipografía (obligatorio)

1. **Identidad real de la marca** (si es marca existente o real): su tipografía o la más cercana. Si no la
   conoces, búscala o pregunta; no la supongas.
2. **Tipografía de las referencias** de la persona y del repositorio (capa 3 de
   `ingenieria-inversa.md`): familia, peso, ancho, caja y tracking.
3. **Vibra del nicho** (menú de abajo). El combo listo es el último recurso, nunca el primero.

**Moda no es lujo por defecto.** Una marca workwear, streetwear o deportiva pide grotesca condensada o
slab industrial, no una serif de lujo. Prueba de marca tapada: si tapas el logo, ¿la letra se sigue
sintiendo de esa marca? Si no, cambia la combinación.

## Menú por vibra / nicho (fuentes reales, disponibles en Canva/Google Fonts)

- **Lujo editorial** (moda de lujo, inmobiliaria premium, belleza high-end): display serif — *Playfair
  Display, DM Serif Display, Cormorant, Bodoni Moda*; apoyo sans — *Montserrat, Jost, Inter*.
- **Streetwear / workwear / heritage / deporte:** grotesca condensada pesada o slab industrial — *Anton,
  Archivo Black, Oswald, Bebas Neue, Alfa Slab One, Roboto Slab (Black)*; apoyo mono o grotesca —
  *Space Mono, IBM Plex Mono, Archivo, Inter*.
- **Street / comida / promo bold:** grotesca pesada o condensada — *Anton, Bebas Neue, Archivo Black,
  Oswald*; bubble redonda — *Fredoka, Baloo 2*; apoyo — *Inter, Work Sans*.
- **Wellness / belleza suave:** serif elegante — *Fraunces, Cormorant Garamond*; humanista — *Nunito,
  Quicksand, Poppins*.
- **Contenido / agencia / tech:** grotesca moderna — *Space Grotesk, Archivo, Syne*; acento mono —
  *Space Mono*; apoyo — *Inter*.
- **Mascotas / juguetón:** redondeadas — *Fredoka, Baloo 2, Quicksand*; apoyo — *Nunito*.
- **Fisioterapia / salud:** sans limpia y legible — *Inter, Work Sans, Poppins, Mulish*; números
  claros para pasos/beneficios.
- **Peluquería / salón:** serif editorial — *Cormorant, Playfair*; apoyo — *Jost, Montserrat*.

## Combos listos (titular / cuerpo) por si la persona quiere un atajo

- Lujo: **DM Serif Display / Montserrat**
- Street-food: **Anton / Inter**  ·  Bubble promo: **Fredoka / Nunito**
- Wellness: **Fraunces / Nunito**
- Agencia-contenido: **Space Grotesk / Inter**
- Mascotas: **Baloo 2 / Quicksand**
- Salud-fisio: **Poppins / Work Sans**
- Salón: **Cormorant / Jost**
- Streetwear-workwear: **Anton / Space Mono**  ·  Heritage-deporte: **Alfa Slab One / Archivo**

## Cómo se presentan: al inicio, como elección aparte y con muestra visual

En toda pieza o campaña con texto, la tipografía se decide **al inicio**, antes de los prompts de las
piezas, como una elección propia (no escondida dentro de cada dirección):

1. Da **2–3 combinaciones** (hasta 5 si pide variedad), cada una con el nombre real de cada fuente, su
   rol (titular, texto, etiquetas), el estilo en una línea, de dónde sale (marca, referencia o nicho) y
   **tu recomendación marcada** con el porqué.
2. **Entrega por iniciativa propia el prompt de muestra tipográfica** (abajo) para que la persona la
   genere en su herramienta y **elija mirando**. Dile: "Genera esta muestra, elige 1, 2 o 3 y seguimos".
3. Con la elegida, sigue el flujo. No construyas tableros HTML para elegir fuentes (REGLA #1 del SKILL).
   En la ruta de marca, la muestra va después del logo aprobado.

Honestidad: el generador aproxima el estilo de la letra; la fuente exacta se aplica en Canva con el
nombre real que le diste.

**Molde del prompt de muestra tipográfica** (se adapta con los textos reales de la pieza):

```
Create a clean professional typography specimen sheet, 4:5 vertical (1080x1350), on a flat [background #HEX] background. Show THREE font pairing options stacked in three equal horizontal bands separated by thin [#HEX] rules. A small number "1", "2" and "3" in a tiny monospaced font sits in the top-left corner of each band.
In every band, set the same three texts so the options can be compared: the headline "[TITULAR REAL]", the brand name "[MARCA]" and one body line "[BAJADA REAL]".
OPTION 1: headline and brand name in [exact style: e.g. ultra-condensed heavy grotesque, uppercase, tight tracking]; body line in [exact style].
OPTION 2: headline and brand name in [exact style]; body line in [exact style].
OPTION 3: headline and brand name in [exact style]; body line in [exact style].
Colors only from the palette: headline [#HEX], body [#HEX], one accent [#HEX].
[Bloque SPANISH TEXT — EXACT RENDERING de corrector-espanol.md, con los tres textos deletreados.]
NO other text. NO photos, NO mockups, NO decorations, NO gradients. Even spacing, sharp letterforms.
```
📎 Sin adjuntos: este prompt es solo texto.

**Más opciones:** para un catálogo amplio por estilo (serif de lujo, condensadas de impacto, redondeadas,
script, mono/tech, grunge/experimental, gótico/terror, retro…) usa `libreria-fuentes.md`. Son todas de
Google Fonts, así que se **renderizan en vivo en el overlay** y se **nombran para Canva**. En el overlay
puedes usar **cualquier** Google Font, no solo las del menú.
