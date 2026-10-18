# Registro de pruebas: prompts-de-contenido v1.7.0

Todas las pruebas corren sobre la v1.7.0. No se cambia la skill hasta terminar las 5, salvo pedido
expreso de la usuaria.

Se corren las 5 pruebas y al final se aplican las correcciones en un solo paquete. Cada hallazgo indica
si la causa es la **skill**, el **generador** o está **por confirmar**.

## Prueba 1: ruta express (café TOSTADO)

**Pedido:** "/prompts-de-contenido hola" → eligió pieza suelta + foto del frente de la bolsa → vender,
texto en la imagen, $75.000 la libra, alto concepto, dos opciones (con persona / solo manos), sin
referencias.

**Resultado:** pieza 1 "SABE A MANDARINA. ES CAFÉ." (mano + explosión de ingredientes) · pieza 2 "DEL
TOLIMA A TU TAZA" (caficultor real junto a la bolsa).

### Lo que funcionó
- Primer mensaje correcto para un "hola" sin contexto: saludo, instructivo, Paso 0.
- Enrutamiento: "pieza suelta" entró a la ruta express con sus 3 preguntas en un mensaje.
- Las preguntas se adaptaron al nicho (look "barra de café, mesa de cata, finca").
- Evaluó la foto: pidió reverso/lateral y ofreció blindar el prompt solo al frente.
- Detectó "CAFE DE ORIGEN" sin tilde en la etiqueta real y lo respetó por fidelidad, avisando que
  se corrija en el arte original. Criterio correcto.
- Pieza 1: titular de contraste excelente, concepto de banco (sesiones #27 + #18), disciplina de color,
  jerarquía clara, tildes correctas.
- El nombre y "marca personal enseñando IA" vienen del perfil de Claude de la usuaria, no de la skill.

### Hallazgos para corregir
| # | Hallazgo | Causa | Corrección propuesta |
|---|---|---|---|
| 1.1 | La altitud de la etiqueta cambia entre piezas (1800M en una, 1950M en otra). | Por confirmar (falta ver los prompts y el dato real). | Si es de la skill: el PRODUCT ACCURACY debe transcribir el texto de la etiqueta línea por línea, y la curaduría debe compararlo entre piezas. Si es del generador: prompt de corrección. |
| 1.2 | Pieza 2: el empaque se ve "pegado" (luz de estudio en escena nublada, casi sin sombra de contacto, sin integración con el pasto). | Por confirmar (ver el prompt). | Bloque de integración producto–escena: misma luz y temperatura que el entorno, sombra de contacto, oclusión parcial (pasto delante), neblina atmosférica sobre el producto. |
| 1.3 | Pieza 2: titular cliché ("Del Tolima a tu taza" ≈ "de la finca a tu taza"). | Skill (copy). | Filtro anti-cliché en `copywriting.md`: descartar fórmulas gastadas de la categoría; el titular debe aprovechar la idea visual. |
| 1.4 | "75.000 mil pesos" es ambiguo (literal: 75 millones) y la skill no lo confirmó. | Skill (menor). | Si un precio es ambiguo, confirmarlo en media línea antes de generar. |
| 1.5 | Desde un "hola" son 3 intercambios hasta el prompt. | Diseño (menor). | Opcional: que la opción "pieza suelta" del Paso 0 traiga ya las 3 preguntas express. |
| 1.6 | Pieza 1: exceso de elementos volando en el borde izquierdo. | Por confirmar. | Si el prompt no limita cantidad: indicar densidad ("8–12 elements, generous negative space around the bag"). |

### Pendiente de esta prueba
- El mensaje de entrega (direcciones, líneas `Base:`, prompts, línea "Revisé").
- La altitud real impresa en la bolsa.

## Prueba 2: extrapolar referencias (camiseta Dickies)

**Pedido:** foto de la camiseta (frente) + 3 referencias (pareja "True." en estudio, chico sentado
subiéndose el cuello, chico con ojo de pez) → texto en la imagen, con modelo (no tiene), hombre y mujer.

**Resultado:** 3 piezas: "UNA PIEZA. DOS ESTILOS." (pareja en estudio caqui), "DE TALLER A LA CALLE."
(modelos acostados sobre la camiseta gigante, cenital), "LA TUYA. LA SUYA." (ojo de pez con el set a la
vista). Pie editorial con línea fina en DM Serif Display.

### Lo que funcionó
- Detectó que las referencias no se cargaron y las pidió de nuevo, en vez de inventarlas.
- Pidió ángulos útiles (logo de cerca, espalda, etiqueta del ruedo) y ofreció blindar si no llegaban.
- Preguntó para quién es (tienda, cliente, portafolio): responsabilidad con marca real.
- "Qué tomé de cada referencia" claro y concreto, más "lo propio" (fondo caqui por el origen workwear).
- Línea `Base:` completa y con extrapolación creativa (Sesión #41 "packaging como máscara" adaptada al
  cuello de la prenda). Paleta con los colores del logo reservados como héroe.
- "DE TALLER A LA CALLE." (giant garment, sesión #8) es una pieza de nivel campaña.
- Cierre correcto de la express: una pieza y tres caminos (variante, otra dirección, carrusel o sesión).
- Preguntó si agregar el @ de la usuaria como firma en vez de insertarlo (regla HEADER).
- Ofreció dejar fijos los modelos para una serie, aunque tarde: debió fijarlos antes de la primera pieza (ver 2.2).

> **Corrección de 2.2 a 2.4 ya redactada y revertida** a pedido de la usuaria, para que las 5 pruebas
> corran sobre la misma versión (v1.7.0). Está guardada en el commit 39d0db6 ("Crear el modelo primero…")
> y entra en el paquete final junto con 2.1.

### Hallazgos para corregir
| # | Hallazgo | Causa | Corrección propuesta |
|---|---|---|---|
| 2.1 | Tipografía serif editorial (DM Serif Display) en una marca workwear/streetwear: no se siente Dickies. | Skill. `tipografia.md` pone "moda" bajo "Lujo editorial" (DM Serif Display es el primer combo) y no tiene vibra streetwear/workwear; en la express no se miró la identidad real de la marca; "Qué tomé" no incluyó la capa de tipografía. | (a) Orden obligatorio para elegir tipografía: identidad real de la marca → capa 3 de las referencias → vibra del nicho; el combo listo es el último recurso. (b) Agregar vibra "Streetwear / workwear / heritage" y aclarar que moda ≠ lujo por defecto. (c) "Qué tomé de cada referencia" incluye tipografía cuando la referencia tiene texto. (d) Curaduría: prueba de marca tapada (sin el logo, ¿la tipografía y el tono se sienten de esta marca?). |
| 2.2 | No preguntó cómo debían ser los modelos (tipo de casting, edad, rasgos, vibra). | **Diseño de la ruta express (error mío).** La express no definía qué hacer si la persona quiere modelo y no lo tiene; creó los modelos inline, saltándose el flujo de `modelo-ugc.md`. | Si en la express la persona quiere persona y no tiene modelo: sale de la express para esa parte. Pregunta en un solo mensaje tipo de casting (agencia / UGC con buen casting / persona real), edad, rasgos y vibra; genera primero el modelo con el molde de avatar (playbook §1) o `personas-reales.md`; con el modelo aprobado como `@imagen`, sigue la pieza. Alternativa para quedarse en express: solo manos o persona sin rostro. |
| 2.3 | Realismo de los modelos flojo: piel pareja y pulida, look catálogo IA. | Skill (consecuencia de 2.2). Sin modelo creado con el molde de avatar, no entra el bloque de realismo del carril de modelos (poros, vello, asimetría, RAW). | Se resuelve con 2.2. Además, curaduría: si hay persona, el prompt debe llevar el bloque de piel del carril correcto (dewy del playbook o natural de `personas-reales.md`), nunca una descripción corta propia. |
| 2.4 | La identidad de los modelos cambia entre piezas (el hombre de "DE TALLER A LA CALLE." no es el mismo de las otras dos). | Skill (consecuencia de 2.2). Sin `@imagen` de modelo no hay identity lock posible en una serie. | Se resuelve con 2.2: en series con persona, el modelo aprobado va siempre como `@imagen`. |
| 2.5 | ~~Entregó 3 piezas con conceptos distintos.~~ **Resuelto: no es error.** Entregó una sola pieza y la usuaria generó las otras desde el cierre (variante y otra dirección). | — | — |

## Prueba 3: servicios (terapia de pareja, Karol Márquez)

**Pedido:** "set de piezas para el feed con texto, solo tengo esta imagen mía" + datos (12 años de
experiencia, terapia de pareja y transpersonal, Edificio Claft, Ciudad de Guatemala, teléfono, consulta
online y virtual). Foto: retrato de la terapeuta en su consultorio.

**Resultado:** set de 5 piezas: "¿Otra vez la misma pelea?" (dos tazas unidas por el hilo rojo, sin
persona), "Volver a escucharse" (pareja con el hilo y la terapeuta al centro), "Eres más que lo que te
pasa." (retrato con el hilo), "Reconectar contigo también es terapia." (hilo entre dos sillones, CTA con
teléfono) y "No vengo a darles la razón." (autoridad). Calificación: 9/10. La usuaria lo considera muy
bueno, después de pedir un prompt para ver las tipografías.

**Lo mejor del resultado:** la identidad de Karol se mantiene en las 4 piezas donde aparece (su foto como
ancla funcionó); el hilo rojo es el único rojo y sostiene la serie como concepto; sistema tipográfico
consistente (serif con una palabra en cursiva + sans + botón); copys de nivel ("No vengo a darles la
razón. Vengo a ayudarlos a entenderse."); tildes correctas (Márquez, también, Histórico, Escríbeme).
Es el resultado de referencia de lo que la skill debe producir.

### Lo que funcionó
- Leyó la foto y escribió la ficha de identidad ("Lo que leí de tu foto, corrígeme si algo no cuadra").
- Abrió los moldes correctos del playbook (personality board, servicios §10, marca personal §13).
- Research real con 6 tendencias y fuentes, y advirtió con honestidad que son blogs del sector y no
  estudios. Incluyó la ética del nicho (sin testimonios de pacientes, sin prometer resultados).
- 3 direcciones distintas, cada una con su `Base:` (bancos + playbook §10.2 y §13). La recomendada es de
  alto concepto ("El hilo rojo") y reserva el rojo como único color héroe, con la lógica del amarillo de
  Nautica.
- El set de 5 piezas sigue la estructura de §10 (gancho de dolor, transformación, autoridad, confianza,
  CTA) y cambió la prueba social por "qué pasa en la primera sesión" por ética. Criterio excelente.
- Revisó datos antes de generar: "presencial y virtual" frente a "online y virtual", la ortografía de
  "Claft" y su zona, y la tilde de Márquez. Preguntó el handle en vez de inventarlo.
- Propuso un modo de texto mixto (B para titulares, A para el teléfono) bien argumentado.
- Con una sola foto, recomendó generar primero el personality board (playbook §1.2) para que la cara no
  se deforme en otros ángulos.
- La tipografía (serif cálida + sans) sí encaja con el nicho, a diferencia del caso Dickies (2.1).

### Hallazgos para corregir
| # | Hallazgo | Causa | Corrección propuesta |
|---|---|---|---|
| 3.1 | Propuso las tipografías solo con nombres (Playfair Display, Fraunces + DM Sans, Fraunces Black + Manrope). La usuaria no podía imaginarlas y tuvo que pedir un prompt para verlas; con eso eligió y el resultado mejoró. | Skill. `tipografia.md` solo ofrece la muestra "si quiere verlas"; no es proactiva. | **Pedido expreso de la usuaria:** siempre que se propongan tipografías, la skill entrega por iniciativa propia un **prompt de muestra tipográfica**: una sola imagen con las 2–3 opciones lado a lado, escritas con palabras reales de la pieza (titular y nombre de la marca), cada una rotulada con su número. Le dice a la persona que lo genere para elegir y que después sigue el flujo. Va como prompt, no como artefacto (REGLA #1). Aclarar que el generador aproxima el estilo y que la fuente exacta se aplica en Canva. Aplica también en la ruta express cuando hay texto. |
| 3.2 | El mensaje de propuesta es largo (lectura de la foto, 6 tendencias, 3 direcciones, set de 5 piezas y 6 grupos de preguntas). | Por confirmar con la usuaria (no se quejó). | Si molesta: mover las preguntas de datos a un mensaje corto aparte, o resumir las tendencias a 3–4 líneas. |
| 3.3 | ~~"Centro Histórico" en la pieza 4.~~ **Resuelto: no es error.** La usuaria dio ese dato. | — | — |
| 3.4 | Las piezas 2 a 5 resaltan una palabra en cursiva ("escucharse", "más", "contigo", "la razón"); la pieza 1 no. | Menor: variación del generador o del prompt (por confirmar). | Si se repite: el recurso tipográfico de la serie se escribe en cada prompt como regla fija del sistema. |

## Prueba 4: campaña de moda (chaqueta New Balance)

**Pedido:** campaña de lanzamiento de una chaqueta (frente y espalda). Respuestas: cliente oficial de New
Balance, orgánico, pósters editoriales, modelo de agencia.

**Resultado:** ruta de 2 semanas con parrilla de 8 pósters y 3 direcciones. La usuaria pidió un prompt para
ver las direcciones (moodboard por dirección). Piezas: "DATE LA VUELTA." y "LA ESPALDA HABLA." (dirección 2,
"La espalda habla": estudio gris, flash duro, titular condensado gigante). Según la usuaria: buen realismo,
pero el diseño (ubicación y letras) necesita referencias.

### Lo que funcionó
- Abrió las bibliotecas y los pósters Nautica del playbook, y armó una ruta de estratega: objetivo,
  público, hueco ("Athletics, Inc.": el uniforme de un club), pilares y parrilla TOFU/MOFU/BOFU donde
  cada póster sale de un molde (Póster 01, 02, 03, 05, 06, 07, 09, 10).
- 3 direcciones distintas, cada una con `Base:`; una de alto concepto ("La pista es la chaqueta", giant
  garment). Rojo-naranja de la chaqueta reservado como color héroe.
- **En la ruta normal sí hizo el casting:** ficha de identidad del modelo de agencia (edad, fenotipo,
  cabello, rasgos, vibra) y personality board primero. Confirma que el hueco 2.2 es solo de la ruta express.
- Fidelidad del producto: detectó que los puños se ven rojos en la foto de frente y crema en la de
  espalda, y preguntó cuál es el real.
- Recomendó solo el branding de New Balance, sin rótulo extra, por ser cliente oficial.
- Los moodboards por dirección no muestran ningún rostro porque el casting aún no existía: buen criterio.
- Realismo del modelo bueno (pecas, poros, cabello) e identidad consistente entre las dos piezas.
  Anton condensada sí encaja con New Balance.

### Hallazgos para corregir
| # | Hallazgo | Causa | Corrección propuesta |
|---|---|---|---|
| 4.1 | No dio opciones de tipografía para elegir: cada dirección traía una sola combinación fija. | Skill. Refuerza 3.1. | **Pedido expreso de la usuaria:** las opciones de tipografía (2–3 combinaciones) se presentan **al inicio**, como decisión aparte, junto con el prompt de muestra tipográfica de 3.1. |
| 4.2 | No pidió referencias visuales; el diseño (ubicación del texto, jerarquía, letras) quedó sin guía. | **Cambio de regla pedido por la usuaria.** Hoy las referencias de estilo son "un plus, no requisito" (bloque 💡 de SKILL.md). | **Pedido expreso:** pedir referencias visuales **sí o sí** para el diseño (layout y tipografía) en piezas y campañas. Si la persona no tiene: la skill busca referencias reales (búsqueda web o de imágenes) y le muestra 4–6 con enlace, o le da términos de búsqueda para Pinterest. **Decisión pendiente:** (a) ¿aplica también en la ruta express? (b) Un "repositorio de imágenes" dentro de la skill solo es viable con imágenes propias de la autora (sus piezas, con derechos); guardar campañas de terceros en una skill que se comparte con alumnas tiene riesgo de derechos. |
| 4.3 | Tuvo que pedir el prompt para ver las direcciones (segunda prueba seguida, ver 3.1). | Skill. Hoy el moodboard se da "si la persona quiere ver". | Proactivo: con las direcciones va siempre el prompt de moodboard de cada una (molde 01), o la oferta explícita en una línea, para elegir mirando. |
| 4.4 | La modelo tapa letras del titular: "LA ESPALDA HABLA." pierde la P y la B; en "DATE LA VUELTA." la cabeza tapa parte de la V y la U. | Skill (prompt de diseño) + generador. | Tipografía detrás del sujeto solo si cada palabra se sigue leyendo: el prompt fija qué zona puede tapar el sujeto (nunca letras clave ni más de una por palabra). La curaduría ya lo exige (punto 3, caso "DIFERENTE"). |
| 4.5 | En "DATE LA VUELTA." el texto secundario "LA ESPALDA HABLA" flota pequeño a la izquierda, sin relación con el titular, y repite el nombre interno de la dirección. | Skill (diseño). Se relaciona con 4.2. | Con referencias de diseño, la jerarquía y la ubicación salen de ellas; el nombre interno de una dirección no se usa como texto visible salvo que sea el copy elegido. |
| 4.6 | El pie "NEW BALANCE / ARCHIVO 01" copia literal el "ARCHIVO 01" del molde Nautica. | Skill (menor). La REGLA #2 manda adaptar los textos del molde. | Los textos del molde (metadata, etiquetas) se reescriben para la marca y la campaña. |
| 4.7 | Toda la parrilla salió de los pósters Nautica. | Skill. La REGLA #2 se está leyendo como "toda la composición sale del molde". | **Pedido expreso de la usuaria:** el molde del playbook aporta la **estructura del prompt** (bloques de referencia, fidelidad, identidad, color, fotografía), no obliga la composición. En cada campaña, al menos una dirección y parte de las piezas exploran composiciones nuevas a partir de las referencias de la persona y de los bancos (referentes, 43 sesiones, conceptos), con su `Base:`. |
| 4.8 | La usuaria quiere que la skill use su carpeta de referencias con imágenes. | **No existe dentro de la skill:** se verificó que no hay ninguna imagen; sus carpetas se destilaron a texto (`nichos.md`, `biblioteca-referentes.md`). | Crear `assets/referencias/<nicho>/` con las imágenes de la usuaria (comprimidas, unas 8–12 por nicho) y un `indice.md` que diga qué enseña cada una (layout, tipografía, concepto, luz). La skill las abre y las lee con `ingenieria-inversa.md` cuando la persona no trae referencias, y aplica la regla 3–2–1 anti-copia. Pendiente: que la usuaria envíe las carpetas. Avisos: hay límite de tamaño para subir una skill, y si la skill se comparte con alumnas, las imágenes de campañas de terceros tienen riesgo de derechos (para uso propio es más tranquilo). |

**Decisión de la usuaria sobre 4.2:** las referencias obligatorias aplican **también a la ruta express**. Prima la
calidad sobre la rapidez.

## Requisitos generales de la usuaria (para el paquete final)

- **R1. Repositorio de referencias propio, siempre consultado.** La usuaria sube su paquete de referencias
  (por nicho y generales). La skill debe **acudir siempre** a ese repositorio antes de proponer, y
  **combinarlo** con las referencias que adjunte la persona, sacando de ambas la mejor propuesta. Debe
  comportarse como una directora creativa: leer, comparar, elegir y justificar, no listar opciones
  genéricas. Las referencias de la persona mandan en estética y medio cuando existen; el repositorio
  completa, sube el nivel y cubre cuando no las hay.

  **Inventario del paquete recibido:** 3 zips con 322 archivos y **227 imágenes únicas**. La carpeta
  "belleza" contiene copia de todos los demás nichos (95 duplicadas). Grupos: variadas (99: conceptos de
  producto y lifestyle de nivel campaña), piezas con texto (21: layouts, grillas de feed, fichas con
  etiquetas), nichos (belleza, bienestar, contenido, fisioterapia, inmobiliaria, mascotas, peluquería,
  restaurantes). Peso comprimido: unos 18 MB a 1000 px o 13 MB a 800 px.
  **Plan para el paquete final:** `assets/referencias/` sin duplicados (general, texto y una carpeta por
  nicho) + `assets/referencias/indice.md` con una línea por imagen: qué enseña (concepto, layout,
  tipografía, luz, paleta), el formato de sesión o concepto del banco que ilustra (#N), y su nivel:
  ★ referente de campaña (para aspirar) o ◦ convención del nicho (muestra lo que hace la categoría, no el
  nivel a copiar). Marcar las que son de marcas reales (Nivea, Rhode, Coca-Cola, Dunkin', Starbucks…).
  **Comportamiento pedido (aclaración de la usuaria):** revisar las imágenes, hacerles ingeniería inversa,
  mezclarlas y dar la mejor propuesta. Diseño: el índice guarda la **lectura ya hecha** de cada imagen
  (mecanismo, por qué funciona, layout, tipografía, luz, paleta, sesión #N), así la skill "conoce" las
  227 siempre sin abrirlas todas. En cada pedido: (1) filtra el índice por nicho, objetivo y medio;
  (2) preselecciona 4–6 y abre esas imágenes para mirarlas de cerca; (3) suma las referencias de la
  persona; (4) mezcla con la regla 3–2–1 dentro del embudo creativo (6–8 combinaciones, muestra las
  mejores); (5) dice qué tomó de cada imagen (con su nombre de archivo) y por qué esa mezcla gana.
  **Decisión de la usuaria:** se incluyen todas; son referencias de uso educativo. La skill las usa solo
  para leer el mecanismo (nunca reproduce logos, nombres ni diseños de esas marcas) y aplica la regla 3–2–1.

## Prueba 5: marca desde cero
_Pendiente._
