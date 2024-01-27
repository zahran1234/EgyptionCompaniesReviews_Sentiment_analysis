# EgyptionCompaniesReviews_Sentiment_Analysis

This project focuses on performing sentiment analysis on reviews of Egyptian companies gathered from Twitter and Google Play. The objective is to understand public sentiment towards these companies by analyzing text data.

## Steps of the Project

### 1. Dataset
- **Sources**: Reviews collected from Twitter and Google Play.
- **Focus**: The dataset comprises user-generated content about various Egyptian companies.

### 2. Data Cleaning
Data preprocessing is crucial for ensuring the quality and reliability of the analysis. The steps include:
- **Removing Headline Emojis**: Cleansing the data of emojis present in the text, which might skew the sentiment analysis.
- **Removing Diacritics**: Diacritics in Arabic can alter the meaning of words and hence are removed for consistency.
- **Removing Stop Words**: Filtering out common words that do not contribute to the overall sentiment of the text.

### 3. Convert Text Data to Numerical Data
To facilitate machine learning, text data is converted into numerical form through:
- **TF-IDF (Term Frequency-Inverse Document Frequency)**: A statistical measure used to evaluate the importance of a word to a document in a collection or corpus.
- **Word2Vec**: Using the average Word2Vec for feature extraction. This involves representing each word by a dense vector which is then averaged for each document.

## 4. Models
The project employs various machine learning and deep learning models to perform sentiment analysis.

### 4.1 Traditional Machine Learning Models
Several models are explored for their effectiveness in sentiment analysis:
- **SVM (Support Vector Machine)**
- **Decision Tree**
- **Random Forest**
- **KNN (K-Nearest Neighbors)**
- **Naive Bayes (NB)**
- **Linear SVM (LSVM)**

### 4.2 Deep Learning Models
Deep learning models offer a more complex and nuanced approach:
- **Forward Neural Network**: A basic neural network structure.
- **Convolutional Neural Network (CNN)**: Particularly effective in text classification for capturing the spatial structure in data.

### 4.3 Sequential Models
These models are adept at handling sequences of data, like text:
- **RNN (Recurrent Neural Network)**
- **GRU (Gated Recurrent Unit)**
- **LSTM (Long Short-Term Memory)**: Known for its ability to retain information over long periods, making it suitable for lengthy texts.

## 5. Best Results
The most effective approach in this project was found to be:
- **Text Representation**: Applying the average Word2Vec for converting text into numerical data.
- **Model of Choice**: GRU (Gated Recurrent Unit) for its efficiency in processing sequences and handling dependencies in text data.

## Conclusion
This project demonstrates the application of various machine learning and deep learning techniques in sentiment analysis of reviews related to Egyptian companies. By analyzing textual data from social media and app reviews, valuable insights into public perception can be garnered, which can be instrumental for businesses in strategy formulation and customer relationship management.
