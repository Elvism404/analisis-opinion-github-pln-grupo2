# Análisis de Opinión en Repositorios Git 
## Descripción del Proyecto

En el desarrollo de software colaborativo, plataformas como GitHub almacenan una gran cantidad de información textual en forma de issues, pull requests y comentarios. Estos mensajes reflejan problemas técnicos, decisiones de diseño y niveles de interacción entre desarrolladores.

El presente proyecto aplica técnicas clásicas de Procesamiento de Lenguaje Natural (PLN) para analizar, clasificar y comparar estos textos, con el fin de construir un observatorio de opinión y evaluar la salud general del proyecto.

Se seleccionó el repositorio público:
https://github.com/scikit-learn/scikit-learn

Este repositorio fue elegido por tratarse de un proyecto activo y ampliamente utilizado en el ámbito del aprendizaje automático, lo que garantiza una cantidad significativa de interacciones textuales entre desarrolladores.


## Objetivo 

Aplicar técnicas clásicas de Procesamiento de Lenguaje Natural para analizar el sentimiento, los temas recurrentes y la similitud textual en mensajes de issues y pull requests de un repositorio Git, con el fin de evaluar patrones de interacción y contenido técnico


## Estructura del Repositorio

```
analisis-opinion-github-pln-grupo2/
│
├── data/
│   └── mensajes.csv
│
├── src/
│   └── proyecto_pln.ipynb
│
└── README.md
```

- **data/**: Contiene el dataset generado en formato CSV.
- **src/**: Contiene el notebook con el código fuente del proyecto.
- **README.md**: Documento descriptivo del proyecto.





## Metodología Implementada

El proyecto incluye:

- Recolección automática de datos desde la API de GitHub (issues, pull requests y comentarios).

- Preprocesamiento del texto (limpieza, eliminación de stopwords y lematización).

- Representación vectorial mediante TF-IDF.

- Identificación de temas mediante agrupamiento K-Means.

- Cálculo de similitud coseno entre mensajes.

- El sistema permite trabajar con más de 200 registros aproximadamente, dependiendo del repositorio analizado


## Instrucciones de Ejecución

1. Subir el archivo ubicado en la carpeta src/ a Google Colab.

2. Verificar que el archivo mensajes.csv se encuentre en la carpeta data/ (si se utiliza el dataset ya generado).

3. Ejecutar todas las celdas del notebook en orden.

El sistema realizará automáticamente:

  - Recolección de datos desde la API de GitHub.
  
  - Preprocesamiento y limpieza del texto.
  
  - Representación TF-IDF.
  
  - Agrupamiento de temas.
  
  - Cálculo de similitud entre mensajes.



