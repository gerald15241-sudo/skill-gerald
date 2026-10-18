# Registro de pruebas: prompts-de-contenido v1.7.0

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

### Hallazgos para corregir
| # | Hallazgo | Causa | Corrección propuesta |
|---|---|---|---|
| 2.1 | Tipografía serif editorial (DM Serif Display) en una marca workwear/streetwear: no se siente Dickies. | Skill. `tipografia.md` pone "moda" bajo "Lujo editorial" (DM Serif Display es el primer combo) y no tiene vibra streetwear/workwear; en la express no se miró la identidad real de la marca; "Qué tomé" no incluyó la capa de tipografía. | (a) Orden obligatorio para elegir tipografía: identidad real de la marca → capa 3 de las referencias → vibra del nicho; el combo listo es el último recurso. (b) Agregar vibra "Streetwear / workwear / heritage" y aclarar que moda ≠ lujo por defecto. (c) "Qué tomé de cada referencia" incluye tipografía cuando la referencia tiene texto. (d) Curaduría: prueba de marca tapada (sin el logo, ¿la tipografía y el tono se sienten de esta marca?). |
| 2.2 | No preguntó cómo debían ser los modelos (tipo de casting, edad, rasgos, vibra). | **Diseño de la ruta express (error mío).** La express no definía qué hacer si la persona quiere modelo y no lo tiene; creó los modelos inline, saltándose el flujo de `modelo-ugc.md`. | Si en la express la persona quiere persona y no tiene modelo: sale de la express para esa parte. Pregunta en un solo mensaje tipo de casting (agencia / UGC con buen casting / persona real), edad, rasgos y vibra; genera primero el modelo con el molde de avatar (playbook §1) o `personas-reales.md`; con el modelo aprobado como `@imagen`, sigue la pieza. Alternativa para quedarse en express: solo manos o persona sin rostro. |
| 2.3 | Realismo de los modelos flojo: piel pareja y pulida, look catálogo IA. | Skill (consecuencia de 2.2). Sin modelo creado con el molde de avatar, no entra el bloque de realismo del carril de modelos (poros, vello, asimetría, RAW). | Se resuelve con 2.2. Además, curaduría: si hay persona, el prompt debe llevar el bloque de piel del carril correcto (dewy del playbook o natural de `personas-reales.md`), nunca una descripción corta propia. |
| 2.4 | La identidad de los modelos cambia entre piezas (el hombre de "DE TALLER A LA CALLE." no es el mismo de las otras dos). | Skill (consecuencia de 2.2). Sin `@imagen` de modelo no hay identity lock posible en una serie. | Se resuelve con 2.2: en series con persona, el modelo aprobado va siempre como `@imagen`. |
| 2.5 | Entregó 3 piezas con conceptos distintos cuando la express promete una dirección. | Por confirmar (falta ver el mensaje de entrega). | Revisar si fue pedido de la usuaria o desvío de la regla. |

## Prueba 3: servicios (fisioterapia)
_Pendiente._

## Prueba 4: campaña de moda
_Pendiente._

## Prueba 5: marca desde cero
_Pendiente._
