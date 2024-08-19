# News-Topic-Classification-Dataset

This repository contains the implementation of a text classification task using various machine learning algorithms. The goal is to preprocess textual data, vectorize it, and classify it using different models, comparing their performance to identify the best approach.

## **Table of Contents**
- [Project Overview](#project-overview)
- [Preprocessing](#preprocessing)
- [Vectorization Techniques](#vectorization-techniques)
- [Machine Learning Models](#machine-learning-models)
- [Performance Evaluation](#performance-evaluation)
- [Conclusion](#conclusion)

## **Project Overview**
This project aims to classify text data into predefined categories using different machine learning models. The text data undergoes several preprocessing steps, is vectorized using two techniques, and is then classified using three different models. The results are compared based on classification reports and confusion matrices.

## **Preprocessing**
The preprocessing steps are performed using NLTK and SpaCy and include:
- **Tokenization:** Breaking down text into individual tokens (words).
- **Lemmatization:** Reducing words to their base form.
- **Data Cleansing:** 
  - Removal of stopwords.
  - Removal of symbols and special characters.
  - Removal of URLs.

## **Vectorization Techniques**
Two vectorization techniques are used to transform the textual data into numerical format:
- **CountVectorizer:** Converts the text into a matrix of token counts.
- **TFIDFVectorizer:** Converts the text into a matrix of TF-IDF features, reflecting the importance of terms relative to the document corpus.

## **Machine Learning Models**
Three machine learning algorithms are used to classify the vectorized text data:
- **Logistic Regression**
- **Support Vector Classifier (SVC)**
- **Random Forest (RF)**

Each model is trained and evaluated using both CountVectorizer and TFIDFVectorizer.

## **Performance Evaluation**
The models are evaluated using:
- **Classification Report:** Precision, recall, and F1-score for each class.
- **Confusion Matrix with Heatmap:** Visual representation of the model's classification performance.

The results indicate that **Logistic Regression with TFIDFVectorizer** provides the best performance, with the highest accuracy and balanced F1-scores across all classes.

## **Conclusion**
The analysis concludes that Logistic Regression with TFIDFVectorizer is the most effective approach for the given text classification task. This combination yields the highest accuracy and consistent performance across different classes, making it the recommended choice for similar tasks.



