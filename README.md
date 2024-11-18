# Twitter Sentiment Analysis NLP

### Introduction

This project leverages the power of machine learning to explore sentiment analysis within the realm of Natural Language Processing (NLP), focusing on Twitter data. It is developed primarily using Python and integrates key libraries such as **Pandas**, **re**, **NLTK**, and **scikit-learn**. The primary objective of this project is to classify Twitter comments or text as either positive or negative, demonstrating an efficient approach to sentiment analysis.

### Data collection and loading

The dataset was sourced from [kaggle sentiment140 ](https://www.kaggle.com/datasets/kazanova/sentiment140) using the Kaggle API. The data was then extracted and loaded into a CSV file for further analysis.

### Text cleaning

To prepare the textual data for analysis, each comment or text undergoes a thorough text-cleaning process. This involves applying a custom function to remove common English stopwords, enabling a focus on the key words that contribute to the sentiment expressed in the content.

### Stemming

The next step involves applying stemming to each word using the **PorterStemmer** from the NLTK library. Stemming is a text normalization technique that reduces words to their root form, effectively removing suffixes while preserving the core meaning of the word. For example, words like *"running,"* *"runner,"* and *"ran"* are transformed into their root word, *"run."* This process helps to standardize the text data, improving consistency and reducing dimensionality, which is crucial for efficient sentiment analysis.

### Feature extraction

The textual data is converted into numerical features using the **Term Frequency-Inverse Document Frequency (TF-IDF)** vectorization technique. This method quantifies the importance of words within the dataset by balancing their frequency in individual comments against their prevalence across the entire dataset. This transformation is a critical step in preparing the data for effective training and evaluation of machine learning models.

### Model training

For sentiment classification, a Logistic Regression model is chosen due to its simplicity and effectiveness in handling text classification tasks. The model is trained on the transformed features, enabling it to learn patterns in the data.

### Model evaluation

This model evaluated using accuracy_score for both traing and test data.

### Save trained model

The trained machine learning model can be efficiently saved using Python's **pickle** library. By storing the model as a `.sav` file, it ensures easy reuse for future predictions without the need for retraining, thereby streamlining the deployment process.
