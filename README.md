[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/yRVxdVvH)
[![Open in Codespaces](https://classroom.github.com/assets/launch-codespace-7f7980b617ed060a017424585567c406b6ee15c891e84e1186181d67ecf80aa0.svg)](https://classroom.github.com/open-in-codespaces?assignment_repo_id=12351959)
# Obligatorio - Machine Learning en Producción 

```text
Master en Big Data

Fecha de entrega: 30-11-2023
Puntaje máximo: 40 puntos
Grupos: Hasta 3 integrantes. 
Importante:  La entrega debe realizarse a través de gestion.ort.edu.uy
```
## Descripción
El objetivo del obligatorio  es llevar a la práctica los conceptos vistos durante el curso construyendo un sistema de Machine Learning de principio a fin. 

La tarea consiste en desarrollar un sistema de clasificación que combine imágenes y/o datos tabulares para resolver un problema de clasificación binaria o multiclase. El proyecto debe incluir la construcción del dataset, la selección de características, la optimización del modelo y la exposición de una API para realizar predicciones online y batch. Se va a prestar especial atención a que se tomen las consideraciones necesarias para prevenir los problemas que pueden surgir al desarrollar sistemas de ML que van ser llevados a producción e interactuar con la realidad. 
## Consigna
### Requerimientos mínimos
#### Dataset
Crear un dataset de imágenes y/o datos tabulares asociados a partir de la fuente de preferencia. Se sugiere aprovechar lo trabajado en la clase de práctico como base, pero se aceptan otras propuestas.
Incluir un análisis exploratorio de los datos (EDA).
#### Representación del problema
Definir un problema de clasificación binaria o multiclase para el cual puedan utilizarse tanto imágenes como datos tabulares.
El target debe ser definido por los estudiantes.
#### Ambiente
Definir las dependencias del proyecto para entornos de desarrollo y producción.
Utilizar Docker para el despliegue del proyecto.
#### Versionado de código
Utilizar Git para para versionar el código. Se va a requerir compartir el repositorio en Github como parte de la entrega. 
#### Desafíos generales
Prevenir data leakage
Prevenir training-serving skew.
#### Exponer una API con el modelo
Desarrollar una API que permita realizar predicciones online y batch. Deberán incluir documentación para el uso de su API. Si utilizan Fast API, pueden aprovechar la documentación automática que genera.
#### Plataforma de despliegue
Se recomienda el uso de AWS a través de AWS Academy para el desarrollo del proyecto.
Si ya están familiarizados con otras plataformas y herramientas pueden optar por usarlas. 
### Requerimientos electivos 
Como mínimo se requiere que implementen 3 de las siguientes técnicas. Cuantos más implementen, mejor. Va a ser tenido en cuenta al momento de la corrección.
Si implementan técnicas de optimización de modelos, se espera que evalúen su impacto en el rendimiento de su modelo y sistema (ej. cómo impacta métricas de ML o la latencia). 
#### Trazabilidad de ML
Considerar versionar:
los experimentos,
los modelos, 
los datos.
#### Explicabilidad
Aplicar técnicas que permitan explicar o interpretar los modelos o sus predicciones.
#### Visualización
Utilizar herramientas como Streamlit o Gradio para interactuar con el modelo a través de una interfaz de usuario. 
#### AutoML
Pueden utilizar AutoML, incluso de manera no-code. Si lo utilizan, el requerimiento de Visualización, mencionado anteriormente, deja de ser electivo y pasa a ser un requerimiento mínimo.
#### Optimización de modelos
Implementar al menos dos de las siguientes optimizaciones.
* 1. Realizar selección de características para datos tabulares.
* 2. Utilizar data augmentation para imágenes.
* Optimizar el modelo mediante técnicas como:
  * 3. ajuste de hiperparámetros,
  * 4. quantization, 
  * 5. pruning,
  * 6. o distillation.

Si deciden implementar otras técnicas avanzadas que sean útiles en el desarrollo y despliegue de sistemas de ML en producción, lo incluyen en el informe de la entrega. 
## Entrega
La entrega del trabajo obligatorio incluye un informe en conjunto con el código base. En el informe deben explicar cómo resolvieron cada uno de los desafíos. Donde corresponda,  agregan referencias al código base o las herramientas que hayan usado para resolver los desafíos. También pueden apoyarse en diagramas de la arquitectura de la solución.
Esperamos que discutan las ventajas y desventajas de las maneras en que resolvieron los diferentes puntos y que comenten posibles alternativas o mejoras. 

Creamos una tarea grupal en GitHub Classroom. Una vez que la acepten, se les va a crear un repositorio automáticamente. Incluyan todo lo que vayan a entregar en el repositorio. No olviden que también deben hacer la entrega formal en gestion.ort.edu.uy. 
### Criterios de Evaluación
Algunos puntos importantes que consideraremos para la corrección del obligatorio serán:
Claridad expositiva. 	
Prolijidad y contenido.
Análisis Exploratorio y Preparación de los datos.
Profundidad adecuada y uso de técnicas vistas en clase.
Resolución exitosa de los desafíos planteados.
## Notas adicionales
Vamos a priorizar el desarrollo end-to-end del proyecto por encima del rendimiento del modelo. Por ello, les recomendamos comenzar con un baseline end-to-end y que recién luego incorporen mejoras en su sistema. 
Se aceptan propuestas para resolver problemas de ML distintos al sugerido.
Se otorgarán puntos extra o compensatorios por la resolución de problemas adicionales o por la implementación de técnicas avanzadas.
