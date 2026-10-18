# Integraciones opcionales (otras skills de Anthropic que elevan el resultado)

Estas skills **suman** cuando están disponibles, pero la habilidad **nunca depende de ellas**. Regla de
oro: intenta usarlas *si existen en el entorno*; si no están, **resuelve igual con tus propias
capacidades** y no menciones que faltan ni falles. No asumas que la persona tiene ningún plugin ni ningún
MCP (Higgsfield incluido).

## Principio de no-dependencia

- **Salida base, siempre garantizada:** los **prompts copia-pega** (y la maqueta/overlay en HTML). Eso
  funciona sin plugins, sin MCP y sin conectores.
- **Generación de la imagen:** NO asumas Higgsfield ni ningún generador conectado. Por defecto entregas
  el prompt para que la persona lo pegue en SU herramienta (Gemini/Nano Banana, Flow, etc.). Solo si
  detectas el Higgsfield MCP (`mcp__Higgsfield__*`) ofreces además generar ahí.
- Si una skill opcional no está, **no la nombres** como faltante: simplemente haz tú esa parte lo mejor
  posible (sabes planear campañas, escribir copy, criticar diseño y armar decks por tu cuenta).

## Las integraciones (qué aporta cada una y cuándo)

**1. Plan de campaña — `marketing:campaign-plan` (si está).**
- Cuándo: la persona no quiere una pieza suelta sino **una campaña/lanzamiento**.
- Aporta: objetivo, público, estrategia de canales, **calendario de contenido** y métricas. Eleva de
  "te hago piezas" a "te armo la campaña" (posicionamiento de agencia).
- Si no está: arma tú un mini-plan (objetivo + público + 1 calendario simple de piezas) con tu criterio.

**2. Copy alrededor de la pieza — `marketing:draft-content` (si está).**
- Cuándo: además del texto EN la imagen, hace falta **caption de Instagram, hooks, email, variantes A/B**.
- Aporta: copy por canal con formato nativo. (El copy dentro de la imagen lo sigue proponiendo esta skill.)
- Si no está: escríbelo tú como copywriter (es una fortaleza propia de la skill).

**3. Ojos extra del curador — `design:accessibility-review` y `design:design-critique` (si están).**
- Cuándo: dentro de la **curaduría** (`curaduria.md`), sobre la maqueta/overlay antes de publicar.
- Aporta: `accessibility-review` mide **contraste texto/fondo real** (refuerza la legibilidad — el caso
  del texto tapado); `design-critique` da feedback de jerarquía, consistencia y usabilidad.
- Si no están: aplica tú el checklist del curador con tu propio juicio de diseño.

**4. De foto a video — `seedance-director` (si está).**
- Cuándo: la persona quiere **animar** una foto/spot (reel, spot de marca, video de producto).
- Aporta: convierte el spot del director de arte (`director-arte-cine.md` + `biblioteca-dp.md`) en guion
  cinematográfico con movimiento de cámara y acción, manteniendo el mismo universo visual de la foto.
- Si no está: redacta tú el prompt de video conservando locación/luz/lente/atmósfera/grade del spot.

**5. Deck para el cliente — Slides / `pptx` (built-in, casi siempre disponible).**
- Cuándo: la persona quiere **presentar la campaña a un cliente/marca** (concepto → piezas → calendario).
- Aporta: cierra ventas mucho mejor que mandar imágenes sueltas. Usa el tipo de artifact Slides si está
  listado; si no, la skill `pptx` para un .pptx.
- Si no aplica: entrega el brief/preview en HTML como hasta ahora.

## Ruta de marca: sin integraciones

Todo lo del estudio de marca (logos, tableros, mockups, artes de impresión, kit de consistencia) se
entrega como **prompts y texto**, porque la persona solo tiene su herramienta de IA para generar. No
dependas ni sugieras plugins, conectores o diseño fuera de su generador para esta ruta. La única pieza
que arma la propia herramienta es el sistema visual (`sistema-visual.md`): página en Claude, documento de
texto en ChatGPT.

## Nota para quien desarrolla/vende la skill (no es parte del flujo del usuario)

Para medir y mejorar la calidad antes de cobrarla, se puede usar `skill-creator` (evals/benchmark) con
casos reales. Eso es trabajo de autor, no algo que la skill invoque durante una sesión normal.
