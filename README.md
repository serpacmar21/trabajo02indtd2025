# Trabajo Decisión Multicriterio: El Deporte Más Completo

* **Autor:** Sergio Pacheco Márquez
* **Asignatura:** Teoría de la Decisión
* **Tema:** Selección del deporte más completo para una vida saludable.

---

## Objetivo del Proyecto

Este repositorio contiene el trabajo práctico de la asignatura, cuyo objetivo es aplicar y comparar diversos métodos de decisión multicriterio para resolver el problema: **"Selección del deporte más completo para una vida saludable"**.

El análisis compara 5 alternativas (Deportes) basándose en una jerarquía multinivel de 8 subcriterios.

---

## Contenido del Repositorio

* `multicriterio.qmd`: Fichero fuente Quarto. Contiene todo el código R, el análisis y las conclusiones del trabajo.
* `multicriterio.html`: Informe final renderizado, listo para su revisión.
* `deportes.ahp`: Fichero de entrada (formato YAML) que define la jerarquía multinivel y las matrices de comparación 2 a 2 para el paquete `ahp`.
* `teoriadecision_funciones_multicriterio.R`, `..._utiles.R`, `..._diagram.R`: Scripts con las funciones personalizadas proporcionadas por la cátedra para ejecutar AHP-R, ELECTRE y PROMETHEE.

---

## Metodología y Ejecución

El análisis en el fichero `.qmd` sigue la estructura de la evaluación, cubriendo:

1.  **AHP (Paquete `ahp`):** Análisis jerárquico usando `ahp::AnalyzeTable` y `ahp::Visualize`.
2.  **AHP (Funciones R):** Réplica del cálculo usando `multicriterio.metodoAHP.variante3.basico` y `...coef.inconsistencia` para validar los resultados y la consistencia.
3.  **ELECTRE I:** Análisis iterativo ("paso a paso") del núcleo usando `multicriterio.metodoELECTRE_I`.
4.  **PROMETHEE II:** Ranking completo usando la función `multicriterio.metodo.promethee_windows`.
5.  **Conclusiones:** Comparativa de los rankings de los tres métodos, justificando las diferencias encontradas.

---
