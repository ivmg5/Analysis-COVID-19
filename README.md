---

# Análisis filogenético de SARS-CoV-2 y otros virus

## Descripción

Este repositorio contiene un análisis filogenético del SARS-CoV-2 en comparación con otros 19 virus. El propósito es identificar las relaciones evolutivas basadas en la información genética y entender la posición del SARS-CoV-2 dentro de este árbol evolutivo.

## Contenido

- **Código RMarkdown**: Un archivo RMarkdown que contiene todo el código necesario para realizar el análisis.
- **Secuencias de virus**: Una lista con los números de acceso de GenBank para 20 virus.
- **Resultados**: Gráficos que representan el análisis filogenético y las comparaciones de bases nucleotídicas.

## Procedimiento

1. Se recuperan las secuencias genéticas de los virus desde GenBank.
2. Se realizan análisis descriptivos de las secuencias, incluyendo la visualización de las bases nucleotídicas.
3. Se alinean las secuencias genéticas para identificar regiones de similitud y diferencia.
4. Se construye un árbol filogenético utilizando el método de Neighbor-Joining (NJ) basado en las secuencias alineadas.
5. Se visualiza el árbol filogenético y se interpretan las relaciones evolutivas.

## Resultados

El análisis muestra que el SARS-CoV-2 comparte similitudes genéticas con otros coronavirus humanos. A través de la comparación de las bases nucleotídicas y el árbol filogenético, es posible identificar patrones y relaciones que pueden ser cruciales para entender la evolución y el comportamiento del virus.

## Cómo ejecutar

1. Asegúrese de tener R y RStudio instalados.
2. Clone este repositorio en su máquina local.
3. Abra el archivo RMarkdown en RStudio.
4. Instale los paquetes necesarios si aún no lo ha hecho.
5. Ejecute el código para obtener los resultados.

## Referencias

- Johns Hopkins Coronavirus Resource Center: [COVID-19 Map](https://coronavirus.jhu.edu/map.html)
- Seguimiento de las variantes del SARS-CoV-2: [World Health Organization](https://www.who.int/es/activities/tracking-SARS-CoV-2-variants)
- Fuentes oficiales para consultar información sobre COVID-19 en países de Iberoamérica: [Fundación Gabo](https://fundaciongabo.org/es/noticias/articulo/fuentes-oficiales-para-consultar-informacion-sobre-covid-19-en-paises-de)
- Zhou, P., et al. (2020). A pneumonia outbreak associated with a new coronavirus of probable bat origin. Nature, 579(7798), 270-273.
- Lam, T. T., et al. (2020). Identifying SARS-CoV-2 related coronaviruses in Malayan pangolins. Nature, 583(7815), 282-285.

---
