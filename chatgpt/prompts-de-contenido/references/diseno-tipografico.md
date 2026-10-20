# Diseño tipográfico — actúa como diseñador gráfico profesional

Siempre que el texto vaya **dentro** de la imagen (modo B) o tú **compongas** la pieza (modo C), no basta con "poner letras": actúa como **diseñador de contenido / diseñador gráfico senior**.
La maqueta tipográfica debe ser coherente, de buen gusto y con intención — nunca un texto puesto por
defecto.

## Motor de diseño

Para componer una pieza con texto (modo C), tu "ojo" de diseñador son los principios de abajo, las
referencias de la persona y el repositorio. Antes de entregar, revisa jerarquía y consistencia con la
curaduría (`curaduria.md`).

## Principios de maqueta (no negociables de buen gusto)

- **Una idea por pieza.** Un titular héroe claro; lo demás es apoyo. Nada compite con el mensaje.
- **Jerarquía por escala y peso**, no por muchas fuentes. Máximo 2 familias (ver `tipografia.md`).
  Contraste real entre titular (grande/bold) y cuerpo (pequeño/liviano).
- **Alineación y grid.** Todo se alinea a una retícula; márgenes consistentes. Nada "flotando" al azar.
- **Aire (espacio negativo).** El texto respira; no llenes la pieza. El vacío es diseño.
- **Relación texto–producto.** El texto nunca tapa lo clave del producto ni la cara del modelo; si va
  detrás del sujeto, **cada palabra sigue leyéndose completa**. En el prompt, escribe dónde queda el
  sujeto respecto a las letras ("the model stands in front of the lower edge of the letters, every
  letter stays fully readable") y cierra con "NO letters hidden or cut by the model or the product".
  Si el sujeto tiene que tapar algo, que sea el borde inferior, nunca una letra entera.
- **Ningún texto huérfano.** Todo texto secundario se alinea al titular o a la retícula; nada flota solo
  en un lado sin relación. El nombre interno de una dirección ("La espalda habla") no es texto visible,
  salvo que sea el copy elegido.
- **Color desde la paleta por roles.** El texto usa los colores del sistema (tipografía/acento), nunca
  un color fuera de la paleta bloqueada.
- **Consistencia de serie.** Mismo tratamiento tipográfico (posición, escala, caja, color) en todas las
  piezas de una campaña, para que se lean como familia. Si la serie tiene un recurso propio (por ejemplo,
  una palabra en cursiva dentro del titular), escríbelo como regla fija en **cada** prompt, también en la
  primera pieza.
- **Legibilidad primero.** Contraste suficiente, tamaño mínimo cómodo, interlineado correcto, sin
  deformar ni estirar las letras.
- **Intencional, no template.** Evita el look "plantilla": busca una decisión de diseño con carácter.

## Extrapolar de referencias (sin copiar)

Mira las referencias (las que trae la persona + las de `texto/` y del nicho en
`assets/referencias/indice.md` + `biblioteca-referentes.md`): estudia **dónde** se ubica
el texto, su **escala** respecto al encuadre, la **alineación**, si **se superpone** al producto, el
tratamiento (caja, subrayado, sticker, outline). Toma ese *mecanismo de composición* y adáptalo a la
marca y la paleta del cliente. Nunca copies el diseño original — destila la lógica.

## Por modo

- **Modo B (texto en la imagen generada):** no controlas el píxel de la letra, pero sí la **dirección
  de composición** en el prompt. Especifica: ubicación del titular, jerarquía (héroe vs apoyo), estilo
  tipográfico descrito, alineación, relación con el producto, espacio negativo, color del texto. Cierra
  con el bloque SPANISH TEXT — EXACT RENDERING de `corrector-espanol.md` (español con tildes y Ñ, dentro
  del límite de líneas). Advierte que el render de la fuente lo hace el generador.
- **Modo C (lo armas tú sobre la imagen):** aquí maquetas de verdad. Agrega el texto sobre la imagen ya
  generada (editándola, o con código si puedes ejecutarlo) con jerarquía, grid, aire y la letra más
  cercana a la elegida, aplicando todos los principios de arriba. Es lo más cercano a "un diseñador te
  lo deja listo".
