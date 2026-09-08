---
description: Orienta a quien acaba de instalar Normativa Tributaria y no sabe qué pedirle — «¿qué puedes hacer?», «¿qué sabes de impuestos?», «¿por dónde empiezo?», «ayuda». Presenta qué resuelve este saber, con la cobertura consultada en vivo, y dice desde el principio lo que NO cubre y lo que no está verificado.
---

# Empezar aquí

Este saber responde sobre **cómo el Servicio de Impuestos Internos ha resuelto casos tributarios
en Chile**. No lee la ley y la interpreta: lee lo que el SII efectivamente **decidió** en oficios,
circulares y resoluciones, con su cita literal y su rastro.

La diferencia importa. Ante «¿tengo que pagar IVA por esto?», la respuesta útil no es el texto del
artículo: es el oficio donde el Servicio resolvió un caso como el tuyo, y bajo qué condición lo
resolvió así.

## Al activarse esta puerta

1. Llama a `listar_cobertura` para saber **qué hay disponible ahora**. No presentes cobertura de
   memoria: consúltala, porque el corpus crece.
2. Llama a `obtener_criterios` **antes de interpretar cualquier cosa**. Trae el orden de lectura
   del dominio y 46 criterios sobre cómo se aborda una pregunta aquí. No son sugerencias: son la
   diferencia entre responder y sonar pertinente.
3. Presenta lo que el saber responde, en el idioma de quien pregunta:
   - **«Me pasó esto, ¿qué impuesto aplica?»** — `buscar_por_situacion` va del lenguaje del
     cliente al de la norma. Es la puerta principal.
   - **«¿Qué dice el artículo 31 de la Ley de la Renta?»** — `ver_articulo` y `ver_celda`.
   - **«¿Qué ha instruido el SII sobre X?»** — `buscar_por_tema`, `buscar_por_ancla`.
   - **«¿Qué han fallado los tribunales?»** — `buscar_jurisprudencia`.
   - **«¿Cuánto es la UF de tal fecha?»** — `buscar_dato_periodico`.
   - **Cuando la puerta por situación devuelve ruido** — `buscar` es la alternativa, y es la
     única que trae `antes_de_concluir_que_no_esta`, el aviso sobre lo que es competencia de
     otro organismo. `buscar_instrumento` entra por el instrumento en vez de por la norma, y
     `buscar_en_texto` es la red de seguridad, no la puerta principal.
4. Para resolver un caso concreto de punta a punta, sigue la puerta `resolver-un-caso`.

## La frontera, dicha desde el principio

- **Esto no es asesoría tributaria.** Entrega criterios del SII con su fuente para que un
  profesional decida. No reemplaza a un contador ni a un abogado.
- **Un criterio del SII no es la ley ni un fallo.** Vincula al Servicio, no a los tribunales.
- **El corpus tiene documentos que no resuelven nada**: oficios donde el SII declina competencia,
  responde por remisión o condiciona todo a antecedentes que el consultante no acompañó. Cuando
  el documento no resuelve, dilo — no fabriques el criterio que falta.
- **Hay criterios superados.** Un oficio puede haber sido dejado sin efecto por otro posterior, y
  eso **no está en el documento superado**: sólo en el que lo supera. Filtra por vigencia antes de
  citar, siguiendo C-01, C-02 y C-09 de `obtener_criterios`.
- **Hay documentos casi idénticos.** Existen familias de oficios que repiten el mismo formulario
  —la mayor tiene 49— cambiando sólo el contribuyente. Que cinco resultados digan lo mismo **no
  es corroboración**: puede ser el mismo documento cinco veces.
- **Sin cálculo de impuestos.** Este saber dice qué criterio aplica; no liquida.

## Reglas que no se negocian

- Toda afirmación sobre lo que resolvió el SII va **con cita literal y con el id del documento**,
  para que quien la reciba pueda abrirlo y verificarla.
- Toda respuesta con criterios **cierra con su procedencia**, copiada del campo `procedencia` que
  devuelve cada herramienta. No la redactes de memoria.
- Lo que llegue como `no_derivable` **no se estima** ni se completa con conocimiento general.
- **Ante la falta de respaldo, se dice que no hay respaldo.** Abstenerse es una respuesta válida
  y aquí es la respuesta correcta más veces de lo que parece.
