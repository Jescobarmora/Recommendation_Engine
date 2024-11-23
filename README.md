# Motor de Recomendación: Biblioteca Luis Ángel Arango

## Descripción

La **Biblioteca Luis Ángel Arango** está en un proceso de digitalización para garantizar los préstamos **EXTERNOS** mediante una plataforma sin necesidad de realizar el trámite de manera presencial. Para ello, la biblioteca almacena toda la información de las interacciones entre usuarios (variable `Identificador Socio`) y libros (variable `Título`).

En épocas de alta demanda, se ha observado que no se dispone de los ejemplares necesarios para atender las necesidades de los usuarios, lo que genera colas de espera y prórrogas para realizar préstamos. Por lo tanto, se requiere desarrollar un **motor de recomendación** que, en tiempo real, sugiera libros a los usuarios para anticipar la cantidad de ejemplares necesarios y así atender la demanda completa, mejorando la experiencia de los usuarios.

La información histórica de préstamos se encuentra en la base de datos `CIRCULA 23 TRANSF S.xlsx`.

## Objetivos

Resuelve el reto mediante las siguientes acciones:

1. **Preparación y Tratamiento de Datos:**
   - Realizar una preparación de datos y tratamiento estadístico adecuado para los libros que han sido leídos una sola vez en toda la historia de la base de datos.
   
2. **Filtrado de Usuarios:**
   - Definir una cantidad razonable de libros que deben leer los usuarios para formar parte del desarrollo del motor de recomendación. Un usuario que haya leído solo un único libro no debería ser considerado.
   
3. **Eliminación de Duplicados:**
   - Evaluar si existen usuarios que lean un mismo libro más de una vez y garantizar que la DATA final del motor no tenga libros duplicados por usuario.
   
4. **Codificación de Datos:**
   - Codificar los usuarios y libros mediante dígitos utilizando técnicas como **Label Encoder**.
   
5. **Desarrollo del Modelo de Recomendación:**
   - Entrenar un motor de recomendación con sistemas embebidos para usuarios y libros mediante IA y redes neuronales (FCNN) con la métrica **HIT RATIO@20**.
   - Realizar pruebas de ensayo y error con el número de dimensiones de los embeddings o el número de neuronas de las capas hasta maximizar la métrica de desempeño predictivo.
