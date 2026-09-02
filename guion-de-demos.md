# Guión de demos

Seis prompts sobre tres documentos reales, con la explicación de por qué cada uno está escrito así.

*Javier Cantón · UNIR*

> **Cómo usar este guión**
>
> 1. Las cajas de código son el prompt, copiable tal cual. No llevan marcas ni comentarios dentro precisamente para eso.
> 2. Debajo de cada caja está el desglose de por qué está escrita así.
> 3. Cada caso incluye un apartado con lo que debería salir y dónde suele fallar.
> 4. Los tres documentos son públicos, así que cualquiera puede repetir las demos.

**Índice**

- [Por qué estos prompts están escritos así](#por-qué-estos-prompts-están-escritos-así)
- [Caso 1 · De la convocatoria al borrador](#caso-1--de-la-convocatoria-al-borrador)
- [Caso 2 · Escuchar a doscientas personas](#caso-2--escuchar-a-doscientas-personas)
- [Caso 3 · Un contenido, muchas versiones](#caso-3--un-contenido-muchas-versiones)

---

## Por qué estos prompts están escritos así

Los seis prompts siguen la misma estructura de seis piezas.

### Las seis piezas

**Rol.** Sitúa la respuesta en un oficio. «Técnico de formulación» y «analista cualitativo» activan vocabularios y criterios de calidad distintos ante la misma tarea.

**Contexto.** Quiénes somos, con qué medios y en qué territorio. Sin esto la respuesta sirve para cualquier entidad, y una respuesta que sirve para cualquiera no sirve para ninguna.

**Tarea.** Numerada y verificable. Cuando hay varias tareas van numeradas para poder señalar cuál falló, en vez de descartar la respuesta entera.

**Formato.** Tabla, número de filas, extensión. Si no se pide, el modelo elige por ti y suele elegir prosa larga.

**Criterios.** Qué hace buena la respuesta y qué no quieres ver. Aquí van las reglas antifabulación.

**Material.** Los documentos adjuntos. Es la pieza que separa una respuesta útil de un texto de relleno.

### Las tres reglas que se repiten en casi todos

**«No inventes nada; si no aparece, escribe que no consta.»** Los modelos rellenan huecos con lo estadísticamente probable. Darles una salida explícita para decir «no sé» reduce mucho ese impulso.

**«Cita la página de cada dato.»** No es burocracia: convierte una respuesta que hay que creerse en una respuesta que se puede comprobar en treinta segundos. Es la diferencia entre confiar y verificar.

**«Si hay contradicción, señálala en vez de elegir.»** El modelo tiende a armonizar. Pedirle lo contrario lo convierte en un detector de incoherencias de tus propios documentos.

> **Ojo con el orden.** El material va adjunto, no pegado dentro del prompt. Si pegas un documento largo en el cuadro de texto, se mezcla con tus instrucciones y el modelo pierde de vista qué es orden y qué es dato.

---

# Caso 1 · De la convocatoria al borrador

Dos prompts encadenados en la misma conversación, sobre las bases de la Convocatoria de Cooperación Internacional 2026 de la Fundación ”la Caixa”. El segundo usa la tabla que devuelve el primero.

**Conversación completa:** [ver el resultado en Claude](https://claude.ai/share/d3b28d9b-a49a-4da9-a44a-462b1b8d646b)

## Prompt 1 · Radiografía de las bases

**Adjunta:** `convocatoria-social-cooperacion-internacional-2026-bases.pdf` — [descargar de la Fundación ”la Caixa”](https://fundacionlacaixa.org/documents/d/guest/convocatoria-social-cooperacion-internacional-2026-bases-pdf)

```
Actúa como técnico de formulación de proyectos de una ONGD pequeña, con
experiencia en convocatorias de fundaciones privadas. Te adjunto las bases
completas de la Convocatoria de Cooperación Internacional 2026 de la
Fundación "la Caixa".

Tarea 1. Devuélveme una tabla con los criterios de valoración y su peso
exacto. Una fila por criterio y, en la última columna, la página de las
bases en la que aparece.

Tarea 2. Debajo, la lista de requisitos excluyentes: los que, si no los
cumplimos, nos dejan fuera antes de que nadie evalúe el proyecto.

Tarea 3. Los límites económicos y de calendario: importe máximo, duración
máxima, porcentaje máximo sobre el coste total del proyecto y fechas.

Reglas:
- No inventes ponderaciones. Si las bases dan un porcentaje para un bloque
  pero no para los subcriterios que contiene, dilo expresamente en lugar
  de repartirlo tú.
- Cita la página de cada dato.
- Si algo de lo que te pido no aparece, escribe "no consta en las bases".
```

### Cómo está construido

- El rol incluye «ONGD pequeña» porque cambia lo que el modelo destaca: una entidad grande no necesita que le adviertan de los límites de facturación.
- Las tres tareas van separadas y numeradas porque responden a tres decisiones distintas: si podemos presentarnos, cuánto podemos pedir y cómo nos van a puntuar.
- La regla sobre las ponderaciones no es genérica: está escrita para este documento en concreto, porque aquí es exactamente donde el modelo se inventa cosas.
- La columna de página convierte la tabla en algo verificable.

### Qué debe salir

Los pesos reales son tres: entidad gestora 15 %, socio local 10 % y proyecto presentado 75 %. Entre los excluyentes están ejecutar en un único país, presentar un solo proyecto por entidad, disponer de socio local con sede en el país, tres años de antigüedad y experiencia, ingresos anuales por debajo de dos millones de euros y no ser entidad académica o investigadora. Los límites: hasta 50.000 euros, dieciocho meses y un máximo del 75 % del coste total, con presentación entre el 15 de abril y el 20 de mayo de 2026 y resolución en noviembre.

> **Aquí está la trampa.** Las bases desglosan el 75 % del proyecto en pertinencia, medios, adecuación a la estrategia, impacto y viabilidad, pero no asignan puntos a cada uno. Muchos modelos se inventan un reparto verosímil. Si pasa, es la demostración en vivo de por qué la regla antifabulación está escrita y de por qué se pide la página.

## Prompt 2 · El índice alineado con quien puntúa

**Adjunta:** nada nuevo. Va en la misma conversación, justo después del prompt 1.

```
Contexto. Somos una fundación de apoyo educativo a adolescentes en riesgo de
abandono escolar. Queremos presentar un proyecto en Ecuador, con un socio
local con sede en Quito con el que llevamos seis años trabajando. Somos ocho
personas contratadas y nuestro presupuesto anual es de 420.000 euros.
Pediríamos 50.000 euros a dieciocho meses. El proyecto encaja en el ámbito de
educación y formación, en la línea de becas para la continuidad educativa y
mentoría comunitaria.

Tarea. Con la tabla de criterios del paso anterior, propón el índice de la
solicitud. Para cada apartado dime:
- A qué criterio de valoración responde y cuánto pesa.
- Qué hay que contar y en cuántas palabras.
- Qué evidencia nuestra debería sostenerlo.
- Una pregunta que tengamos que respondernos antes de escribirlo.

Las bases definen cuatro herramientas de innovación social: escucha,
cocreación, prototipado y escalado. Dime en qué apartado del índice debe
aparecer cada una y con qué nivel de detalle.

Comprueba también si nuestras cifras encajan con lo que las bases consideran
favorable y avísame si algo no cuadra.

Antes de escribir el índice, hazme las preguntas que necesites.
```

### Cómo está construido

- El contexto lleva números concretos —ocho personas, 420.000 euros, seis años— porque son justo los datos con los que las bases deciden si somos elegibles y si el importe es razonable.
- El índice se pide criterio a criterio, no por capítulos temáticos. Ese es el giro que sube la nota y el mensaje central del caso 1.
- La pregunta pendiente en cada apartado convierte el índice en un plan de trabajo: señala qué información hay que ir a buscar.
- Los cuatro conceptos de innovación social se citan por su nombre porque son el vocabulario propio de esta convocatoria. Un proyecto que no los usa se lee como escrito para otra.

### Qué debe salir

Con 50.000 euros solicitados, las bases consideran favorable no superar el 60 % del coste total, lo que sitúa el proyecto por encima de unos 83.000 euros. Un buen resultado detecta eso solo. También debería avisar de que el 25 % restante lo aporta la entidad o un cofinanciador, nunca las personas destinatarias.

> **Detalle que da mucho juego.** Las bases valoran expresamente la incorporación de inteligencia artificial para optimizar decisiones y diseñar intervenciones. Es decir, el propio financiador ya cuenta con ella.

---

# Caso 2 · Escuchar a doscientas personas

Sobre el CSV de respuestas del cuestionario de satisfacción. **Los datos son ficticios.**

**Conversación completa:** [ver el resultado en Claude](https://claude.ai/share/6115b846-ab1e-4496-a99b-c987c9cec24a)

## Prompt 3 · Categorización de respuestas abiertas

**Adjunta:** [`respuestas-cuestionario-programa-educativo.csv`](datos/respuestas-cuestionario-programa-educativo.csv)

```
Actúa como analista cualitativo. Te adjunto un CSV con 207 respuestas a la
pregunta abierta "¿Qué es lo que más te ha aportado el programa y qué
cambiarías?", recogidas entre adolescentes participantes en un programa de
apoyo educativo. Las columnas son: id, sede, edad, meses_en_programa y
respuesta.

Tarea:
1. Propón entre cinco y ocho categorías que emerjan de las propias
   respuestas. No uses categorías predefinidas. Muchas respuestas dicen a
   la vez algo que valoran y algo que cambiarían: clasifícalas por el tema
   del que hablan, no por si son positivas o negativas.
2. Define cada categoría en una frase.
3. Asigna cada respuesta a una sola categoría, citando su id.
4. Dame el recuento por categoría y dos citas literales de cada una, con
   su id.
5. Aparta en una lista final las respuestas sin contenido, las
   ininteligibles y las que estén en otro idioma. No las fuerces dentro de
   ninguna categoría.

No interpretes más allá de lo que dicen las respuestas. Si alguna incluye un
dato personal identificable, señálamelo en lugar de reproducirlo.
```

### Cómo está construido

- «Que emerjan de las propias respuestas» es la instrucción metodológica clave. Sin ella el modelo aplica las categorías de manual de cualquier evaluación de programas y deja de escuchar a los datos.
- La aclaración sobre respuestas mixtas evita el error más frecuente en este tipo de análisis: acabar con dos categorías, «positivo» y «negativo», que no sirven para tomar ninguna decisión.
- «Una sola categoría» y «citando su id» permiten verificar. Sin id no hay forma de comprobar nada, y todo el ejercicio se convierte en un acto de fe.
- El punto 5 protege la calidad: obliga a declarar lo que no encaja en vez de repartirlo para que los números queden redondos.

## Prompt 4 · Cruce y verificación

```
Ahora dos cosas más:

1. Cruza las categorías con la columna sede y dime si alguna preocupación
   se concentra claramente en una sede. Si las diferencias son pequeñas,
   dilo en lugar de forzar una conclusión.
2. Elige veinte respuestas al azar y muéstrame, en una tabla, su id, su
   texto completo y la categoría que le asignaste, para que yo pueda
   comprobar a mano si la clasificación es correcta.
```

### Cómo está construido

- El punto 1 lleva incorporado el freno estadístico. Sin él, cualquier diferencia se presenta como un hallazgo, y con doscientas respuestas repartidas en cinco sedes casi ninguna lo es.
- El punto 2 es la regla que no se salta convertida en instrucción. Que la muestra de verificación la genere el propio modelo hace que el paso cueste diez segundos, y por eso se hace.

### Qué debe salir

Deberían emerger categorías cercanas a estas ocho: apoyo académico, vínculo con la persona tutora, confianza y autoestima, horarios y frecuencia, instalaciones y materiales, grupo de iguales, orientación de futuro y comunicación con las familias. Si salen cinco muy amplias, pídele que desdoble la más numerosa: también es una demostración útil.

> **Busca el fallo.** En las veinte de verificación suele aparecer al menos una mal clasificada, casi siempre una respuesta mixta que menciona dos temas. Localízala, apúntate su id y enséñala.

---

# Caso 3 · Un contenido, muchas versiones

Sobre la Memoria Anual 2025 de Save the Children España.

**Conversación completa:** [ver el resultado en Claude](https://claude.ai/share/e1e7d2c3-f68a-4974-babd-3760f89e3fd1)

## Prompt 5 · Adaptación a lectura fácil

**Adjunta:** `MemoriaAnual2025_0.pdf` — [descargar de Save the Children](https://www.savethechildren.es/sites/default/files/2026-07/MemoriaAnual2025_0.pdf)

```
Te adjunto la Memoria Anual 2025 de Save the Children España.

Tarea. Adapta a lectura fácil la sección "Nuestros programas en España",
para que puedan leerla los propios adolescentes que participan en esos
programas.

Reglas:
- Frases de menos de quince palabras, una idea por frase.
- Vocabulario cotidiano. Si un término es imprescindible, explícalo la
  primera vez que aparezca.
- Sin siglas sin explicar y sin cifras en formato complejo.
- Títulos cortos y listas.
- Habla de las personas como protagonistas, nunca como beneficiarias
  pasivas de una ayuda.

Al final, enumera los términos que has sustituido, por si alguno era
institucionalmente necesario y hay que recuperarlo.
```

### Cómo está construido

- Se nombra la sección exacta. Pedir «adapta la memoria» sobre un documento entero devuelve un resumen, no una adaptación.
- Se nombra a quién va dirigido, y son los propios adolescentes. El destinatario cambia el registro más que cualquier regla de estilo.
- La lista de términos sustituidos es el control de calidad: a veces se pierde algo que jurídica o institucionalmente tenía que estar.

> **Recuérdalo en voz alta.** La lectura fácil se valida con personas destinatarias y tiene sello de calidad. Esto acelera el borrador, no sustituye la validación.

## Prompt 6 · De la memoria a LinkedIn

```
De la misma memoria, extrae los cinco datos o historias con más potencial
comunicativo y conviértelos en cinco publicaciones para LinkedIn.

Para cada una:
- Primera línea con el dato o la frase que hace parar el scroll.
- Cuerpo de tres o cuatro frases, sin jerga del sector.
- Una llamada a la acción concreta.

Reglas:
- Ninguna cifra puede inventarse ni redondearse al alza.
- Detrás de cada cifra, indica entre corchetes la página de la memoria de
  la que sale.
- Si dos partes de la memoria dan cifras distintas sobre lo mismo,
  señálamelo en lugar de elegir una por tu cuenta.
- Nada de lenguaje paternalista ni compasivo sobre las personas de las que
  hablamos: son protagonistas, no casos.
- Si alguna historia identifica a un menor por su nombre, avísame antes de
  usarla.
```

### Cómo está construido

- La página entre corchetes es lo que permite que alguien de comunicación publique sin haberse leído las cuarenta páginas, y siga respondiendo de cada cifra.
- La regla sobre cifras contradictorias está puesta a propósito para este documento. Da resultado.

### Qué debe salir

Hay material de sobra: 113 respuestas a emergencias, 15.021 niños y niñas atendidos en España, 5.500 profesionales formados en prevención de violencia, y un reparto del gasto con un 67 % destinado directamente a programas. Y tres historias personales, que son las que de verdad funcionan en redes.

> **El hallazgo de la demo.** El texto de apertura habla de 13,6 millones de niños y niñas alcanzados en las emergencias, mientras la página de impacto global da 37,8 millones de niños atendidos. Son magnitudes distintas que miden cosas distintas, pero conviven en el mismo documento sin explicarlo.

---

*Guión de demos · Foro UNIR · Javier Cantón*
[Versión editable en DOCX](materiales/Guion-demos-prompts.docx) · [CC BY 4.0](LICENSE)
