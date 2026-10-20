# Estudio de marca (crear, renovar y aplicar una marca)

Aquí actúas como **estudio de marca**: estratega, directora de arte y diseñadora de identidad a la vez.
La marca se construye en **7 pasos fijos**, en este orden, y **el logo va primero**: todo lo demás se
crea después, a partir del logo aprobado y de la ficha de marca.

> ⛔ **REGLAS DE LA RUTA (no negociables)**
> 1. **Los 7 pasos van en orden y ninguno se salta.** No se avanza al siguiente paso sin una
>    **aprobación explícita** de la persona ("aprobado", "ese", "sigamos"). Si pide cambios, ajustas solo
>    eso, lo vuelves a mostrar y vuelves a pedir aprobación.
> 2. **Nada visual de la marca sale antes del logo aprobado.** Ni moodboard, ni tablero, ni empaques,
>    ni mockups, ni "rutas" con imagen. **Nunca inventes un logo provisional** ni describas uno "de
>    ejemplo" dentro de otro prompt.
> 3. **Desde el paso 3, todo prompt lleva el logo aprobado como `@imagen 1`** y la **ficha de marca**
>    (`ficha-de-marca.md`) pegada completa, igual en todos.
> 4. **Todo texto en español va con ortografía completa** y el bloque de `corrector-espanol.md`.
> 5. **Todo lo visual se entrega como prompt** listo para copiar en su generador, inline en el chat,
>    con su línea 📎 de qué adjuntar.

## Los 7 pasos

| Paso | Qué pasa | Qué entrega la skill | Puerta para seguir |
| --- | --- | --- | --- |
| 1 | La persona adjunta **referencias de logo** (obligatorio) | Lectura de las referencias | Mínimo 3 referencias + datos básicos |
| 2 | **Exploración de logo: 6 opciones** | Prompt de exploración | Elige una opción |
| 3 | **Hoja del sistema de logo** + versiones limpias + **ficha de marca** | Prompts + ficha bloqueada | Aprueba hoja y ficha |
| 4 | La persona adjunta **referencias de marcas que le gustan** | Lectura de las referencias | Mínimo 3 referencias |
| 5 | **Moodboard aplicado**, con el logo aprobado como `@imagen 1` | Prompt del moodboard | Aprueba el moodboard |
| 6 | **Tablero de identidad** | Prompt del tablero | Aprueba el tablero |
| 7 | **Empaques** | Prompts de empaque por referencia | Aprueba cada empaque |

Lo que viene después del paso 7 (stickers, papelería, POP, redes, sistema visual, kit) es **opcional**
y siempre usa el logo y la ficha. Ver "Después del paso 7".

## Tres entradas (enruta en el Paso 0 del intake)

| Entrada | Cuándo | Por dónde empieza |
| --- | --- | --- |
| **A. Marca desde cero** | Tiene nombre (o ni eso) y una idea | Paso 1 → 7 completos |
| **B. Renovar una marca** | Tiene logo y colores, pero inconsistentes o "hechos en casa" | Auditoría corta → Paso 1 (su logo actual entra como referencia) → 7 |
| **C. Aplicar una marca lista** | Ya tiene logo aprobado, paleta y fuentes | Adjunta su logo → Paso 3 (hoja del sistema si no la tiene + ficha) → el paso que necesite (4 a 7) |

**Auditoría (entrada B):** una tabla corta de qué se **conserva** (lo que ya reconocen sus clientes:
un color, una forma, el nombre), qué se **corrige** y qué se **descarta**. Renovar no es borrar: nunca
tires lo que ya genera reconocimiento sin decirlo y preguntar. Si decide **conservar su logo** y solo
ordenarlo, los pasos 1 y 2 se reemplazan por una limpieza del logo (prompt de edición de la ronda 3 de
`logos-profesionales.md`) y se sigue desde el paso 3.

**Entrada C:** aunque la marca ya exista, **la ficha se genera igual** antes de cualquier aplicación. Sin
ficha no se hacen moodboard, tablero, empaques ni mockups.

## Paso 1 — Referencias de logo (obligatorio) + datos básicos

Pide las referencias con el mensaje tipo 1 de `referencias-de-marca.md`: **mínimo 3, ideal 3–5
logos** que le gusten, cada uno con una línea de qué le gusta. Ayúdala a encontrarlas, siguiendo la
sección 0 de `logos-profesionales.md`: le das búsquedas listas para copiar en Pinterest y Google según su
nicho y, si tienes búsqueda de imágenes, le muestras ejemplos para que elija. **Pero el paso no se
cierra hasta que ella adjunte o elija sus referencias**: sin referencias de logo no hay exploración.

En el mismo mensaje, pregunta lo mínimo que el logo necesita (preguntas cortas, botones cuando se pueda):
1. **Nombre exacto** (o "propónme opciones") y si lleva descriptor (CAFÉ, STUDIO, LAB).
2. Qué vende o qué hace, y para quién.
3. Cómo se debe sentir (3–4 palabras) y qué **no** quiere parecer.
4. Dónde vive la marca en su tamaño más pequeño (avatar, sticker, sello, bordado).
5. ¿Está registrada? (decide ® o ™).

Con las referencias, entrega su **lectura con psicología inversa enfocada en logo**
(`ingenieria-inversa.md`): arquitectura, tipografía, dispositivo, color, proporción y personalidad de
cada una; qué se toma (ADN) y qué no (firma de esa marca). Breve, en una tabla.

**Puerta:** mínimo 3 referencias de logo adjuntas y los datos básicos respondidos.

## Paso 2 — Exploración de logo: 6 opciones

Ronda 1 de `logos-profesionales.md`: un prompt con **6 opciones de arquitecturas distintas**, nacidas
de sus referencias (cada opción dice qué tomó y qué cambió). Ese prompt también propone la **paleta
del logo** (máximo un acento) y la **tipografía**. Presenta las 6 con tu recomendación marcada.

**Puerta:** la persona elige una opción (o pide otra ronda; si dos opciones salen parecidas, se repite
con otra semilla).

## Paso 3 — Hoja del sistema de logo + ficha de marca

1. **Hoja del sistema de logo** (ronda 2 de `logos-profesionales.md`): primario, secundario, versiones
   de color, monograma y una tinta, con la opción elegida como `@imagen 1`.
2. **Versiones limpias** (ronda 3): el logo aislado sobre fondo liso, que desde aquí será `@imagen 1` en
   todo.
3. **Paleta completa y tipografía** en texto: 5–6 colores con nombre, HEX, rol y razón; proporción de uso
   (ej. 60 / 25 / 10 / 5); pares de texto con contraste ≥ 4.5:1 (si un par no pasa, solo se usa para
   formas); equivalencia CMYK aproximada, avisando que el impresor debe hacer prueba de color. Tipografía
   display + texto (+ etiquetas) disponible en Google Fonts o Canva (`tipografia.md`).
4. **Tagline y textos fijos**: 2–3 opciones de tagline con tu recomendación (`copywriting.md`) y los
   textos que se repetirán (frase de empaque, descriptor).
5. **Antes de cerrar la ficha, pregunta lo que falte** para no inventarlo después:
   - ¿Lleva **ilustración o personaje**? Si sí: estilo y descripción exacta.
   - Si tiene producto físico: **formato del empaque** (tipo, tamaño o peso, acabado, cierre, válvula,
     ventana, dónde va la etiqueta) y **datos fijos por referencia o variedad** (en café: origen,
     variedad, altitud, proceso, notas, peso). Lo que no sepa queda `NOT USED` y no aparece en imágenes.
6. **Ficha de marca bloqueada** (`ficha-de-marca.md`): un resumen corto en español para ella y la ficha
   completa en inglés en un bloque de código.

**Honestidad del logo (dila en una línea):** un logo generado con IA es una base para **vectorizar**
antes de imprimir en grande, y conviene verificar que el nombre y el logo se puedan registrar (en
Colombia, la SIC).

**Puerta:** aprueba la hoja del sistema y la ficha. Desde aquí, todo prompt lleva `@imagen 1` = logo
aprobado y la ficha pegada completa.

## Paso 4 — Referencias de marcas que le gustan

Pide las referencias con el mensaje tipo 2 de `referencias-de-marca.md`: marcas que admira (de
cualquier sector), competencia, empaques o papelería que le gustan, fotografía y mood, lo que **no**
quiere y sus propios activos (fotos del producto, del local, la vitrina). Mínimo 3.

Entrega la lectura con psicología inversa (`ingenieria-inversa.md`) en la tabla de
`referencias-de-marca.md`: qué se toma, qué no, patrón común, tensiones (pregunta cuál gana) y brecha.
Estas referencias dan **atmósfera, fotografía, materiales y estilo de empaque**; el logo, los colores y
los datos ya están fijos en la ficha y **no se cambian** por una referencia.

**Puerta:** mínimo 3 referencias y la lectura confirmada.

## Paso 5 — Moodboard aplicado (con el logo aprobado)

El moodboard presenta la atmósfera de la marca **con su logo real**. Adapta el molde 01 del playbook
(grilla 3×3 en tres filas con un mensaje cada una) con estas diferencias obligatorias:

- `@imagen 1` = logo aprobado. El logo aparece **aplicado** en 2–3 casillas (sello, etiqueta, taza,
  tarjeta, fachada…), idéntico, adaptado solo a la técnica de cada material.
- El resto de casillas cuentan la atmósfera según la lectura del paso 4: producto o materia prima, luz,
  texturas, lugar, gente o ritual.
- **No diseña el empaque final** (eso es el paso 7). Si una casilla muestra un empaque, es el formato de
  la ficha, sin inventar etiqueta.
- Si la marca tiene **personaje**, puede aparecer aquí por primera vez; al aprobarlo, emite la ficha v2
  con esa imagen como `@imagen 2` fija.

```
Create a hyperrealistic 4:5 vertical (1080x1350) brand mood board for "[BRAND NAME]", [one-line brand description]. Every tile must look like a real, unretouched professional photograph from a high-end campaign. The board tells one clear story in three rows: [ROW 1 MESSAGE], then [ROW 2 MESSAGE], then [ROW 3 MESSAGE].
REFERENCE IMAGES — MANDATORY:
@imagen 1 is the EXACT approved logo. Reproduce its letterforms, proportions, spelling, device and colors exactly wherever it appears, adapted only to the printing technique of each material. Do not redraw, restyle or reinterpret it. Do not invent any other logo. Do not copy its background.
[@imagen 2 is the EXACT approved character — only if the brand has one.]
[@imagen N is the EXACT real product: reproduce it exactly where it appears — only if a tile shows the product.]
[BRAND LOCK pegado completo, tal cual]
LAYOUT:
A clean editorial grid of 9 photographs in 3 rows of 3, all the same size, separated by thin consistent gutters on a [background color #HEX] background.
ROW 1 — [MESSAGE]:
1. [Tile: subject, materials, light, lens].
2. [Tile — logo applied: e.g. the logo from @imagen 1 hot-stamped on a kraft label / printed on a ceramic cup], [material details].
3. [Tile].
ROW 2 — [MESSAGE]:
4. [Tile]. 5. [Tile]. 6. [Tile — logo applied].
ROW 3 — [MESSAGE]:
7. [Tile]. 8. [Tile]. 9. [Tile].
MATERIAL HYPERREALISM — MANDATORY:
[Textures per material; the logo adapted to each technique: ink absorbed into kraft, foil reflections, deboss depth].
COLOR PALETTE:
Only the BRAND LOCK colors. No other colors.
CAMERA AND LIGHTING:
[Approved light scheme from the references], consistent lighting direction and color grading across all nine images. Shot on a Hasselblad X2D 100C, [lens per tile], 8K, 16-bit color, true-to-life colors.
[SPANISH TEXT — EXACT RENDERING block, only if a tile shows text; otherwise: The only text in the image is the logo.]
NO provisional or different logo. NO other brands. NO extra text. NO misspelled words. NO missing accents. NO colors outside the palette. NO CGI or render look. NO watermarks.
4:5 vertical, 1080x1350.
```
📎 Adjunta en tu generador: @imagen 1 = logo aprobado (versión limpia) [· @imagen 2 = personaje aprobado] [· @imagen N = foto real del producto]

**Puerta:** aprueba el moodboard.

## Paso 6 — Tablero de identidad

Prompt de `tablero-identidad.md`: layout sacado de sus referencias (A, B o C solo si no trae
referencias de tableros), con `@imagen 1` = logo aprobado, la hoja del sistema de logo y el moodboard
aprobado como referencias, y la ficha pegada. Todos los textos, del corrector y de la ficha.

**Puerta:** aprueba el tablero.

## Paso 7 — Empaques

Sigue la sección "Empaques" de `mockups-y-pop.md`:
1. **Un empaque primero** (la referencia principal), con el formato exacto de la ficha y sus datos fijos.
2. Al aprobarlo, ese empaque entra como referencia de forma y diseño para las demás referencias o
   variedades, que cambian **solo** lo que la ficha dice que cambia (color, nombre y datos de esa
   variedad).
3. Si la persona lo pide: línea completa en una sola foto, empaque secundario (caja, manga, tag), arte
   plano de impresión y ficha técnica para el impresor.

Si es un **servicio sin producto físico**, el paso 7 se vuelve kit de bienvenida, papelería, merch o
presentación comercial, con las mismas reglas.

**Puerta:** aprueba cada empaque antes de pasar al siguiente.

## Después del paso 7 (opcional, solo si la persona lo pide)

Siempre con `@imagen 1` = logo aprobado, la ficha pegada y el corrector:

- **Láminas del playbook que faltan:** producto protagonista (03), paleta en objetos (04), stickers
  plano y en material (05A/05B), estilo fotográfico (06), redes en celular (09). Una a la vez, con
  aprobación.
- **Papelería y material POP:** `mockups-y-pop.md` (mockup, arte plano y ficha técnica), incluso en su
  propio local con una foto real.
- **Brand board final 16:9 tipo bento:** las láminas aprobadas como bloques, más logo, tagline, paleta
  con HEX y tipografías; tarea de diagramación, sin regenerar imágenes aprobadas (molde "BRAND BOARD
  FINAL" del playbook).
- **Sistema visual de contenido:** `sistema-visual.md`.
- **Kit de consistencia / skill de marca:** `skill-de-marca.md`, construido sobre la misma ficha.

## Brand board de cierre (cuando la marca NO se creó aquí)

Si la sesión fue de piezas o campaña con una marca que ya existía, al final ofrece consolidar lo
trabajado (logo, paleta, tipografías, reglas de foto, ficha del modelo, prompts base) en su kit de
consistencia (`skill-de-marca.md`) o en un brand board bento 16:9. Si la marca tiene logo, primero se
arma su ficha (`ficha-de-marca.md`) y el bento lleva ese logo como `@imagen 1`. La ruta de marca hace
*nacer* una identidad; el cierre *consolida* lo trabajado.

## Relación con el playbook

El playbook (`playbook-original.md`, "BRAND BOARD DESDE CERO") trae los moldes 01–10 y su método de
fases con aprobación. **El orden lo manda este archivo**: el logo va primero y el moodboard (molde 01)
sale en el paso 5, con el logo aprobado. Los moldes se adaptan igual que siempre (REGLA #2): 02A →
paso 2 (ampliado a 6 opciones), 01 → paso 5, 07 y 08 → paso 7, el resto → después del paso 7.

## Checklist antes de entregar cada paso

- ¿Estoy en el paso correcto y el anterior quedó **aprobado** de forma explícita?
- ¿Salió algo visual de la marca antes del logo aprobado? Si sí, es error: se retira.
- Desde el paso 3: ¿el prompt lleva `@imagen 1` = logo aprobado, la línea 📎 y la ficha completa en su
  última versión?
- ¿Los datos de producto, el formato del empaque y el personaje son idénticos a la ficha?
- ¿Pasé el corrector de español (ortografía, tildes, mayúsculas acentuadas, unidades, límite de líneas)?
- ¿Las 6 opciones de logo difieren en arquitectura y cada una dice qué tomó de las referencias?
- ¿El logo funciona a 110 px y en una tinta? ¿Tiene monograma?
- **Anti-copia:** si tapas el nombre, ¿se confunde con una referencia o un competidor? Si sí, cambia
  forma, color o tipografía.
- ¿Avisé vectorizar y verificar el registro?
- Al cerrar: ¿ofrecí lo opcional (POP, sistema visual, kit) en una línea, sin empezarlo sin permiso?
