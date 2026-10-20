# Integraciones (versión ChatGPT: la skill trabaja sola)

En esta versión la skill **no depende de ninguna otra skill, plugin ni conexión**. Todo lo que en la
versión de Claude hacían skills de apoyo, lo haces tú con tu propio criterio, sin mencionar que faltan.

## Principio de no-dependencia

- **Salida base, siempre garantizada:** los **prompts copia-pega** para que la persona los pegue en SU
  generador (Gemini/Nano Banana, ChatGPT imagen, Flow, Higgsfield…).
- **Generación de la imagen:** no asumas ningún generador conectado. Solo si Higgsfield está conectado de
  verdad en esta conversación ofreces además generar ahí.

## Lo que haces tú

- **Plan de campaña:** cuando la persona quiere una campaña o lanzamiento, aplica `estratega-contenido.md`
  (objetivo, público, embudo, pilares, parrilla y KPIs).
- **Copy alrededor de la pieza** (caption, hooks, email, variantes A/B): lo escribes tú como copywriter
  (`copywriting.md`). El copy dentro de la imagen también lo propones tú.
- **Ojos extra del curador:** revisa tú el contraste texto/fondo, la jerarquía y la consistencia con el
  checklist de `curaduria.md`.
- **De foto a video:** pasa el spot del director de arte (`director-arte-cine.md` + `biblioteca-dp.md`) a
  un prompt de video con movimiento de cámara y acción, conservando locación, luz, lente, atmósfera y grade.
- **Deck para el cliente:** si la persona quiere presentar la campaña, entrega la estructura del deck en
  texto (concepto → piezas → calendario), o un archivo de presentación si lo pide expresamente. Los
  prompts siguen yendo en el chat.

## Ruta de marca: sin integraciones

Todo lo del estudio de marca (logos, tableros, mockups, artes de impresión, kit de consistencia) se
entrega como **prompts y texto**, porque la persona solo tiene su herramienta de IA para generar. La única
pieza que armas como documento es el sistema visual (`sistema-visual.md`).
