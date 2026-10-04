# Cambios · Normativa Tributaria

<!-- Generado al derivar el paquete desde cambios.yaml. No editar a mano. -->

Qué cambia para quien usa este saber, versión por versión. Lo que corre de verdad el servicio lo dice su herramienta `ver_cambios`; esto es la copia del paquete.

## v0.3.56 · 2026-10-04

Cuando un documento de la lista tiene un cambio de criterio verificado por autores académicos, el aviso dice ahora DE QUÉ TRATA ese cambio y no sólo que existe. Y el procedimiento pide dos cosas nuevas: contrastar la ley con la circular que la instruye cuando la pregunta es de régimen, y agotar lo que ya está a la vista antes de declarar que el corpus no tiene algo.

EL AVISO DECÍA SÓLO QUE HABÍA ALGO. Con `{posturas: 0, cambio_verificado: true}` quien recorre una lista no puede saber si ese cambio toca su pregunta, así que no abre la ficha. En una prueba real el agente escribió que «ningún documento revisado decide si una simple cuenta por pagar basta» para el abono en cuenta, y los documentos que lo deciden estaban en su propia lista con el cambio verificado. Ahora el aviso trae la cuestión entera: cortarla la dejaba a media frase y una pregunta truncada no deja decidir si toca la tuya. Son 68 documentos en todo el corpus y cuesta 0,23% de una respuesta cuando aparece.
LA LEY Y LA INSTRUCCIÓN SE LEEN JUNTAS. Medido sobre cuatro respuestas a la misma pregunta: todas citaron una de las dos voces y ninguna las contrastó. El artículo 14 enumera seis escalones de imputación; la Circular 73 de 2020 añade que uno de ellos sólo debe calcularse cuando hay devolución de capital. Quien respondió sólo con la ley mandó al lector a un cálculo que el propio Servicio declara innecesario. Y si las dos voces no concuerdan, ahora se declara la discrepancia en vez de elegir.
ANTES DE DECIR «NO ENCONTRÉ», tres comprobaciones: abrir el documento que uno mismo nombró, buscar por la materia exacta y mirar la doctrina que la lista ya entregó. De los límites que un agente declaró en una prueba, tres de tres eran falsos y el documento que resolvía estaba a su alcance. Esto NO cambia la abstención, que sigue siendo correcta cuando el corpus no alcanza: lo que cambia es abstenerse sin haber mirado.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `registrar_impresion`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.55 · 2026-10-04

Cuando un documento no rige del todo, las listas dicen ahora QUÉ acto lo dejó así y HASTA DÓNDE alcanza. Antes sólo decían «sin efecto», y con eso una respuesta llegó a recomendar buscar la circular que reemplazó a la Circular 73 de 2020, que no existe: lo único que reemplaza algo de ella es una tabla de su página 48. Además, cuando el SII sólo estampa «modificada por» sin decir cuánto, la respuesta ya no lo cuenta como si afectara al documento entero: dice que el alcance no está declarado. Y el bloque de procedencia separa lo que sirve para decidir de lo que sirve para verificar.

«TOTAL» NO ERA SIEMPRE UN HALLAZGO. De las 207 relaciones con alcance total, 103 venían sólo de una estampa —el sello que el SII imprime en el PDF del documento afectado—, y una estampa dice quién lo afectó, nunca cuánto. El saber ponía «total» porque tenía que poner algo. Ahora esas se declaran como alcance no declarado, y las que el texto sí acota conservan su nombre: «sólo Página 48», «sólo Capítulo IV».
LO QUE CUESTA: entre 0,08 y 0,46 KB por respuesta, del 0,1% al 0,5%, y sólo lo llevan los documentos que no rigen sin más.
LA PROCEDENCIA, en dos tramos. Primero lo que un profesional usa para decidir si se fía —hasta cuándo alcanza el corpus, qué no es derivable—; al final, bajo un rótulo que dice para qué sirven, los identificadores técnicos. La huella de cada documento se mantiene COMPLETA: es lo único del bloque con un uso ejecutable, y es lo que permite comprobar una cita sin depender de nosotros. Y el articulado dice ahora cómo comprobarlo, incluido que el SII no publica una página enlazable por artículo.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `registrar_impresion`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.54 · 2026-10-04

Al pedir el artículo 14 de la Ley de la Renta —el del régimen de las empresas— el saber entregaba el texto que estuvo vigente hasta el 31 de diciembre de 2019, el del régimen de renta atribuida que la Ley 21.210 reemplazó. Lo entregaba como «fuente primaria», sin advertencia, sólo porque es el texto más largo que el SII guarda de ese artículo. Ahora entrega uno que rige, nombra cuál está leyendo y deja la versión antigua a la vista para quien la pida. Lo mismo con los artículos 149 y 150 del Código Tributario, que la Ley 21.713 eliminó: ahora avisan.

EL SII YA LO DECÍA Y EL SABER NO LO LEÍA. El Administrador de Contenido Normativo marca estas situaciones en el propio título o en la glosa —«(vigente hasta el 31.12.2019)», «ELIMINADO por el art. 1 N° 55 de la Ley N° 21.713», «DEROGADO por la Ley N° 20.780»— y esa marca no se miraba. Son 53 de las 1.136 piezas del articulado. En cuatro artículos la pieza marcada era justamente la que se servía: el 14 de la Renta, el 84 de la Renta, y el 60 y el 153 del Código Tributario.
QUÉ CAMBIA AL PEDIR UN ARTÍCULO: se entrega la pieza más extensa que el SII NO marca como derogada; la respuesta dice por su nombre cuál es —antes decía sólo «el texto más extenso», así que no se sabía si se estaba leyendo la letra A) o la D)—; y las piezas derogadas siguen en el índice, marcadas, para poder pedirlas. Si se pide una, se entrega con la frase literal del SII sobre por qué ya no rige.
LO QUE SIGUE SIN PODERSE SABER, y ahora se declara en cada respuesta: el SII no consolida todas las derogaciones. El N° 3 del artículo 31 sigue publicando la devolución del impuesto de primera categoría como pago provisional, que la Ley 21.210 eliminó desde el 1 de enero de 2024, y nada en el texto lo advierte. Se comprobó contra el SII en vivo que su texto es idéntico al que el saber guarda: es un límite de la fuente, no un retraso de la cosecha.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `registrar_impresion`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.53 · 2026-10-04

Siete circulares que el saber daba por derogadas enteras vuelven a regir, porque lo que el SII dejó sin efecto en ellas fue sólo una parte. La más importante es la Circular 73 de 2020, la instrucción principal del régimen de empresas de la Ley 21.210: se descartaba de las búsquedas por artículo porque «reemplaza tabla incluida en la página 48» se había leído como un reemplazo de la circular entera. Las otras seis son la 39 de 2022, la 12, la 70 de 2015, la 20 y la 41 de 2014 y la 2 de 2017. Y cuando el cálculo de vigencia del saber no coincide con lo que el SII marca en su índice, la respuesta ya no lo da por seguro: lo dice.

LO DETECTÓ UN AGENTE en una prueba con preguntas de clientes: entró por otra puerta, abrió la circular que supuestamente derogaba a la 73, leyó que sólo cambiaba una tabla y siguió usándola. Estaba así desde la primera versión con registro.
TRES FORMAS DE LEER MAL, corregidas las tres: se perdía lo que limita lo derogado («una tabla», «el apartado 2.8», «en lo pertinente», «salvo el N° 4 de su Capítulo II»); no se entendía el plural «Circulares N°s 20 y 41», y el «parcialmente» que lo precedía se perdía; y una derogación se extendía a las circulares de la lista de referencias, que sólo se citan.
Además, la Circular 40 de 2015 pasa a figurar con partes sin efecto, como dice la Circular 41 de 2021 («Deroga: en parte Circular Nºs 40 de 2015 y 33 de 2015»), que antes no se leía.
LA REGLA NUEVA: si el saber calcula que una circular no rige y el SII no la marca sin efecto —o al revés—, `buscar_por_ancla` ya no la descarta, y la ficha responde `rige_hoy: no_derivable` con la discrepancia y el acto que habría que abrir. Hoy no queda ninguna; la regla es para la próxima mala lectura.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `registrar_impresion`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.52 · 2026-10-03

Entrega lo que la 0.3.51 no llegó a publicar. Lo que más se nota: algunos documentos traen ahora lo que autores académicos han escrito sobre ellos —1.557 documentos anotados a partir de 443 artículos de la Revista de Estudios Tributarios (U. de Chile) y la Revista de Derecho Tributario (U. de Concepción), entre 2010 y 2026—, también los anteriores a 2013. Además, 1 documento nuevo del SII y las correcciones que el Servicio hizo sin anunciarlas a las circulares 26 de 2026 y 12 de 2021.

La etiqueta 0.3.51 se empujó y su publicación se detuvo en las pruebas contra staging, así que nadie la recibió. Todo lo suyo viaja aquí, y su entrada de más abajo —que describe la doctrina académica en detalle— se queda como registro de esa etiqueta.
LO ÚNICO QUE CAMBIA RESPECTO DE LO QUE ELLA DESCRIBE: los 272 documentos anotados anteriores a 2013 —136 con posturas o cambios de criterio verificados, justo las circulares antiguas que los autores más discuten— ahora traen su doctrina al abrirlos. En la 0.3.51 se abrían sin ella.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `registrar_impresion`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.51 · 2026-10-03  ·  ⚠ QUEMADA

> **Esta versión no debe servirse.** La etiqueta se empujó y su publicación se detuvo en las pruebas contra staging, así que nadie llegó a recibirla. Su contenido era bueno salvo en una cosa: los documentos anteriores a 2013 se abrían SIN su doctrina académica, porque la herramienta los sirve por un camino propio. Lo detectó uno de sus propios casos de prueba —22 de 23—. Todo viaja en la 0.3.52, con eso corregido.

Algunos documentos traen ahora lo que autores académicos han escrito sobre ellos: 1.557 documentos anotados a partir de 443 artículos de la Revista de Estudios Tributarios (U. de Chile) y la Revista de Derecho Tributario (U. de Concepción), entre 2010 y 2026. Aparece al abrir un documento, en un apartado propio, con el autor, el año y la página; en las listas sólo se avisa de que existe. Además añade 1 documento que el SII publicó desde la versión anterior (el oficio 2572 de 2026) e incorpora las correcciones que el SII hizo sin anunciarlas a las circulares 26 de 2026 y 12 de 2021: el texto que el saber cita de esos documentos es ahora el que el Servicio publica hoy.

ES UNA TERCERA VOZ Y NO CAMBIA NINGUNA DE LAS DOS QUE YA HABÍA. Lo que un autor opina no es criterio del SII, no es un fallo y no vincula a nadie, así que va siempre con esa advertencia y nunca mezclado con el criterio, las advertencias del documento ni la jurisprudencia. Que un autor critique un oficio no lo deja sin efecto: el estado de vigencia y el del criterio salen igual que antes, y hay una comprobación que lo exige.
QUÉ TRAE CADA DOCUMENTO: hasta tres posturas, cada una con el documento nombrado, el autor, el año y la página; los cambios de criterio que un autor afirmó Y que se comprobaron contra los dos textos, con su veredicto; las alertas de vigencia —cuando el autor analizó una versión anterior de la ley— y la referencia completa para citar.
LO QUE NO TRAE, y cada cosa por su razón: el texto de las revistas, porque se cita con paráfrasis propia y una frase breve; la tesis de cada artículo, porque al resumirla volvía firme lo que el autor plantea como hipótesis; y los cambios de criterio que los autores afirman y no resistieron la comparación, que son el 26%.
No cambia qué documentos encuentran las búsquedas ni en qué orden. Y las respuestas de búsqueda ahora respetan de verdad el tamaño que declaran: antes el reparto se calculaba con el peso MEDIO de una ficha y las respuestas largas se pasaban del techo.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `registrar_impresion`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.50 · 2026-10-02

Añade 2 documentos que el SII publicó desde la versión anterior (la resolución 133 de 2026 y la resolución 134 de 2026).

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `registrar_impresion`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.49 · 2026-10-02

Cuando una búsqueda avisa de que también hay resultados en el corpus antiguo, ahora dice bien de qué años habla. Lo llamaba «doctrina anterior a 2001» y en realidad llega hasta 2012: de cada cinco documentos de ese corpus, cuatro eran posteriores a 2001, y los propios ejemplos que la respuesta ofrecía lo desmentían. Quien leyera esa etiqueta podía descartar un tramo de once años que sí está y sí se puede leer. El rango se calcula ahora del corpus, así que seguirá siendo cierto cuando crezca. Por dentro, y sin efecto en lo que se responde: la comprobación que vigila que las búsquedas sigan devolviendo lo mismo vuelve a servir de algo. Se renovaba en cada actualización del corpus sin decir qué había cambiado, y así pasó inadvertido en septiembre que doscientos nueve documentos habían dejado de encontrarse. Ahora distingue lo que sólo mueve el orden de los resultados de lo que saca un documento del alcance de las búsquedas, y nombra cuáles.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `registrar_impresion`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.48 · 2026-10-01

Un dictamen que este saber dejó de servir en septiembre —porque identifica a una persona— deja también de aparecer en los datos que el saber publica. No llegaba a nadie: el servicio ya lo filtraba al responder. Lo que quedaba era su rastro dentro de los ficheros del corpus, incluidos trescientos de sus términos en el índice de búsqueda, y uno de ellos sólo aparecía en él. De paso, ese documento dejaba de contar en el total con que se calcula el orden de los resultados, de modo que el ranking de todo el corpus se corrige un poco. Y una circular cuya ficha estaba sellada contra un texto que el SII ya había cambiado vuelve a corresponder al texto de hoy.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `registrar_impresion`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.47 · 2026-09-30

Tres mil veintisiete circulares y resoluciones anteriores a 2013 ya se pueden abrir y citar. El saber tenía su texto guardado y los encontraba al buscar por palabras, pero al pedir cualquiera de ellos respondía que no lo había cosechado y remitía al sitio del SII: quien encontraba el documento no podía leerlo. Ahora se entregan enteros y sellados, diciendo lo que de ellos no está derivado —a qué artículos tocan y si siguen rigiendo—, y los 1.822 que de verdad sólo constan en el catálogo lo siguen declarando. Con esto el saber declara correctamente lo que cubre: pasa de anunciar 10.517 documentos legibles a los 13.544 que ya tenía.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `registrar_impresion`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.46 · 2026-09-30

Doscientos nueve oficios vuelven a encontrarse por búsqueda de texto: estaban en el catálogo y con su texto guardado, pero habían quedado fuera del índice léxico, de modo que preguntar por sus palabras no los devolvía. Y el orden de los resultados en el corpus anterior a 2013 vuelve a ser el correcto: seis circulares que el SII publica comprimidas habían entrado con su contenido ilegible y desplazaban la puntuación de todo ese tramo. Añade además 5 documentos nuevos del Servicio e incorpora la corrección que el SII hizo a la circular 34 de 2018 sin anunciarla: el texto que el saber cita de ese documento es ahora el que el Servicio publica hoy.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `registrar_impresion`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.45 · 2026-09-28

El SII publicó un mismo dictamen dos veces —una versión con los datos del consultante y otra sin ellos— y este saber servía las dos. Ahora sirve sólo la anonimizada, y dice que la otra existe.

El ORD. N° 1798, de 17.05.2000 está en dos páginas del sitio del SII. Una reemplaza los datos del consultante por «xxxx»; la otra nombra su cargo diplomático, sus destinaciones y su nombramiento, que juntos identifican a una persona concreta. El saber entregaba una o la otra según por dónde se hubiera preguntado.
El criterio es ser fiel al tratamiento que hace el SII: cuando publica el mismo dictamen anonimizado y sin anonimizar, se sirve el anonimizado. Pedir el retirado ya no responde «no encontrado» —sería falso, el documento existe y el SII lo publica— sino que explica la decisión, dice quién la tomó y remite al que sí se sirve. Y su texto sale de lo servido, que es lo que hace que el dato deje de tratarse y no sólo de difundirse; sigue en el área de trabajo, porque retirar del servicio no es borrar la cosecha.
LO QUE ESTO NO GARANTIZA, y la propia respuesta lo dice: que el corpus esté libre de datos que identifiquen a una persona. Es un documento revisado a mano. La identificación por combinación de atributos —un cargo, unas fechas, un destino— no es detectable automáticamente, y este caso no lleva ni un RUT ni un nombre.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `registrar_impresion`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.44 · 2026-09-28

La cobertura distingue lo que está catalogado de lo que se puede leer. De las 3.780 circulares del corpus, 2.903 son fichas sin texto: constan, y no se pueden citar ni buscar por contenido.

Esa diferencia estaba en los datos y no se decía en ninguna parte. La cobertura anunciaba 3.780 circulares desde 1974 y la procedencia de la misma respuesta decía 877: las dos ciertas —una cuenta lo catalogado, la otra lo que tiene texto— y ninguna decía cuál era cuál. Leídas juntas parecían un descuadre; leídas por separado prometían cosas distintas.
Ahora cada capa dice cuántos se pueden leer y cuántos sólo constan, y las dos cifras cuadran.
También se corrigió un motivo que era falso: el saber decía no alcanzar los actos anteriores a 2013 «porque el SII no publica índices de circulares antes de ese año». Sí los publica —la ficha de la Circular 92 de 1974 viene de su índice de 1974—; lo que falta es el texto. Y el criterio que guía las respuestas decía «este corpus sólo tiene circulares desde 2013», que hacía descartar 2.903 documentos que sí constan.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `registrar_impresion`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.43 · 2026-09-28

Cuando el saber dice que nadie cambió el criterio de un documento, ahora dice también cuántas declaraciones de cambio tiene detectadas y no pudo atribuir a nadie. Y detecta una forma de confirmar que se le escapaba.

«Ningún documento del corpus declara haber cambiado ni confirmado el criterio de éste» era la frase, y había 145 declaraciones expresas detectadas que no llegaban a ninguna ficha. En la mayoría porque el propio texto no dice sobre qué criterio cambia —«se modifica el criterio de este Servicio», sin nombrar cuál—, que es un límite de la fuente y no del saber. Pero quien leía esa frase no podía saberlo. Ahora la ficha trae la cifra y aclara que ninguna de ellas es necesariamente sobre el documento que se está mirando.
Lo segundo sí era nuestro: un oficio que dice «la interpretación contenida en el Oficio N° 708, de 1986, se encuentra plenamente vigente» está confirmando un criterio, y no lo cazaba ningún patrón porque el verbo no es «confirmar». Son diez casos en el corpus, y siete nombran el documento que confirman.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `registrar_impresion`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.42 · 2026-09-28

El registro de cambios puede decir que una versión no debe servirse. La primera así marcada es la 0.3.35, cuya publicación falló a medias y que nadie llegó a recibir.

Hasta ahora, cuando una versión se retiraba, eso sólo constaba en un mensaje de commit. Y revertir el código no mueve lo que cada entorno sirve —es deliberado, y es lo que permite probar antes de que la reciba nadie—, así que una versión retirada podía quedarse servida sin que nada lo dijera. Pasó con la 0.3.23, que estuvo un día entero en producción después de revertirse.
Ahora la marca viaja en el registro, se ve en el CAMBIOS.md del paquete y la lee el script que mueve a producción, que se niega a promover una versión quemada. La marca exige el motivo: no es lo mismo una versión que rompía algo —y entonces nada suyo debe volver— que una cuya publicación falló a medias, como ésta.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `registrar_impresion`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.41 · 2026-09-28

Cuando el saber corrige el identificador de un oficio, ahora explica por qué el índice del SII no lo nombraba bien —y son dos motivos distintos, no uno—. Y deja de servir dos notas que se contradicen sobre el mismo par de documentos.

La explicación de las correcciones era una sola frase: «el índice lo rotula con el número del oficio que cita». Eso es cierto en 33 de 566 casos. En los otros 533 el SII sencillamente publicó el documento sin número, y el identificador salía del nombre de su página. La causa estaba en el propio identificador y ahora se lee de ahí.
Lo segundo: cuando alguien había comparado dos documentos a mano y establecido que son el mismo dictamen, la ficha seguía sirviendo además una nota automática que los presentaba como dos oficios distintos y sugería nombrar los dos «para reforzar la cita». Seguir esa sugerencia era citar el mismo dictamen dos veces. Ahora lo derivado calla sobre los pares que ya se miraron, y sólo sobre ésos: los gemelos que nadie ha abierto siguen apareciendo.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `registrar_impresion`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.40 · 2026-09-28

Una circular sin efecto que conserva trámites en curso ya no muestra la cláusula como si fuera suya: la dicta el acto que la dejó sin efecto, y ahora lo dice. Y la fecha desde la que dejó de regir viene explicada por lo que la produjo, no por otra cosa.

La cláusula que dice «las solicitudes ya presentadas continuarán tramitándose» nunca está en el texto de la circular que la muestra: habla de las circulares que su autor desplaza, así que viene del acto posterior. Quien la citara como texto de la circular que estaba leyendo citaba mal, y ese campo es justamente el que le dice a alguien que no la descarte.
Lo segundo es de la misma familia. La fecha desde la que una circular dejó de regir venía acompañada de un motivo que explicaba una pregunta distinta —por qué no se puede derivar cuándo ENTRÓ en vigencia—. Son dos de las cuatro dimensiones del estado y no se responden con lo mismo. Ahora el motivo nombra el acto que la afectó y aclara qué no está diciendo.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `registrar_impresion`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.39 · 2026-09-28

Un documento que sabemos que es otro deja de fecharse con la fecha del que no es, y dice por cuál hay que citarlo. Afecta al Oficio 708 de 1986, que en realidad es el N° 774 de 2000.

El SII publicó ese dictamen en dos secciones de su sitio, y a una de las dos copias le puso el número del oficio que el texto CITA. Una revisión a mano de los dos originales lo estableció hace dos días, y esa revisión estaba guardada y no llegaba a la respuesta: la ficha seguía fechando el documento el 28-02-1986, que es la fecha del oficio de 1986.
Ahora la ficha no afirma esa fecha —dice por qué no puede— y trae `citar_por` con el identificador correcto, quién lo estableció y cuándo. La fecha del índice se conserva aparte, porque es la vía por la que el SII lo publica y perderla rompería la traza.
Se remite y no se redirige, a propósito: son dos ficheros distintos con el mismo dictamen, y hacer que uno devuelva el otro daría la copia equivocada a quien pida la correcta.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `registrar_impresion`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.38 · 2026-09-28

La procedencia que cierra cada respuesta se escribe en texto plano. Plegarla en un bloque de HTML dejaba los tags a la vista del lector, justo en la parte que sostiene lo verificable.

Las skills decían qué pegar y no decían en qué forma, así que la elegía el asistente. Uno eligió un `<details>` para plegarla —razonable si el cliente renderiza HTML, y la mayoría no lo hace— y el lector se encontró las etiquetas encima y debajo del bloque.
Ahora las dos skills lo dicen y dicen por qué: la procedencia lleva los sellos SHA-256, las fechas de cosecha y lo que no es derivable, así que es el bloque que menos puede verse roto. Es el que le pide a quien lee que se fíe.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `registrar_impresion`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.37 · 2026-09-28

Un documento del que no se puede saber de qué año es ya no pasa los filtros por año. Antes atravesaba cualquiera de los dos: los mismos 17 oficios salían pidiendo «hasta 1993» y pidiendo «desde 2026». Ahora quedan fuera, y la respuesta dice cuántos son y cómo verlos.

El año se busca primero donde el SII fecha el documento en su índice y, si ahí no hay nada, en el sello que el propio documento lleva impreso. Así `oficio:1999:sn-jul01` —que el índice no fecha y cuyo texto dice «Oficio Nº 3.116, del 11.08.1999»— se filtra como lo que es, de 1999.
Los que no tienen ninguna de las dos cosas quedan fuera del filtro, porque una consulta por fecha no puede responder por lo que no tiene fecha. Pero no se van en silencio: la respuesta trae cuántos fueron, cuáles, y que se ven repitiendo la consulta sin acotar por año. Lo mismo en `buscar_por_situacion`, donde el defecto era el contrario y dejaba pasar siempre lo indatable.
Salió de la ronda de pruebas de la 0.3.36 y estuvo latente mucho tiempo: mientras la fecha de esos oficios se rellenaba con un valor armado a partir del nombre de la página del SII, ningún documento tenía el campo vacío y el fallo no se veía. Dejar de inventar esa fecha —que además era falsa— lo sacó a la luz.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `registrar_impresion`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.36 · 2026-09-27

Entrega lo que la 0.3.35 no llegó a publicar. Lo que más se nota: la serie histórica —3.027 documentos anteriores a 2013 que hasta ahora eran inalcanzables— ya se puede buscar por texto, y esa búsqueda dejó de mezclar corpus: pedir el histórico devolvía documentos del otro índice.

La etiqueta 0.3.35 se empujó y su publicación falló antes de terminar, así que nadie la recibió. Todo lo suyo viaja aquí, y su entrada de más abajo se queda como registro de esa etiqueta.
Lo que cambia para quien pregunta, además de lo anterior: un oficio superado ya no vuelve sólo con «no_aplica», sino diciendo quién se pronunció después; `buscar_por_ancla` deja de ofrecer apartados que el propio texto del documento desmiente; y lo que el saber ha aprendido resolviendo conflictos entre documentos —que existe otra copia del mismo oficio, cuál conviene citar y por qué— ahora viaja con la respuesta, con la procedencia de cada dato para poder rastrear de dónde sale lo que no está escrito en el documento citado.
También incorpora la corrección que el SII hizo a la circular 34 de 2018 sin anunciarla.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `registrar_impresion`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.35 · 2026-09-25  ·  ⚠ QUEMADA

> **Esta versión no debe servirse.** La etiqueta se empujó y su publicación falló antes de terminar, así que nadie llegó a recibirla. No es que su contenido fuera malo: todo viaja en la 0.3.36, que es la que hay que servir. El fallo fue una guarda que aprobó con una colección de más y saltó dentro del build, con la etiqueta ya puesta.

Incorpora la corrección que el SII hizo a la circular 34 de 2018 sin anunciarla: el texto que el saber cita de ese documento es ahora el que el Servicio publica hoy.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `registrar_impresion`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.34 · 2026-09-24

Termina lo que la 0.3.33 dejó a medias. Las listas de anclas que acompañan a una búsqueda seguían ofreciendo leyes modificatorias como siguiente paso, aunque esa puerta las rechaza, y el mensaje del rechazo mandaba a buscar por el número de la ley —un camino que no funciona—.

La 0.3.33 marcó la ficha de un documento y dejó intactas las listas de `anclas_que_concentran`, que son las que MÁS invitan porque llevan la llamada siguiente escrita. Había tres copias del mismo código armando esa lista y sólo se arregló una; ahora hay una función y las tres la usan.
Y la sugerencia del rechazo estaba rota: buscar «20732», «20.732» o «Ley N° 20.732» devuelve cero documentos aunque el texto de la circular la nombre varias veces, porque el índice léxico no conserva los números con punto de miles. Ahora el mensaje manda a buscar por la MATERIA y declara esa limitación en vez de empujar hacia ella.
La prueba también estaba a medias y por eso pasó con el defecto puesto: cubría una superficie de tres. Ahora exige lo mismo en las listas.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `registrar_impresion`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.33 · 2026-09-24

La ficha de un documento ya no ofrece caminos que no llevan a ninguna parte. Cuando cita una ley modificatoria —«ley:21210»— lo dice y advierte que no se puede seguir por ahí; y si aun así se intenta, la respuesta explica QUÉ es esa referencia en vez de decir sólo que no la conoce.

Salió de una impresión de un experto. La lista de anclas de un documento mezclaba dos cosas distintas con la misma forma: un cuerpo legal con su artículo —«LIR:art14», que la puerta gobernada sirve con vigencia y cambios de criterio— y una ley modificatoria que el documento cita, que ninguna puerta sirve. Como las instrucciones dicen «con ese artículo sigue por buscar_por_ancla», tomar la segunda llevaba a un rechazo correcto pero mudo, con el agravante de que el ancla la habíamos ofrecido nosotros.
Son 620 anclas de esa clase en los datos y cero servidas. La circular que responde la consulta sobre contribuciones entrega dos de ellas junto a la buena.
Lo que se exige ahora no es la marca sino el contrato completo: que toda ancla ofrecida se pueda seguir, que toda marcada se rechace explicando, y que la marca no se coma las buenas. Esa última mitad es la que impide arreglarlo marcándolo todo.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `registrar_impresion`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.32 · 2026-09-24

Dos oficios más se sirven con su identidad real. Uno se llamaba «oficio:2000:2584» y es el Oficio N° 3161 de 26-06-2003; el otro figuraba como de 2020 y es de 2005. Con eso quedan DOS identidades falsas en todo el corpus comprobable, frente a las 73 con que empezó el problema.

Ninguno entró por un solo testigo. El primero lo declaran su propio encabezado, la migaja de navegación y la URL, los tres de acuerdo en 2003.
El segundo tiene un matiz que conviene decir: su número —4.646— sí era correcto y su encabezado lo confirma, pero el año que ese encabezado trae es «205», una errata del SII. El año lo ponen la migaja, la URL y el índice, los tres en 2005, y así queda declarado en la entrada: el número sale del documento, el año no.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `registrar_impresion`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.31 · 2026-09-24

Lo mismo que la 0.3.30, que no llegó a publicarse. Cambiar los datos exige volver a sellarlos y declarar el sello nuevo en el manifiesto, y eso se olvidó: la imagen no se construyó porque su propia comprobación detectó que el corpus no era el que su manifiesto declaraba.

La guarda hizo justo lo que debe: paró en la construcción de la imagen, antes de desplegar nada. Ninguna versión mal sellada llegó a servirse.
Queda anotado el descuido, porque es reutilizable: `instantanea.py --check` pasó y por eso se dio por buena la comprobación. Son dos guardas distintas —una cuenta documentos y anclas, la otra sella el CONTENIDO de las 41 colecciones— y sólo la segunda ve un cambio en `identidad_oficios_override.jsonl`. Pasar una no dice nada de la otra.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `registrar_impresion`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.30 · 2026-09-24

Siete oficios que se servían sin número —con un identificador provisional como «oficio:2002:sn-ja400»— pasan a llamarse por su número real. Eran documentos que el índice del SII publica sin número en el título, así que la cosecha les puso un nombre derivado del fichero para no inventar una cita falsa. El número sí estaba: en el encabezado que el propio índice guarda al lado, y que nadie estaba leyendo. Ahora se pueden citar por su nombre.

Ninguno entró por una sola fuente. Cada uno se aceptó sólo cuando el encabezado del índice y el del PROPIO DOCUMENTO coinciden en número y año, que es la misma disciplina de dos testigos con la que se aceptaron las 44 identidades anteriores.
De once candidatos quedaron siete. Tres no tienen su texto cosechado, así que no hay segundo testigo y NO se aceptan: se dicen no comprobables en vez de darlos por buenos. Y uno queda fuera por un motivo distinto y más interesante: «oficio:2002:sn-ja246» es el Oficio N° 432 de 2002, pero esa casilla la ocupa hoy otro documento —que a su vez es el Oficio N° 2525 de 2003—. Meterlo dejaría dos documentos respondiendo al mismo nombre según el orden de búsqueda, que es exactamente lo que no se puede hacer.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `registrar_impresion`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.29 · 2026-09-24

La pregunta por la calidad de la respuesta ya no se salta. En la 0.3.28 el saber tenía el dato y conocía la regla, y aun así terminaba respuestas largas sin preguntar: el paso iba al final de un procedimiento de siete, justo después de la instrucción que dice «cierra». Ahora la obligación se declara antes de empezar, se dice explícitamente que la procedencia cierra la respuesta pero no el turno, y se nombra el modo de fallo medido. Lo que ves: al terminar una respuesta con cita te va a preguntar cómo te resultó, sin que tengas que pedirlo. El procedimiento además TERMINA en ese paso: antes venían dos secciones después, así que lo último que se leía era otra cosa.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `registrar_impresion`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.28 · 2026-09-24

Ahora también responde con el procedimiento completo cuando preguntas por una norma o un impuesto —«¿las contribuciones las pagan los mayores de 65?»— y no sólo cuando cuentas un caso. Antes esas preguntas se contestaban por fuera del procedimiento: con citas, sí, pero sin la comprobación de que están vigentes, de que el documento resuelve de verdad y de que los límites se declaran. Salió de las dos primeras consultas reales de un experto, que fueron las dos de esa clase. Y se arregla el registro de impresiones, que desde 0.3.27 no guardaba NINGUNA: la pregunta de calidad se hacía, la respuesta se recogía y se perdía ahí mismo, porque el servicio no lograba resolver de quién era. Lo que se recogió entre 0.3.27 y esta versión no está.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `registrar_impresion`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.27 · 2026-09-24

La pregunta por tu impresión ahora funciona entres por donde entres. En la 0.3.26 el saber sólo decía si la recogida estaba abierta cuando la consulta pasaba por la búsqueda general; si preguntabas por un artículo o abrías un documento, no lo decía y la pregunta no aparecía. Ahora ese dato va en la procedencia, que acompaña a todas las respuestas. Y la recogida queda ACTIVA por defecto: al terminar una respuesta con cita te preguntará cómo te resultó, y tu respuesta y la consulta se guardan para afinar el saber.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `registrar_impresion`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.26 · 2026-09-24

Sin cambios para quien lo usa. La 0.3.25 no llegó a publicarse: le faltaba un caso de prueba para la herramienta nueva y la verificación contra staging la rechazó, que es lo que tiene que pasar.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `registrar_impresion`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento` · aparece `registrar_impresion`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.25 · 2026-09-24

Cuando resuelve un caso con cita, ahora puede preguntarte cómo te resultó —resuelto, resuelto con reserva, no sirvió— y pedirte una línea si no quedó limpia. Tu respuesta y la consulta se guardan para afinar el saber, y la pregunta te lo dice. VIENE APAGADO: el servicio declara en qué modo está y mientras esté cerrado no pregunta nada, así que esta versión no cambia lo que ves hasta que se encienda. Nunca pregunta cuando se abstiene: ahí la pregunta útil es otra.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.24 · 2026-09-22

44 oficios que el índice del SII rotula con el número de OTRO documento —el que ellos mismos citan— dejan de contradecirse entre puertas y dejan de fecharse mal. Hasta ahora, encontrar uno buscando por su texto lo devolvía con un identificador y pedir su ficha lo devolvía con otro: quien lo encontraba y después lo pedía recibía otro documento, o nada. Ahora las dos puertas lo nombran igual, y cuando el rótulo del índice difiere del nombre real se entrega también ese rótulo, porque es con el que hay que buscarlo en la fuente para verificarlo. La fecha va con la identidad: la entrada del índice traía también la fecha del otro documento, así que un oficio de 2003 se servía fechado en 1980. Esa fecha deja de darse como suya —se declara como lo que es, la de la entrada del índice— y la fecha citable, la que el propio documento lleva impresa, viaja en su sello. Y uno de ellos deja de llamarse «oficio del año 3003»: su firma traía esa errata, mientras su cabecera, el índice del SII y el catálogo decían los tres 2003. Los demás oficios no cambian.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.22 · 2026-09-22

520 documentos que se entregaban sin materia, sin fecha y sin enlace vuelven a traerlos: su texto estaba en el saber, pero bajo un identificador que el catálogo ya había corregido, y las búsquedas los devolvían sin decir de qué documento eran. De paso, 26 oficios dejan de llevar la advertencia de procedencia no confirmada, porque al corregirse su identificador su texto y su nombre vuelven a coincidir; quedan 47 con esa advertencia. Y los cuatro índices semánticos vuelven a cubrir el corpus completo, así que los documentos incorporados en las dos versiones anteriores ya se encuentran también por significado y no sólo por texto.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

## v0.3.21 · 2026-09-22

Sin cambios para quien lo usa: las mismas búsquedas devuelven los mismos documentos con las mismas puntuaciones. El índice de texto completo pasa a cargarse por filas, y con eso el servicio necesita un tercio de la memoria que necesitaba — 318 MB donde antes usaba unos 700. Se comprobó documento a documento sobre las 131.124 consultas que cubren los 65.362 términos del índice.

- Herramientas: `buscar`, `buscar_dato_periodico`, `buscar_en_texto`, `buscar_instrumento`, `buscar_jurisprudencia`, `buscar_por_ancla`, `buscar_por_situacion`, `buscar_por_tema`, `listar_cobertura`, `obtener_criterios`, `preguntas_abiertas`, `ver_articulo`, `ver_cambios`, `ver_celda`, `ver_documento`
- Skills: `empezar-aqui`, `resolver-un-caso`
- Datos: sin manifiesto

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
