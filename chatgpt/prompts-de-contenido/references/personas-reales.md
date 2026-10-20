# Personas reales (gente común, NO modelos)

A veces no se quiere una "modelo", sino una **persona real de la vida real**: un cliente de testimonio, un
rostro cotidiano, un personaje, un "extra", un equipo/fundadores, caras para un casting o para poblar una
escena. Gente creíble con edad real, rasgos promedio, imperfección y ropa simple — lo contrario del look
de modelo pulido. Este módulo es para eso. (Método inspirado en decks tipo "FACES"; aquí va destilado, no
se copian prompts ajenos.)

## Cuándo usarlo

- Testimonios / UGC con "persona real", caras de cliente, reseñas.
- Personajes para una historia, casting diverso, extras, multitud, equipo/fundadores ficticios.
- Avatares de marca que deben sentirse humanos y cotidianos, no editoriales.
- Cualquier "quiero una persona que parezca de verdad, no una modelo".

Se combina con: nivel de producción (`modelo-ugc.md`) e IDENTITY LOCK si la persona se repite. Para UGC con
producto, sigue aplicando el product lock. **OJO — carril distinto al de modelos beauty:** aquí el look es
**natural de open-shade, sin glamour**; NO apliques el realismo dewy de modelos (`realismo-anti-ia.md` es del
carril beauty, no de este). Una persona real no debe salir con glow de campaña.

## Principio: común ≠ modelo

El objetivo es **gente normal y creíble**. Pide explícito lo que un casting de modelos evitaría:
- Edad real y visible (líneas, canas, ojeras suaves, textura de piel madura si aplica).
- Rasgos **promedio y asimétricos**, no simétricos ni "perfectos".
- Peso/complexión variados, dientes normales (no blanqueados), piel con poros, pecas, lunares, marcas.
- Ropa **sencilla, de un color**, cotidiana (no moda de pasarela).
- Expresión neutra y relajada, mirada directa y tranquila.
Esto, más los negativos de abajo, es lo que hace que NO parezca modelo ni render.

## Prompt maestro (plantilla con variables)

Rellena los `[corchetes]` y deja fijo el resto. En inglés, para el generador:

> "Create a photorealistic candid portrait of a fictional **[EDAD + ORIGEN]** person, with **[TONO DE PIEL
> + SUBTONO]**, **[OJOS: color/forma]**, **[FORMA DE CARA + UN RASGO MEMORABLE]**, **[CABELLO]**, wearing
> **[ROPA SENCILLA EN UN SOLO COLOR]**. Eye-level smartphone main-camera perspective, straight-on, head and
> upper chest in frame. Calm direct eye contact, relaxed closed lips, neutral expression. **[ESCENARIO:
> calle/lugar real]** behind them, recognizable but gently out of focus. Soft daylight in open shade,
> natural shadows that keep real skin colour. Realistic irregular pores, fine facial hair, subtle
> asymmetry, natural tonal variation, real age texture. Sharp eyes, gradual falloff in focus. An ordinary
> real person, NOT a model.
> NEGATIVE: fashion-model look, perfect symmetry, flawless/retouched skin, beauty filter, waxy smoothing,
> skin lightening, heavy makeup, glamour lighting, airbrushed, glossy render, 3D render, illustration,
> whitened teeth, head tilt, text, logos, collage."

**Variables que cambian por persona:** edad + origen, tono/subtono de piel, ojos, forma de cara + 1
detalle, cabello, 1 color de ropa, escenario real.
**Lo que queda fijo:** encuadre frontal a nivel de ojos, luz de open-shade, textura de piel real, y los
mismos negativos.

## Serie / casting consistente (si son varios)

Para que un set de personas se lea como **una sola serie** (galería, casting, equipo):
- **Fija el encuadre igual en todos:** mismo recorte (cabeza + pecho), cara frontal centrada, ojos y
  labios a la misma altura (p. ej. ojos ~40% desde arriba, labios ~51%, cara ~42% del ancho). Así ningún
  rostro "salta" respecto a los otros.
- **Contrasta vecinos:** alterna género, edad y tono de piel entre caras seguidas para que la serie tenga
  variedad y no se mezclen entre sí.
- Cambia por persona solo las variables de arriba; todo lo demás, idéntico.

## Línea CHECK por persona (verificación)

Como el deck original, cierra cada persona con una **línea CHECK** corta de 2–3 cosas que deben cumplirse,
para revisarla (entra en la curaduría, `curaduria.md`). Ej.: "CHECK — canas visibles · piel sin aclarar ·
fondo sin texto". Si falla, corrige con una edición, no regeneres todo.

## Honestidad

El generador aproxima; a veces hay que iterar. "Persona real, no modelo" se logra con rasgos comunes +
imperfección + los negativos anti-modelo/anti-filtro, manteniendo 8K y foto real. Si es una persona
inventada, que quede claro que es ficticia; no recrees a una persona real identificable sin su permiso.
