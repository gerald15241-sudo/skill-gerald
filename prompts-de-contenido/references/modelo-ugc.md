# Flujo de modelo (UGC / híbrido)

Cuando el enfoque es UGC o híbrido, este es el **paso 0 obligatorio**: nunca inventes la modelo por
tu cuenta ni generes slides sin resolver la identidad primero.

**¿Qué tipo de casting?** Antes de nada, pregunta con botones qué tipo de persona quiere, explicando cada
opción en una línea:

- **Modelo UGC de agencia de modelos** — modelos con el **estándar de las grandes marcas** (agencia
  profesional): rostro pulido, proporciones y presencia aspiracionales, calidad editorial — **pero que
  siguen siendo REALES**, con piel y textura humana (no plásticos, no cara de catálogo falso, no CGI). Para
  marcas que quieren imagen premium pero creíble.
- **Modelo UGC más casual (pero con buen casting)** — se ve cercana, real y creíble, NO de pasarela, pero
  igual bien elegida y atractiva: la cara de "creador de contenido" que conecta. El UGC que más convierte.
  Para que salga **atractiva sin volverse plástica ni promedio**, aplica el balance de `realismo-anti-ia.md`:
  anclar belleza con la **estructura ósea** (armonía facial, ojos claros y vivos, pómulos, buen grooming,
  luz halagadora), piel sana **dewy y luminosa** (brillo natural roto por los poros, nunca mate ni waxy),
  y **generar 3–4 y elegir la mejor** (así es un casting real). Si tienes una cara atractiva de referencia,
  úsala como `@imagen` para fijar la belleza.
- **Persona real de la vida real (no modelo)** — gente común con edad y rasgos reales, para **otro tipo de
  contenido**: testimonios creíbles, personajes, casting diverso, equipo/fundadores, extras, documentales.
  Usa el módulo `personas-reales.md` (prompt maestro con variables + negativos anti-modelo).

Las tres siguen el mismo flujo (identidad, ángulos, nivel de producción, realismo); solo cambia el "tipo de
cara". Si la persona no sabe, propón tú la que mejor sirva al objetivo y explica por qué.

## Ofrece REFERENCIAS en el casting — las lees TÚ, no el generador

Al elegir UGC casero con casting, **proponle a la persona adjuntarte referencias A TI (en el chat de la
skill)** antes de generar. Punto clave del método: **la persona NO adjunta fotos en el generador.** Tú
**lees los detalles de cada referencia y los describes dentro del prompt de texto**; el generador solo
recibe ese texto. Así no se clona a nadie y no hace falta subir imágenes al generador.

Qué pedir, y qué extraes de cada una (en el prompt lo escribes en inglés):
- **Referencia de CARA / modelo (la más importante) — INSPIRACIÓN, no copia.** Mírala y **describe en
  palabras** su nivel de atractivo y tipo: estructura ósea (pómulos, mandíbula, forma de cara), armonía,
  ojos, labios, vibra. Luego generas una **persona NUEVA y distinta** con ESE nivel, cambiando a propósito
  rasgos (edad, fenotipo, cabello) para que no se parezca a la original. En el prompt: "an attractive woman
  with [rasgos de belleza leídos de la referencia], a clearly different unique person — not a copy". Esto
  **sube la belleza** sin clonar ni adjuntar nada.
- **Referencia de ILUMINACIÓN / mood.** Lee el esquema (dirección, dureza, temperatura, aireada o penumbra)
  y descríbelo en el prompt (ver `biblioteca-dp.md`).
- **Referencia de ATUENDO / estilo.** Lee prenda, colores y vibra; descríbelos como vestuario.
- **Referencia de ESCENA / lugar.** Lee el tipo de espacio y descríbelo como fondo.
- **Referencia del PRODUCTO** (si va en la toma): describe el producto fiel (product accuracy).

Regla: **tú eres los ojos.** Analizas las referencias, destilas los detalles y entregas **un prompt de solo
texto** listo para pegar — la persona no sube imágenes al generador. Di en una línea de dónde salió cada
decisión (trazabilidad). Si no trae referencias, propónle 2–3 direcciones de casting en texto para que elija, o usa búsqueda de
imágenes para mostrarle opciones.

**Excepción — solo si la persona QUIERE la misma modelo fija:** ahí sí puede usar su generador con imagen de
referencia/identity lock (`@imagen`) para repetir la MISMA cara. Pero eso es la excepción (modelo recurrente),
no el flujo normal de casting variado.

## Atajo: crear el modelo antes de una pieza (ruta express o pieza suelta)

Cuando la persona pide una pieza **con persona** y **no tiene modelo**, nunca lo inventes dentro del
prompt de la pieza: se pierde tu bloque de realismo y la identidad cambia entre piezas. Créalo primero,
con los moldes de la autora, en tres pasos:

1. **Un solo mensaje de casting** (botones + campo abierto):
   - Tipo de casting: agencia · UGC con buen casting · persona real (explica cada uno en una línea).
   - Por cada persona: género, rango de edad, fenotipo y tono de piel, cabello (color, largo, tipo),
     rasgos distintivos y vibra.
   - Referencia de cara: obligatoria en UGC con buen casting (bloque 💡 de SKILL.md); opcional en los
     otros dos. Si no trae, ofrécele 2–3 direcciones de casting en texto.
2. **El prompt del modelo, adaptado del molde que corresponde al tipo de casting (REGLA #2).** Cada
   casting tiene su molde; no los mezcles:
   - **Agencia** → `playbook-original.md` §1.1 (avatar base, retrato editorial de estudio). Si después hace
     falta más de una toma, §1.2 (personality board) o el set mínimo de §1.3 (frente, 3/4 y cuerpo entero).
     Se cambia solo la identidad: rasgos y, si es hombre, el género y las menciones de maquillaje
     ("woman", "minimal makeup", "glossy lips"). Los poros, el vello, la cámara y el RAW quedan intactos.
   - **UGC con buen casting** → **NO uses el avatar de estudio de §1.1** (es el look de agencia). Sigue el
     flujo de casting de arriba, tal cual:
     1. Pide la **referencia de cara** (obligatoria) y **léela tú** en el chat: estructura ósea, armonía,
        ojos, labios, vibra. Si no la trae, no generes: ayúdala a conseguirla o propón 2–3 direcciones de
        casting en texto para que elija.
     2. Pregunta el **nivel de producción** (sección E): estudio, locación o casera; si es casera, el
        lugar y el encuadre (selfie, espejo, brazo extendido…).
     3. Escribe un prompt **de solo texto** para una persona **nueva y distinta** con el nivel de esa
        referencia ("a clearly different unique person — not a copy"), con la estructura y la piel de
        `realismo-anti-ia.md` (§3 y la mini-receta §7) y la escena, luz y cámara del nivel de producción
        (§E; en casera, el texto de "Casera (pro)"), nunca el set de estudio editorial. Al generador no
        se adjunta la referencia.
     4. **Genera 3–4 y quédate con la mejor**, como en un casting real.
   - **Persona real** → prompt maestro de `personas-reales.md`, con su look natural de open-shade.
   - **Varias personas** (pareja, grupo): una ficha y un prompt por persona, generados por separado. En la
     pieza, cada una va con su propio `@imagen` y se prohíbe intercambiar rasgos entre ellas (como los
     perros de GUAUKIES, `playbook-original.md` §7.3).
3. **Aprobación y anclaje:** la persona genera el modelo, elige el mejor y lo adjunta; desde ahí va como
   `@imagen` en la pieza, con IDENTITY LOCK, en esa pieza y en todas las siguientes de la serie.

Si la persona no quiere ese paso extra, ofrece quedarse en solo producto, solo manos o persona sin
rostro. Si aun así quiere una persona sin crearla antes (una sola pieza, sin serie), el prompt de la pieza
lleva **el bloque completo de piel y cámara del carril** copiado del molde, nunca una descripción corta
propia, y se le avisa que esa persona no se podrá repetir igual en otra pieza.

## A. ¿Modelo propia o la creamos?

Pregunta siempre:
- **Ya tengo mi modelo** → la persona sube su set (mood board o fotos en varios ángulos). Ese set se
  vuelve el ancla de identidad. Escribe la **ficha de identidad** mirando las fotos (no la inventes).
- **La creamos desde cero** → pasa a la ficha de identidad (abajo).
- **La creamos, pero con ajustes** → propón y deja que corrija.

## B. Ficha de identidad (si la creamos)

Pregunta lo esencial con botones, **siempre con un campo abierto** para que la persona agregue por
escrito (una cicatriz, pecas, un tatuaje, un estilo). Dimensiones:
- Género · Rango de edad · Fenotipo/aspecto (latina, europea, afro, asiática, mestiza…) · Tono de
  piel · Color y largo de cabello · Tipo de cabello · Rasgos/detalles distintivos (abierto) ·
  Vibra/estilo (deportivo, editorial, cotidiano…).

Con eso escribe el **identity lock** (ver `bloques-obligatorios.md` §2), que se repetirá idéntico en
cada pieza.

## C. Ángulos: propón tú según el objetivo

No generes los ~22 ángulos del playbook por default. **Propón el set mínimo útil** para lo que se va
a hacer, del catálogo del playbook. Ejemplos:
- Carrusel storytelling (5 slides): frente neutro + tres cuartos + cuerpo entero + una expresión
  (risa/sonrisa). Perfil de repuesto.
- Product board: frente neutro + 3/4 izq + 3/4 der + lateral + cuerpo entero (mapeo M1–M5).

Catálogo de ángulos del playbook: frente · 3/4 izq · 3/4 der · perfil izq · perfil der · mirando
arriba · mirando abajo · cabeza inclinada. Expresiones: risa abierta · sorpresa · cantando ·
pensativa · sonrisa emocionada · adormilada. Cuerpo: frontal · espalda · saludando · saltando ·
sentada · caminando · señalando · bailando.

## D. Personality board

Para crear la modelo, usa los prompts del playbook: primero el **personality board en una imagen**
(grid ~8 paneles, misma mujer, identity lock, negative prompt), o **imagen por imagen** anteponiendo
el bloque de identidad a cada prompt de ángulo/expresión.

## E. Nivel de producción (pregúntalo SIEMPRE en UGC)

Antes de generar las fotos UGC, pregunta **qué tipo de toma quiere** —cambia por completo la luz, el
fondo y la cámara, pero **nunca** el hiperrealismo—:

1. **Estudio fotográfico** — set controlado: fondo seamless/ciclorama o color sólido, luz de estudio
   (softbox/beauty dish), look limpio y editorial. Para catálogo, e-commerce premium, campaña pulida.
2. **Profesional en locación** — luz cuidada pero en un entorno real (cafetería, calle, interior con
   estilo), estética de producción de marca, con dirección de arte. Pro, pero no de estudio.
3. **Casera / casual (UGC real) — pero de CALIDAD profesional.** Se ve hecha por la persona en casa:
   luz natural, encuadre espontáneo, imperfección creíble (el look que más convierte en UGC) — **pero
   nítida y bien capturada**, no una foto mala. "Casero" es la vibra, no la calidad. Usa el módulo
   `realismo-anti-ia.md`. **Si elige esta, pídele dos cosas:**
   - **Lugar/escenario:** dónde ocurre (baño frente al espejo, cocina, cama, sala, carro, exterior…).
   - **Ángulo/encuadre:** selfie a pulso, brazo extendido, espejo, cenital sobre la mesa, POV, trípode
     a media distancia… Propón opciones si no sabe.

   **Este nivel también sirve para SESIONES completas tipo lifestyle** (no solo una foto UGC suelta): una
   mini-sesión "en casa / lugar casual" con varias tomas que se ven de **la misma sesión** — misma modelo
   o persona, mismo lugar y luz, cambiando pose/encuadre/acción. Ideal para product board casual, catálogo
   cercano o feed de marca que no quiere verse de estudio. Mantén el look (luz natural, calidad alta, piel
   real) constante en toda la serie, igual que una sesión real; varía escena y gesto, no el estilo.

**Regla de oro — el hiperrealismo NO se negocia según el nivel.** En las tres opciones los prompts
mantienen **8K, foto real, microdetalles** (poros, textura de piel y cabello, tela, reflejos reales) y
el `AVOID` anti-CGI/piel plástica. Lo que cambia es el *entorno y la cámara*, no la calidad:
- Estudio → "studio lighting, seamless backdrop, 8K, hyperreal skin texture, sharp micro-detail".
- Profesional → "cinematic natural light on location, shallow depth of field, 8K, hyperreal micro-detail".
- Casera (pro) → "candid at-home photo, natural window light, modern smartphone portrait mode / 50mm
  look, shallow depth of field, sharp focus, clean high quality, 8K photoreal skin with real pores and
  micro-detail, no CGI, no plastic skin — natural but good quality, NOT a bad/blurry/grainy phone photo".
  El look "casero" es la *vibra* (luz natural, encuadre espontáneo), nunca baja calidad ni cara deformada.

Mantén esta decisión constante en toda la sesión/carrusel (igual que paleta e identidad), salvo que la
persona quiera mezclar a propósito.

**Para que NO parezca IA** (sobre todo en casera/UGC, pero aplica a las tres): usa siempre el módulo de
`realismo-anti-ia.md` — micro-detalle humano (poros, brillo, rojez, pecas, cejas sin peinar, baby hairs,
asimetría) + negativo fuerte contra piel lisa/cera, simetría perfecta, retoque de belleza, filtro y look
CGI. Es lo que separa un retrato creíble de uno "de IA". Mantén 8K; la imperfección es textura, no baja
calidad.

## F. Regla de consistencia clave

**Genera la slide/imagen 1 primero, apruébala, y úsala como `@imagen` de referencia en las
siguientes.** Es lo que garantiza que sea la misma persona en todo el carrusel/sesión. En cada pieza
corren identity lock (fotos del modelo) + product lock (foto del producto) en paralelo.
