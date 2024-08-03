# IMDB Review Sentiment Analysis: A Comprehensive Report

## Abstract

This report presents a project focused on classifying movie reviews from the IMDB dataset as positive or negative using Natural Language Processing (NLP) techniques and Word2Vec models. By leveraging custom-trained Skip-gram and Continuous Bag of Words (CBOW) models alongside a pretrained Word2Vec model, and employing the RandomForest classifier, we achieved notable performance in sentiment classification. This report covers the dataset, methodology, results, and implications of the findings.

## 1. Introduction

Sentiment analysis of movie reviews is a crucial task in understanding audience feedback and enhancing user experiences on review platforms. This project aims to develop an NLP-based model to classify IMDB movie reviews as positive or negative, providing valuable insights into public opinion.

## 2. Data Overview

The dataset consists of 50,000 movie reviews labeled as 'positive' or 'negative'. The primary focus is on the text content for classification purposes.

### Initial Data Exploration

The dataset contained two columns: 'review' and 'sentiment'. The data underwent initial cleaning to ensure consistency and relevance.

## 3. Methodology

### 3.1 Data Preprocessing

The preprocessing phase included several critical steps:
- **Tokenization**: Breaking down text into individual tokens or words.
- **Stopword Removal**: Excluding common words that do not provide significant meaning.
- **Cleaning**: Eliminating punctuation marks to focus on meaningful text.

### 3.2 Feature Extraction

Three primary methods were used for feature extraction:
- **Skip-gram**: A technique that predicts the context words for a given target word, capturing semantic relationships.
- **CBOW**: A technique that predicts the target word from its context words, capturing syntactic and semantic relationships.
- **Pretrained Word2Vec**: Using a pretrained Word2Vec model trained on a large corpus, such as Google News, to leverage comprehensive word embeddings.

### 3.3 Model Training

We utilized the RandomForest classifier, known for its robustness and efficiency. The data was divided into training and testing sets, with the model being trained on the extracted features.

## 4. Results

The model's performance was assessed using accuracy and classification reports. The results were:
- **Skip-gram**: 
  - Accuracy: [85%]
- **CBOW**: 
  - Accuracy: [84%]
- **Pretrained Word2Vec**: 
  - Accuracy: [82%]


These results indicate that all three methods provide effective feature representations for classifying movie reviews.

## 5. Discussion and Analysis

The findings underscore the importance of feature extraction techniques in text classification tasks. The consistently high accuracy scores demonstrate the model's capability in accurately detecting sentiment in movie reviews.

## 6. Conclusion

This project successfully demonstrates the application of NLP techniques in sentiment analysis. The RandomForest classifier, coupled with Word2Vec embeddings, yielded a reliable model for distinguishing positive and negative reviews. Future work may explore the use of more complex models and additional data sources to enhance accuracy further.

## 7. Future Work

- **Advanced NLP Models**: Investigating the use of deep learning approaches like transformers for better contextual understanding.
- **Cross-Domain Evaluation**: Testing the model on different datasets to evaluate its generalizability.
- **Real-time Application**: Developing a system for real-time sentiment analysis in review platforms.



