# Preview visual — tablero de opciones (para que la persona ELIJA mirando, no leyendo)

Principio: a la gente no le gusta leer briefs largos. Antes de generar prompts, **muéstrale un tablero
visual** con 2–3 direcciones y deja que elija con el ojo. Aplica a **todos los nichos**, no solo moda.

El preview tiene **dos momentos** (no mezclarlos):
- **Momento 1 — tablero de direcciones:** 2–3 direcciones distintas para que elija el rumbo (concepto +
  paleta + letras + medio). Es lo de más abajo en "Qué es".
- **Momento 2 — maqueta de la pieza + variantes de paleta:** una vez eligió dirección, muéstrale **cómo
  quedaría la pieza real** (maqueta a tamaño correcto, y cada slide si es carrusel) y ofrécele **2–3
  variantes de esa misma paleta** para afinar. Ver secciones "Maqueta de la pieza" y "Variantes de la
  paleta elegida". Recién después de esto generas los prompts.

Honestidad: la maqueta es un **montaje de diseño en HTML/CSS** que aproxima la pieza (composición, color,
tipografía, dónde va el texto y el producto) — **no** es la imagen final del generador. Sirve para que la
persona apruebe el layout y el sistema mirando, antes de gastar generaciones. Dilo así de claro.

## Qué es

Un **artifact HTML autónomo** (una sola página) titulado "Tablero de opciones — <producto/marca>", con
2–3 tarjetas de **dirección creativa** lado a lado. Cada tarjeta muestra, de forma visual:

1. **Nombre del CONCEPTO + 1 línea de gran idea + MEDIO** (no solo una vibra). Ej.: "Entrega épica —
   helicóptero sobre la ciudad · foto hiperreal" / "Zine paranormal — póster rasgado estilo periódico
   vintage · collage/grunge". Incluye **al menos una de alto concepto** (`conceptos-creativos.md`) y,
   cuando las referencias lo sugieran, **al menos un medio NO fotográfico** (editorial/collage/mixto;
   ver `estetica-y-medio.md`). No ofrezcas solo "fotos bonitas".
2. **Paleta por roles:** fila de muestras de color (swatches) con su **HEX** y su rol debajo
   (fondo · tipografía · acento · héroe del producto).
3. **Tipografía en vivo:** el titular renderizado grande + el cuerpo, **cargando las fuentes reales con
   Google Fonts** (`<link>` a fonts.googleapis.com), con el nombre de cada fuente. Así la persona *ve*
   la combinación de letras, no la imagina.
4. **Mini-mockup aplicado:** una miniatura de pieza (un rectángulo 4:5) compuesta con esa paleta +
   esas fuentes + un placeholder del producto (silueta/caja o, si hay, la foto del producto), para que
   vea el sistema *aplicado*.
5. **(Opcional) Tira de referencias:** 2–3 miniaturas o enlaces reales obtenidos con **búsqueda de
   imágenes** (ver abajo). Si no se pueden incrustar con fiabilidad, usa "chips" descriptivos + enlaces.

Cierra con una línea: "Elige 1, 2 o 3 — o combina (ej. paleta de la 1 + letras de la 3)".

## Cómo construirlo

- Publícalo con la herramienta de artifacts (HTML de un solo archivo). Fuentes: solo Google Fonts.
- Hazlo responsive (se ve en celular), con buen contraste, y **sin texto largo** — es para mirar.
- Las paletas y fuentes salen del research + `tipografia.md` + `nichos.md`. Las 2–3 direcciones deben
  ser **distintas entre sí** (no el mismo mood), y reflejar la marca real y las tendencias reales (ver
  `investigacion-mercado.md`, regla anti-default).
- Deja el HEX visible en cada swatch (la persona a veces lo copia a Canva).
- Si el entorno no permite artifacts, cae a un preview compacto: nombres de dirección + swatches en
  bloque de código + nombres de fuentes + enlaces de referencia. Dilo con honestidad.

## Referencias visuales (todos los nichos)

- Usa **búsqueda de imágenes** (si está disponible) para traer referencias reales del nicho/marca/
  tendencia — sirve para moda, comida, mascotas, inmobiliaria, salud, belleza, etc.
- **Pinterest** es buena fuente de inspiración, pero la skill **no puede navegarlo por dentro** (login/
  bloqueo). No prometas "busqué en Pinterest"; si quieres, sugiere a la persona un término de búsqueda
  de Pinterest y/o pídele que pegue un par de pins como referencia.
- Las referencias son **apoyo**; el preview confiable y fuerte son paleta + tipografía + mini-mockup.

## Maqueta de la pieza (ver cómo quedaría antes de generar)

Después de que elige dirección, no saltes directo a los prompts: **muéstrale la pieza compuesta** en un
segundo artifact (o una segunda sección del mismo) titulado "Maqueta — <producto/marca>". Es el mismo
mini-mockup, pero **en grande y terminado**, para que juzgue el resultado mirando.

- **Tamaño real del destino:** 4:5 o 1:1 para post, 9:16 para story/reel, 16:9 para banner. Usa la
  proporción del formato elegido (`formatos-anuncio.md`), no un cuadro genérico.
- **Compuesta de verdad:** fondo con el color de rol, **la foto real del producto** si la subió (o
  silueta/caja si no), el **titular/bajada/CTA en su posición** con las fuentes reales (Google Fonts en
  vivo), jerarquía y aire como diseñador (`diseno-tipografico.md`). El texto es el **copy que TÚ
  propones**, no "lorem ipsum".
- **Carrusel = una maqueta por slide:** muestra las 3–6 slides en fila (portada → desarrollo → cierre/
  CTA) para que vea el hilo visual y el reparto de texto por slide. Numéralas.
- **Respeta el MEDIO:** si la dirección es editorial/collage/grunge, la maqueta también lo es (textura,
  capas, recortes) — no una foto limpia (`estetica-y-medio.md`).
- **Qué NO es:** no es la imagen del generador ni un render fotográfico; es el **layout aprobable**.
  Dilo en una línea y aclara que al generar, la foto/escena la produce el generador siguiendo el prompt.

Cierra con: "¿Apruebas esta maqueta, cambias algo (color, letra, posición del texto) o vemos variantes
de paleta?". Cuando aprueba, ese layout es el molde de los prompts.

## Variantes de la paleta elegida (afinar sin cambiar de dirección)

Si la persona ya eligió paleta pero quiere ver opciones, ofrécele **2–3 variantes de esa MISMA paleta**
(no paletas nuevas) sobre la maqueta, lado a lado, para que compare mirando:

- **Clara vs oscura:** mismo sistema en fondo claro y en fondo oscuro (modo día / modo noche).
- **Saturada vs apagada:** acentos vivos vs versión más sobria/premium.
- **Reparto de roles:** qué color manda como fondo y cuál como acento (intercambiar fondo↔acento), o
  cuánto peso tiene el acento (fondo neutro con un solo golpe de color vs bloques de color).
- **Regla fija:** el **color héroe del producto NO cambia** entre variantes (sigue reservado al
  producto; `COLOR` en `bloques-obligatorios.md`). Solo varían fondo, tipografía y acento.
- Muestra el **HEX** de cada variante (lo copia a Canva) y nómbralas ("A clara / B noche / C sobria").

Esto también sirve si no eligió aún: presenta 2–3 repartos de la paleta sugerida y deja que elija el que
mejor se ve aplicado, no en abstracto.

## Selector de tipografías (5 combos renderizados — elige mirando)

Igual que con la paleta, no describas las letras: **muéstralas**. En la maqueta (o una sección aparte del
artifact) presenta **5 combinaciones** de tipografía (titular + cuerpo) **renderizadas en vivo con Google
Fonts** (`<link>` a fonts.googleapis.com), aplicadas al titular/bajada real de la pieza, para que la
persona elija con el ojo.

- **Cada combo es una tarjeta** con: el titular grande en la fuente display, una línea de cuerpo en la
  fuente de apoyo, y debajo **los nombres** ("Anton / Inter") para copiar a Canva.
- **5 opciones variadas, no 5 parecidas:** sácalas de familias distintas acordes al nicho/medio/concepto
  (ver `libreria-fuentes.md` y `tipografia.md`). Ej. para algo joven: una condensada de impacto, una
  grotesca moderna, una serif editorial con contraste, una display con carácter y una redondeada —
  cada una da una personalidad distinta a la misma pieza.
- **Marca TU recomendación:** señala 1 combo como "⭐ Recomendado" y di en una línea **por qué** encaja
  (con el nicho, la marca real, el concepto o la tendencia investigada). La persona decide, pero con tu
  criterio de diseñador al frente — no la dejes sola ante 5 opciones mudas.
- **Respeta las reglas de pareo** (`tipografia.md`): máximo 2 familias por combo, contraste real, y si la
  marca tiene fuente propia, ese combo va primero y marcado como el de marca.
- **Render honesto:** en el overlay/preview estas fuentes se ven de verdad (Google Fonts en vivo). En el
  prompt para el generador la letra se *describe* y el generador la aproxima; el nombre exacto sirve para
  Canva. Dilo claro.

Cuando elige combo, ese es el bloqueado para toda la campaña (titulares y cuerpo), junto con la paleta.

## Después de elegir

Cuando la persona elige (o combina) dirección, maqueta, variante de paleta y combo tipográfico, **fija
ese sistema** (paleta por roles + combo tipográfico + dirección + layout de la maqueta) y úsalo como el
sistema bloqueado de toda la campaña. Ese mismo sistema alimenta luego el brand board de cierre. Recién
ahí generas los prompts.

## Ejemplo de estructura HTML (guía, no copiar literal)

```html
<!doctype html><html lang="es"><head><meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Tablero de opciones</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Anton&family=Inter:wght@400;700&family=Fraunces:wght@400;600&display=swap" rel="stylesheet">
<style>/* grid de 3 tarjetas, swatches con su HEX, titular con la fuente display, mini-mockup 4:5 */</style>
</head><body>
  <!-- Tarjeta 1: nombre+vibra · swatches(HEX+rol) · titular en fuente real · mini-mockup · refs -->
  <!-- Tarjeta 2 ... Tarjeta 3 ... -->
  <!-- Pie: "Elige 1, 2 o 3 — o combina" -->
</body></html>
```
