# Cambios · Normativa Tributaria

<!-- Generado al derivar el paquete desde cambios.yaml. No editar a mano. -->

Qué cambia para quien usa este saber, versión por versión. Lo que corre de verdad el servicio lo dice su herramienta `ver_cambios`; esto es la copia del paquete.

## v0.3.20 · 2026-09-21

Añade 26 documentos que el SII publicó desde la versión anterior, e incorpora la corrección que el SII hizo a la circular 12 de 2021 sin anunciarla: el texto que el saber cita de ese documento es ahora el que el Servicio publica hoy.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.19 · 2026-09-20

Sin cambios para quien lo usa. Arregla que el chequeo de salud del servicio no llegaba a declarar qué versión del corpus sirve: decía que no había manifiesto cuando sí lo había.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.18 · 2026-09-20

Cada respuesta dice ahora de qué versión del corpus salió, no sólo qué versión del saber la produjo. Hoy coinciden —los datos viajan dentro del servicio— pero dejarán de hacerlo cuando el corpus se actualice a diario, y entonces esa distinción es lo que permite verificar una cita.

Por dentro: un manifiesto declara qué colecciones sirve esta versión y con qué huella, y `/readyz?sonda=1` comprueba contra el índice de vectores que ambas mitades del corpus son de la misma versión. Si se reindexara una y no la otra, el saber citaría documentos que su índice ya no conoce sin dar ningún error.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.17 · 2026-09-19

Sin cambios para quien lo usa. Por dentro, todo el texto del corpus se extrae ahora con una sola biblioteca y una sola versión, en vez de depender de la que estuviera instalada en la máquina que cosechara. Es lo que permitirá que la actualización deje de depender de un equipo concreto.

Cambia el espaciado del texto de 6.849 documentos —resoluciones y oficios—, no su contenido: las respuestas a las 165 preguntas de control son exactamente las mismas que antes del cambio. Dos fichas de significado quedan marcadas para relectura porque alguna de sus citas ya no aparece literalmente.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.16 · 2026-09-19

Dos resoluciones de 2026 dejan de mostrar el RUT de un funcionario. El SII lo había borrado de sus propias resoluciones y nosotros seguíamos sirviendo la versión anterior: el documento se había vuelto a descargar, pero su texto no se había rehecho. El saber vuelve a decir lo que dice hoy la fuente.

Afecta a las resoluciones 107 y 109 de 2026. El resto del corpus no cambia, y las respuestas a las preguntas conocidas siguen siendo las mismas.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.15 · 2026-09-18

El saber empieza a ver lo que el SII cambia sin anunciarlo. Dos circulares antiguas —la 34 de 2018 y la 12 de 2021— ahora dicen que fueron modificadas por la Circular 26 de 2026, porque el SII lo añadió a su índice después de publicarlas; y tres documentos que el SII rehízo en silencio se volvieron a descargar, dejando constancia de la huella anterior y de cuándo se detectó el cambio.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.14 · 2026-09-18

La ficha de procedencia ya no dice una fecha de cosecha equivocada. Antes, para circulares y resoluciones, mostraba cuándo se había modificado el fichero en disco —lo advertía, pero mostraba esa— y ahora declara el día en que el catálogo se comprobó de verdad contra el SII.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.13 · 2026-09-18

Entran quince documentos que el SII publicó entre el 2 y el 16 de septiembre: las circulares 36, 37 y 38 de 2026 —reajustes, impuesto único y UF de octubre— y las resoluciones exentas 117 a 128. Y veinticuatro circulares antiguas que informan datos periódicos vuelven a reconocerse como tales: su materia se había extraído vacía del PDF y ahora se toma del índice del SII cuando eso ocurre, declarando de dónde viene el dato.

La cobertura de documentos periódicos pasa de 959 a 986 circulares sin perder ninguna. Una de las quince, la resolución 124 de 2026, es un documento escaneado: entra en el catálogo pero su texto no se puede buscar todavía.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.12 · 2026-09-18

Sin cambios para quien lo usa. Por dentro, las pruebas que autorizan una publicación dejan de fijar los conteos del corpus: ahora comprueban que cada herramienta responde bien, y las cifras se revisan aparte contra los datos. Es lo que permitirá publicar una cosecha nueva sin que la barrera falle por diseño.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.11 · 2026-09-18

Sin cambios para quien lo usa. Por dentro, el chequeo de salud del servicio ahora comprueba que puede leer el registro de contratos: si no puede, el despliegue queda en rojo en vez de pasar en verde con el servicio rechazando a todo el mundo.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.10 · 2026-09-17

Cuando una búsqueda cae al respaldo porque Pinecone no responde, la traza ahora dice con precisión cuánto rinde ese respaldo: recupera 11 de los 20 aciertos que se pierden (55 %) y el 80 % de la calidad de orden medida como MRR. Antes decía que recuperaba «cuatro quintas partes de lo que se pierde» junto a los porcentajes de aciertos, y para los aciertos eso no era cierto.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

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
