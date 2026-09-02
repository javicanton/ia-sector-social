# Cómo usar la IA para el sector social

**Herramientas, prompts y gestión para entidades sociales.**

Materiales completos de la intervención de [Javier Cantón](https://javiercanton.com) en el Foro UNIR sobre inteligencia artificial en el sector social. Todo lo que se ve en el taller está aquí: las plantillas, los prompts exactos de las demos y las conversaciones reales con sus resultados.

> **La IA no hace intervención social. Te devuelve las horas para hacerla.**

Dirigido a ONG, fundaciones, administraciones y entidades sociales. Perfil práctico: no hace falta saber nada técnico.

---

## Empieza por aquí

| Si quieres… | Ve a |
| --- | --- |
| Diez plantillas listas para usar hoy mismo | **[Kit de prompts](kit-de-prompts.md)** |
| Ver cómo se construye un prompt bueno, paso a paso | **[Guión de demos](guion-de-demos.md)** |
| Ver los resultados reales, sin cortes | **[Los tres casos](casos/README.md)** |
| Leer la charla entera sin descargar nada | **[La presentación, en texto](presentacion.md)** o en **[PDF](materiales/presentacion.pdf)** |
| El kit y el guión en formato editable | **[materiales/](materiales/)** |
| Practicar con el dataset del caso 2 | **[datos/](datos/)** |

Si solo vas a leer una cosa: el [kit de prompts](kit-de-prompts.md). Cada plantilla tiene un botón de copiar arriba a la derecha de la caja gris.

---

## Los tres casos

Los tres se hicieron sobre documentos públicos reales, así que se pueden repetir en casa con los mismos ficheros.

**1 · De la convocatoria al borrador.** Subes las bases de una convocatoria, extraes los criterios de valoración con su peso, y generas el índice del proyecto con un apartado por criterio. El error más común es pedir «escríbeme un proyecto». Lo que funciona es «ajústalo a estos criterios y dime qué me falta para puntuar alto».
→ [Ver la conversación completa](https://claude.ai/share/d3b28d9b-a49a-4da9-a44a-462b1b8d646b) · [Bases de la convocatoria (PDF)](https://fundacionlacaixa.org/documents/d/guest/convocatoria-social-cooperacion-internacional-2026-bases-pdf)

**2 · Escuchar a doscientas personas en diez minutos.** Doscientas siete respuestas abiertas de un cuestionario convertidas en categorías temáticas con recuentos, citas literales y tabla lista para pegar en la memoria. Con su regla de verificación incluida.
→ [Ver la conversación completa](https://claude.ai/share/6115b846-ab1e-4496-a99b-c987c9cec24a) · [Descargar el CSV](datos/respuestas-cuestionario-programa-educativo.csv)

**3 · Un contenido, muchas versiones.** Una memoria anual convertida en lectura fácil, guión de taller e hilo para redes. Aquí la IA sí amplía a quién llegas.
→ [Ver la conversación completa](https://claude.ai/share/e1e7d2c3-f68a-4974-babd-3760f89e3fd1) · [Memoria Anual 2025 (PDF)](https://www.savethechildren.es/sites/default/files/2026-07/MemoriaAnual2025_0.pdf)

El detalle de cada caso, con los documentos de partida y lo que hay que buscar en cada resultado, está en **[casos/README.md](casos/README.md)**.

---

## La fórmula

Los diecisiete prompts de este repositorio están construidos con las mismas seis piezas:

1. **Rol** — desde qué oficio quieres que te responda.
2. **Contexto** — quiénes sois, con quién trabajáis, en qué territorio y con qué medios.
3. **Tarea** — una sola, concreta y verificable.
4. **Formato** — tabla, extensión, apartados. Si no lo pides, te lo inventa.
5. **Criterios** — qué hace buena la respuesta y qué no quieres ver.
6. **Tu material** — documentos, datos, textos previos.

La sexta es la que marca la diferencia. Sin tu material, la respuesta es genérica y se nota.

---

## Tres líneas que no se cruzan

**Datos sensibles, fuera.** Expedientes, datos de menores, información de salud o de situación administrativa y migratoria no entran nunca en una herramienta de IA de uso general. Anonimiza antes.

**Sobre personas, decide una persona.** Ninguna adjudicación de ayuda, selección de participantes o triaje se automatiza. La IA prepara información para que alguien decida; no decide. En muchos ordenamientos, además de un criterio ético es una obligación legal.

**Lo que firmas, lo verificas.** Si lleva el logo de tu entidad, respondes tú de cada cifra, cada cita y cada referencia. Los modelos inventan datos con aplomo, y sobre todo en lo que más se parece a un dato: porcentajes, fechas, nombres de normas y bibliografía.

---

## Qué hay en este repositorio

```
kit-de-prompts.md      Diez plantillas por bloques: financiación, análisis,
                       materiales y comunicación, gestión interna.
guion-de-demos.md      Los siete prompts de las demos, con el desglose de
                       por qué cada uno está escrito así y dónde suele fallar.
presentacion.md        Las doce diapositivas en texto, legibles y buscables.
casos/                 Los tres casos con enlace a la conversación completa.
materiales/            Kit y guión en DOCX editable, y la presentación en PDF.
datos/                 Las 207 respuestas del caso 2, en CSV. Datos ficticios.
```

---

## Cómo usar esto en tu entidad

1. **Sustituye los corchetes.** Todo lo que va entre `[CORCHETES]` son los datos reales de tu entidad. Un prompt sin contexto propio devuelve una respuesta genérica.
2. **Adjunta tus documentos.** Las bases, la memoria, el borrador. El material propio separa una respuesta útil de un texto de relleno.
3. **Que lo lea una persona antes de salir.** Siempre.
4. **Anonimiza antes de pegar nada.**

Tres cosas para empezar mañana:

- Elige la tarea repetitiva que más detestes y cronométrala antes y después. Sin dato no hay conversación con tu dirección.
- Escribe vuestra política de uso con el [prompt 10](kit-de-prompts.md#10-vuestra-política-de-uso-de-ia-en-una-página). Se hace en una tarde.
- Prueba los prompts 1 a 4 con una convocatoria real, no con un ejemplo de juguete.

---

## Licencia

Los materiales de este repositorio se publican bajo [Creative Commons Atribución 4.0 Internacional (CC BY 4.0)](LICENSE). Puedes copiarlos, adaptarlos y usarlos en tu entidad, incluso comercialmente, citando la autoría.

Los documentos de terceros usados en las demos (bases de convocatoria y memorias anuales) no se redistribuyen aquí: se enlazan a su fuente original y pertenecen a sus autores.

---

## Autoría y contacto

**Javier Cantón** — UNIR
[javiercanton.com](https://javiercanton.com) · javier.canton@unir.net

Si adaptas estos materiales para tu entidad o los traduces, cuéntamelo. Me interesa saber qué funciona en contextos distintos al mío.
