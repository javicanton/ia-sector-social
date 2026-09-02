# Kit de prompts para el sector social

Diez plantillas listas para usar en proyectos, financiación, análisis, materiales y gestión interna.

*Javier Cantón · UNIR · Foro UNIR sobre IA en el sector social*

> **Cómo usar este kit**
>
> 1. Sustituye todo lo que está entre `[CORCHETES]` por los datos reales de tu entidad. Un prompt sin contexto propio devuelve una respuesta genérica, y se nota.
> 2. Adjunta tus documentos siempre que puedas: las bases, la memoria, el borrador. El material propio es lo que separa una respuesta útil de un texto de relleno.
> 3. Ningún resultado sale de la entidad sin que lo lea una persona. Si lleva vuestro logo, respondéis vosotros de cada dato.
> 4. No introduzcas datos personales de las personas con las que trabajáis. Anonimiza antes.

**Índice**

- [Anatomía de un prompt que funciona](#anatomía-de-un-prompt-que-funciona)
- **Bloque 1 · Financiación y formulación de proyectos**
  - [1. Radiografía de una convocatoria](#1-radiografía-de-una-convocatoria)
  - [2. El índice alineado con quien puntúa](#2-el-índice-alineado-con-quien-puntúa)
  - [3. Marco lógico e indicadores realistas](#3-marco-lógico-e-indicadores-realistas)
  - [4. El evaluador implacable](#4-el-evaluador-implacable)
- **Bloque 2 · Analizar la información que ya tenéis**
  - [5. Respuestas abiertas de un cuestionario](#5-respuestas-abiertas-de-un-cuestionario)
  - [6. El acta que sí sirve para algo](#6-el-acta-que-sí-sirve-para-algo)
- **Bloque 3 · Materiales y comunicación**
  - [7. Adaptación a lectura fácil](#7-adaptación-a-lectura-fácil)
  - [8. Guión de una sesión formativa](#8-guión-de-una-sesión-formativa)
  - [9. De la memoria anual a las redes](#9-de-la-memoria-anual-a-las-redes)
- **Bloque 4 · Gestión interna**
  - [10. Vuestra política de uso de IA, en una página](#10-vuestra-política-de-uso-de-ia-en-una-página)
- [Tres líneas que no se cruzan](#tres-líneas-que-no-se-cruzan)

---

## Anatomía de un prompt que funciona

Las diez plantillas de este kit están construidas con estas seis piezas. Si escribes las tuyas propias, comprueba que no te falte ninguna.

| | | |
| --- | --- | --- |
| **1 · Rol**<br>Desde qué oficio quieres que te responda: técnico de proyectos, analista, evaluador. | **2 · Contexto**<br>Quiénes sois, con quién trabajáis, en qué territorio y con qué medios. | **3 · Tarea**<br>Una sola, concreta y verificable. Dos tareas en un prompt salen peor que dos prompts. |
| **4 · Formato**<br>Tabla, extensión máxima, apartados. Si no lo pides, te lo inventa. | **5 · Criterios**<br>Qué hace que la respuesta sea buena, y qué no quieres ver en ella. | **6 · Tu material**<br>Documentos, datos, textos previos. La pieza que más cambia el resultado. |

**Dos frases que puedes añadir a cualquier prompt del kit:**

> **«Antes de responder, hazme las preguntas que necesites.»** Convierte un monólogo en una conversación. Úsalo cuando el encargo sea importante.
>
> **«Dame un borrador, no un resultado final.»** Pide tres versiones y quédate con lo mejor de cada una. Criticar es más rápido que escribir desde cero.

---

# Bloque 1 · Financiación y formulación de proyectos

## 1. Radiografía de una convocatoria

*Cuando se publican las bases y hay que decidir rápido si os presentáis.*

```
Actúa como técnico o técnica de formulación de proyectos con diez años de
experiencia en entidades sociales. Te adjunto las bases de la convocatoria
[NOMBRE Y ORGANISMO].

Tarea. Devuélveme una tabla con:
1. Cada criterio de valoración y su puntuación máxima.
2. Qué evidencia concreta pide para otorgar esa puntuación.
3. Requisitos excluyentes: si nos falta alguno, quedamos fuera.
4. Plazos, formato y límite de extensión de cada documento.

Después, en un apartado aparte:
- Los tres criterios que más pesan en la nota final.
- Qué información necesitas de nosotros que no esté en las bases.

No inventes nada. Si algo no aparece en el documento, escribe "no consta
en las bases".
```

> **Consejo.** Este es el prompt que hay que ejecutar siempre primero. El resto del kit se apoya en la tabla de criterios que devuelve.

## 2. El índice alineado con quien puntúa

*Antes de escribir una sola línea del proyecto.*

```
Contexto. Somos [ENTIDAD], dedicada a [QUÉ HACÉIS] en [TERRITORIO].
Trabajamos con [COLECTIVO], somos un equipo de [N] personas y nuestro
presupuesto anual ronda los [IMPORTE].

Te adjunto: (a) la tabla de criterios de valoración del paso anterior y
(b) [MEMORIA ANUAL O PROYECTO SIMILAR YA PRESENTADO].

Tarea. Propón el índice del proyecto con un apartado por cada criterio de
valoración. Para cada apartado indica:
- Qué hay que contar y en cuántas palabras.
- Qué dato o evidencia nuestra debería sostenerlo.
- Qué tenemos ya y qué nos falta conseguir.

Antes de escribir el índice, hazme las preguntas que necesites para no dar
nada por supuesto.
```

> **Consejo.** El error más común es pedir «escríbeme un proyecto». Lo que sube la nota es ajustar la estructura a cómo os van a puntuar.

## 3. Marco lógico e indicadores realistas

*Cuando el formulario pide indicadores y no queréis prometer lo que no podréis demostrar.*

```
A partir del proyecto que estamos formulando, construye una matriz de marco
lógico: objetivo general, objetivos específicos, resultados esperados,
actividades, indicadores y fuentes de verificación.

Condiciones:
- Cada indicador debe poder medirse con los medios de una entidad pequeña.
  Nada que exija una evaluación externa cara.
- Para cada indicador, indica quién lo recoge, con qué instrumento y cada
  cuánto tiempo.
- Distingue los indicadores de proceso (¿lo hicimos?) de los de resultado
  (¿cambió algo en la vida de las personas?).
- Señala expresamente los indicadores que no vamos a poder demostrar con
  nuestros recursos y propón alternativas más modestas.
```

> **Consejo.** Revisa que ningún indicador exija datos personales que no podéis recoger legalmente. Es un fallo caro que reaparece después, en la justificación.

## 4. El evaluador implacable

*Con el borrador terminado y tiempo todavía para corregirlo.*

```
Vas a hacer de persona evaluadora de la convocatoria [NOMBRE], no de asesora
nuestra. Tu trabajo es puntuar, no animarnos.

Te adjunto: (a) los criterios de valoración con su puntuación y (b) nuestro
borrador.

Tarea:
1. Puntúa cada criterio y justifica la nota en una sola frase.
2. Señala las tres frases más flojas del borrador y explica por qué.
3. Marca toda afirmación que no esté respaldada por un dato.
4. Termina con los cinco cambios que más subirían la puntuación, ordenados
   por impacto.

Sé duro. Si este proyecto no llegaría al corte, dilo con claridad.
```

> **Consejo.** Funciona mucho mejor que pedir «mejora este texto». Al cambiar el rol, deja de complacerte y empieza a encontrar agujeros.

---

# Bloque 2 · Analizar la información que ya tenéis

## 5. Respuestas abiertas de un cuestionario

*Cuando se acumulan respuestas sin analizar y nadie encuentra el hueco para hacerlo.*

```
Actúa como analista cualitativo o cualitativa. Te adjunto [N] respuestas a la
pregunta abierta "[PREGUNTA]", recogidas entre [PERSONAS PARTICIPANTES EN EL
PROGRAMA X].

Tarea:
1. Propón entre cinco y ocho categorías que emerjan de las propias
   respuestas. No uses categorías predefinidas.
2. Define cada categoría en una frase.
3. Asigna cada respuesta a una sola categoría, citando su número.
4. Dame el recuento por categoría y dos citas literales representativas
   de cada una.
5. Aparta las respuestas ambiguas o que no encajen en ninguna categoría.

No interpretes más allá de lo que dicen las respuestas. Si alguna es
ininteligible, márcala como tal en vez de forzarla en una categoría.
```

> **La regla que no se salta.** Coge veinte respuestas al azar y comprueba a mano que están bien clasificadas. Si fallan, cambia el prompt, nunca los datos.

## 6. El acta que sí sirve para algo

*Después de cualquier reunión de equipo, junta o comisión.*

```
Te paso la transcripción de una reunión de [EQUIPO / JUNTA / COMISIÓN]
del [FECHA].

Devuélveme, en este orden y en un máximo de una página:
1. Decisiones tomadas. Solo lo que se decidió, no lo que se debatió.
2. Tareas: qué, quién y para cuándo. Si no se asignó responsable o fecha,
   escribe "sin asignar".
3. Temas que quedaron abiertos.
4. Discrepancias relevantes que convenga dejar registradas.

No incluyas nada que no aparezca en la transcripción.
```

> **Consejo.** El punto 2 es el que cambia las reuniones. «Sin asignar» escrito en negro sobre blanco obliga a asignar.

---

# Bloque 3 · Materiales y comunicación

## 7. Adaptación a lectura fácil

*Siempre que un texto vaya dirigido a las personas de las que habla, y no solo al financiador.*

```
Adapta el siguiente texto a lectura fácil, dirigido a [personas con
discapacidad intelectual / con bajo nivel de alfabetización / que están
aprendiendo español].

Reglas:
- Frases de menos de quince palabras, una idea por frase.
- Vocabulario cotidiano. Si un término técnico es imprescindible,
  explícalo la primera vez que aparezca.
- Voz activa y orden sujeto, verbo, complemento.
- Sin metáforas, sin siglas sin explicar y sin cifras complejas:
  escribe "casi la mitad" en lugar de "el 47,3 %".
- Estructura con títulos cortos y listas.

Al final, enumera los términos que has sustituido, por si alguno era
jurídicamente necesario y hay que recuperarlo.
```

> **Aviso.** La lectura fácil se valida con personas destinatarias y tiene sello de calidad. La IA acelera el borrador; no sustituye la validación.

## 8. Guión de una sesión formativa

*Para formar a voluntariado o al propio equipo sin dedicarle una semana.*

```
Diseña el guión de una sesión formativa de [90] minutos sobre [TEMA],
dirigida a [voluntariado / equipo técnico / familias], con [N] participantes
y un nivel de partida [bajo / medio / alto].

Formato: tabla con minutaje, actividad, objetivo de aprendizaje, materiales
y quién conduce.

Condiciones:
- Nunca más de quince minutos seguidos de exposición.
- Al menos dos actividades participativas y una de cierre que permita
  comprobar qué se ha aprendido.
- Materiales realistas: papelógrafo y fotocopias, no plataformas de pago.
- Incluye tres preguntas para arrancar el debate y qué hacer si el grupo
  no participa.
```

> **Consejo.** Pídele después que te genere la hoja de evaluación de la sesión. Son dos minutos y os ahorra la discusión de si funcionó o no.

## 9. De la memoria anual a las redes

*Cuando el documento en el que tanto trabajasteis lo han leído seis personas.*

```
Te adjunto nuestra memoria anual [AÑO].

Tarea. Extrae los cinco datos o historias con más potencial comunicativo y
conviértelos en cinco publicaciones para [LinkedIn / Instagram / X].

Para cada una:
- Primera línea con el dato o la frase que hace parar el scroll.
- Cuerpo de tres o cuatro frases, sin jerga del sector.
- Una llamada a la acción concreta.

Reglas:
- Ninguna cifra puede inventarse ni redondearse al alza.
- Cita entre corchetes la página de la memoria de la que sale cada dato,
  para que podamos verificarlo antes de publicar.
- Nada de lenguaje paternalista ni compasivo sobre las personas de las que
  hablamos: son protagonistas, no casos.
```

> **Consejo.** La última regla es la que más veces hay que repetir. Los modelos tienden por defecto al tono caritativo de los años noventa.

---

# Bloque 4 · Gestión interna

## 10. Vuestra política de uso de IA, en una página

*Antes de que cada persona del equipo acabe improvisando por su cuenta.*

```
Ayúdame a redactar la política de uso de inteligencia artificial de
[ENTIDAD], en una sola página y en lenguaje claro.

Contexto. Somos [N] personas, trabajamos con [COLECTIVO] y manejamos
[TIPO DE DATOS]. Estamos sujetos a [NORMATIVA DE PROTECCIÓN DE DATOS
APLICABLE].

Debe cubrir:
1. Qué usos están permitidos y cuáles no.
2. Qué información no se introduce nunca en una herramienta de IA.
3. Quién revisa antes de publicar o de enviar algo a un financiador.
4. Cómo se informa a las personas destinatarias.
5. Qué hacer cuando un uso de IA provoca un error.

Hazme primero las preguntas que necesites. Redáctalo para que lo entienda
todo el equipo, no solo la dirección.
```

> **Consejo.** Una página que todo el mundo lee vale más que un protocolo de veinte que nadie abre. Ponedle fecha de revisión.

---

## Tres líneas que no se cruzan

**Vale para los diez prompts.**

**Datos sensibles, fuera.** Expedientes, datos de menores, información de salud o de situación administrativa y migratoria no entran nunca en una herramienta de IA de uso general. Anonimiza antes: sustituye nombres por códigos y elimina cualquier dato que permita identificar a una persona.

**Sobre personas, decide una persona.** Ninguna adjudicación de ayuda, selección de participantes, priorización o triaje se automatiza. La IA prepara información para que alguien decida; no decide. Esto no es solo una cuestión ética: en muchos ordenamientos es además una obligación legal.

**Lo que firmas, lo verificas.** Si el texto lleva el logo de vuestra entidad, respondéis vosotros de cada cifra, cada cita y cada referencia que contiene. Los modelos inventan datos con total aplomo, y lo hacen sobre todo en lo que más se parece a un dato: porcentajes, fechas, nombres de normas y bibliografía.

---

## Tres cosas para empezar

1. Elige la tarea repetitiva que más detestes y cronométrala antes y después. Sin dato no hay conversación con tu dirección.
2. Escribe vuestra política de uso con el [prompt 10](#10-vuestra-política-de-uso-de-ia-en-una-página). Se hace en una tarde.
3. Prueba los prompts 1 a 4 con una convocatoria real, no con un ejemplo de juguete.

---

*Javier Cantón · UNIR · [javiercanton.com](https://javiercanton.com)*
[Versión editable en DOCX](materiales/Kit-prompts-sector-social.docx) · [CC BY 4.0](LICENSE)
