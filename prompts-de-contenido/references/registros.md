# Registros / estilos de pieza

El **registro** (no el enfoque) define el *lenguaje visual*. Ofrécelo siempre en el intake. Enfoque
(quién aparece: producto/UGC/híbrido) y registro (cómo se ve) son dimensiones distintas. Ejemplos
textuales completos de cada uno están en `playbook-original.md`.

## 1. Editorial de campaña (estilo Nautica)

Pósters de campaña de alto nivel. No es "foto de celular": es arquitectura escultórica, tipografía
monumental detrás del modelo (sin taparle la cara), serie con metadata ("ARCHIVO 01"), color héroe
reservado al producto. Ideal para moda/calzado y marcas *heritage*.

Serie típica de ~10 pósters (adáptala): Hero · Colección 2x2 · Movimiento · Detalle/desde el suelo ·
Declaración de marca · Todos los ángulos (frente/3-4/espalda) · Actitud (tipografía apilada) ·
Sistema de la prenda (flat lay) · Historia del material (macro) · Cierre.

Estructura de cada póster: REFERENCE IMAGES (mapeo @imagen) → TEXT LANGUAGE → PRODUCT ACCURACY →
MODEL IDENTITY → STYLING → POSE → ENVIRONMENT → COMPOSITION → HEADLINE/SECONDARY → HEADER → COLOR →
PHOTOGRAPHY → NO/avoid. Relación 3:4 o 4:5.

## 2. Product board (sesión de fotos de producto)

Sesión completa producto + modelo, "de acuerdo a la tendencia del mercado". Dos sub-sesiones:
- **Por locaciones** (estilo L1–L10): escenas reales acordes a la marca (sendero, muelle, café,
  calle…) + tomas de solo-detalle y solo-producto.
- **Fondo neutro** (estilo N1–N10): estudio, poses y ángulos variados sobre fondo de papel liso.

Usa el **prompt-director** del playbook (ROLE → INPUTS → STEP 1 analizar referencias con model lock y
product lock → STEP 2 aplicar tendencias → STEP 3 estructura de 10 tomas → STEP 4 escribir cada
prompt con el formato fijo → STEP 5 output). Pídele que, tras analizar, haga las preguntas que
falten o complete los corchetes. Mínimo 3–5 fotos del modelo + 1 foto del producto (más si tiene
detalles).

También existe la variante **solo producto** (sin modelo): pide N prompts en contextos distintos
emulando una sesión de producto (hero monocromo, low-key de lujo, lifestyle, flat lay, macro…).

## 3. UGC candid

Estética "tomada con celular": luz natural, encuadre candid, un solo sticker de texto, se siente
auténtico y no como anuncio. Doble ancla (identity + product). Para consistencia, **genera la slide
1 primero y úsala como @imagen de referencia** en las siguientes. Cámara de smartphone, grano
natural. No subir fotos del modelo riendo si la acción ya cambia la expresión (deforma la cara).

## 4. Promo social / venta

Piezas de venta directa: precios, badges starburst, damero, tipografía bubble/condensada gigante,
sparkles. Estructura tipo EAT AND JOY (lanzamiento, precio individual, combo, 2x1, happy hour, menú
en historias, UGC mordida, nocturno, domicilio, combo grupal). Precios deletreados dígito por dígito.
Aquí es donde entran promociones; si la persona no las tiene, sugiérelas.

## 5. Avatar / personality board

Genera el modelo consistente antes del UGC (ver `modelo-ugc.md`). Personality board en una imagen
(grid de ~8 paneles) o imagen por imagen (ángulos y expresiones), con identity lock y negative
prompt.

## 6. Brand board

Desde cero (la ruta de marca de 7 pasos, con el logo primero) o de cierre, con sus aplicaciones
(empaques, mockups y material POP). Ver `estudio-de-marca.md`, `ficha-de-marca.md` y `mockups-y-pop.md`.

---

**Regla de scope:** para moda/calzado, la salida por defecto es la **sesión** (avatar → pósters →
product board), entregada por bloques, no una pieza suelta. Deja que la persona recorte.
