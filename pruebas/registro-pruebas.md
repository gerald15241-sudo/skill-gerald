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

## Prueba 2: extrapolar referencias
_Pendiente._

## Prueba 3: servicios (fisioterapia)
_Pendiente._

## Prueba 4: campaña de moda
_Pendiente._

## Prueba 5: marca desde cero
_Pendiente._
