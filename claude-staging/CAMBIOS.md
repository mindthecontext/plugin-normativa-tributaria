# Cambios · Normativa Tributaria

<!-- Generado al derivar el paquete desde cambios.yaml. No editar a mano. -->

Qué cambia para quien usa este saber, versión por versión. Lo que corre de verdad el servicio lo dice su herramienta `ver_cambios`; esto es la copia del paquete.

## v0.3.9 · 2026-09-16

Cuando buscas por palabras filtrando por tipo de documento, el saber ya no te dice que no hay ninguno cuando sí los hay. Antes tomaba los mejores resultados del corpus entero y filtraba después: como los oficios son la gran mayoría, una búsqueda filtrada a circulares podía quedarse sin ninguna y responder «ningún documento de tipo circular calza», aunque varias contenían esas palabras. Ahora busca dentro del tipo pedido, y si de verdad no hay ninguno, dice sobre cuántos documentos lo comprobó.

Lo que esto no cambia: que vengan documentos del tipo pedido no garantiza que venga el que mejor responde. El orden de los resultados sigue siendo el mismo de antes dentro de cada tipo, y las búsquedas sin filtro de tipo no cambian en nada.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.8 · 2026-09-16

El aviso que acompaña al criterio de un oficio ya no contradice a su propia ficha. Decía siempre que no se había derivado si su criterio fue superado, incluso cuando la misma ficha mostraba quién lo superó y con qué cita; ahora dice lo que sí se sabe y hasta dónde llega. Y la versión que aparece en la procedencia de cada respuesta es la desplegada: decía «0.12.0», un número que no correspondía a ninguna versión del saber y que llegaba impreso a la sección de fuentes de las respuestas.

El aviso no se eliminó, porque que no aparezca un cambio de criterio sigue sin significar que el criterio esté vigente. Ahora lo explica: cuántas declaraciones y aristas reúne el grafo de cambios de criterio —leídas de los datos, no escritas a mano—, que su recall no está medido y que no ve los cambios tácitos.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.7 · 2026-09-16

Cuando otro pronunciamiento posterior cambió el criterio de un documento, su ficha ahora lo dice en `criterio`. Antes eso sólo aparecía si el propio Servicio lo había publicado como cambio de criterio bajo el artículo 26 del Código Tributario: en 27 de los 32 documentos superados que el saber conoce, la ficha traía la cita literal de quien lo superó y, en el mismo objeto, un «sin noticia de cambio» que afirmaba que nadie había declarado nada.

Cada entrada declara de qué capa viene —lo que el SII publica por el artículo 26, o la lectura curada de la conclusión del documento que supera—, porque no se saben igual aunque las dos se lean del texto. Lo que un tercero NARRA sobre un documento sigue sin mover el estado, por ser un origen que reconstruimos nosotros, y ahora se declara aparte en vez de quedar como si nadie hubiera dicho nada. Un verbo de supersesión que el saber no sepa interpretar tampoco mueve el estado: se declara y se deja ver.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.6 · 2026-09-16

Si tu cuenta está autenticada pero no tiene habilitado este servicio, ahora te lo dice: el conector aparece conectado, y al usarlo recibes el motivo y a quién pedir la habilitación. Antes aparecía como si faltara autorizar, y volver a autorizar no lo arreglaba. Si el registro de contratos no responde, el aviso de reintentar también llega al usarlo.

La 0.3.5 traía esto mismo, pero sus respuestas de rechazo no cumplían la revisión 2026-07-28 del protocolo y los clientes las descartaban antes de mostrarlas: se veía como si el servicio estuviera caído. La 0.3.5 se quedó en staging y no llegó a producción.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.5 · 2026-09-15

Si tu cuenta está autenticada pero no tiene habilitado este servicio, ahora te lo dice: el conector aparece conectado, y al usarlo recibes el motivo y a quién pedir la habilitación. Antes aparecía como si faltara autorizar, y volver a autorizar no lo arreglaba. Si el registro de contratos no responde, el aviso de reintentar también llega al usarlo.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.4 · 2026-09-14

Si tienes un asiento y es la primera vez que te conectas —o te conectas desde una cuenta que el servicio todavía no conoce, con tu mismo correo—, ahora entras en tu primera consulta. Antes podías recibir «no tienes habilitado este servicio» hasta haber entrado alguna vez a Mi Cuenta.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.3 · 2026-09-14

El saber dice qué cambió de una versión a otra y en qué versión está corriendo: aparece `ver_cambios`. Lo que ya respondía sigue igual.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## Línea base · v0.3.2 · 2026-09-14

Así está el saber cuando empieza este registro. Responde cómo el SII ha resuelto casos tributarios en Chile sobre 15.469 documentos de 1971 a 2026 —circulares, resoluciones y oficios—, 3.536 fallos de tribunales y el articulado de la ley, con la cita literal para verificar cada criterio, su vigencia declarada y la condición bajo la cual se resolvió así. Tiene catorce herramientas: `buscar`, la entrada recomendada para una situación descrita en palabras corrientes; `buscar_por_ancla`, cuando la pregunta ya nombra el artículo; y otras para casos parecidos, jurisprudencia, texto literal, documentos, datos periódicos, instrumentos y criterios de interpretación. No es asesoría tributaria ni calcula impuestos: entrega criterios con su fuente para que un profesional decida, y dice qué materias el SII no resuelve antes de concluir que algo no está.

- Herramientas: no derivable
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

Antes de v0.3.2 no hay registro de cambios.
