# Restaurant_Reviews

This dataset has been downloaded from Kaggle as ‘.tsv’ file.

It consists of two different features one is reviews submitted by users and another is a binary classifiers with 0’s & 1’s where *0 means negative* and *1 means positive reviews*.

As the first column is filled with text data, I’ve separated it for further text cleaning and pre-processing. For this **‘Natural Language Tool Kit (nltk)’** & **‘regular expression (re)’** libraries being used.
In this step all the characters other than capital A to Z and small a to z has been dropped then converting all the capital letters into small ones. After that each of the sentences has been splitted into words to check whether they belong to the stop-words defined by thee nltk library.
After cleaning a Bag-Of-Words model has been created & the text data has been fed into it. 
Then for this classification problem two of the most powerful Machine Learning algorithms has been used. 1. Logistic Regression & 2. Multinomial Naïve Bayes Classifier

## Bag Of Words:
A bag-of-words model is a way of extracting features from text for use in modelling, such as with machine learning algorithms.The approach is very simple and flexible, and can be used in a myriad of ways for extracting features from documents.

A bag-of-words is a representation of text that describes the occurrence of words within a document. It involves two things:
1.	A vocabulary of known words.
2.	A measure of the presence of known words.
It is called a “bag” of words, because any information about the order or structure of words in the document is discarded. The model is only concerned with whether known words occur in the document, not where in the document.

Finally, creating the respective **Confusion Matrices** to check the True Positive, True Negative, False Positive & False Negative. And calculating the respective accuracy scores.
At the end 10-Fold Cross Validation has been used to check whether the accuracy came as a sheer good luck.
