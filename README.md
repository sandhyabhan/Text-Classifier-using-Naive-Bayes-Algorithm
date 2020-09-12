# Text-Classifier-using-Naive-Bayes-Algorithm
# Aim
Train the model from the imported data and based on the model classify the test data into 4 different categories by implementing Naive Bayes algorithm and computing the accuracy score.

Data imported from sklearn.datasets.fetch_20newsgroups
https://www.kaggle.com/crawford/20-newsgroups

# Methodology
Naive Bayes is a classification technique based on Bayes’ Theorem with an assumption of independence among predictors.A Naive Bayes classifier assumes that the presence of a particular feature in a class is unrelated to the presence of any other feature.


Formula = P(A|B) = P(B|A) * P(A) / P(B).


Here , P(A)= probability of class/category.


P(B)=Probability of testing document


P(B|A)= Probability of the document given that it belongs to the particular class.

In this model,we first count the frequency of each word in the text by using CountVectorizer tool provided by the scikit-learn library in Python.Next we have to find the Term Frequency and Inverse Document Frequency of each word.It adds a particular weight to a word based on its importance.It is achieved using TfidfTransformer from sklearn library.
Next,we used MultinomialNB which is one of the part of Naive Bayes classifier. Using this we can directly train our model with the matrix obtained from tdidf transformer.

# Result
Got an accuracy of 83%

# Contributor
Sandhya Bhan(sandhyabhan22@gmail.com)




