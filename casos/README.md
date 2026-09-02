# Los tres casos

Las tres demos del taller, con enlace a la conversación completa. Se pueden repetir en casa: los documentos de partida son públicos y el dataset del caso 2 está en este repositorio.

Los prompts exactos, con el desglose de por qué están escritos así y qué debe salir, están en el [guión de demos](../guion-de-demos.md).

---

## Caso 1 · De la convocatoria al borrador

**Captación de financiación.** Cuatro pasos: subes las bases, extraes los criterios de valoración con su peso exacto, generas el esqueleto de la solicitud con un apartado por criterio, y de ahí sale el marco lógico.

- **Documento:** [bases de la Convocatoria de Cooperación Internacional 2026 de la Fundación ”la Caixa” (PDF, 4,1 MB)](https://fundacionlacaixa.org/documents/d/guest/convocatoria-social-cooperacion-internacional-2026-bases-pdf), desde [la página de la convocatoria](https://fundacionlacaixa.org/es/convocatorias-sociales-cooperacion-internacional). La convocatoria ya está cerrada —se presentó entre el 15 de abril y el 20 de mayo de 2026—, pero las bases siguen publicadas y sirven igual para practicar.
- **Prompts:** [1 y 2 del guión](../guion-de-demos.md#caso-1--de-la-convocatoria-al-borrador), encadenados en la misma conversación.
- **Conversación completa:** [ver el resultado en Claude](https://claude.ai/share/d3b28d9b-a49a-4da9-a44a-462b1b8d646b)

El error más común es pedir «escríbeme un proyecto». Lo que funciona es «ajústalo a estos criterios de valoración y dime qué me falta para puntuar alto».

**El momento interesante:** las bases desglosan el 75 % del proyecto en cinco subcriterios pero no asignan puntos a cada uno. Muchos modelos se inventan un reparto verosímil. Por eso el prompt lleva la regla antifabulación y la columna de página.

---

## Caso 2 · Escuchar a doscientas personas en diez minutos

**Análisis de información.** Doscientas siete respuestas abiertas de un cuestionario a personas participantes, convertidas en categorías temáticas emergentes, con recuento, citas literales que sostienen cada categoría y tabla lista para pegar en la memoria.

- **Documento:** [`respuestas-cuestionario-programa-educativo.csv`](../datos/respuestas-cuestionario-programa-educativo.csv), 207 filas. **Datos ficticios**, generados para la demo; se pueden usar libremente para practicar o para formar a un equipo.
- **Prompts:** [3 y 4 del guión](../guion-de-demos.md#caso-2--escuchar-a-doscientas-personas).
- **Conversación completa:** [ver el resultado en Claude](https://claude.ai/share/6115b846-ab1e-4496-a99b-c987c9cec24a)

**La regla que no se salta:** coge veinte respuestas al azar y comprueba que están bien clasificadas. Si fallan, cambia el prompt, no los datos.

Sirve igual para entrevistas transcritas, actas de asamblea o mensajes del equipo de campo.

---

## Caso 3 · Un contenido, muchas versiones

**Materiales y comunicación.** Una memoria anual convertida en tres cosas distintas: una adaptación a lectura fácil para las personas de las que habla el documento, un guión de taller de 90 minutos para voluntariado, y un hilo de cinco piezas para redes.

- **Documento:** [Memoria Anual 2025 de Save the Children España (PDF)](https://www.savethechildren.es/sites/default/files/2026-07/MemoriaAnual2025_0.pdf), desde [la página de la memoria](https://www.savethechildren.es/memoria-2025).
- **Prompts:** [5 y 6 del guión](../guion-de-demos.md#caso-3--un-contenido-muchas-versiones).
- **Conversación completa:** [ver el resultado en Claude](https://claude.ai/share/e1e7d2c3-f68a-4974-babd-3760f89e3fd1)

Accesibilidad y adaptación cultural: aquí la IA sí amplía a quién llegas.

**El hallazgo de la demo:** la memoria da 13,6 millones de niños y niñas alcanzados en emergencias en un sitio y 37,8 millones atendidos en otro. Miden cosas distintas, pero conviven en el mismo documento sin explicarlo. Pedirle al modelo que señale las contradicciones en vez de armonizarlas lo convierte en un detector de incoherencias de tus propios documentos.

---

## Nota sobre los documentos de terceros

Las bases de la convocatoria y la memoria anual no se redistribuyen en este repositorio. Son documentos públicos de sus respectivas organizaciones y se descargan desde sus webs. Se usan aquí como material de demostración, sin relación ni respaldo de ninguna de las dos entidades.
