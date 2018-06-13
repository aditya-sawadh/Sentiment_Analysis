# Sentiment_Analysis
This project in this repository takes a supervised learning approach towards sentiment analysis.
We build a Logistic regression and Naiye Bayes classifier models for sentiment analysis of tweets and IMDB movie reviews.

The  feature vectors for classifiers are generated using two approaches

(1) A more traditional NLP technique where the features are simply “important” words and the feature vectors are 
simple binary vectors  
(2) the Doc2Vec technique where document vectors are learned via artificial neural networks

Datasets

The IMDB reviews and tweets can be found in the data folder. These have already been divided
into train and test sets.

a) The IMDB dataset contains already split train and test data. A negative review has a score <= 4 out of 10, and a positive
review has a score >= 7 out of 10. Thus reviews with more neutral ratings are not included in the train/test sets.

b) The Twitter Dataset, contains 900,000 classified tweets split into 750k train and 150k test sets. 
The overall distribution of labels is balanced (450k pos and 450k neg).

The sentiment_analysis.py contains the code for this project. The python packages that you will need for this project are scikitlearn, nltk, and gensim.

As a point of reference, Stanfords Recursive Neural Network code (https://nlp.stanford.edu/sentiment/code.html)
produced an accuracy of 51.1% on the IMDB dataset and 59.4% on the Twitter data.

