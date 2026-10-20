# Kit de consistencia (skill de marca): que sus imágenes salgan siempre iguales

Cuando una marca queda aprobada (fin del estudio de marca, o una campaña con paleta, modelo y producto
bloqueados), **ofrécele su kit de consistencia**. Es lo que hace que cada imagen nueva que genere en SU
herramienta de IA salga con el mismo logo, colores, luz, modelo y producto, sin volver a explicar nada.

## Cuándo ofrecerlo (una sola vez, en una línea)

- Después del paso 7 del estudio de marca, si la persona lo pide (`estudio-de-marca.md`).
- Al cerrar una campaña o sesión con modelo (identity lock), producto (product lock) y paleta bloqueados.
- Cuando diga "quiero que siempre me salga igual" o "lo voy a usar todos los meses".

Mensaje tipo: "Tu marca ya tiene sus reglas. ¿Te armo tu kit de consistencia? Así cada imagen que generes
después sale con el mismo logo, colores, luz y modelo."

## Qué lleva el kit (todo en texto + las imágenes que ya generó)

**1. Ficha de marca:** la **misma ficha bloqueada** (BRAND LOCK) que se generó al aprobar el logo
(`ficha-de-marca.md`), en su última versión y sin reescribirla: logo, HEX por rol, tipografía, estilo de
ilustración y personaje, formato del empaque, datos fijos por referencia o variedad y textos aprobados.
Se le suma, en texto: esencia, personalidad y tagline · versiones del logo (® o ™) · proporción de color
y color héroe · equivalentes en Canva · forma madre y dispositivo · reglas de foto (luz, lente, ángulos,
fondos, grade, medio) · ficha de identidad de cada modelo · descripción exacta de cada producto · voz (sí
decimos / no decimos, palabras propias) · prohibiciones. Si la marca no pasó por la ruta de marca,
primero se arma su ficha con la plantilla de `ficha-de-marca.md`.

**2. Prompt de memoria de marca** (en inglés, en bloque de código): el BRAND LOCK completo, más las
reglas de foto, y el bloque SPANISH TEXT de `corrector-espanol.md`, para **pegar al inicio de una
conversación de su generador**, seguido de "Apply this brand system to every image in this conversation".
Desde ahí, cada pedido nuevo solo dice la escena, el texto y el formato. El BRAND LOCK no se resume: se
pega igual.

**3. Imágenes que se adjuntan siempre** (lista con su `@imagen`, en el orden fijo de la ficha):
`@imagen 1` = logo aprobado limpio, `@imagen 2` = personaje aprobado (si hay), y después la hoja del
sistema de logo, la hoja del modelo (personality board / ángulos), los empaques aprobados y las fotos del
producto. Dile que las guarde
juntas en una carpeta "KIT [MARCA]".

**4. Prompts base aprobados (5–8):** los que ya funcionaron en la sesión, con huecos `[ESCENA]`,
`[TEXTO]`, `[FORMATO]` y su línea 📎. Uno por tipo de pieza que más usa.

**5. Cómo usarlo, en tres líneas:** abrir una conversación nueva en su generador → pegar el prompt de
memoria y adjuntar las imágenes del kit → pedir piezas con los prompts base. Si su herramienta permite
guardar instrucciones fijas y archivos (un GPT propio, un Gem, un proyecto), que pegue ahí la ficha y suba
las imágenes del kit para no repetirlo cada vez. No inventes pasos de la interfaz de ninguna herramienta.

**No incluyas el playbook, las referencias internas ni los moldes completos de esta herramienta.** El kit
lleva solo los candados de la marca y sus prompts ya adaptados; la metodología sigue siendo de esta
herramienta.

## Versión skill (si usa la herramienta en Claude)

Si la persona trabaja en Claude, el mismo kit se le puede entregar como **su propia skill de marca**:
- Usa la plantilla `assets/plantilla-skill-de-marca.md` como `SKILL.md`, con nombre `marca-[nombre]`
  (minúsculas y guiones, sin "claude" ni "anthropic") y una descripción que diga cuándo usarla.
- Agrega en `assets/` el logo limpio y 2–4 imágenes del kit.
- Si hay ejecución de código, empaquétala como `.skill` (zip de la carpeta); si no, entrega el SKILL.md
  como texto para que la cree.
- Para instalarla, que la suba en la sección de skills de su cuenta; ante dudas, la ayuda oficial de
  Claude. En ChatGPT, el equivalente es pegar la ficha en las instrucciones de un GPT propio.

## Mantenimiento

Cuando cambie algo (nueva modelo, nuevo producto, ajuste de paleta), el kit se regenera completo y se
vuelve a entregar. Para clientes de agencia es un entregable vendible: "tu marca, lista para producir sola".
