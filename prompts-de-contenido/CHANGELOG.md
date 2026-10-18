# Cambios de la skill prompts-de-contenido

## v1.9.3 — realismo de modelos idéntico a la v1.4.0

- En `SKILL.md` se restauran **palabra por palabra** desde la v1.4.0 el bloque "REALISMO DE ROSTRO/PIEL —
  SEGÚN EL CARRIL" (piel dewy y luminosa), el IDENTITY LOCK, el paso 6 del intake (tipos de casting y
  nivel de producción) y el párrafo de personas de "Libertad creativa". La v1.9.0 los había resumido.
- Verificado contra la v1.4.0: `realismo-anti-ia.md`, `personas-reales.md`, `realismo-fotografico.md`,
  `estetica-y-medio.md` y los 126 renglones de avatares del playbook son idénticos; la REGLA #2 también.

## v1.9.2 — corrige la modelo UGC con buen casting

- **Error introducido en la v1.8.0:** el paso "crear el modelo primero" mandaba la UGC con buen casting al
  avatar de estudio del playbook (§1.1, retrato editorial tipo Vogue), y salía con look de agencia.
- Se restaura el flujo de UGC que ya tenía la skill: referencia de cara obligatoria leída en el chat,
  persona nueva de ese nivel, prompt de solo texto con `realismo-anti-ia.md` y la escena del nivel de
  producción (casera, locación o estudio), generar 3–4 y elegir. El avatar §1.1 queda solo para agencia
  (`modelo-ugc.md`, `flujo-intake.md`, `SKILL.md`, `curaduria.md`, índice del playbook).

## v1.9.1 — dentro del límite de 200 archivos

- La plataforma acepta máximo 200 archivos por skill y la v1.9.0 tenía 285. Las 227 imágenes del
  repositorio se agrupan en **59 hojas de 4** (grilla 2×2, cada imagen a su resolución, con su código
  impreso en la esquina). La skill queda en **103 archivos**.
- `assets/referencias/indice.md` explica cómo abrir una imagen por su hoja y trae la tabla "Dónde está
  cada imagen". Las 227 lecturas no cambian.

## v1.9.0 — SKILL.md más liviano, sin perder contenido

- `SKILL.md` pasa de 681 a 464 líneas. Las secciones largas quedan en versión operativa y su **texto
  completo** se mueve, palabra por palabra, a `references/detalle-skill.md` (intake, salida, reglas no
  negociables, curaduría, formatos, integraciones, marcas reales, trazabilidad, estudio de marca, cierre
  y la descripción completa de cada archivo).
- Verificado con un script: de las 624 líneas con texto del `SKILL.md` anterior, todas siguen existiendo
  en `SKILL.md` o en los archivos de referencia, salvo 2 cambiadas a propósito (REGLA #1: el moodboard va
  siempre con las direcciones, como pidió la usuaria en la prueba 4).
- Mapa de archivos en una línea por archivo, agrupado por uso. Marcas de máxima prioridad: de 78 a 58.
- Sin cambios en: las 4 reglas ⛔, el bloque de referencias, el protocolo de bibliotecas y repositorio, la
  ruta express, la ruta de marca, el playbook, las plantillas y el repositorio de imágenes.

## v1.8.0 — paquete de correcciones de las pruebas

Sale de las 5 pruebas de octubre de 2026 (registro completo en `pruebas/registro-pruebas.md` del repo).
No cambia el playbook, las plantillas ni el sistema de `@imagen`.

- **Repositorio de referencias** (`assets/referencias/`): 227 imágenes de la autora, sin duplicados, en
  `general/`, `texto/` y 8 nichos, con `indice.md` (lectura de cada imagen, nivel ★/◦, formato o concepto
  del banco y buscador rápido por mecanismo). La skill lo consulta siempre antes de proponer (REGLA #4),
  abre 4–6 imágenes, las cruza con las referencias de la persona y declara cuáles usó en `Base:`.
- **Referencias pedidas siempre**, según lo que se construye (tabla en `instructivo-referencias.md`),
  también en la ruta express. Si la persona no tiene, se usa el repositorio y se le dice.
- **Tipografía al inicio**, como elección aparte, con 2–3 combinaciones y **prompt de muestra
  tipográfica**; orden marca real → referencias → nicho; vibra streetwear/workwear; moda no es lujo por
  defecto; prueba de marca tapada.
- **Prompt de moodboard** entregado siempre junto con las direcciones.
- **Molde = estructura, no composición:** el realismo y los bloques del playbook se mantienen; la
  composición se explora desde referencias, repositorio y bancos. Los textos del molde se reescriben.
- **Modelos creados primero**, con el casting y el molde de avatar, nunca inventados dentro de la pieza
  (opción "con modelo, pero no tengo" en la express; ajuste de género y maquillaje para hombres).
- **Logos:** lectura visible, patrón común y 6 opciones como mezclas declaradas de las referencias.
- **Producto:** texto de la etiqueta transcrito línea por línea e idéntico en la serie; bloque de
  integración producto–escena.
- **Diseño:** ninguna letra tapada por el sujeto, ningún texto huérfano, recurso tipográfico de la serie
  fijo en cada prompt.
- **Copy:** filtro anti-cliché. **Precios ambiguos** se confirman antes de generar.
- Curaduría actualizada con una verificación por cada corrección.

## v1.7.0

- **Embudo creativo:** antes de proponer, la skill arma en borrador 6–8 combinaciones (concepto +
  formato de sesión + spot DP), descarta las que fallan y muestra las que más frenan el scroll.
- **Extrapolación de referencias:** las referencias de la persona se cruzan con los bancos (estructura
  de la referencia + ejes de su marca + elemento propio del banco o del producto), y se le dice qué se
  tomó de cada una (`SKILL.md`, `ingenieria-inversa.md`, `curaduria.md`).

## v1.6.0

- **Ruta express para piezas sueltas.** Tres preguntas (para qué y formato · texto y precio · look y
  persona), la foto y el primer prompt en máximo dos mensajes. Una sola dirección, con su línea `Base:` y
  todos los bloques obligatorios; sin research web. Carruseles, campañas, ruta de marca, crear modelo y
  UGC con buen casting siguen por el intake completo (`flujo-intake.md`, `SKILL.md`, `curaduria.md`).

## v1.5.0

- **Playbook navegable.** `references/playbook-original.md` tiene ahora un índice al inicio y títulos
  `##` por sección (1 a 8). El texto original de los prompts no se modificó: solo se insertaron títulos.
- **Secciones nuevas del documento del curso** (9 a 13), copiadas tal cual: prompt maestro de product
  board solo producto, servicios (fisioterapia ReActiva), imágenes conceptuales sin modelo, inmobiliaria
  (Marfil) y marca personal / creador.
- `SKILL.md`: el playbook se consulta desde su índice y entra en la consulta obligatoria de
  bibliotecas como molde del prompt.
- `nichos.md`: cada nicho con molde real apunta a su sección del playbook.
- `curaduria.md`: revisa que el prompt parta de la sección correcta y conserve intacto su bloque de
  realismo.

## v1.4.1

- **REGLA #4 y consulta obligatoria de bibliotecas** antes de cualquier propuesta creativa, con línea
  `Base:` visible por dirección y prueba anti-genérico (`SKILL.md`, `curaduria.md`,
  `investigacion-mercado.md`, `conceptos-creativos.md`).
- `biblioteca-referentes.md`: conteo corregido a 43 formatos de sesión.
- `director-arte-cine.md`: el spot se refleja en el prompt de moodboard (la maqueta HTML está archivada).

## v1.4.0

- Versión base importada.
