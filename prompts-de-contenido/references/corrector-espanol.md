# Corrector de español (aplica a TODA la skill)

Todo texto en español que produce la skill sale **con ortografía completa**: tildes, Ñ, mayúsculas
acentuadas, signos de apertura (¿ ¡) y unidades bien escritas. Aplica a:

- textos que van **dentro de la imagen** (prompts de piezas, logos, tableros, empaques, mockups, POP);
- **copys** (titular, bajada, CTA), **captions** y **hojas de texto para Canva**;
- **prompts de corrección**.

> ⛔ Ya no existe la regla de "evitar tildes y Ñ en textos grandes". Quitar tildes no evita errores:
> los crea ("NARINO", "CAFE"). El texto se escribe correcto y se le ordena al generador reproducirlo
> exacto.

## 1. Cómo va el texto dentro de cada prompt

- Cada texto visible va **entre comillas**, en español, escrito exactamente como debe verse.
- Todos los textos de la pieza se listan en **un solo bloque**, con su rol y su posición.
- Las palabras con tilde o Ñ se deletrean en el prompt la primera vez que aparecen, indicando dónde
  va la marca: `"NARIÑO" (N-A-R-I-Ñ-O, with a tilde over the N)`.
- En piezas de marca, los textos salen **solo** de la ficha (`ficha-de-marca.md`): APPROVED SPANISH
  TEXTS y FIXED PRODUCT DATA, copiados carácter por carácter.

Bloque fijo (en inglés; pégalo en cada prompt que tenga texto):

```
SPANISH TEXT — EXACT RENDERING — MANDATORY:
Render ONLY the texts listed below, in Spanish, exactly as written between quotes, character by character. Keep every accent mark (Á É Í Ó Ú), the Ñ and the opening marks ¿ ¡, also on UPPERCASE letters (CAFÉ, NARIÑO, AÑO). Do not translate, do not drop or move accents, do not change letters, do not add any other word, letter, number or symbol.
- [Role and position]: "[TEXT]"
- [Role and position]: "[TEXT]" ([L-E-T-T-E-R-S], with [the accent over the É / a tilde over the N])
- [Role and position]: "[TEXT]"
No other text anywhere in the image.
```

Y al cierre del prompt, siempre: `NO misspelled words. NO missing accents. NO extra text.`

Los precios se deletrean dígito por dígito: `"$45.000" — dollar sign, 4, 5, period, 0, 0, 0. The period
is a thousands separator.`

## 2. Límite de líneas por pieza (menos texto, menos errores)

| Pieza | Máximo de líneas de texto | Qué va |
| --- | --- | --- |
| Frente de empaque | 5 | marca (logo) · nombre o variedad · origen · notas · peso |
| Reverso o etiqueta técnica | 6 | origen · variedad · altitud · proceso · notas · peso o tostión |
| Post, anuncio o slide de carrusel | 3 (+ precio si aplica) | titular · bajada · CTA |
| Sticker, sello, hablador, wobbler | 2 | frase corta |
| Hoja de logo y tablero de identidad | lista cerrada de máximo 25 cadenas (sin contar HEX ni nombres de fuentes) | etiquetas, nombre, tagline, nombres de color |

- Cada línea, **máximo unas 6 palabras**; un titular, máximo 5.
- Si hace falta más texto, **no se amontona**: se divide en más piezas o se lleva al caption o a Canva.
- Los datos técnicos (altitud, proceso) no compiten con el frente: van al reverso o a una etiqueta
  aparte, salvo que la persona pida lo contrario.

## 3. Unidades, números y formatos

| Dato | Se escribe | Nunca |
| --- | --- | --- |
| Altitud | `1.900 msnm` (metros sobre el nivel del mar) | MSN, m.s.n.m, msn, 1900msnm |
| Peso | `250 g`, `1 kg` (espacio, sin punto, minúscula) | 250gr, 250 G, 250grs, 1 KG. |
| Volumen | `500 ml`, `1 l` | 500ML, 500 mls |
| Temperatura | `92 °C` | 92 grados C, 92ºc |
| Porcentaje | `100 %` o `100%` (el mismo en toda la marca) | mezclar ambos |
| Miles | punto: `1.900`, `45.000` | coma: 1,900 |
| Decimales | coma: `4,5` | punto: 4.5 |
| Precio | `$45.000` | $45000, $45,000 |

La forma exacta de cada unidad se fija **una vez en la ficha** y se copia igual en toda la marca. Si la
persona escribe la unidad de otra forma, se le propone la correcta en una línea y se usa la que apruebe.

## 4. Mayúsculas acentuadas y palabras trampa

En español **las mayúsculas llevan tilde**: CAFÉ, NARIÑO, AÑO, TOSTIÓN. Palabras que más se dañan:

- **Café y proceso:** CAFÉ, TOSTIÓN, CATACIÓN, AROMÁTICO, CÍTRICO, BORBÓN, AZÚCAR, PANELA, LIMÓN,
  MANÍ, CARAMELO, DURAZNO, JAZMÍN, EDICIÓN, ÚNICO, PEQUEÑO, PRODUCCIÓN, ORIGEN (sin tilde), LAVADO,
  NATURAL, HONEY, CASTILLO, CATURRA, GEISHA.
- **Regiones de Colombia:** NARIÑO, BOYACÁ, QUINDÍO, BOGOTÁ, MEDELLÍN, POPAYÁN, IBAGUÉ, CÚCUTA;
  sin tilde: HUILA, CAUCA, TOLIMA, CALDAS, RISARALDA, ANTIOQUIA, SANTANDER, CUNDINAMARCA.
- **Generales:** AÑO, MAÑANA, ESPAÑA, SEÑOR, NIÑOS, DISEÑO, CAMPAÑA, MÁS (cantidad) / MAS (pero),
  SÍ (afirmación) / SI (condición), TÚ / TU, ÉL / EL, ¿…? y ¡…! completos.

Si dudas de una palabra, **verifícala** antes de entregar; nunca la escribas sin tilde "por si acaso".

## 5. Revisión obligatoria antes de entregar cualquier cosa

Pasa este control sobre **cada texto** de prompts, copys, captions, hojas de texto y correcciones:

1. **Ortografía:** cada palabra bien escrita, letra por letra.
2. **Tildes y Ñ:** presentes donde van, también en mayúsculas.
3. **Signos:** ¿ ¡ de apertura; comillas cerradas; sin dobles espacios.
4. **Unidades y números:** según la tabla de la sección 3 y la ficha.
5. **Coherencia con la ficha:** cada nombre, dato de producto y texto aprobado es **idéntico**
   carácter por carácter a la ficha y corresponde a la referencia correcta (no mezclar variedades).
6. **Límite de líneas** de la sección 2.
7. **El bloque SPANISH TEXT — EXACT RENDERING** está en el prompt y el cierre incluye
   `NO misspelled words. NO missing accents. NO extra text.`

Si algo falla, corrígelo antes de mostrarlo. En la línea de "revisé esto" de la curaduría, nombra este
control en pocas palabras (por ejemplo: "Revisé ortografía, tildes, unidades y datos contra la ficha").

## 6. Si el generador escribe mal un texto (prompt de corrección)

No se regenera toda la pieza ni se quita la tilde: se corrige solo el texto dañado.

```
Edit @imagen 1: change ONLY the text "[WRONG TEXT]" so it reads exactly "[CORRECT TEXT]" ([L-E-T-T-E-R-S], with [the accent over the É / a tilde over the N]). Keep the same font, size, color, position and everything else in the image pixel-identical. Do not add any other text.
```
📎 Adjunta en tu generador: @imagen 1 = la imagen con el error

Ejemplo: `change ONLY the text "NARINO" so it reads exactly "NARIÑO" (N-A-R-I-Ñ-O, with a tilde over the N)`.

Si después de dos intentos sigue saliendo mal, dilo con honestidad y ofrece poner ese texto en Canva
con la hoja de texto (modo A de `modo-texto.md`), **escrito correctamente**.

## 7. Copys y captions

- Se escriben en español natural, con la misma ortografía completa.
- Los datos de producto que aparezcan en un caption (origen, altitud, proceso, notas) salen de la
  ficha, iguales.
- Las hojas de texto para Canva llevan cada texto exacto, con tildes, más fuente, color HEX y posición.
