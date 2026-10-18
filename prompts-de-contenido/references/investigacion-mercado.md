# Investigación de mercado + brief creativo

Para que los prompts sean de nivel profesional (no genéricos), la skill hace su **propia
investigación** antes de generar y **elige lo que mejor funciona**, en vez de inventar a ciegas.
Hazlo rápido (no es una tesis) y, salvo que la persona diga "sáltalo", en todo pedido de marca/nicho.

## Proceso (BÚSQUEDA REAL, no de memoria)

La investigación **no es opcional ni de memoria**: ejecuta búsqueda web/de imágenes de verdad y
**mira referencias reales** antes de opinar. Aplica a **TODOS los nichos** (comida, mascotas,
inmobiliaria, salud, belleza, moda, etc.), no solo moda. Si tienes **búsqueda de imágenes**, úsala
para ver la estética actual del nicho/marca; **Pinterest** es buena fuente de inspiración pero la skill
no puede navegarlo por dentro (login/bloqueo) — no digas que "buscaste en Pinterest"; si acaso, sugiere
a la persona un término de búsqueda o pídele un par de pins. Si solo hay búsqueda web, úsala. Si no
puedes buscar, **dilo** y pide a la persona 3–6 referencias visuales — no inventes un "look seguro".

1. **La marca (si es marca real) — PRIMERO y literal.** Busca sus **campañas recientes reales** y
   refleja su tono *verdadero*, no el que asumirías. Muchas marcas de moda (ej. Bimba y Lola) son
   **coloridas, gráficas, con humor y tipografía dibujada** — no lujo oscuro. No le pongas a una marca
   un mood que no es suyo.
2. **Convenciones del nicho:** cómo se ven los anuncios que funcionan hoy en esa categoría. Apóyate en
   `references/nichos.md` + búsqueda real.
3. **Tendencias actuales (míralas, no las supongas) — MODO PERPLEXITY.** Las tendencias se mueven rápido
   y **no se sacan de memoria**: investíga como lo haría Perplexity. Cómo:
   - **Varias búsquedas dirigidas, no una.** Lanza 3–5 queries con ángulos distintos: nicho + año en
     curso, la marca real + "campaign/ad", plataforma ("Instagram ads trends <nicho> <año>"), estética
     ("visual trends <categoría> <año>"), competencia. Usa el **año/fecha actual** en las queries.
   - Para tendencias usa **búsqueda extendida/a fondo** (es tema fresco y cambiante), y **búsqueda de
     imágenes** para ver la estética real, no solo leerla.
   - **Sintetiza, no copies:** destila **4–6 tendencias concretas** aplicables a ESTE producto/nicho,
     cada una en una línea + **fuente real** (de dónde la sacaste). Nada de "tendencias" genéricas de
     relleno.
   - **Muéstraselo a la persona** como un mini-informe de tendencias (lista corta con fuentes) ANTES del
     preview, para que vea que la investigación es de verdad y actual. De ahí salen las direcciones.
   - No hay un set fijo de tendencias "de este año": las que apliquen salen de la búsqueda de hoy, no de
     esta lista. (Ejemplos que han aparecido: colocación surrealista del producto, tipografía dibujada,
     color pop/Y2K, humor con props, editorial limpio con logo gigante — pero **verifícalo buscando**,
     no los des por vigentes.)
4. **Competencia:** qué ángulos ya ocupan y qué **hueco** hay para diferenciarse.
5. **Audiencia y plataforma:** a quién le habla y dónde vive la pieza (afecta formato y copy).

## ⚠️ Anti-default (el error a evitar)

El fallo más común es **colapsar todo a un solo mood "premium oscuro/editorial"** (fondo negro, mármol,
flat lay sobrio). Es seguro pero genérico y muchas veces **no es la marca ni la tendencia**. Reglas:

- **Deriva la dirección de referencias reales**, no de un reflejo de "lujo = oscuro".
- **Propón 2–3 direcciones creativas DISTINTAS** (no variaciones del mismo mood) para que la persona
  elija: p. ej. una fiel a la marca, una más tendencia/atrevida, una más editorial limpia. Enséñale
  en qué se diferencian.
- **Direcciones = GRANDES IDEAS, no solo estéticas.** Cada dirección debe tener un **concepto con
  gancho**, no un mood. Incluye **siempre al menos UNA de alto concepto** del banco
  (`conceptos-creativos.md`): juego de escala, colocación surrealista, entrega épica, tipografía como
  set, etc. Si la persona quiere "wow/viral/atrevido", **lidera con conceptos**, no con el editorial
  seguro. Nómbralas por su idea ("Entrega épica: la zapatilla sobre la ciudad"), no por su paleta.
- Si la marca o la tendencia piden **color, humor, surrealismo o tipografía gráfica**, ve por ahí —
  no lo "suavices" a premium oscuro.
- Muestra (describe o enlaza) las **referencias reales** en las que te apoyas, para que la persona
  valide que captaste bien el tono.

## Elige y justifica: el BRIEF CREATIVO

Con eso, antes de escribir prompts, entrega un brief corto (5–7 líneas) y **recomienda** —no listes
todo—:

- **Ángulo/positioning** elegido (y por qué gana sobre otros).
- **Hook / gran idea** de la campaña.
- **2–3 direcciones visuales distintas** (registro, composición, luz) apoyadas en referencias reales —
  no un solo mood. Marca cuál recomiendas y por qué.
- **Paleta** sugerida por roles (o la de la persona/marca).
- **Tipografía** sugerida (combo de `references/tipografia.md` o la de la marca).
- **Formato recomendado** (ver `references/formatos-anuncio.md`): tipo de pieza, nº de slides, aspect
  ratio, plataforma.

**Presenta las direcciones cortas y comparables, no un brief largo.** A la gente no le gusta leer:
entrega 2–3 direcciones en texto (nombre del concepto, una línea de gran idea, paleta por roles con HEX,
fuentes reales y medio), con tu recomendación marcada. No construyas tableros HTML para elegir (REGLA #1
del SKILL); si la persona quiere ver una dirección antes de decidir, dale un **prompt de moodboard** por
dirección para su generador (si la marca tiene logo aprobado, va como `@imagen 1`).

La persona aprueba/elige o ajusta; recién ahí generas los prompts. Lo elegido alimenta luego el brand
board de cierre.

**Alimenta al estratega de contenido.** Si el pedido es una campaña/ruta/parrilla, este research es el insumo
directo del estratega (`estratega-contenido.md`): las **tendencias** definen el mix de formatos y ángulos, la
**competencia** el hueco/diferenciador, la **audiencia** el mensaje por etapa del embudo, y la
**estacionalidad** la cadencia. No entregues una ruta sin este research detrás; cada decisión de la ruta debe
poder rastrearse a un hallazgo (trazabilidad).

## Reglas

- **Siempre cita fuentes** cuando el brief o las tendencias se apoyen en búsqueda web (lista corta al
  final, estilo Perplexity: afirmación → fuente). Si una "tendencia" no tiene fuente, no la presentes
  como tendencia: márcala como tu criterio.
- Distingue siempre de dónde viene cada decisión (ver Trazabilidad en SKILL.md): nicho, marca,
  tendencia o tu dirección de arte.
- Si no hay acceso a búsqueda o la persona la salta, dilo y construye el brief con el playbook + el ADN
  del nicho + tu criterio, marcándolo como propuesta sin research fresco.
