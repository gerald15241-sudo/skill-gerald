# Curaduría / autocrítica — control de calidad ANTES de publicar

Cereza del pastel: antes de entregar prompts, maqueta o brand board, la skill **se revisa a sí misma**
como lo haría un director de arte exigente, corrige lo que falle, y solo entonces publica. No es un paso
opcional ni cosmético: es la diferencia entre "foto bonita genérica" y "pieza a nivel campaña".

Honestidad: esto es un **criterio de revisión** que tú (Claude) aplicas con tu propio juicio, no un
validador automático infalible. Pero hacerlo explícito sube muchísimo la calidad y evita los errores que
ya se repitieron.

## Cómo se hace (pasa / corrige / publica)

1. Termina el borrador (prompts / maqueta / brand board) **sin mostrarlo todavía**.
2. Córrelo contra el **checklist** de abajo, punto por punto, con ojo crítico y honesto.
3. Si algo falla → **corrígelo en silencio** y vuelve a revisar. No entregues con fallas conocidas.
4. Si algo no se puede corregir sin la persona (falta la foto en un ángulo, el dato de precio, una
   decisión de marca) → **no lo tapes**: dilo en una línea y pregunta.
5. Publica. Al entregar, agrega **una línea corta de "revisé esto"** nombrando lo que verificaste (no un
   informe largo): ej. "Revisé: producto fiel, paleta disciplinada, ortografía y tildes, datos iguales a
   la ficha".

Para piezas de alto impacto (campaña completa, pieza para cliente, algo que se va a vender), haz la
revisión con **mirada fresca**: léelo como si lo viera un cliente por primera vez, no como quien lo
escribió. Si está disponible y la pieza lo amerita, puedes apoyarte en un subagente/segunda pasada para
que critique sin el sesgo de haberlo creado.

**Ojos extra (si están disponibles; ver `integraciones.md`).** Sobre la maqueta/overlay puedes apoyarte en
`design:accessibility-review` (mide el **contraste texto/fondo real** — refuerza el punto 3 de
legibilidad) y en `design:design-critique` (jerarquía, consistencia, usabilidad). Son refuerzo: **si no
están, aplica tú el checklist igual** con tu propio criterio; nunca dependas de ellas ni avises que faltan.

## Checklist del curador

**1. Fidelidad del producto (lo más importante).**
- ¿Cada prompt describe el producto EXACTO de la foto (forma, color real, logo, etiqueta, textura,
  proporciones)? ¿Nada inventado ni "parecido"?
- ¿Se usan las fotos/ángulos que la persona dio, y se pidieron los que faltan?
- Si el producto tiene texto impreso (etiqueta, ficha, datos): ¿se transcribió línea por línea, tal como
  está en la foto, e **idéntico en todas las piezas** de la serie (caso de la altitud 1800 / 1950)?
- Si el producto va dentro de una escena real: ¿lleva el bloque de integración (misma luz y temperatura,
  sombra de contacto, oclusión, atmósfera) para que no se vea "pegado"? ¿El producto respira, o lo
  saturan los elementos alrededor?

**2. Disciplina de color.**
- ¿La paleta respeta los roles fijados (fondo · tipografía · acento · héroe)?
- ¿El **color héroe sigue reservado al producto** y no se coló otro color fuera de la paleta (como el
  rojo que se metió sin estar en los colores bloqueados)? Si aparece un color nuevo, es error: quítalo o
  justifícalo con la persona.

**3. Legibilidad del texto.**
- ¿El texto se lee completo, sin quedar tapado por el producto, el modelo o un borde? (caso "DIFERENTE"
  medio oculto = error).
- Si el texto va detrás de la persona o del producto: ¿se lee **cada palabra completa**? ¿El prompt dice
  dónde queda el sujeto respecto a las letras y cierra con "NO letters hidden or cut"?
- ¿Algún texto flota solo, sin relación con el titular o la retícula? ¿Se usó el nombre interno de una
  dirección como texto visible?
- ¿Contraste suficiente texto/fondo? ¿Jerarquía clara (titular > bajada > CTA)?
- **Tipografía:** ¿se eligió en orden (marca real → referencias → nicho), se dieron 2–3 opciones **al
  inicio** con sus prompts de social media board (3 sistemas distintos en paleta, letra y recurso), y pasa la prueba de marca tapada (sin el logo, la letra
  se siente de la marca)? Si la serie tiene un recurso tipográfico (palabra en cursiva), ¿está escrito
  en **todos** los prompts?
- En modo con texto en imagen: ¿textos cortos, dentro del límite de líneas, en español correcto con
  tildes y Ñ, con el bloque SPANISH TEXT — EXACT RENDERING? ¿Se avisó que hay que revisar letra por letra?

**4. Medio / estética correctos (anti "safe zone").**
- ¿El medio coincide con las referencias de la persona? Si dio collage/editorial/grunge, ¿la pieza es de
  ese medio y NO una foto hiperrealista limpia? (ver `estetica-y-medio.md`).
- ¿La pieza se sale de la "foto bonita por defecto"? ¿Hay un concepto real, no solo un mood agradable?
- ¿El bloque de hiperrealismo se aplicó solo cuando el medio es foto (condicional), no siempre?
- Si es **UGC casera**: ¿se aplicó la psicología inversa (`realismo-anti-ia.md`) — micro-detalle humano +
  negativo fuerte contra piel lisa/retoque/simetría? ¿Tiene imperfección real (poros, brillo, asimetría,
  baby hairs) y NO cara de cera? Y a la vez, ¿se ve **de buena calidad** (nítida, bien iluminada), no
  borrosa/granulada/foto mala? Casero es la vibra, no baja calidad.

**5. Concepto y nivel campaña.**
- ¿Hay una **gran idea** con gancho, no solo estética? ¿Al menos una dirección fue de alto concepto?
- ¿Las 2–3 direcciones eran **distintas entre sí** (no el mismo mood con otro color)?
- ¿Se siente como publicidad oficial de esa marca/nicho, apoyada en campañas reales investigadas?
- **Repositorio:** ¿se abrió `assets/referencias/indice.md`, se eligieron y **abrieron** 4–6 imágenes, y
  la línea `Base:` dice cuáles (`Repo: gen-059 + …`)? Si la persona trajo referencias, ¿se cruzaron con el
  repositorio? Si no trajo, ¿se le dijo qué imágenes del repositorio se usaron?
- ¿Se **abrieron de verdad** en esta sesión las bibliotecas (`conceptos-creativos.md`,
  `biblioteca-referentes.md`, las secciones completas de los formatos elegidos en
  `sesiones-foto-producto.md`, la receta de `biblioteca-dp.md`) antes de proponer? Si no, ábrelas y rehaz.
- ¿Cada dirección lleva su línea `Base:` (concepto · sesión #N · receta DP · research), con nombres y
  números que existen en los archivos? ¿Las 2–3 direcciones salen de combinaciones distintas?
- **Embudo:** ¿lo mostrado salió de 6–8 combinaciones en borrador, o es la primera idea que apareció?
  ¿Frena el scroll frente a lo que ya hace la categoría?
- **Referencias de la persona:** ¿se dijo qué se tomó de cada una? ¿Se cruzaron con un concepto o
  formato del banco? ¿La pieza pasa la prueba anti-copia (tapando el nombre, no se confunde con la
  referencia)?
- **Prueba anti-genérico:** ¿alguna dirección se pudo escribir sin los bancos (“editorial limpio”, “flat
  lay minimalista”, “producto sobre mármol”)? Si sí, reemplázala.
- En los prompts, ¿la escena sigue la composición clave del formato de sesión elegido y la luz/lente de
  la receta DP, o se diluyó en una escena genérica?
- ¿Cada prompt parte de la sección más cercana del playbook (buscada en su índice) y conserva intacto su
  bloque de realismo, cámara y AVOID? Si se reescribió o se resumió ese bloque, es error: restáuralo.
- ¿Los textos del molde se reescribieron para esta marca (nada de "ARCHIVO 01" o titulares de Nautica
  copiados)? En campañas, ¿al menos una dirección explora una composición que no sale de un molde?
- ¿Con las direcciones se entregó su vista previa sin que la persona la pidiera: **social media board** si
  las piezas llevan texto, moodboard si no? ¿El board usa titulares reales y ningún handle inventado?

**6. Copy (siempre lo propone la skill — ver `copywriting.md`).**
- ¿Hay titular, bajada y CTA propuestos por TI, aunque la persona solo diera el precio (o nada)?
- ¿Se eligió un **ángulo** claro (no frase genérica) y el titular usa una fórmula probada?
- ¿Se presentaron 2–3 opciones con tu recomendación marcada? ¿Una sola idea por pieza? ¿Un solo CTA?
- ¿El copy es de nivel copywriter (claro, con gancho, en la voz del nicho y en español natural), no
  relleno? ¿El precio va enmarcado, no pelado, y sin inventar descuentos/promesas?
- **Anti-cliché:** ¿el titular podría firmarlo cualquier competidor ("de la finca a tu taza")? Si sí,
  reemplázalo por uno que aproveche la idea visual de la pieza.

**6b. Personas en la pieza.**
- ¿Hay una persona sin `@imagen` de modelo aprobado? Solo vale si es solo manos o persona sin rostro, o
  si la persona aceptó una pieza única sin serie; si no, primero va el casting y el modelo (atajo de
  `modelo-ugc.md`).
- ¿Se preguntó el tipo de casting, la edad, los rasgos y la vibra antes de crear a la persona?
- ¿El prompt lleva el bloque completo de piel y cámara del carril correcto, y no una descripción corta
  propia? Agencia: §1 del playbook. **UGC con buen casting: referencia de cara leída + `realismo-anti-ia.md`
  + escena del nivel de producción; si salió con el set de estudio editorial de §1.1, es error (se ve de
  agencia, no UGC).** Persona real: `personas-reales.md`.
- Si hay varias personas: ¿cada una tiene su `@imagen` y se prohíbe intercambiar rasgos?

**7. Consistencia de familia.**
- ¿Toda la campaña/carrusel comparte paleta, tipografía, modelo (IDENTITY LOCK) y producto (PRODUCT
  LOCK), cambiando solo escena/encuadre/copy? ¿Se lee como UNA familia?
- En carrusel: ¿la secuencia tiene hilo (portada → desarrollo → cierre/CTA)?

**8. Intake completo (no asumir).**
- ¿Se preguntó lo que decide la pieza y no estaba claro? Sobre todo: **¿tiene precio?** y **¿la persona
  pone los textos o los pongo yo / modo de texto?** (errores que ya pasaron por no preguntar). Si el
  precio llegó ambiguo ("75.000 mil", "75k"), ¿se confirmó antes de generar?
- ¿Se **pidieron referencias visuales del tipo que corresponde** al entregable (tabla de
  `instructivo-referencias.md`), también en la express? Si no las tenía, ¿se usó el repositorio y se le
  dijo? Son **obligatorias** en dos casos: modelo UGC con buen casting (foto de cara) y ruta de marca
  (referencias de logo en el paso 1 y de marcas que le gustan en el paso 4).
- ¿Cada prompt dice **qué fotos adjuntar en el generador** (@imagen = producto/modelo-lock), o aclara que
  es solo texto? ¿NO se pidió adjuntar al generador las referencias de estilo (esas las describe el texto)?
- ¿Los prompts se entregaron **inline en el chat** (texto para copiar), NO en artefacto?
- **Ruta express:** las 3 preguntas cubren objetivo, formato, precio, modo de texto y look; no se exige
  el resto del intake ni 2–3 direcciones. Pero ¿la dirección única tiene su `Base:`, pasa la prueba
  anti-genérico y el prompt lleva todos los bloques obligatorios? ¿Se pidieron referencias, se cruzó con
  el repositorio y, si hay texto, se eligió la tipografía con la muestra antes del prompt? ¿El cierre
  ofrece variante, otra dirección o pasar a campaña?

**9. Marca real — responsabilidad.**
- ¿Logo y producto fieles, sin deformar?
- ¿NO se inventan como reales anuncios, alianzas, respaldos, precios o promos que la marca no autorizó?

**10. Privacidad / datos del autor.**
- ¿NO se filtró el handle personal ni "CONCEPTO CREATIVO IA" de la autora como default? El header/handle
  es **de quien usa la skill** o se omite (ver regla HEADER en SKILL.md).

**11. Ruta de marca y aplicaciones (solo en la ruta de marca; ver `estudio-de-marca.md`).**
- **Orden:** ¿estoy en el paso correcto de los 7 y el anterior quedó **aprobado** de forma explícita?
- **Logo primero:** ¿salió algo visual de la marca (moodboard, tablero, empaque, mockup) antes del logo
  aprobado, o aparece un logo provisional o distinto? Si sí, es error: se retira.
- **Referencias:** ¿hay mínimo 3 referencias de logo antes de la exploración y mínimo 3 de marcas antes
  del moodboard? ¿Se leyeron con psicología inversa (`ingenieria-inversa.md`) y regla 3–2–1?
- **Logo:** ¿se mostró la lectura de cada referencia y el patrón común antes de las opciones? ¿Las 6
  difieren en arquitectura, cada una es una mezcla declarada ("tipografía de la Ref A + dispositivo de la
  Ref C…"), al menos 4 combinan 2 o más referencias y 1 es un contraste deliberado? ¿Nombre
  deletreado con sus tildes? ¿® solo si está registrada? ¿La hoja tiene primario, secundario, versiones
  de color, monograma y una tinta? ¿Se avisó vectorizar y verificar el registro?
- **Ficha:** desde el paso 3, ¿cada prompt lleva `@imagen 1` = logo aprobado, la línea 📎 y la ficha
  completa en su última versión? ¿Datos de producto, formato del empaque y personaje idénticos a la ficha
  y a la referencia correcta? ¿Algo que no está en la ficha? Si sí, para y pide aprobación.
- **Moodboard:** ¿lleva el logo aprobado aplicado, sin diseñar el empaque final?
- **Tablero:** ¿lista cerrada de textos? ¿Mapa de grilla? ¿Una sola luz, la del moodboard?
- **Empaques:** ¿primero una referencia aprobada y después las demás cambiando solo lo que dice la
  ficha? ¿Frente máximo 5 líneas y reverso máximo 6?
- **Mockups y POP:** ¿el logo se adapta a la técnica de cada material (no "pegado")? ¿Escala real? ¿La
  luz coincide con el espacio? Si se usó la foto del local, ¿se prohibió redecorarlo? En arte plano y
  ficha técnica: ¿proporción real, margen de seguridad, sangrado, CMYK, acabados y aviso de que las
  medidas son de referencia?
- **Anti-copia:** si tapas el nombre, ¿se confunde con una referencia o un competidor?
- **Sistema visual** (`sistema-visual.md`): ¿cada decisión sale de SUS referencias o de su idea?
- Todo lo visual de la ruta de marca, ¿se entregó como prompt? Al cerrar, ¿se ofreció lo opcional (POP,
  sistema visual, kit) en una línea?

**12. Ortografía en español (TODA la skill; ver `corrector-espanol.md`).**
- ¿Cada texto visible, copy, caption, hoja de texto y prompt de corrección está bien escrito, con
  tildes, Ñ, mayúsculas acentuadas (CAFÉ, NARIÑO) y ¿ ¡?
- ¿Unidades y números correctos (`1.900 msnm`, `250 g`, `$45.000`) e iguales a la ficha?
- ¿El prompt tiene el bloque SPANISH TEXT — EXACT RENDERING y el cierre `NO misspelled words. NO
  missing accents. NO extra text.`?
- ¿Se respetó el límite de líneas de la pieza?
- ¿Algún texto distinto entre piezas de la misma marca (una palabra, un dato, una unidad)? Si sí, se
  unifica con la ficha.

## Resultado

Solo pasa a la persona lo que sobrevive al checklist. Si algo quedó pendiente de su decisión, se lo dices
claro en vez de entregar una pieza con un hueco disimulado.
