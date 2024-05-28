# Arabic Text Classification

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Dataset](#dataset)
- [Preprocessing](#preprocessing)
- [Model Training](#model-training)
- [Evaluation](#evaluation)


## Introduction

This project aims to develop a text classification system for Arabic language using Machine Learning and Deep Learning techniques. The system will be able to classify Arabic text documents into 7 predefined categories. The categories are as follows:

1. Politics
2. Sports
3. Finane
4. Medical
5. Tech
6. Culture
7. Religion

## Installation

## Installation

To install the necessary dependencies and set up the project environment, follow these steps:

1. Clone the repository to your local machine:
    ```
    git clone https://github.com/your-username/Arabic-Text-Classification.git
    ```

2. Navigate to the project directory:
    ```
    cd Arabic-Text-Classification
    ```

3. Create a virtual environment:
    ```
    python -m venv env
    ```

4. Activate the virtual environment:
    - For Windows:
      ```
      .\env\Scripts\activate
      ```
    - For macOS and Linux:
      ```
      source env/bin/activate
      ```

5. Install the required packages:
    ```
    pip install -r requirements.txt
    ```

6. You are now ready to use the project!

## Dataset

The dataset used for training and testing the text classification model is [[Arabic News Articles Dataset](https://www.kaggle.com/datasets/haithemhermessi/sanad-dataset)]. The dataset consists of 6500 documents per class, each labeled with one of the seven predefined categories mentioned earlier.

Before using the dataset for training, several preprocessing steps were applied. These steps include tokenization, normalization, stop word removal, and other text cleaning techniques. These preprocessing steps help to ensure that the text data is in a suitable format for training the classification model.

## Preprocessing

Explain the preprocessing steps performed on the Arabic text data before training the classification model. This may include tokenization, normalization, stop word removal, and other text cleaning techniques.

The preprocessing steps used in this project include:

1. Tokenization: The text data is split into individual words or tokens. This helps in breaking down the text into smaller units for further processing.

2. Diacritics: The text data is cleaned from the arabic diacritics.

3. Stop Word Removal: Commonly occurring words that do not carry much meaning, such as articles, prepositions, and pronouns, are removed from the text data. This helps in reducing noise and improving the efficiency of the classification model.

4. Text Cleaning: Various text cleaning techniques are applied to remove unwanted characters, symbols, and punctuation marks from the text data. This helps in ensuring that the text data is in a suitable format for training the classification model.

These preprocessing steps are essential in preparing the text data for training the classification model and improving its performance.

## Model Training

The models that were used in this notebook was Support Vector Classifer and CNN model. The Support Vector Classifier was trained using the TF-IDF features extracted from the text data. The CNN model was trained using the word embeddings generated using the Word2Vec model.

## Evaluation

## Evaluation

The performance of the text classification system was evaluated using the following metrics:

1. Test Set: The evaluation was performed on a separate test set that was not used during the model training process. This ensures an unbiased assessment of the model's performance.

2. Accuracy: The accuracy metric measures the overall correctness of the model's predictions. It is calculated as the ratio of the number of correctly classified instances to the total number of instances in the test set.

3. Precision: Precision measures the proportion of correctly predicted positive instances out of all instances predicted as positive. It is calculated as the ratio of true positives to the sum of true positives and false positives.

4. Recall: Recall, also known as sensitivity or true positive rate, measures the proportion of correctly predicted positive instances out of all actual positive instances. It is calculated as the ratio of true positives to the sum of true positives and false negatives.

5. F1-score: The F1-score is the harmonic mean of precision and recall. It provides a balanced measure of the model's performance by considering both precision and recall. It is calculated as 2 times the product of precision and recall divided by the sum of precision and recall.

These evaluation metrics help assess the performance of the text classification system and provide insights into its accuracy, precision, recall, and overall effectiveness in classifying Arabic text documents into the predefined categories.
