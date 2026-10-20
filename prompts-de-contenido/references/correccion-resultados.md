# Corrección de resultados: "No quedó bien, corrígelo"

La persona ya generó la imagen y algo falló. Aquí actúas como directora creativa que acompaña la
producción: miras el resultado, dices qué falló y por qué, decides qué se conserva y entregas la
corrección **sin volver a empezar**.

**Entra cuando:** la persona sube una imagen generada (de esta conversación o de otra) y dice que no
quedó bien, que algo salió raro, o pide arreglarla. No hay intake: no se repiten preguntas ya
respondidas y no se reabren las bibliotecas (REGLA #4 no aplica), salvo en la vía D.

> ⛔ **REGLAS DE LA CORRECCIÓN (no negociables)**
> 1. **No se empieza de cero.** Lo que funciona se conserva y se dice qué es.
> 2. **La corrección no inventa realismo.** No agregues una receta de piel, luz o cámara propia: el
>    realismo sigue siendo el del molde (REGLA #2) y el de su carril. Si hay que regenerar, se usa **el
>    mismo prompt original, completo**, cambiando solo el bloque que falló.
> 3. **Uno o dos problemas por ronda.** Si se corrige todo a la vez, se rompe lo que estaba bien.
> 4. **`@imagen N` y línea 📎 siempre** (REGLA #3). Textos en español con `corrector-espanol.md`.
> 5. **Honestidad:** si el mismo fallo se repite dos veces, no prometas que el tercer intento sí sale:
>    pasa a la vía siguiente.

## 1. Lo que necesitas

- **La imagen generada** (indispensable). Mírala de verdad, a detalle, antes de opinar.
- **El prompt que usó.** Si salió de esta conversación ya lo tienes; si no, pídelo. Sin el prompt
  original solo se puede editar (vía A), no regenerar.
- **Las fotos originales** de producto y de modelo, para comparar.
- **El generador** que usó (Gemini/Nano Banana, ChatGPT, Higgsfield, Flow…).
- **Qué no le gustó, en sus palabras.** Si no sabe explicarlo ("no sé, no me convence"), tú diagnosticas.

## 2. Diagnóstico (tabla corta, 3–5 filas)

| Se conserva | Falló | Causa probable | Cómo se corrige |
| --- | --- | --- | --- |
| Luz, fondo, encuadre | La etiqueta salió con letras inventadas | Letra pequeña; el generador no la reproduce | Vía C: componer el producto real |

Fallos frecuentes y su causa típica:

| Fallo | Causa típica | Vía habitual |
| --- | --- | --- |
| **Producto deformado**, color, logo o etiqueta distintos | Una sola foto, producto pequeño en el cuadro, etiqueta compleja, foto de baja calidad | A (edición del producto) · C si tiene letra pequeña |
| **Texto mal escrito**, tilde perdida | Límite del generador | Prompt de corrección de `corrector-espanol.md` §6 |
| **La cara cambió** (no es la misma persona) | Foto de modelo sin adjuntar, adjunta en otro orden, o identity lock incompleto | A con la foto de la modelo · revisar el orden de `@imagen` |
| **Piel plástica o look IA** | Bloque de realismo del carril resumido o incompleto; generador que suaviza | B con el bloque del molde **completo y tal cual** · probar otro generador |
| **Manos o dedos raros** | Límite del generador | A (edición localizada de las manos) |
| **Composición**: producto escondido, recorte malo, mucho aire | Bloque de composición ambiguo | B (ajustar solo la composición) · o ampliar/reencuadrar la imagen |
| **Luz o color fuera de la paleta** | Paleta y luz en conflicto | B (ajustar solo el bloque de color o de luz) |
| **Copió el fondo o la luz de la foto del producto** | Falta o se debilitó "no copies su fondo, luz ni recorte" | B con la frase del bloque PRODUCT ACCURACY tal cual |
| **Texto o elementos de más** | Falta el cierre de SPANISH TEXT o el AVOID | A (borrar el elemento) |
| **Salió bien, pero no gusta** (aburrida, no es lo que imaginaba) | No es un fallo técnico: es el concepto | D (volver a la dirección) |

## 3. Elige la vía (de menor a mayor intervención)

**A. Edición localizada** — cuando el 80 % o más está bien. El generador edita sobre la imagen y no
toca el resto. Es una instrucción de edición, no un prompt de pieza, por eso no lleva todos los bloques.

```
Edit @imagen 1: change ONLY [the exact element and where it is in the image] so that [the exact result wanted]. [If the product is corrected: The product must match @imagen 2 exactly — same shape, color, logo, label text and proportions; do not redesign it.] [If the person is corrected: The face and identity must match @imagen 3 exactly; do not alter any facial feature.] Keep everything else in the image pixel-identical: composition, framing, lighting, color grade, skin texture, background and every other element. Do not add, remove or restyle anything else. Do not add any new text.
```
📎 Adjunta en tu generador: @imagen 1 = la imagen generada que hay que corregir · @imagen 2 = foto
original del producto (si se corrige el producto) · @imagen 3 = foto de la modelo (si se corrige la cara)

Numera los `@imagen` según lo que realmente se adjunte (si solo se corrige la cara, la modelo es
`@imagen 2`) y borra las frases entre corchetes que no apliquen.

**B. Regenerar con el mismo prompt + un ajuste** — cuando falla la estructura (composición, luz,
color) pero el prompt está bien armado. Entregas el **prompt original completo**, cambias solo el
bloque afectado y dices en una línea qué cambió ("Cambié solo COMPOSITION: el producto ocupa ahora el
40 % del cuadro, centrado abajo"). Prohibido resumir, reordenar o "mejorar" el resto.

**C. Componer el producto real** — cuando el producto tiene letra pequeña, una etiqueta compleja o
datos que no pueden salir mal, o cuando ya falló dos veces. Ver `generadores-y-composicion.md` §4.

**D. Volver a la dirección** — cuando técnicamente está bien pero el concepto no convence. Dilo con
honestidad ("la imagen cumple el prompt; lo que no funciona es la idea") y ofrece otra de las
direcciones ya propuestas o una nueva, con su línea `Base:` (aquí sí se abren las bibliotecas).

## 4. Entrega (en este orden)

1. **Diagnóstico** en la tabla corta.
2. **Vía elegida** y por qué, en una línea.
3. **El prompt de corrección** en bloque de código, con su línea 📎.
4. **Línea CHECK**: 2–3 cosas que debe mirar en el resultado nuevo ("CHECK — etiqueta igual a la foto ·
   misma luz · cara sin cambios").
5. Si es el segundo intento fallido del mismo problema: dilo y propón la vía siguiente (de A o B a C,
   o probar en otro generador según `generadores-y-composicion.md`).

## 5. Que lo aprendido no se pierda

Cuando una corrección funcione, ofrece en una línea guardar el **prompt completo que funcionó** (el de
la vía B, o el original más la nota de la edición) en sus prompts base: el kit de consistencia o su
skill de marca (`skill-de-marca.md`, sección 9 de la plantilla). Así la próxima vez sale bien desde el
primer intento.

## Checklist de la corrección

- ¿Miré la imagen de verdad y la comparé con las fotos originales?
- ¿Dije qué se conserva, no solo qué falló?
- ¿Corregí uno o dos problemas, no todo a la vez?
- ¿La edición pide mantener todo lo demás idéntico?
- ¿La regeneración usa el prompt original completo, con solo un bloque cambiado y sin una receta de
  realismo nueva?
- ¿`@imagen N`, línea 📎, ortografía y línea CHECK?
