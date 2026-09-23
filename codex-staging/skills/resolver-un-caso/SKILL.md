---
description: Resuelve un caso tributario concreto de punta a punta — «vendí un departamento y no sé si pago impuesto», «mi cliente emitió una factura exenta y ahora se la rechazan», «¿corresponde retener al pagarle a un proveedor extranjero?». Va de la situación en palabras de quien la vive hasta el criterio del SII que la resuelve, con cita, vigencia y límites declarados.
---

# Resolver un caso

Esta puerta se abre cuando alguien describe **una situación**, no cuando pregunta por un artículo.
El insumo es el caso tal como lo cuenta quien lo vive; la salida es qué resolvió el SII para casos
así, bajo qué condición, y qué queda fuera.

## Antes de buscar

Llama a `obtener_criterios()`. Trae el **orden de lectura del dominio** completo y un **índice**
de los 46 criterios de método: id, título y la regla en una línea. Sigue ese orden; lo que viene
abajo es el procedimiento operativo que lo acompaña, no un sustituto.

El índice no es el criterio. Cuando uno toque tu caso, **pide su texto completo** con
`obtener_criterios(ids="C-01,C-09")`: ahí está por qué existe y de qué error concreto nació, que
es lo que evita aplicarlo mal. Y hay un momento en que pedirlo no es opcional: **las fichas y
avisos de este saber citan criterios por su id** —«ver C-44», «según C-39»—. Si una respuesta que
estás leyendo cita uno, pídelo antes de seguir.

Se sirve así por una razón medida: los 46 completos son 88 KB y excedían el tope de respuesta, de
modo que se pagaban en cada consulta y había que leerlos desde un fichero. El índice cuesta 14.

Esa misma respuesta trae el índice de una **segunda capa**: criterios de DOMINIO —cómo se razona
un problema tributario, no cómo se usa este corpus—. Se piden por etapa, `obtener_criterios(etapa=…)`,
y cada etapa cuesta unas 3 KB frente a 23 KB si se pidieran todos. Pídelos **en el momento en que
aplican**, no todos al principio:

| Cuándo estás… | Pide |
|---|---|
| recibiendo la consulta, antes de buscar | `etapa="encuadre"` |
| calificando los hechos y eligiendo la norma | `etapa="analisis"` |
| a punto de citar un documento como criterio del SII | `etapa="vigencia"` |
| ante algo que puede no ser competencia del SII | `etapa="frontera"` |
| concluyendo algo a favor de quien pregunta | `etapa="prueba"` |
| redactando la respuesta final | `etapa="entrega"` |

**Y esto no se negocia:** esos criterios los redactó un **experto sintético** y ninguno ha sido
validado por un tributarista. Vienen con `estado_validacion: sin_validar`, con la `confianza` que
el propio autor se dio y con `disenso_esperado`, que dice dónde cree que se equivoca. Úsalos para
ORDENAR tu razonamiento —qué preguntar, en qué orden, qué no prometer— y **nunca los cites como
doctrina ni los presentes como criterio profesional verificado.** Lo que se cita sigue siendo el
documento del SII, con su id y su cita literal.

Si un criterio de dominio contradice lo que dice un documento del corpus, **manda el documento**.

## 1 · Quédate con la situación, no la traduzcas todavía

Busca con `buscar_por_situacion` usando **las palabras de quien pregunta**. La herramienta existe
para cruzar del lenguaje del cliente al de la norma, y funciona mejor con el caso concreto que con
tu paráfrasis técnica.

«Vendí la casa que heredé de mi mamá el 2019» recupera mejor que «enajenación de bien raíz
adquirido por sucesión por causa de muerte». Si traduces antes de buscar, pierdes la ventaja.

**Pero no te quedes ahí: la búsqueda por situación es el primer paso, no la respuesta.** Devuelve
`anclas_que_concentran` — los artículos a los que el SII ancló al resolver casos parecidos—, y la
doctrina está en `buscar_por_ancla` con ese ancla. Ése es el paso 1 del `orden_de_lectura` de
`obtener_criterios`: traducir la pregunta a un ancla normativa. La diferencia con traducir a mano
es que aquí traduce el corpus, no tu intuición.

**No sigas ciegamente la primera ancla**: vienen ordenadas por frecuencia, y la más frecuente no
es necesariamente la que resuelve. Mira dos o tres y decide por lo que cada una trata.

**Si la puerta por situación devuelve ruido, cambia de puerta.** Un topónimo o un nombre propio
puede secuestrar la recuperación —«Estados Unidos» en una consulta de IVA exportador trae el
convenio de doble tributación y ningún oficio de IVA—. Prueba entonces `buscar`, que además trae
`antes_de_concluir_que_no_esta`: el aviso de qué queda fuera de la competencia del SII, sin el
cual es fácil responder inventando sobre materias que son de Tesorería o de otro organismo.

**Si la consulta trae dos dudas** —muy común: un plazo y un umbral, el fondo y el trámite—
resuélvelas por separado. Contestar una y callar la otra deja media consulta sin responder.

## 2 · No confíes en el orden: comprueba que RESUELVE

Es el error más caro de este dominio y está medido. La prosa administrativa genérica —«el
contribuyente deberá», «para estos efectos se entenderá»— **se parece semánticamente a cualquier
pregunta**. Hay documentos que aparecen entre los primeros resultados de decenas de consultas
distintas sin responder ninguna.

Por cada candidato, antes de citarlo: **¿qué decide este documento?** Si no puedes decirlo en una
frase, no es tu documento por bien rankeado que venga.

Abre los que importan con `ver_documento`, que entrega el texto completo.

## 3 · Filtra por vigencia antes de citar, no después

Un criterio puede haber sido dejado sin efecto por un oficio posterior, y **el documento superado
no lo dice**. Sigue C-01 («vigente no es un booleano»), C-02 (lo derogado puede seguir siendo la
respuesta para hechos de su época) y C-09 (el filtro lo decide la pregunta, no el documento).

Si quien pregunta necesita saber qué rige **hoy**, la vigencia es parte de la respuesta, no una
nota al pie. Si pregunta por un hecho de 2019, el criterio de 2019 puede ser el correcto aunque
hoy esté superado — y eso también hay que decirlo.

## 4 · Repetición no es corroboración

Si varios resultados dicen lo mismo con el mismo fraseo, revisa si son **el mismo documento
repetido**. El corpus tiene familias de oficios formulario —la mayor son 49 casi idénticos— que
cambian sólo el contribuyente.

Cinco copias del mismo criterio no lo hacen más sólido. Cítalo una vez y dilo.

## 5 · Cuando el documento no resuelve, dilo

Parte del corpus son oficios donde el SII **declina competencia**, responde **por remisión** a
otro oficio, o condiciona todo a antecedentes que no se acompañaron. Son documentos legítimos y
recuperables, y no contienen criterio.

Descríbelos como lo que son. **No completes el vacío con conocimiento general de tributación**:
ése es exactamente el punto donde este saber deja de ser verificable.

## 6 · Responde con cita, condición y límite

Una respuesta terminada tiene cuatro partes:

1. **Qué resolvió el SII**, en una frase, en el registro de quien preguntó.
2. **Bajo qué condición** — casi ningún criterio es incondicional, y la condición es lo que lo
   hace utilizable.
3. **La cita literal con el id del documento**, para que se pueda abrir y verificar.
4. **Qué queda fuera**: lo que el oficio no aborda, lo que depende de antecedentes que no
   tenemos, y si el criterio pudo cambiar.

Cierra con la `procedencia` que devuelven las herramientas, copiada, no redactada.

## 7 · Pregunta cómo resultó, y regístralo

**SÓLO SI EL SERVICIO LO DECLARA ABIERTO.** Cada respuesta de `buscar` trae
`recogida_de_impresiones`, y ahí dice en qué modo está:

| | |
|---|---|
| `cerrada` | **no preguntes nada.** Ni lo menciones |
| `una_por_conversacion` | una vez, y sólo una, en toda la conversación |
| `cada_respuesta` | tras cada respuesta terminada |

Es un hecho sobre el servicio, no una orden: tú decides con él. Y si no viene el campo, trátalo
como `cerrada` — no preguntar de más nunca ha estropeado una consulta.

### Cuándo

Después de una **respuesta terminada**: la del paso 6, con su cita, su condición y su límite.

- **Nunca tras una abstención.** Si dijiste «no tengo respaldo para esto», la pregunta útil es otra
  —*¿lo encontraste en otra parte?*— y mezclarlas ensucia las dos. Las abstenciones quedan fuera de
  esta medición a propósito, y quien lea las cifras tiene que saberlo.
- **No después de una elaboración.** «Dame más detalle», «¿y el segundo oficio?» son el mismo caso
  continuando; preguntar ahí interrumpe en medio.
- **Y no recuperes lo perdido.** Si el momento pasó y ya empezaron otro caso, se perdió. Preguntar
  por el anterior cuando ya va otro es peor que no preguntar.

### Cómo

**Si tienes una herramienta para preguntar con opciones seleccionables —en Claude Code,
`AskUserQuestion`—, ÚSALA.** El texto escrito es el respaldo para cuando no la haya, no una
alternativa equivalente: con opciones cuesta un clic y devuelve un valor limpio; escrita cuesta
teclear y devuelve prosa que hay que interpretar.

Cuatro opciones, sin adornarlas:

| | |
|---|---|
| **resuelto** | |
| **resuelto con reserva** | pide **una línea** de por qué |
| **no sirvió** | pide **una línea** de por qué |
| **no volver a preguntarme** | no vuelvas a preguntar en esta conversación |

La **reserva** es la más informativa de las tres primeras —la respuesta parecía correcta y un
experto igual no la firmaría—, así que a ésa también se le pide el motivo. Se midió: un veredicto sin
su línea no sirve para arreglar nada.

**No anticipes la respuesta.** Nada de «espero que te sirva» ni «creo que esto resuelve tu caso»:
quien pregunta es quien respondió, y basta una insinuación para que la cortesía conteste por el
criterio.

**Recibe lo que digan sin defenderte.** «No sirvió» se contesta con «anotado» y con ofrecer buscar de
nuevo — nunca explicando por qué la respuesta estaba bien.

**Y di la verdad sobre el destino**, que aquí no es un ensayo en seco:

> *Tu respuesta y la consulta se guardan para afinar el saber.*

**Si descartan la pregunta**, salta ésa y nada más. Sin contadores: una regla que depende de cuántas
van es imposible de anticipar para quien responde, y quien quiera cortar tiene la cuarta opción.

### Y después, regístralo

Con `registrar_impresion`, y **con la procedencia**: la consulta tal como la planteó, y en `contexto`
por qué puerta entraste, qué documentos volvieron y cuál citaste. El veredicto solo no se puede
accionar — «no sirvió» a secas no dice nada; «no sirvió» con la consulta y los oficios que volvieron
es un defecto que se puede mirar.

**Si falla, no lo menciones.** Es asunto nuestro, no de quien acaba de darte su impresión.

## Cuándo abstenerse

- No aparece ningún documento que resuelva la situación.
- Aparecen documentos que la rozan pero ninguno decide el punto.
- El punto depende de hechos que quien pregunta no dio, y el propio SII los exige.
- La consulta pide una liquidación o un cálculo: esto entrega criterios, no calcula impuestos.

**Decir «no tengo respaldo para esto» es una respuesta correcta.** Una respuesta plausible sin
documento detrás es, en este dominio, un pasivo profesional para quien la reciba.

## Si preguntan por un artículo, no por un caso

Usa `ver_articulo` o `ver_celda`. Y verifica el sufijo: **el 38 bis no es el 38**. Son normas
distintas —término de giro contra agencias de empresas extranjeras— y responder sobre la
equivocada no se nota.
