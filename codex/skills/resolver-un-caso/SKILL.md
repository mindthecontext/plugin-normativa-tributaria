---
description: Resuelve un caso tributario concreto de punta a punta — «vendí un departamento y no sé si pago impuesto», «mi cliente emitió una factura exenta y ahora se la rechazan», «¿corresponde retener al pagarle a un proveedor extranjero?». Va de la situación en palabras de quien la vive hasta el criterio del SII que la resuelve, con cita, vigencia y límites declarados.
---

# Resolver un caso

Esta puerta se abre cuando alguien describe **una situación**, no cuando pregunta por un artículo.
El insumo es el caso tal como lo cuenta quien lo vive; la salida es qué resolvió el SII para casos
así, bajo qué condición, y qué queda fuera.

## Antes de buscar

Llama a `obtener_criterios()`. Trae el **orden de lectura del dominio** y 46 criterios de método.
Sigue ese orden; lo que viene abajo es el procedimiento operativo que lo acompaña, no un
sustituto.

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
