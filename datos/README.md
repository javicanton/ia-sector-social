# Datos

## [respuestas-cuestionario-programa-educativo.csv](respuestas-cuestionario-programa-educativo.csv)

Doscientas siete respuestas a la pregunta abierta *«¿Qué es lo que más te ha aportado el programa y qué cambiarías?»*, atribuidas a adolescentes participantes en un programa de apoyo educativo.

> **Los datos son ficticios.** Se generaron íntegramente para esta demostración. No corresponden a ninguna persona real, ninguna entidad real y ningún programa real. Se pueden usar libremente para practicar o para formar a un equipo.

**Columnas:** `id`, `sede`, `edad`, `meses_en_programa`, `respuesta`. Doscientas siete filas, cinco sedes (Bogotá, Lima, Guayaquil, Ciudad de México y Quito), edades de 12 a 17 años y entre 3 y 24 meses de permanencia en el programa.

El dataset incorpora ruido a propósito, porque un fichero limpio no enseña nada: doce respuestas de menos de quince caracteres (desde «ok» hasta «asdasd»), dos escritas en inglés y dos que mencionan por su nombre a una persona tutora. Eso es lo que el prompt tiene que apartar en vez de forzarlo dentro de una categoría, y las dos últimas son las que activan la instrucción de señalar datos identificables en lugar de reproducirlos.

**Cómo se usa:** con los [prompts 3 y 4 del guión de demos](../guion-de-demos.md#caso-2--escuchar-a-doscientas-personas), o con el [prompt 5 del kit](../kit-de-prompts.md#5-respuestas-abiertas-de-un-cuestionario) si lo que quieres es adaptarlo a tus propios datos.

**Resultado de la demo:** [ver la conversación en Claude](https://claude.ai/share/6115b846-ab1e-4496-a99b-c987c9cec24a)
