# Twitter Sentiment Analysis NLP

### Introduction

This project leverages the power of machine learning to explore sentiment analysis within the realm of Natural Language Processing (NLP), focusing on Twitter data. It is developed primarily using Python and integrates key libraries such as **Pandas**, **re**, **NLTK**, and **scikit-learn**. The primary objective of this project is to classify Twitter comments or text as either positive or negative, demonstrating an efficient approach to sentiment analysis.

### Data collection and loading

The dataset was sourced from [kaggle sentiment140 ](https://www.kaggle.com/datasets/kazanova/sentiment140) using the Kaggle API. The data was then extracted and loaded into a CSV file for further analysis.

### Text cleaning

To prepare the textual data for analysis, each comment or text undergoes a thorough text-cleaning process. This involves applying a custom function to remove common English stopwords, enabling a focus on the key words that contribute to the sentiment expressed in the content.
