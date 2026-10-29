# Evaluación de `cms.md` y `ssg.md`

## 1. Criterios de evaluación puntuados

**Escala utilizada:** cada criterio se puntúa de 0 a 2 puntos.

- **0 puntos:** no se cumple o falta información importante.
- **1 punto:** se cumple parcialmente; hay aspectos que aclarar o completar.
- **2 puntos:** se cumple correctamente y con suficiente claridad.

La rúbrica concreta de 16 criterios no venía incluida en el material recibido. Por ello, se propone una rúbrica explícita de 16 criterios basada en los contenidos y objetivos visibles de ambos documentos. Si existe una rúbrica oficial de clase, las puntuaciones deberán adaptarse a ella.

| N.º | Criterio | Evidencia concreta | Observación | Puntuación |
|---:|---|---|---|:---:|
| 1 | Definición del concepto principal | `cms.md`, apartado **«¿Qué es un CMS?»**; `ssg.md`, apartado **«¿Qué es un SSG?»** | Ambos documentos definen el concepto y desarrollan las siglas. Las definiciones son comprensibles para un lector principiante. | 2/2 |
| 2 | Explicación de la finalidad | `cms.md`, **«¿Para qué sirve?»**; `ssg.md`, **«¿Para qué sirve?»** | Se explica la utilidad de cada tecnología, aunque se podrían incluir casos de uso concretos en ambos apartados. | 1/2 |
| 3 | Explicación del funcionamiento | `cms.md`, **«¿Cómo funciona?»**; `ssg.md`, **«¿Cómo funciona?»** | El CMS se explica mediante la publicación y consulta del contenido; el SSG mediante la combinación de contenido y plantillas. Los pasos podrían detallarse más. | 2/2 |
| 4 | Ejemplos prácticos o código | `cms.md`, bloque de pseudocódigo PHP; `ssg.md`, ejemplo Markdown con *front matter* | Los dos incluyen un ejemplo relacionado con su explicación. El ejemplo PHP es muy simplificado y no explica cómo se obtienen o validan los datos; el de SSG no muestra el comando de generación. | 1/2 |
| 5 | Apoyo visual | `cms.md`, imágenes `img/proceso_cms.png` e `img/cuota_cms.png`; `ssg.md`, imagen `img/proceso_ssg.png` | Se incluyen referencias a imágenes que pueden ayudar a comprender el contenido. Conviene comprobar que los archivos existen en el repositorio, se cargan y tienen texto alternativo descriptivo. | 1/2 |
| 6 | Ventajas e inconvenientes | `cms.md`, **«Ventajas e inconvenientes»**; `ssg.md`, tabla **«Ventajas e inconvenientes»** | Se presentan ventajas y limitaciones de ambos enfoques. En la tabla del SSG, la última fila no incluye un inconveniente correspondiente, por lo que podría completarse o reorganizarse. | 1/2 |
| 7 | Clasificación y variedad de ejemplos | `cms.md`, **«Tipos de CMS y ejemplos»** | Se clasifican CMS por propósito y arquitectura, con ejemplos como WordPress, Moodle, Strapi y Contentful. Es una sección amplia y útil. | 2/2 |
| 8 | Comparación de herramientas | `ssg.md`, **«Comparativa: Jekyll, Hugo y Astro»** | La tabla compara lenguaje, contenido, instalación, usos y ventajas. Sería útil indicar versiones o fecha de revisión, porque las herramientas evolucionan. | 1/2 |
| 9 | Comparación directa CMS frente a SSG | `cms.md`, **«CMS dinámico frente a SSG»** | La tabla compara almacenamiento, generación HTML, servidor, seguridad, rendimiento y publicación. Es una de las partes más útiles para relacionar ambos documentos. | 2/2 |
| 10 | Precisión de las afirmaciones técnicas | `cms.md`, tabla comparativa sobre seguridad y rendimiento; `ssg.md`, ventajas y tabla de Astro | Las explicaciones son válidas como introducción, pero algunas frases pueden parecer absolutas: un SSG no elimina todos los riesgos y el rendimiento depende de la configuración. Astro también puede trabajar con renderizado bajo demanda, como indica la tabla. | 1/2 |
| 11 | Fuentes y datos verificables | `cms.md`, **«Los CMS más usados»**, con datos atribuidos a W3Techs y fecha de consulta | Se indica la fuente y la fecha, pero la referencia `[^1]` no tiene una nota al pie definida en el contenido revisado. Debe añadirse el enlace directo y la referencia completa. | 1/2 |
| 12 | Organización e índice | Índices al comienzo de ambos archivos y apartados ordenados | La estructura es clara y los índices anticipan el contenido. Conviene comprobar que todas las anclas funcionan después de cualquier edición. | 2/2 |
| 13 | Navegación entre documentos | `cms.md`, enlace a `ssg.md`; `ssg.md`, enlace de vuelta a `cms.md` | Los archivos se enlazan entre sí, lo que facilita la consulta. El enlace de retorno de `ssg.md` aparece al principio; podría añadirse también al final. | 2/2 |
| 14 | Claridad del lenguaje y terminología | Ambos documentos emplean términos como *backend*, *frontend*, API, *build*, *hosting* y *headless* | El lenguaje general es accesible, pero algunos términos técnicos aparecen sin definición breve. Un glosario ayudaría a lectores que empiezan. | 1/2 |
| 15 | Ortografía, formato y consistencia Markdown | Tablas, listas, bloques de código, títulos y enlaces en ambos documentos | El formato es consistente y legible. Conviene revisar la nota al pie sin definir, los textos alternativos de las imágenes y la consistencia de términos y nombres. | 1/2 |
| 16 | Conclusiones y orientación para elegir tecnología | `ssg.md`, **«Conclusiones»**; `cms.md`, comparación dinámica frente a estática | `ssg.md` recomienda herramientas según el contexto. Falta una conclusión conjunta que resuma cuándo elegir un CMS, un SSG o una solución híbrida. | 1/2 |
|  | **TOTAL** |  |  | **22/32** |

## 2. Suma de puntos y nota justificada

- **Puntuación obtenida:** 22 puntos.
- **Puntuación máxima:** 32 puntos.
- **Conversión a nota sobre 10:** \(22 / 32 \times 10 = 6,875\).
- **Nota propuesta:** **6,9/10**.

**Justificación:** los documentos presentan definiciones claras, una estructura ordenada, ejemplos de herramientas y una comparación directa entre CMS y SSG. Esto permite comprender los conceptos principales. La nota no es más alta porque faltan algunos elementos de verificación y desarrollo: la referencia de W3Techs no está completada, los ejemplos prácticos no muestran todo el proceso, algunos términos técnicos no se explican y varias afirmaciones de seguridad y rendimiento necesitan matices. La calificación es orientativa y se basa en la rúbrica propuesta, no en una rúbrica oficial proporcionada por el docente.

## 3. Dos puntos fuertes del trabajo

1. **Buena organización y lectura sencilla.** Ambos archivos incluyen índice, títulos jerarquizados, listas y tablas. Esto permite localizar rápidamente la información y consultar los conceptos por partes.
2. **Comparaciones y ejemplos relevantes.** `cms.md` contrasta CMS dinámicos y SSG con criterios concretos, mientras que `ssg.md` compara Jekyll, Hugo y Astro. Los ejemplos de PHP y Markdown ayudan a relacionar la explicación con situaciones técnicas.

## 4. Propuestas de mejora

### P1. Mejora de `cms.md`: completar las fuentes y contextualizar los datos de uso

**Apartado exacto:** `## Los CMS más usados`, especialmente la frase «Según W3Techs[^1]...» y la tabla de cuotas.

**Qué se observa:** se ofrecen porcentajes concretos para WordPress, Shopify, Wix, Squarespace y Joomla, y se indica una fecha de consulta. Sin embargo, en el archivo revisado se utiliza la referencia `[^1]` sin incluir la definición de esa nota al pie. De este modo, el lector no dispone de una referencia bibliográfica completa desde el propio documento.

**Cómo mejorarlo:**
- Añadir al final del documento la definición de la nota al pie con el enlace directo a la página de W3Techs consultada.
- Mantener la fecha de consulta y aclarar qué mide la tabla (por ejemplo, la distribución entre los sitios que utilizan un CMS, según la metodología de la fuente), para que los porcentajes no se interpreten como una cuota de todas las webs sin distinción.
- Revisar los datos antes de entregar el trabajo y actualizar las cifras si la fuente ya muestra valores diferentes.
- Añadir una frase que explique la conclusión principal de los datos, en lugar de dejar que la tabla hable por sí sola.

**Mejora de información:** esta propuesta mejora la verificabilidad y la interpretación de los datos, no solo el formato del documento.

### P2. Mejora de `ssg.md`: explicar el proceso completo de generación y publicación

**Apartado exacto:** `## ¿Cómo funciona?` y `### ¿En qué momento se genera el HTML?`, junto al ejemplo de `## Archivos de partida`.

**Qué se observa:** el documento explica que el generador combina contenido y plantillas y que el HTML se produce durante el *build*. Incluye un ejemplo de Markdown con *front matter*, pero no muestra qué comando ejecutaría el usuario ni cómo comprobaría el resultado generado.

**Cómo mejorarlo:**
- Añadir un ejemplo sencillo y rotulado como ilustrativo con los pasos: crear `index.md`, asociarlo a una plantilla, ejecutar el comando de compilación del SSG elegido, revisar la carpeta de salida y publicar los archivos generados.
- Si se usa Hugo como ejemplo, indicar un comando típico como `hugo` para generar el sitio y explicar que la carpeta de salida depende de la configuración del proyecto.
- Mostrar una estructura de carpetas mínima, por ejemplo `content/`, `layouts/` y `public/`, aclarando que los nombres varían entre herramientas.
- Explicar qué ocurre si hay un error de plantilla o si se cambia el contenido: se vuelve a generar el sitio y se publica la nueva versión.
- Matizar que algunas herramientas, como Astro, también permiten renderizado bajo demanda; el comportamiento depende de la configuración y del modo de despliegue.

**Mejora de la explicación:** el lector pasaría de conocer la idea general a entender los pasos reales de trabajo y la diferencia entre editar el contenido, generar el sitio y publicarlo.

## 5. Orden recomendado de aplicación

1. Aplicar **P1** en `cms.md` para que las cifras y su fuente sean verificables.
2. Aplicar **P2** en `ssg.md` para completar la explicación práctica.
3. Revisar los demás puntos de la tabla, especialmente la nota al pie, el texto alternativo de las imágenes, el glosario y los matices sobre seguridad y rendimiento.

---
*Documento elaborado a partir de los contenidos revisados de `cms.md` y `ssg.md`. Las puntuaciones son una evaluación orientativa mediante la escala propuesta de 0 a 2 puntos por criterio.*
