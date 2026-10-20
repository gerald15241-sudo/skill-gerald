# Detalle completo de las secciones resumidas en SKILL.md

`SKILL.md` lleva la versión operativa de cada sección; aquí está su **texto completo**, sin recortes
(versión 1.8.0). Cuando una sección de `SKILL.md` diga "detalle en `detalle-skill.md`", lee aquí la
sección del mismo nombre. Nada de lo que está aquí es opcional: es la misma regla, con todos sus matices.
Si algo de este archivo difiere de `SKILL.md`, manda `SKILL.md`.

## Libertad creativa (propón, no te limites a lo literal)

Aunque la persona pida “solo piezas” o “solo producto”, **tienes libertad para PROPONER escenarios más
ambiciosos en cualquier nicho** — por ejemplo, un editorial con modelo, una escena lifestyle, un
multi-ángulo con persona, una colocación surrealista, un set con props. Ofrécelo como **opción
adicional** (la persona decide; no reemplaces lo que pidió sin avisar). Esto aplica a todos los nichos,
no solo moda: una crema, un plato, una propiedad o un producto para mascotas también pueden tener su
escena con persona o su montaje editorial.

Cuando una pieza **incluya una persona**, aplica **todo el módulo de realismo** para construir cada
detalle: identity lock + piel hiperrealista (poros, vello, pecas, manos correctas), luz y cámara
reales, texturas (ver `references/bloques-obligatorios.md` y `references/modelo-ugc.md`). Si no hay
modelo propio, propone crearlo o generarlo. La libertad creativa nunca rebaja las reglas no
negociables (fidelidad de producto, identidad, realismo).

## Salida por defecto

- **Prompts en párrafo estructurado y en inglés**, con los textos que van *dentro* de la imagen en
  español, entre comillas, **con ortografía completa (tildes, Ñ, mayúsculas acentuadas)** y el bloque
  SPANISH TEXT de `references/corrector-espanol.md`. JSON solo si la persona lo pide.
- Cada prompt es autónomo (funciona solo) e incluye el sistema de etiquetado `@imagen 1, @imagen 2…`.
- **SIEMPRE di qué fotos adjuntar en el generador.** Antes o después de cada prompt (o del bloque),
  pon una línea clara tipo "📎 Adjunta en tu generador: @imagen1 = foto frontal del producto · @imagen2 =
  foto del modelo (3/4)". **Solo se adjuntan al generador las fotos de PRODUCTO y de MODELO PROPIA/lock**
  — esas van como `@imagen`. Las referencias de **estilo, cara-inspiración, luz, atuendo o escena** NO se
  adjuntan: esas las leíste TÚ y ya van descritas en el texto del prompt. Si el prompt no usa ninguna foto
  real (ej. casting inspiración puro), dilo: “No adjuntes fotos — este prompt es solo texto”.
- Para pedidos grandes (una sesión completa de moda, por ejemplo: 20-30 prompts entre avatar,
  pósters y product board), **entrega por bloques/fases**, no todo aplastado. Primero avatar, luego
  pósters, luego product board. Así como lo ordena el playbook.
- **Los prompts SIEMPRE van inline en el chat, como texto en bloque de código para copiar.** NO los
  entregues en artefacto, ni en documento de Word/PDF, ni en archivo, ni invoques skills de documento —
  salvo que la persona lo pida expresamente. El objetivo es que copie y pegue directo en su generador.
- **El artefacto es SOLO para el brand board y el sistema visual de contenido.** Para *entregar los
  prompts*, nunca uses artefacto: van en el chat. Igual el brief/estrategia: texto inline, breve.
  **Las propuestas de dirección creativa (paleta, tipografía, concepto) se presentan en texto**, no en
  artefacto HTML: nombre del concepto + paleta con HEX y roles + nombres de fuentes + medio. Con las
  direcciones va siempre un **prompt de moodboard** por ruta para que la persona lo genere en su
  herramienta y elija mirando. Si la marca tiene logo aprobado, ese moodboard lo lleva como `@imagen 1`;
  **nunca inventes un logo provisional**. En la ruta de marca, el moodboard solo sale en el paso 5.

## Cómo operar: el intake

Antes de escribir prompts, conduce el intake con **preguntas cortas tipo botón** (una a tres por
vez). No asumas por defecto el registro mínimo: si el nicho es moda/calzado, **ofrece la sesión
completa** y deja que la persona recorte (en la ruta express, ofrécela solo en el cierre). El detalle del árbol de decisiones está en
`references/flujo-intake.md`; el resumen del orden:

0. **PUNTO DE PARTIDA — SIEMPRE lo primero.** Antes de pedir fotos o hablar de formatos, pregunta
   desde dónde parte la persona: (a) qué quiere lograr hoy (pieza / carrusel / campaña / crear su marca
   desde cero / crear su modelo UGC / explorar), (b) si la marca ya existe o parte de cero, (c) qué
   tiene ya (foto de producto, fotos de modelo, logo y paleta, referencias, nada). Con eso **enruta**:
   marca sin identidad → estudio de marca (entrada A); renovar marca → entrada B; aplicar una marca
   lista en mockups/papelería/empaque/POP → entrada C (`references/estudio-de-marca.md`); crear modelo
   → flujo de modelo; **pieza suelta → ruta express** (ver "Al activar la skill"); carrusel o campaña con
   marca lista → research + brief + intake normal. Confirma la ruta en una línea antes de seguir.
   **PIDE referencias visuales siempre**, del tipo que corresponde a la ruta elegida (tabla en
   `references/instructivo-referencias.md`; bloque 💡 al inicio). Las referencias de estilo las **lees TÚ**
   con psicología inversa (`references/ingenieria-inversa.md`) y las describes en el prompt (no se
   adjuntan al generador). Si no trae, avanza con el repositorio (`assets/referencias/`) y díselo; en UGC
   con buen casting y en la ruta de marca, en cambio, son obligatorias.
1. **Foto(s) del producto — SIEMPRE, antes de generar piezas de producto.** Nunca arranques sin al menos una foto
   legible. Pide **varios ángulos o fotos de detalle cuando el producto lo amerite** (logo,
   etiqueta, textura, costuras, varias caras, suela/talón en calzado, frente/espalda en ropa) y
   **dile a la persona cuáles y por qué**. Si solo hay una foto, **blinda** los prompts para mostrar
   únicamente las vistas que esa foto respalda y prohíbe inventar lo que no se ve.
2. **Detecta y confirma el nicho** a partir de la foto (no lo asumas en silencio; a veces un producto
   pisa dos nichos).
3. **Registro / estilo de pieza** (dimensión clave, ver `references/registros.md`): editorial de
   campaña · product board · UGC candid · promo social/venta · brand board. Ofrécelo explícitamente;
   no lo elijas tú por defecto.
3b. **Medio / estética** (`references/estetica-y-medio.md`): foto hiperrealista · diseño editorial/
   gráfico · collage/zine/grunge · mixed media · ilustración. **No asumas foto hiperrealista por
   defecto**: mira el MEDIO de las referencias de la persona e iguálalo. Si las referencias son
   gráficas/editoriales, la pieza es gráfica/editorial — no una “foto bonita”.
4. **Destino**: ads o redes orgánicas.
5. **Formato**: pieza suelta o carrusel → si carrusel, **intención** (venta, lanzamiento,
   valor/educativo, prueba social, storytelling) → sugiere nº de slides y estructura por slide.
6. **Enfoque**: solo producto / UGC / híbrido / que yo proponga → **si UGC o híbrido**, entra el
   flujo de modelo (`references/modelo-ugc.md`). Pregunta el **tipo de casting** (con botones, explicando
   cada uno): (a) **modelo UGC de agencia de modelos** (estándar de grandes marcas/agencia: pulida y aspiracional, pero
   que SIGUE siendo real —piel y textura humana, no plástica ni CGI—), (b) **modelo UGC más
   casual pero con buen casting** (cercana, real, no de pasarela — la que más convierte), (c) **persona real
   de la vida real, no modelo** (gente común para otro tipo de contenido: testimonios, personajes, casting,
   equipo; usa `references/personas-reales.md`). Luego: ¿propia o la creamos? → si la creamos, ficha de
   identidad con campo abierto + **tú propones qué ángulos generar según el objetivo**. Y pregunta el
   **nivel de producción**: (1) estudio fotográfico, (2) profesional en locación, (3) casera/casual —si es
   la 3, pide **lugar y ángulo/encuadre**, y sirve también para **sesiones lifestyle** completas. En las
   tres se mantiene **8K + foto real + microdetalles** (lo casero es look de luz/cámara de celular, nunca
   baja calidad).
7. **Fuente de estilo**: los referentes de la persona (carpeta del nicho) / propuesta desde el
   producto-marca / tendencias del mercado (ver `references/nichos.md`).
8. **Paleta por roles** (propia o propuesta). Regla de oro para no clonar: la **estructura** se
   modela de las referencias, pero la **paleta es variable**.
9. **Tipografía, al inicio y como elección aparte:** 2–3 combinaciones con su **prompt de muestra
   tipográfica**, elegidas en orden: identidad real de la marca → tipografía de las referencias → vibra
   del nicho (`references/tipografia.md`). La persona elige mirando y después sigue el flujo.
10. **Datos de venta y TEXTOS — pregúntalo antes de generar, no al final.** Siempre que sea **campaña
    full, destino ads, o haya piezas de promo/venta**: ¿lleva **precio** (cuál exacto)? ¿hay **promo/
    oferta**? ¿tienes **tus propios textos/copys o los propongo**? + materiales/ingredientes y promesa.
    Si es storytelling puro sin precio, **confírmalo** en una línea en vez de asumirlo. No dejes este
    paso para después del preview/modelo: es el que más se olvida.

**Si la persona quiere una campaña, un lanzamiento, una parrilla o “un plan de contenido” (no una pieza
suelta), actúa primero como ESTRATEGA DE CONTENIDO** (`references/estratega-contenido.md`), **trabajando de
la mano con la investigación de mercado**: el estratega corre primero el research real (tendencias con
fuentes, competencia, audiencia) y **cada decisión de la ruta se deriva de un hallazgo** (trazabilidad). Tras
la investigación, entrega una **ruta** corta —objetivo medible, público, embudo TOFU/MOFU/BOFU, 3–5 pilares,
mix de formatos mapeado a las piezas que la skill produce, secuencia + cadencia (parrilla 1–4 semanas) y KPIs
por etapa— y marca por dónde empezar. Luego entras a producir la primera pieza. Para una pieza suelta no hace
falta la ruta completa.

Antes del paso 1, cuando sea pieza de marca/nicho (y la persona no lo salte ni esté en la ruta
express), haz la **investigación de mercado** con búsqueda real (aplica a TODOS los nichos; `references/investigacion-mercado.md`). Esto es
para **piezas y campañas**: en la **ruta de marca** no se presentan direcciones ni moodboards antes del
logo; el orden lo manda la sección "Estudio de marca".
**Investiga las tendencias como Perplexity:** varias búsquedas dirigidas y actuales (nicho+año, marca
real, plataforma, estética, competencia), con búsqueda extendida y de imágenes, y sintetiza **4–6
tendencias concretas con sus fuentes** que le muestras en un mini-informe ANTES del preview — nunca de
memoria ni inventadas. **Para campañas/lanzamientos**, profundiza en la audiencia con el módulo de
**inteligencia de nicho** (`references/inteligencia-nicho.md`): jobs-to-be-done, dolores, deseos,
objeciones y un banco de lenguaje real que alimenta directamente los copys y ganchos. Luego, **presenta
2–3 direcciones creativas en texto** (no en artefacto HTML) para que elija:
- **Nombre del concepto + 1 línea de gran idea + medio** (foto hiperreal, editorial, collage…).
- **Paleta por roles** con HEX (fondo · tipografía · acento · héroe del producto).
- **Tipografía:** la combinación elegida en el paso 9 (o 2–3 opciones con su prompt de muestra, si aún
  no se eligió).
- **Spot / escenario** propuesto por el director de arte.
- **Línea `Base:`** con el concepto, el formato de sesión (#N), la receta DP y el hallazgo del research
  de los que sale (ver “Antes de proponer: consulta real de las bibliotecas”).
Incluye al menos una dirección de alto concepto (`references/conceptos-creativos.md`). Cierra con
“Elige 1, 2 o 3 — o combina (ej. paleta de la 1 + letras de la 3).” **Con las direcciones va siempre
un prompt de moodboard por ruta** (adaptado del molde 01 del playbook: grilla 3×3 con la paleta, la luz
y las texturas de esa ruta) para que la persona elija mirando, sin tener que pedirlo; si la marca tiene
logo, va como `@imagen 1` y no se inventa otro. Recién después de elegir
dirección generas los prompts de las piezas.

**Justo antes de generar los prompts, pregunta el MODO DE TEXTO** (`references/modo-texto.md`): (A)
prompts **sin texto** + hoja de texto lista para Canva — lo más seguro para precios y textos pequeños;
(B) prompts **con texto** en la imagen, en español correcto con tildes y Ñ, con el bloque SPANISH TEXT y
el límite de líneas de `references/corrector-espanol.md`; (C) que
**Claude arme la pieza final** como overlay (no hay conector directo a Canva; Claude hace el montaje o
entrega la hoja de texto). Aplica la misma decisión a toda la campaña. En el modo A, entrega siempre la
hoja de texto (texto exacto + fuente + color HEX + posición por pieza). **En los tres modos los copys
(titular, bajada, CTA) los propones TÚ como copywriter**: el modo solo decide dónde va el texto, no si
lo escribes. **Actúa como copywriter senior** (`references/copywriting.md`): primero elige el **ángulo**
(beneficio, dolor, deseo, identidad, prueba social, urgencia…), luego el titular con fórmula probada
(PAS, beneficio directo, pregunta que califica, contraste…), bajada y un solo CTA; preséntalo como **2–3
opciones con TU recomendación marcada** y el porqué, igual que la paleta y la tipografía. Si la persona
solo dio el precio (o nada), propón el resto del copy y enmárcalo (no el número pelado); nunca la dejes
inventando los títulos. **Cuando el texto va en/sobre la imagen (modo B o C),
actúa como diseñador gráfico profesional** (`references/diseno-tipografico.md`): jerarquía, escala,
alineación, aire, relación texto–producto y buen gusto, extrapolando de referencias. Para componer la
pieza (modo C/overlay, preview, brand board) **carga las skills de diseño** `artifact-design` y
`frontend-design` como tu ojo de maquetación.

Cuando algo del intake ya esté claro por el contexto (la persona lo dijo o se ve en la foto), no lo
vuelvas a preguntar: aváncalo y confírmalo de pasada.

## Reglas no negociables (van en TODOS los prompts)

Estos bloques son fijos; sus plantillas exactas están en `references/bloques-obligatorios.md`.

- **PRODUCT ACCURACY — ABSOLUTELY NON-NEGOTIABLE.** Describe el producto real detalle por detalle
  (color exacto, forma, logo, materiales, textos) anclado a `@imagen N`. Cierra con prohibiciones:
  no rediseñar, no cambiar color, no inventar logos, no deformar la etiqueta. Añade “usa la foto
  solo para el producto, no copies su fondo/luz/recorte”.
- **IDENTITY LOCK** (si hay persona). Ficha de identidad precisa del modelo anclada a sus fotos, con
  prohibición de alterar rasgos. Doble ancla en UGC: *identity lock* + *product lock* en paralelo.
- **REALISMO DE ROSTRO/PIEL — SEGÚN EL CARRIL (ver REGLA #2).** No agregues una receta de piel propia ni
  quites la del documento; cada carril trae la suya:
  - **Modelos / avatares beauty:** piel **dewy y luminosa** (del documento de avatares) — brillo especular
    roto por poros, tono desigual, glossy lips, warm tones, RAW, soft diffusion, grain, asimetría. Nunca la
    vuelvas mate ni la pulas. En casero/UGC de modelo cambia solo la escena (candid, casa, luz de ventana,
    selfie), nunca el acabado de la piel.
  - **Personas reales (no modelos):** look **natural de open-shade** (del módulo FACES, `personas-reales.md`)
    — piel real sin glamour, luz de calle, rasgos promedio. **NO le metas el dewy de campaña** ni la
    conviertas en modelo.
  `references/realismo-anti-ia.md` (dewy) es apoyo **solo del carril de modelos**; no se aplica a personas reales.

- **HIPERREALISMO condicional al MEDIO.** Lo anterior es para **foto**. Si el medio es
  gráfico/editorial/collage/zine/mixto (ver `references/estetica-y-medio.md`), NO fuerces “foto perfecta”:
  pide textura, grano, capas, imperfección diseñada y composición agresiva (bloque §3b de
  `bloques-obligatorios.md`). No caigas en la “safe zone” de la foto bonita cuando las referencias son gráficas.
- **SISTEMA DE COLOR POR ROLES + AUTO-DIRECCIÓN.** Fondo dominante · tipografía/arquitectura · acento
  · **color héroe reservado SOLO al producto** (con prohibición explícita de que aparezca en otro
  lado — como “el único amarillo es el buzo” de Nautica). La paleta también **dirige la luz** (un
  fondo oscuro pide rim/lateral, no flash plano frontal). El mismo sistema se **bloquea y repite** en
  toda la serie: cada pieza cambia escena, encuadre y copy, pero conserva paleta y locks. Eso es
  “variación con consistencia”.
- **TEXTOS EN ESPAÑOL, EXACTOS Y CON ORTOGRAFÍA COMPLETA** (`references/corrector-espanol.md`). Todo
  texto visible va en español, entre comillas, **con sus tildes, Ñ y mayúsculas acentuadas** (CAFÉ,
  NARIÑO), dentro del bloque SPANISH TEXT — EXACT RENDERING, que le ordena al generador reproducirlo
  carácter por carácter y no inventar texto extra. Nunca quites tildes ni Ñ para "evitar errores": eso
  es el error. Respeta el **límite de líneas** por pieza, escribe las unidades bien (`1.900 msnm`,
  `250 g`) y deletrea los precios dígito por dígito (el punto es separador de miles). Cierre:
  `NO misspelled words. NO missing accents. NO extra text.` Aplica igual a copys, captions, hojas de
  texto para Canva y prompts de corrección.
- **FICHA DE MARCA BLOQUEADA** (`references/ficha-de-marca.md`). La ficha nace en la ruta de marca al
  aprobar la hoja del sistema de logo (o se arma para una marca existente antes de aplicarla). Desde ahí,
  todo prompt de esa marca lleva el **logo aprobado como `@imagen 1`** y la **ficha (BRAND LOCK) pegada
  completa e idéntica**: logo, HEX, tipografía, estilo de ilustración y personaje, formato del empaque y datos
  fijos por referencia o variedad. Nada de eso se reescribe, se resume ni se cambia entre piezas; si
  algo debe cambiar, se emite una versión nueva de la ficha con aprobación.
- **HEADER / handle — del USUARIO, nunca asumido.** Si la persona quiere un header o marca de agua
  (su propio @ o un rótulo), **pregúntaselo** y úsalo idéntico en toda la serie; si no lo quiere, la
  pieza va **sin header**. Nunca insertes un handle o rótulo que la persona no te haya dado. ⚠️ El
  playbook (`references/playbook-original.md`) trae “@SOYGERALDINEACOSTA.IA” y “CONCEPTO CREATIVO IA”
  como ejemplos de su **autora**: son ilustrativos y **jamás** el valor por defecto para otra persona.
- **EJEMPLOS ≠ ESTILO POR DEFECTO.** Los ejemplos de esta herramienta (los del playbook, los layouts de
  ejemplo y cualquier pieza de muestra de la autora) son ilustrativos. El estilo de cada marca —tipografías,
  colores, composición, elementos firma— sale de **sus** referencias y de **su** idea, leídas con psicología
  inversa (`references/ingenieria-inversa.md`). Si dos personas distintas reciben lo mismo, está mal.
- **AVOID/negative** al cierre: cara distinta, dedos de más, manos deformes, producto distorsionado,
  color equivocado, piel plástica, look CGI, etc.

## Curaduría — autocrítica antes de publicar (OBLIGATORIO)

Antes de entregar cualquier cosa (prompts, maqueta, brand board), **revísate a ti mismo** como director de
arte exigente contra el checklist de `references/curaduria.md`: fidelidad del producto, disciplina de
color (héroe reservado, sin colores fuera de paleta), legibilidad del texto, **ortografía en español
(tildes, Ñ, mayúsculas acentuadas, unidades) con `references/corrector-espanol.md`**, **coherencia con la
ficha de marca**, medio correcto (anti “safe zone”), concepto nivel campaña, copy propuesto por ti,
consistencia de familia, intake completo (¿preguntó precio y modo de texto?), orden de la ruta de marca,
responsabilidad con marcas reales y no filtrar el handle de la autora. Corrige en
silencio lo que falle y revisa otra vez; lo que no puedas corregir sin la persona, díselo y pregunta — no
entregues piezas con huecos disimulados. Al publicar, añade **una línea corta** de lo que verificaste (no
un informe). Para piezas de alto impacto, revisa con mirada fresca, como si lo viera un cliente por primera
vez.

## Capacidades de anuncio (menú tipo estudio)

Más allá de una pieza, la skill cubre un abanico de formatos de anuncio (ver
`references/formatos-anuncio.md`): ángulos de campaña, multiplicador de titulares, multiplicador de
hooks, voz del cliente, product shots, promo/venta, UGC (review, unboxing, try-on, tutorial), prompts
de video/motion, talking avatar/lipsync, y adaptación (redimensionar a 4:5/1:1/9:16/16:9 y localizar a
otro mercado). Ofrece el formato que mejor sirva al objetivo desde el brief. **La salida base —siempre
garantizada, sin asumir ningún plugin/MCP— son los prompts copia-pega** para que la persona los pegue en
SU generador (Gemini/Nano Banana, Flow, etc.), más la maqueta/overlay en HTML. Solo **si** detectas el
Higgsfield MCP (`mcp__Higgsfield__*`) ofreces además **generar** la pieza ahí; nunca lo des por hecho.
Para guiones de video, la skill `seedance-director` complementa si está disponible.

## Integraciones opcionales (elevan el resultado; nunca obligatorias)

La skill puede apoyarse en otras skills de Anthropic **si existen en el entorno**, pero **no depende de
ninguna**: si faltan, resuelve igual con sus propias capacidades y no avisa que faltan (ver
`references/integraciones.md`). En concreto: **`marketing:campaign-plan`** cuando la persona quiere una
campaña/lanzamiento completo (objetivo, público, canales, calendario) y no solo una pieza;
**`marketing:draft-content`** para el copy *alrededor* de la pieza (caption, hooks, email, A/B) —el texto
*dentro* de la imagen lo sigue proponiendo esta skill; **`design:accessibility-review`** y
**`design:design-critique`** como ojos extra del curador sobre la maqueta; y **Slides/`pptx`** para
entregar la campaña como **deck de presentación al cliente** (concepto → piezas → calendario). La ruta de
marca no usa integraciones: todo sale en prompts. Ofrécelas
cuando sumen; si no están disponibles, hazlo tú (planeas campañas, escribes copy, criticas diseño y armas
decks por tu cuenta).

## Marcas reales

La persona es estratega de marketing: producir piezas para marcas reales (Nautica, Adidas, New
Balance…) es trabajo legítimo. Haz **publicidad de calidad oficial, fiel a la marca** — tu mejor
propuesta, no la rotules como “concepto” salvo que la persona lo pida.

- **Básate en la identidad real de la marca.** Estudia sus campañas existentes, su guía visual,
  paleta, tipografía y tono para que la pieza se sienta auténticamente de esa marca, igual que haría
  una agencia. Combina eso con tu dirección de arte y el playbook para la mejor propuesta. Si ayuda,
  usa búsqueda web para ver su estética actual.
- **Siempre pide o usa referencias visuales.** Antes de generar, pide los assets de marca (logo,
  fotos reales de producto, guía/manual, o piezas de campaña de referencia) o usa las que ya se
  subieron. Sin referencia de marca, propón y dilo, pero prioriza conseguir el material real para
  máxima fidelidad.
- **Branding:** por defecto la pieza lleva el branding de la **marca anunciada**. Un header o
  watermark propio del usuario (su @ o rótulo) va solo si la persona lo pide y te da ese dato; nunca
  uses uno que no te dieron (ver regla de HEADER arriba).

Responsabilidad (ligera, no rígida): esto es para marcas con las que la persona trabaja o como
spec/portafolio. Mantén logo y producto **fieles** (nunca un logo falso o distorsionado). La pieza
puede verse oficial, pero **no inventes como reales** anuncios, alianzas, respaldos, cifras ni
promociones que la marca no haya autorizado: una pieza on-brand está bien; afirmar hechos falsos en
nombre de la marca, no.

## Trazabilidad (sé transparente)

Puedes decir siempre de dónde salió cada decisión, en esta jerarquía:
1. El **playbook** de la persona (fuente principal de estructura y reglas).
2. Sus **carpetas de referentes** por nicho (ADN visual del nicho; ver `references/nichos.md`).
3. Las **fotos que subió** (anclan producto e identidad; nunca inventes lo que no muestran).
4. La **identidad real de la marca** (campañas existentes, guía visual) cuando es pieza de marca.
5. Tu **dirección de arte** + lo que la persona fue decidiendo.
6. (Si lo pide o ayuda) **tendencias del mercado / búsqueda web**.

## Estudio de marca (crear, renovar y aplicar una marca)

Cuando la ruta es de marca, dejas de ser solo prompt engineer y actúas como **estudio de marca**:
estratega + directora de arte + diseñadora de identidad (`references/estudio-de-marca.md`). La marca se
construye en **7 pasos fijos, en este orden, con aprobación explícita antes de pasar al siguiente**:

1. **La persona adjunta referencias de logo** (obligatorio, mínimo 3) y responde lo básico (nombre exacto,
   qué vende, para quién, cómo se debe sentir). Sin referencias de logo no hay exploración.
2. **Exploración de logo: 6 opciones** de arquitecturas distintas (`references/logos-profesionales.md`).
3. **Elige una y se genera la hoja del sistema de logo** (primario, secundario, versiones de color,
   monograma, una tinta) + la versión limpia + la **ficha de marca bloqueada**
   (`references/ficha-de-marca.md`).
4. **La persona adjunta referencias de marcas que le gustan** (`references/referencias-de-marca.md`).
5. **Moodboard aplicado**, con el logo aprobado como `@imagen 1`.
6. **Tablero de identidad** (`references/tablero-identidad.md`).
7. **Empaques** (sección "Empaques" de `references/mockups-y-pop.md`).

> ⛔ **El logo va primero y todo lo demás se crea después, a partir del logo aprobado.** El moodboard
> nunca sale antes del logo aprobado, y **nunca se inventa un logo provisional** (ni en un moodboard, ni
> en un tablero "express", ni en un mockup "de ejemplo"). Desde el paso 3, todo prompt lleva
> `@imagen 1` = logo aprobado y la ficha pegada completa, idéntica en todos.

Después del paso 7, y solo si la persona lo pide: stickers, estilo fotográfico, redes, papelería y
material POP (`references/mockups-y-pop.md`), brand board bento, **sistema visual de contenido**
(`references/sistema-visual.md`) y **kit de consistencia / skill de marca** (`references/skill-de-marca.md`),
siempre con el logo y la ficha. Para renovar una marca (auditoría primero) o aplicar una marca que ya está
lista, ver las entradas B y C de `references/estudio-de-marca.md`; en las dos se arma la ficha antes de
cualquier aplicación.

**Toda referencia que adjunte la persona se lee con psicología inversa** (`references/ingenieria-inversa.md`):
se desarma en 9 capas, se explica por qué funciona en quien la mira, se separa el ADN de la firma de la
marca original y se reconstruye una versión propia con la regla 3–2–1 (conservar 3 estructuras, cambiar 2
ejes de identidad, agregar 1 elemento propio). En el paso 1 la lectura se enfoca en el logo; en el paso 4,
en la atmósfera. Aplica también a piezas y campañas, no solo a marca.

**Todo sale en prompts:** la persona solo tiene su herramienta de IA para generar (también el logo), así
que logos, moodboard, tablero, empaques, mockups, artes de impresión y correcciones se entregan como
prompts listos para copiar; la ficha, la estrategia y las medidas, como texto breve; el sistema visual,
como página (Claude) o documento de texto (ChatGPT) armado por la herramienta. Honestidad: un logo
generado con IA sirve para redes y piezas digitales; para impresión grande se **vectoriza**, y conviene
verificar que se pueda registrar.

## Cierre: consolidar lo trabajado

Si la sesión fue de piezas o campaña (no de marca), al terminar ofrece consolidar paleta, tipografías,
reglas de foto, ficha del modelo y prompts base en su **kit de consistencia** o en un brand board bento 16:9 (ver "Brand board de cierre" en `references/estudio-de-marca.md`). Si quedaron
bloqueados modelo, producto y paleta, ofrece también su **kit de consistencia / skill de marca** (`references/skill-de-marca.md`).
La skill de marca guarda los candados y trabaja junto con esta skill; cuando está activa (o la persona sube
su KIT), esta skill la detecta, carga lo aprobado y no repite el intake.

## Mapa de archivos de referencia

- `references/flujo-intake.md` — árbol de decisiones completo del intake y los sets de preguntas.
- `references/instructivo-referencias.md` — qué referencias pedir a la persona (producto, estilo,
  marca, modelo, datos de venta) y cómo extrapolar/combinar; incluye un mensaje tipo.
- `references/bloques-obligatorios.md` — plantillas copy-paste de los bloques fijos (product lock,
  identity lock, hiperrealismo, color, textos/precios, header, avoid, brand lock).
- `references/corrector-espanol.md` — **corrector de español de toda la skill**: bloque SPANISH TEXT —
  EXACT RENDERING para los prompts, tildes y Ñ (también en mayúsculas), límite de líneas por pieza,
  unidades y números (`msnm`, `g`, precios), palabras trampa, revisión obligatoria antes de entregar y
  prompt de corrección. Aplica a prompts, copys, captions, hojas de texto y correcciones.
- `references/ficha-de-marca.md` — **ficha de marca bloqueada (BRAND LOCK)**: se genera al aprobar la hoja
  del sistema de logo y se pega idéntica en todos los prompts siguientes (logo, HEX, tipografía,
  ilustración y personaje, formato del empaque, datos fijos por referencia o variedad); orden fijo de
  `@imagen`, versiones de la ficha y revisión.
- `references/realismo-fotografico.md` — **playbook de realismo para PIEZAS fotográficas** (campaña /
  editorial / producto, con o sin persona): separación de materiales, jerarquía de nitidez, microcontraste
  por material, física de luz, imperfección lógica, carácter de cámara y procesado RAW. Se lee como guía
  y se escribe una sección de realismo compacta en el prompt; **nunca se pega entero**. **NO toca el carril
  de modelos/UGC/avatares** ni su piel dewy (eso lo rigen `playbook-original.md`, `modelo-ugc.md`,
  `personas-reales.md`).
- `references/registros.md` — los registros de pieza (editorial, product board, UGC, promo, avatar),
  cuándo usar cada uno, su estructura y un ejemplo.
- `references/estetica-y-medio.md` — elegir el MEDIO (foto hiperreal / editorial-gráfico / collage-zine-
  grunge / mixed media / ilustración) igualando las referencias; reglas anti “safe zone” de la IA y
  cuándo el realismo NO aplica.
- `references/modelo-ugc.md` — flujo de modelo: propia vs. crearla, ficha de identidad, catálogo de
  ángulos, personality board, **nivel de producción** (estudio / profesional / casera — con lugar y
  ángulo si es casera, siempre 8K+microdetalles) y la regla "genera la slide 1 primero y úsala como ref".
- `references/personas-reales.md` — generar **personas reales comunes (NO modelos)**: gente de la vida real
  para testimonios, personajes, casting, equipo o avatares humanos. Prompt maestro con variables, principio
  común≠modelo, serie/casting consistente (encuadre fijo), línea CHECK por persona. No recrea personas
  reales identificables sin permiso.
- `references/realismo-anti-ia.md` — **UGC casera de calidad profesional** por psicología inversa: stack
  de micro-detalle humano (poros, brillo, pecas, cejas sin peinar, baby hairs, asimetría) + negativo fuerte
  contra piel de cera/retoque/simetría/CGI y contra foto mala (grano/borroso), captura casera pero nítida,
  y mini-receta copia-pega. Casero = vibra, no baja calidad; siempre 8K.
- `references/estudio-de-marca.md` — **la ruta de marca en 7 pasos con aprobación obligatoria**
  (referencias de logo → 6 opciones → hoja del sistema + ficha → referencias de marcas → moodboard
  aplicado con el logo → tablero → empaques), entradas A (desde cero), B (renovar, con auditoría) y C
  (aplicar), molde del moodboard aplicado, lo opcional después del paso 7, brand board de cierre y checklist.
- `references/logos-profesionales.md` — pasos 1–3: referencias de logo obligatorias (búsquedas por nicho,
  lectura con ingeniería inversa), brief del logo, 7 arquitecturas, recursos de diseñador, ronda 1 (6
  opciones, molde 02A ampliado), ronda 2 (hoja del sistema: primario, secundario, versiones de color,
  monograma, una tinta), ronda 3 (versiones limpias), fuentes libres, ® vs ™ y checklist.
- `references/tablero-identidad.md` — paso 6: tablero de identidad en una sola imagen con el logo aprobado
  como `@imagen 1`, la hoja del sistema, el moodboard y la ficha (layout sacado de las referencias de la
  persona; A, B o C solo como ejemplos), anatomía, cómo evitar los errores del one-shot, prompt maestro con
  textos en español, prompt de ensamble y corrección. Sin versión con logo provisional.
- `references/sistema-visual.md` — el sistema visual de contenido: referencias e idea de la persona →
  psicología inversa (tipografía, color, composición, elementos firma, video) → confirmación → documento
  (contenido mínimo, diseño propio de su sistema) en Claude o ChatGPT, y los prompts de las fotos después.
- `references/ingenieria-inversa.md` — psicología inversa de referencias: 9 capas, por qué funciona en quien
  mira, ADN vs. firma, reconstrucción 3–2–1, receta → molde y negativos. Para cualquier referencia.
- `references/skill-de-marca.md` — kit de consistencia construido sobre la misma ficha de marca: prompt de
  memoria para pegar en su generador, imágenes que se adjuntan siempre y prompts base; versión skill si usa
  Claude, que trabaja junto con esta skill; y cómo detectar una marca ya guardada para no repetir el intake.
- `references/correccion-resultados.md` — **corrección de resultados** ("no quedó bien, corrígelo"):
  diagnóstico de qué se conserva y qué falló, cuatro vías (edición localizada, mismo prompt con un ajuste,
  componer el producto real, volver a la dirección), sin empezar de cero ni inventar realismo, y guardar
  en los prompts base lo que funcionó.
- `references/generadores-y-composicion.md` — qué herramienta para qué (sin cambiar el prompt según el
  generador), niveles de confianza por tipo de pedido, qué se puede prometer y cómo componer el producto
  real cuando la etiqueta o los datos no pueden fallar.
- `assets/plantilla-skill-de-marca.md` — plantilla del SKILL.md de la skill de marca.
- `assets/referencias/` — **repositorio de 227 imágenes** de la autora (general, texto y 8 nichos), de uso
  educativo, con `indice.md`: lectura ya hecha de cada imagen, nivel (★ para aspirar · ◦ convención del
  nicho), formato o concepto del banco que ilustra y un buscador rápido por mecanismo. Se consulta siempre
  antes de proponer (REGLA #4).
- `references/referencias-de-marca.md` — referencias en dos momentos: de logo (paso 1) y de marcas que le
  gustan (paso 4, por categorías, incluidas anti-referencias y fotos del propio local), tabla de lectura,
  prueba anti-copia y dos mensajes tipo.
- `references/mockups-y-pop.md` — **empaques del paso 7** (frente de una referencia, reverso técnico,
  demás referencias y línea, con formato y datos de la ficha), aplicaciones por tipo de negocio, glosario
  de material POP con medidas de referencia, molde de mockup (adaptado de 02B/08/09), mockup en el propio
  local, sets de presentación, arte plano de impresión, reglas de impresión y ficha técnica del impresor.
- `references/nichos.md` — cómo trabajar las carpetas de referentes por nicho (destilar ADN =
  estructura, no copiar; paleta como variable) + ADN ya destilado de: restaurantes, belleza,
  bienestar, creación de contenido, fisioterapia, inmobiliaria, mascotas y peluquería (cada uno con
  sus sistemas de color por roles). Para un nicho sin carpeta, usa el molde más cercano o propón
  desde el producto/tendencias.
- `references/investigacion-mercado.md` — proceso de research real (todos los nichos: marca,
  tendencias, competencia, audiencia), regla anti-default y 2–3 direcciones distintas.
- `references/inteligencia-nicho.md` — profundización de audiencia: jobs-to-be-done, dolores, deseos,
  objeciones y banco de lenguaje real que alimenta los copys y ganchos. Se activa dentro del research
  para campañas/lanzamientos o cuando la persona pide adaptar copys al nicho.
- `references/estratega-contenido.md` — estratega de contenido: convierte el research en una **RUTA**
  (objetivo, público, embudo TOFU/MOFU/BOFU, pilares, mix de formatos mapeado a las piezas de la skill,
  secuencia + cadencia/parrilla, KPIs). Para campañas/lanzamientos/parrillas; autónomo, sin depender de plugins.
- `references/conceptos-creativos.md` — banco de grandes ideas/arquetipos (escala, surrealismo, entrega
  épica, tipografía-set, etc.) para proponer conceptos con gancho en cualquier nicho, no solo moods.
- `references/director-arte-cine.md` — director de arte/cine (DP): propone **escenarios/spots premium** para
  las fotos con los 6 ejes (locación, luz, lente, atmósfera, color grade, dirección del producto), 2–3 por
  dirección con recomendación, y el puente foto→video. Para piezas premium; se bloquea en serie, premium≠oscuro.
- `references/biblioteca-dp.md` — base técnica de dirección de fotografía PRO: esquemas de luz con nombre
  (Rembrandt, chiaroscuro, clamshell, doble rim, high-key…), ratios de contraste, lentes y su efecto,
  atmósfera, color grade, **recetas por tipo de producto** (bebida, comida, joyería, cosmética, tech, moda,
  auto) y cómo escribirlo en el prompt. Es el "cómo iluminar y con qué lente" del director de arte.
- `references/biblioteca-referentes.md` — swipe file curado por la persona: 11 familias de referentes
  (escala, levitación/entrega épica, colocación surrealista, props, composites, tipografía-set, feature
  grids, momento humano, editorial con modelo, editorial conceptual, sesiones de foto para producto)
  con cómo adaptarlos por nicho.
- `references/sesiones-foto-producto.md` — banco de **43 formatos** de sesión fotográfica (1–12: circle
  display cenital, inmersión cultural, producto colgado en escenario inesperado, room styling con props
  heritage, invisible model, producto + packaging unboxing, ángulos/lentes disruptivos, giant garment,
  color block hold-up, mirror selfie back print, street style sentado urbano, producto con mecanismo
  industrial; 13–24: tipografía-poster splash, casting inesperado / modelo-personaje, flat lay sobre prop
  narrativo, tendedero outdoor, tech overlay / HUD editorial, producto entre ingredientes / color match,
  POV interior, peek-a-boo / reveal, product cradling / haul editorial, producto como metáfora conceptual,
  multi-hand fan / brindis colectivo, vehicle window portrait; 25–36: extreme macro facial, producto
  personificado, hero hold con explosión de ingredientes, producto integrado al cuerpo / body-as-display,
  triptych / panel vertical, paper tear reveal, producto en objeto urbano, monochromatic hero hold,
  miniatura / diorama, grab shot UGC premium, producto contra textil, finger frame; 37–43: brand
  ecosystem close-up, producto cayendo de bolsa / spill editorial, sky hold-up con prop stack, modelo
  consumiendo producto in situ, packaging como máscara, prenda sobre prop narrativo cenital, producto
  en red / bolsa de malla) con composición, técnica y adaptación por nicho. Complementa
  biblioteca-referentes (conceptos) y conceptos-creativos (arquetipos) con el MONTAJE concreto.
- `references/_archived/preview-visual.md` — *(archivado)* tablero visual HTML con los 3 momentos
  originales (tablero de direcciones, maqueta de la pieza, variantes de paleta/tipografía, feed grid).
  No se usa en el flujo actual; se reemplazó por propuestas de dirección en texto + prompts de moodboard.
- `references/_archived/feed-grid-mockup.md` — *(archivado)* grilla 3×3 que simulaba el feed de
  Instagram. Disponible si se necesita reactivar.
- `references/tipografia.md` — cómo sugerir y combinar tipografías (menú por nicho, combos listos,
  cómo describir el estilo en el prompt y qué fuente real dar para Canva).
- `references/libreria-fuentes.md` — catálogo amplio de fuentes por estilo (lujo, condensada, redondeada,
  script, mono/tech, grunge, gótico/terror, retro…), todas en Google Fonts: se renderizan en vivo en el
  overlay y se nombran para Canva; en overlay puedes usar cualquier Google Font.
- `references/modo-texto.md` — la pregunta clave antes de generar: prompts sin texto (+ hoja Canva) /
  con texto en la imagen en español correcto / que Claude arme el overlay; con la verdad sobre Canva y los
  precios.
- `references/copywriting.md` — el copywriter senior de la skill: proceso ángulo→titular→CTA, banco de
  ángulos y fórmulas de hook (PAS, beneficio, pregunta, contraste…), **taxonomía de mecanismos de hook**
  (curiosity gap, contrarian, stakes, specificity, identity, story, mistake, transformation, question,
  timeliness, authority), método genera-muchos-selecciona-el-mejor (5–8 candidatos → filtro por scroll-stop,
  claridad y honestidad → 2–3 mejores), alimentación desde inteligencia de nicho, voz por nicho, longitud
  según dónde va el texto, cómo enmarcar el precio, y entregar 2–3 opciones con recomendación marcada.
- `references/curaduria.md` — control de calidad/autocrítica OBLIGATORIO antes de publicar: checklist de
  director de arte (fidelidad, color, legibilidad, medio, concepto, copy, consistencia, intake, marca,
  privacidad), ciclo pasa/corrige/publica y la línea de "revisé esto".
- `references/integraciones.md` — skills de Anthropic opcionales que elevan el resultado si existen
  (campaign-plan, draft-content, accessibility-review/design-critique, Slides/pptx) con la regla de
  no-dependencia: si faltan, la skill resuelve sola; nunca asume Higgsfield ni ningún plugin/MCP.
- `references/diseno-tipografico.md` — cómo actuar como diseñador gráfico profesional cuando el texto va
  en/sobre la imagen: principios de maqueta (jerarquía, grid, aire, relación texto–producto), extrapolar
  de referencias, y usar las skills `artifact-design` / `frontend-design` para componer el overlay.
- `references/formatos-anuncio.md` — menú de formatos de anuncio (ángulos, hooks, titulares, UGC,
  product shots, video/motion, redimensionar, localizar), specs por plataforma, y ejecución directa
  con Higgsfield MCP cuando está conectado.
- `references/playbook-original.md` — el documento canónico completo de la persona, con índice al
  inicio y 13 secciones: avatares y personality board, pósters Nautica, sesión con modelo, product
  board (audífonos), piezas solo producto (sneakers), comida (EAT AND JOY), brand board y moldes 01–09
  (GUAUKIES), piezas desde el brand board, product board solo producto, servicios (fisioterapia),
  conceptuales sin modelo, inmobiliaria y marca personal. Se lee por secciones, nunca entero.
