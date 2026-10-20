# Biblioteca de dirección de fotografía (DP profesional)

Esta es la base técnica para que el director de arte (`director-arte-cine.md`) proponga y escriba spots a
nivel de productora real, no "fondo bonito". Úsala para traducir una intención ("que se vea caro",
"apetitoso", "tecnológico") en **decisiones concretas de luz, lente y cámara**, y para redactar esa parte
del prompt con precisión. Todo en inglés en el prompt final (el generador responde mejor).

## 1) Luz — el 70% del resultado

**Esquema base (3 puntos) y sus roles:**
- **Key (principal):** define forma y dirección. Su ángulo y dureza marcan el carácter.
- **Fill (relleno):** suaviza o no las sombras. Decide el **ratio de contraste**.
- **Rim/back (contra):** separa el sujeto/producto del fondo con un borde de luz. Clave para "premium".

**Ratio de contraste (el dial de "mood"):**
- 1:1–2:1 → plano, limpio, catálogo/e-commerce, high-key.
- 3:1–4:1 → editorial con volumen (lo más usado en premium).
- 8:1+ → dramático, clave baja, lujo/misterio.
En el prompt se dice con palabras: "soft low-contrast even light" vs. "high-contrast dramatic lighting,
deep shadows".

**Calidad de la luz:**
- **Suave** (softbox grande/ventana/nublado): sombras graduales, piel y texturas amables. "soft diffused
  light, large softbox, gentle gradual shadows".
- **Dura** (haz directo/sol/flash desnudo): sombra marcada, moda/street, energía. "hard direct light,
  crisp defined shadows, single bare flash".

**Esquemas con nombre (úsalos por intención):**
- **Rembrandt:** key a 45° arriba, triángulo de luz en la mejilla. Retrato con carácter.
- **Loop / split:** sombras de nariz controladas / media cara en sombra (dramático).
- **Butterfly (paramount):** key frontal alta, sombra bajo la nariz. Belleza/beauty.
- **Chiaroscuro:** un solo haz, el resto en negro. Producto que emerge de la sombra (lujo).
- **Clamshell:** key arriba + fill abajo (bandeja/reflector). Beauty y joyería, piel impecable.
- **Rim doble / kicker:** dos contras laterales. Bebidas, tech, cosmética — bordes brillantes.
- **Golden hour / contraluz:** sol bajo detrás, halo cálido, flare. Aspiracional, lifestyle.
- **High-key:** fondo blanco, luz envolvente, casi sin sombra. Premium minimal, clean.
- **Neón / práctica de color:** geles o luces de escena (letreros, LED). Nocturno, tech, bebidas.

## 2) Lente y cámara — cómo se "siente" la imagen

- **Distancia focal:**
  - 24–35mm: contexto/escena, leve drama de perspectiva (gran angular → épico, cuidado con distorsión en caras).
  - 50mm: natural, documental, lifestyle honesto.
  - 85–135mm: retrato premium, **compresión** halagadora, fondo que se derrite (bokeh). El clásico de moda/beauty.
  - Macro: textura y detalle extremo (gota, poro del producto, trama del textil, burbujas).
- **Apertura:** f/1.4–2.8 → fondo cremoso, sujeto aislado (premium). f/8–f/16 → todo nítido (product shot
  de catálogo, grupo). "shot on 85mm, f/1.8, shallow depth of field" vs. "50mm, f/11, deep focus".
- **Mirada de cine:** "anamorphic lens" (flares horizontales, bokeh ovalado, cinemático); "tilt-shift"
  (plano de enfoque selectivo/maqueta); "probe/macro lens" (meterse en la escena del producto).
- **Ángulo de cámara:** nivel de ojos (neutro/honesto), contrapicado (poder/épica), picado (control/flat
  lay), cenital 90° (lujo de mesa), holandés (tensión/energía), eye-level de celular (UGC real).

## 3) Atmósfera y textura (lo que separa "caro" de "plano")

Haze/niebla de set, humo, partículas en el haz de luz, vapor (comida/bebida caliente), condensación y gotas
(bebida fría), salpicadura congelada (splash), polvo dorado, lluvia a contraluz, reflejos sobre superficie
mojada o espejo. En el prompt: "atmospheric haze in the light beam, fine water droplets, condensation on the
glass, frozen splash, steam rising".

## 4) Color grade

- **Teal & orange** (cine comercial), **ámbar cálido** (apetito/acogedor), **frío editorial** (tech/limpio),
  **monocromático de marca**, **desaturado premium**, **alto contraste punchy**.
- Regla de la skill: respeta la paleta por roles; el **color héroe se reserva al producto** y el grade no lo
  contamina. "warm cinematic grade, teal shadows, the only saturated color is the product".

## 5) Recetas por tipo de producto (punto de partida pro)

- **Bebida fría / lata / botella:** fondo oscuro o de color, **doble rim** para bordes brillantes,
  condensación y gotas, salpicadura congelada, 100mm macro, f/4. Hielo y burbujas reales.
- **Bebida caliente / café:** luz de ventana cálida lateral, vapor subiendo a contraluz, madera/cerámica,
  85mm f/2, grade ámbar.
- **Comida:** luz suave lateral/posterior (nunca flash frontal), 3:1, props mínimos, cenital o 45°, macro para
  textura, vapor si es caliente, frescura (gotas, hierbas). "appetizing, natural soft side light".
- **Joyería / relojes:** clamshell + rim, fondo limpio o terciopelo, macro, foco apilado (todo nítido),
  reflejos controlados, cero huellas. Lujo = negro mate o blanco high-key.
- **Cosmética / skincare:** beauty clamshell, piel/gel impecable pero real, gotas de producto, mármol/acrílico,
  rim de color suave, 100mm macro para textura de crema.
- **Tech / electrónica:** clave baja + rims de neón/color, superficie reflectante, haze, anamórfico, grade
  frío de alto contraste. Minimal, futurista.
- **Moda / textil:** luz dura o golden hour, 85mm, movimiento de tela, locación real, flare; o editorial
  high-key. El material manda (brillo del cuero, caída de la seda).
- **Auto / grande:** golden hour o estudio con softbox gigante de barrido, rims largos, reflejos limpios en
  carrocería, gran angular controlado.

## 6) Cómo se escribe en el prompt (orden sugerido)

> [escena/locación] + [esquema de luz + calidad + ratio] + [lente + apertura + ángulo] + [atmósfera] +
> [color grade] + [dirección del producto] + [realismo 8K + AVOID].

Ejemplo: "Luxury product shot of @imagen1 perfume bottle on a black stone pedestal, single hard key light
from the left (chiaroscuro, 8:1 high contrast), two subtle color rim lights, 100mm macro lens at f/4, slight
eye-level angle, atmospheric haze in the light beam, warm high-contrast cinematic grade — the only saturated
color is the amber perfume. 8K, photorealistic, sharp micro-detail. AVOID: CGI look, plastic reflections,
fingerprints, wrong logo."

Honestidad: el generador aproxima la física de la luz; itera ajustando dureza/ratio/ángulo. Esta biblioteca
es para **decidir y describir** como un DP, no un control de luces real.
