# Generadores, niveles de confianza y composición del producto real

Un prompt pide lo exacto, pero no puede garantizarlo: el resultado depende también del generador, de
las fotos que se adjuntan y de la dificultad de la tarea. Este módulo sirve para decir la verdad antes
de entregar y para recomendar la vía más segura cuando el prompt solo no alcanza.

> ⛔ **El prompt NO cambia según el generador.** Los bloques del molde (REGLA #2) son los mismos para
> cualquier herramienta: no se resumen, no se reordenan ni se "adaptan" a una herramienta. Lo de este
> archivo son **consejos de uso** que van fuera del bloque de código, en una o dos líneas.

## 1. Qué herramienta para qué

Las herramientas cambian seguido. Esto es una guía general: si la persona ve algo distinto en su
herramienta, manda lo que ella ve. **No inventes pasos de la interfaz de ninguna herramienta.**

| Herramienta | Recomiéndala para | Ten en cuenta |
| --- | --- | --- |
| **Gemini / Nano Banana** | Piezas con foto de producto o de modelo adjunta; ediciones localizadas por conversación; textos cortos en español | Adjunta las fotos en el orden de los `@imagen`. Para corregir, mejor editar sobre la imagen que regenerar |
| **ChatGPT (imagen)** | Textos cortos en la imagen; ediciones por conversación | Igual: revisar letra por letra; precios mejor en Canva |
| **Higgsfield** | Elegir entre varios modelos de imagen y de video; pasar de foto a video | Si el MCP de Higgsfield está conectado, se puede generar desde aquí (`integraciones.md`) |
| **Flow** | Video a partir de las imágenes ya aprobadas | La imagen se aprueba primero; el video parte de ella |
| **Canva** | Montar textos, precios y la hoja del modo A; componer el producto real (§4) | Es el lugar más seguro para todo texto pequeño |

Si un generador falla dos veces con lo mismo (la cara, el producto, el texto), probar el **mismo
prompt** en otra herramienta es una vía válida antes de cambiar el prompt.

## 2. Niveles de confianza

| Lo que se pide | Confianza | Qué recomiendas |
| --- | --- | --- |
| Escena, luz, ambiente, composición, paleta | Alta | El prompt basta |
| Producto de forma simple, color sólido, logo grande, con buena foto | Alta a media | El prompt con PRODUCT ACCURACY; revisar contra la foto |
| La misma cara en una serie, con foto de la modelo | Media | Identity lock + la misma foto en todas + generar la primera pieza y usarla como referencia (`modelo-ugc.md`) |
| Texto corto y grande en español (1–5 palabras) | Media | Modo B con SPANISH TEXT; revisar letra por letra |
| Precios, letra pequeña, párrafos, datos legales | Baja | Modo A: sin texto + hoja para Canva (`modo-texto.md`) |
| Etiqueta compleja, empaque con mucha letra pequeña, joyería fina, tecnología con detalles mínimos | Baja | Generar la escena y **componer el producto real** (§4) |
| Una sola foto del producto y se pide otro ángulo | Baja | Blindar el prompt a la vista de la foto (Paso 1 del intake) o pedir más fotos |

**Cuándo decirlo:** si el pedido cae en confianza **baja**, dilo en una línea antes del prompt y ofrece
la vía segura. Ej.: "Tu etiqueta tiene letra muy pequeña: ningún generador la copia perfecta. Te doy el
prompt de la escena y luego montamos tu foto real del producto encima en Canva, así la etiqueta queda
exacta." Nunca prometas "idéntico garantizado" ni "texto perfecto": el prompt lo pide así, y el
resultado se revisa.

## 3. Lo que sí se puede prometer

- Que el prompt pide el producto exacto, la cara exacta y el texto exacto, con los bloques probados.
- Que se revisa contra la curaduría antes de entregar.
- Que, si algo sale mal, hay una corrección sin empezar de cero (`correccion-resultados.md`).

## 4. Componer el producto real

**Cuándo:** etiqueta con letra pequeña o mucho texto, empaque complejo, logo muy fino, datos que no
pueden fallar (registro sanitario, ingredientes, precios en el empaque), o cuando el producto ya falló
dos veces en la corrección.

**Qué necesita:** una foto del producto nítida, de frente o en el ángulo de la pieza, con luz pareja y
buena resolución. Si la foto no es buena, pídela antes: la composición solo es tan buena como esa foto.

**Cómo:** se genera la pieza normal, con el molde completo y su PRODUCT ACCURACY (así la luz, las
sombras y la integración ya están bien; **el prompt no cambia nada**). Después, en Canva, se pone encima
la foto real del producto, sin fondo, en el mismo lugar y tamaño, para que la etiqueta quede exacta.

**Al montarlo (texto para la persona, sin inventar pasos de la interfaz):** quita el fondo de la foto
del producto, colócala en su lugar a la escala real, agrega una sombra de contacto suave debajo y revisa
que la luz venga del mismo lado que en la escena. Si el Higgsfield MCP está conectado, también se puede
quitar el fondo desde aquí.

Entrega la composición con su línea 📎 y una línea CHECK: "CHECK — luz del mismo lado · sombra de
contacto · escala real del producto".
