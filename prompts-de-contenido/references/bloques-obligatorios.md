# Bloques obligatorios (plantillas copy-paste)

Estos bloques se ensamblan dentro de cada prompt. Adáptalos al producto/modelo reales; no cambies su
lógica. Los prompts van en inglés; los textos dentro de la imagen en español y entre comillas.

## 1. PRODUCT ACCURACY (siempre)

```
PRODUCT ACCURACY — ABSOLUTELY NON-NEGOTIABLE:
Use the [product] from @imagen 1 exactly as provided. Preserve its exact [color], [silhouette/shape],
[materials/finish], [logo/label with placement], [distinctive details], with their exact shape, size
and placement. Do not redesign, reinterpret, simplify or invent any part. Do not change the [color].
Do not add other logos, prints or text. Use @imagen 1 ONLY for the product: do not copy its
background, lighting or cropping.
```
Si solo hay una vista, añade: `Show only the front / three-quarter front. Do not show or invent the
back or any detail not visible in the reference.`

## 2. IDENTITY LOCK (si hay persona)

```
MODEL IDENTITY — ABSOLUTELY NON-NEGOTIABLE:
The exact same [woman/man] from @imagen [N]: [age range], [phenotype], [skin tone + undertone],
[freckles/marks], [eye color/shape], [brows], [nose], [lips], [hair color/length/texture], [notable
details]. Minimal makeup, [expression]. Do not beautify, slim, age, smooth or reshape. Do not remove
freckles/marks. Do not straighten or recolor the hair. Do not change the eye color. Use @imagen [N]
ONLY for identity: do not copy its background, lighting, cropping or clothing.
```
En UGC/híbrido corren **dos anclas en paralelo**: identity lock (fotos del modelo) + product lock
(foto del producto), cada uno con sus referencias.

## 3. HIPERREALISMO (CONDICIONAL — solo si el medio es foto hiperrealista)

⚠️ Primero decide el **medio/estética** (ver `estetica-y-medio.md`). Este bloque aplica **solo** cuando
la pieza es **fotografía hiperrealista**. Si el medio es **gráfico/editorial/collage/zine/mixto**, NO
uses este bloque: usa en su lugar el bloque de textura/imperfección de §3b. La fidelidad de producto y la
identidad del modelo se mantienen en ambos casos.

```
SKIN & MATERIAL HYPERREALISM — MANDATORY:
Raw, unretouched skin with visible pores, fine vellus peach fuzz, natural texture and small
imperfections, freckles intact where present; individual eyebrow/lash hairs; natural lip texture.

MATERIAL REALISM — per surface, never one global finish:
Give EACH material its own distinct texture and reflectance — never share the same smoothness or
sharpening across the whole image. [fabric: visible weave/knit + natural creasing] · [denim/canvas:
worn fading, seams, stitching] · [suede: directional fibers, irregular nap] · [mesh: woven structure]
· [leather: grain + soft specular] · [rubber/sole: micro-scuffs, reflectance different from fabric] ·
[concrete/wall: pores, tonal variation, small stains, irregular roughness] · [metal/glass: true
specular] · [food: wet gloss vs dry crumb]. Keep visible stitching and realistic reflections.

CAMERA CHARACTER: real full-frame capture, natural optical sharpness on the subject, realistic
highlight roll-off, subtle sensor noise in shadow areas, slight lens falloff at the edges. Minimally
processed RAW look, true-to-life colors. Photographed, not rendered.

NO airbrushing. NO skin smoothing. NO beauty filter. NO waxy or plastic skin. NO porcelain look.
Resolution / "hyperreal" wording alone does NOT create realism — it must come from the per-material
texture above. NO clarity filter. NO global smoothing or uniform sharpening across the whole image.
NO HDR glow. NO CGI or 3D render look. NO over-polished advertising gloss.
```
Cámara/luz reales según la toma: Hasselblad X2D 100C + XCD 120mm macro (texturas), 90mm (retrato/
producto), 55mm (escena), 28mm (gran angular); flash duro Profoto (B10X/D2) con sombras nítidas +
relleno suave — **salvo** que la paleta pida otra luz (ver §4). Para UGC usa cámara de smartphone
(iPhone 16 Pro, 24–26mm, grano natural). Para look film nombra la película (Portra 400, etc.).

➕ **Playbook de realismo (solo piezas):** para piezas fotográficas —con o sin persona— apóyate en
`realismo-fotografico.md` y escribe en el prompt las reglas que ese caso necesite: **jerarquía de
nitidez** (sujeto/producto nítidos, fondo y bordes más suaves), **microcontraste por material** (pelo
con hebras, piel con poros sutiles no "crunchy", caucho más liso, fondo con menos detalle), **física de
luz** (una dirección clara, sombras densas creíbles con penumbra, roll-off natural, sin HDR ni rim
falso) e **imperfección lógica** (arrugas de tela, micro-rayones, concreto imperfecto — nunca daño
aleatorio). Léelo como guía; **no pegues ese documento entero en el prompt**. Recuerda: "premium" no es
superficie pulida, es dirección de arte + luz + materiales reales.

## 3b. ESTÉTICA GRÁFICA / EDITORIAL (cuando el medio NO es foto limpia)

Para piezas gráficas/editoriales/collage/zine/mixtas, reemplaza el bloque de hiperrealismo por dirección
de **medio diseñado** (ver `estetica-y-medio.md`). En el prompt pide, según el caso:
```
MEDIUM & TEXTURE — [editorial poster / collage-zine / grunge / mixed media]:
Designed graphic piece, not a clean photo. [film grain / photocopy texture / torn & taped paper /
halftone / overprint misregistration / ink bleed / stains / scanlines / cutout layering]. Layered
composition with overlaid graphic elements and pasted typography. Aggressive, intentional layout:
[dutch angle / cropped framing / asymmetry / extreme scale]. A specific, strange, memorable moment
(not a generic pretty scene).
```
Mantén: fidelidad de producto, identidad del modelo, textos (según modo), color por roles. Evita el
render 3D genérico ("NO generic 3D render") salvo que la estética elegida sea 3D a propósito.

## 4. SISTEMA DE COLOR POR ROLES + AUTO-DIRECCIÓN

```
COLOR:
[Dominant/background color] dominant, [architecture/typography color], [accent color] accent. The
only [hero color] belongs to the [product]. Do not introduce [hero color] anywhere else, and do not
introduce [other colors] in the environment or typography.
```
- El **color héroe** se reserva SOLO al producto (comida cálida, buzo amarillo, etc.).
- La paleta **dirige la luz**: fondo oscuro/low-key → luz lateral/rim cálida, NO flash plano frontal
  ("NO flat frontal flash"); fondo claro saturado → flash duro directo que hace "pop".
- El **mismo sistema se repite** en toda la serie; cada pieza varía escena, encuadre y copy pero
  conserva paleta + locks. Auto-dirección de escenas: entornos, poses y luces distintas entre piezas,
  nunca dos iguales.

## 5. TEXTOS Y PRECIOS EXACTOS (según el MODO DE TEXTO elegido — ver `modo-texto.md`)

Regla de toda la skill: los textos en español van **con ortografía completa** (tildes, Ñ, mayúsculas
acentuadas, ¿ ¡), dentro del **límite de líneas** de cada pieza y con las unidades bien escritas. El
detalle y la revisión obligatoria están en `corrector-espanol.md`. **Nunca se quitan tildes ni Ñ.**

**Modo A (sin texto en la imagen):** el prompt pide la imagen **limpia** (`no text, no typography, no
watermark`, salvo logos o grabados que ya están en el producto). Aparte, entrega la **hoja de texto para
Canva** por cada pieza, con los textos ya corregidos:
```
HOJA DE TEXTO (para Canva):
Titular: "TEXTO EXACTO" — fuente [Display], color [#HEX], posición [arriba/centro…]
Bajada: "…" — fuente [Body], color [#HEX]
Precio/CTA: "$XX.XXX" / "PÍDELO YA" — fuente/ubicación
```

**Modo B (texto en la imagen):** incluye el bloque fijo de `corrector-espanol.md`:
```
SPANISH TEXT — EXACT RENDERING — MANDATORY:
Render ONLY the texts listed below, in Spanish, exactly as written between quotes, character by character. Keep every accent mark (Á É Í Ó Ú), the Ñ and the opening marks ¿ ¡, also on UPPERCASE letters (CAFÉ, NARIÑO, AÑO). Do not translate, do not drop or move accents, do not change letters, do not add any other word, letter, number or symbol.
- [Rol y ubicación]: "TEXTO EXACTO"
- [Precio dentro de badge]: "$XX.XXX"
No other text anywhere in the image.
The price must read exactly: dollar sign, [dígitos deletreados], period, [dígitos]. The period is a thousands separator.
```
Las palabras con tilde o Ñ se deletrean la primera vez, indicando dónde va la marca (`"NARIÑO"
(N-A-R-I-Ñ-O, with a tilde over the N)`). Cierra con `NO misspelled words. NO missing accents. NO extra
text.`

**Modo C (overlay por Claude):** genera el prompt como Modo A (imagen limpia) y, con la imagen ya
generada, Claude compone el texto encima con las fuentes exactas y la misma ortografía.

**Si hay marca con ficha** (`ficha-de-marca.md`): los textos salen de la ficha (APPROVED SPANISH TEXTS y
FIXED PRODUCT DATA), copiados carácter por carácter.

## 6. HEADER / watermark (OPCIONAL — solo con datos del usuario)

Úsalo **solo si la persona quiere un header/watermark propio y te dio su @ y/o rótulo**. Si no, omite
este bloque: la pieza va sin header. Los textos de abajo son *placeholders*: reemplázalos por lo que la
persona dé. **Nunca** uses un handle o rótulo que no te dieron (no asumas "@SOYGERALDINEACOSTA.IA" ni
"CONCEPTO CREATIVO IA" — esos son ejemplos de la autora del playbook, no un valor por defecto).

```
MANDATORY HEADER:
Upper-left: "<ROTULO DEL USUARIO, si lo quiere>"
Upper-right: "<@HANDLE DEL USUARIO>"
Identical position, scale and treatment across every piece in the series.
```

## 7. AVOID / negative (cierre)

```
NO CGI. NO plastic food/skin. NO face alteration. NO removed freckles. NO distorted anatomy. NO extra
fingers. NO warped clothing. NO incorrect/invented logo. NO wrong product color. NO misspelled words.
NO missing accents. NO extra text. NO other brand logos. [aspect ratio].
```

## 8. Etiquetado de referencias

Nombra las fotos `@imagen 1, @imagen 2…` en el orden en que las adjunta la persona, y di al inicio del
prompt qué es cada una y para qué se usa (producto / identidad / proporciones / expresión / ángulo).
Si el generador no usa @, se adjuntan en el orden que el prompt menciona.
**Excepción — marca con ficha de marca:** el orden es fijo (`ficha-de-marca.md`): `@imagen 1` = logo
aprobado, `@imagen 2` = personaje aprobado (si hay), y después lo propio de cada prompt.

## 9. BRAND LOCK (si la marca tiene ficha de marca)

Cuando la marca ya tiene logo aprobado y ficha, **todo prompt** de esa marca lleva:
- `@imagen 1` = logo aprobado, versión limpia, con su línea 📎;
- la **ficha de marca completa** (`ficha-de-marca.md`), pegada tal cual justo después de las imágenes de
  referencia, en su última versión.

```
REFERENCE IMAGES — MANDATORY:
@imagen 1 is the EXACT approved logo. Reproduce it identically, adapted only to the printing technique of each material. Never redraw, restyle, replace it or invent a provisional logo. Do not copy its background.
[BRAND LOCK — "[BRAND NAME]" — v[N] — pegado completo]
```
Logo, colores, tipografía, personaje, formato del empaque y datos de producto **no se reescriben** en el
resto del prompt: se toman de la ficha.

