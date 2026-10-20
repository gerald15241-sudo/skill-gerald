# Menú de formatos de anuncio

La skill cubre un abanico de formatos tipo "estudio de anuncios" (inspirado en lo que ofrecen
plataformas como Higgsfield). Para cada uno produce **prompts profesionales listos**; y cuando el
Higgsfield MCP esté conectado en la sesión, puede **ejecutarlos directo** (ver abajo). Elige el formato
desde el brief creativo y ofrécelo en el intake.

## Estáticos (imagen)

- **Ángulos de campaña (Ad Strategist):** a partir de la investigación, genera varias versiones del
  mismo producto explorando *ángulos distintos* (beneficio, problema→solución, estatus, precio,
  comunidad). Cada ángulo = su prompt.
- **Multiplicador de titulares (Headline Multiplier):** mismo visual, varios titulares para testear.
  Entrega el prompt del visual + N opciones de copy/titular.
- **Voz del cliente (Customer Voice Ads):** piezas construidas desde testimonios/lenguaje real del
  cliente (la persona los aporta o se sugieren con base en research).
- **Product shots (solo producto):** hero monocromo, low-key de lujo, lifestyle, flat lay, macro de
  detalle. Ver registros en `references/registros.md`.
- **Promo / venta:** precios, badges, combos, 2x1, happy hour, domicilio (estilo EAT AND JOY del
  playbook). Precios deletreados exactos.

## Video / motion

- **Hooks de apertura (Hook Multiplier):** varias aperturas distintas para el mismo video/para la
  slide 1 de un carrusel, para testear atención.
- **Prompts de video** (para Flow, Higgsfield, Seedance): describe toma, movimiento de cámara, acción,
  ritmo. Los guiones de video estilo Seedance los escribes tú.
- **UGC en video:** review de producto, unboxing, try-on, tutorial/demo — estilo creador, con el
  modelo consistente (ver `references/modelo-ugc.md`).
- **Talking avatar / lipsync:** vocería a cámara; si se usa Higgsfield, su Lipsync Studio.

## Adaptación

- **Redimensionar (Ad Resizer):** la misma pieza en varios aspect ratios manteniendo el foco en el
  producto: 4:5 (feed), 1:1 (feed/catálogo), 9:16 (stories/reels/TikTok), 16:9 (web/YouTube).
- **Localizar (Ad Localizer):** adaptar copy y detalles a otro mercado/idioma conservando la marca.

## Specs por plataforma (aplícalas al prompt)

- Instagram feed: **4:5** (o 1:1). Stories/Reels/TikTok: **9:16**. Catálogo/web: **1:1 / 16:9**.
- Ads vs. orgánico: en ads, copy más directo + CTA claro + espacio para texto; en orgánico, más
  storytelling. Define esto desde el brief.

## Ejecución directa con Higgsfield (si está conectado)

Si la sesión tiene las herramientas `mcp__Higgsfield__*`, además de entregar el prompt puedes
**generar** la pieza: `generate_image` / `generate_video`, o `show_marketing_studio_v2` para
UGC/ads/posters. Para recetas con nombre (product-shot, motion, etc.) sigue las instrucciones del
servidor Higgsfield (get_presets / get_preset_instructions). Media local: usa el widget de subida del
propio Higgsfield, no rutas del sistema. Si no está conectado, entrega los prompts copia-pega — que es
la salida por defecto de esta skill.
