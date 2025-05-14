# NLP Sentiment Models Comparison

**Español al final**

## Overview

This project explores the classification of movie review sentiment using various NLP preprocessing techniques and machine learning models. We built a pipeline to clean and vectorize textual data, and trained multiple classifiers to distinguish between positive and negative reviews using IMDB data.

## Objectives

* Analyze sentiment from natural language text (movie reviews)
* Compare different text preprocessing methods (NLTK vs. spaCy)
* Evaluate traditional ML models for text classification

## Dataset

The dataset contains labeled movie reviews from IMDB with binary sentiment values:

* `review`: The text of the movie review
* `pos`: Sentiment label (1 = positive, 0 = negative)
* `ds_part`: Indicates whether the review belongs to the train or test set

## Models Compared

We tested and evaluated the following models:

| Model   | Preprocessing | Vectorizer | Classifier         |
| ------- | ------------- | ---------- | ------------------ |
| Model 1 | NLTK          | TF-IDF     | LogisticRegression |
| Model 2 | spaCy         | TF-IDF     | LogisticRegression |
| Model 3 | spaCy         | TF-IDF     | LGBMClassifier     |

## Results

All models surpassed the target F1 score of 0.85. Model 3 showed the highest confidence and consistency on personalized review predictions. Evaluation included F1, ROC AUC, and Average Precision Score (APS) for both training and test sets.

## Usage

1. Clone the repo:

```bash
git clone https://github.com/Hacanaval/nlp-sentiment-models-comparison.git
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Run the notebook:
   Open `nlp-sentiment-models-comparison.ipynb` and execute all cells.

## Requirements

See `requirements.txt` for a full list of libraries.

## Folder Structure

```
nlp-sentiment-models-comparison/
├── src/                      # Optional helper functions
├── nlp-sentiment-models-comparison.ipynb  # Main notebook
├── requirements.txt
├── README.md
└── .gitignore
```

---

## Comparación de Modelos de Sentimiento con NLP

## Descripción

Este proyecto analiza cómo clasificar el sentimiento de reseñas de películas usando diferentes técnicas de procesamiento de lenguaje natural y modelos de aprendizaje automático. Construimos una tubería de limpieza, vectorización y clasificación de texto basada en datos de IMDB.

## Objetivos

* Analizar sentimientos en texto natural (reseñas de películas)
* Comparar enfoques de preprocesamiento (NLTK vs. spaCy)
* Evaluar modelos de clasificación tradicionales

## Modelos Comparados

| Modelo   | Preprocesamiento | Vectorizador | Clasificador       |
| -------- | ---------------- | ------------ | ------------------ |
| Modelo 1 | NLTK             | TF-IDF       | LogisticRegression |
| Modelo 2 | spaCy            | TF-IDF       | LogisticRegression |
| Modelo 3 | spaCy            | TF-IDF       | LGBMClassifier     |

## Resultados

Todos los modelos superaron el umbral de F1 = 0.85. El Modelo 3 destacó por su mayor consistencia y confianza. Las métricas evaluadas incluyeron F1, ROC AUC y Precisión Promedio (APS).

## Uso

1. Clona el repositorio:

```bash
git clone https://github.com/Hacanaval/nlp-sentiment-models-comparison.git
```

2. Instala las dependencias:

```bash
pip install -r requirements.txt
```

3. Ejecuta el notebook:
   Abre `nlp-sentiment-models-comparison.ipynb` y ejecuta todas las celdas.

## Requisitos

Consulta `requirements.txt` para ver las librerías necesarias.

