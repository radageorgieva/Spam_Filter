# SPAM FILTER

This is part of a group assignment I completed during the Machine Learning module of my MSc studies. The underlying dataset consists of SMS data from the UCI Machine Learning Repository. The main goal of this assignment is to build a Naive Baye's Spam Filter.

## Installation 
### Downloading the Data
- Dowload the Spam Filter.ipybn notebook and open in virtual environment
- Download the data files from https://archive.ics.uci.edu/ml/machine-learning-databases/00228/

    
### Installing the requirements
- The python version is Python 3.8
- You're better off using virtual environment 
- Find all required packages and their corresponding version in the file requirements.txt

## Full Article
The provided Jupyter Notebook contains extensive comments on the data processing, model fitting and optimization and anlysis of the observed results.

## Conclusions of the project

Both the Bernoulli and the Multinomial models perform very well in terms of weighted accuracy. However, as we said in the beginning, we have an imbalanced dataset skewed towards "ham" text messages. Hence, it is important to look at sensitivity and specificity scores for the two classes. What we can conclude, is that while the two have similar weighted accuracy, MultinomialNB is better in predicting "ham" text messages, while Bernoulli is better at predicting "spam" messages. If the goal of the task is to filter out spam, we would probably be better off using the Bernoulli Naive Bayes. Overall, both models show very good results, generalization is not an issue and none of the scores showing performance of separate classes raise concerns unless we are looking for a classifier that has zero tolerance in spam.

A random classifer that labels emails as spam, ham emails randomly based on the historical fraction of ham/spam emails already recieved (86.6% ham and 13.4% spam) will overall accuracy = 1- ((0.1340.866)+(0.8660.134)) = 0.77 (based on Gini index idea), and hence it's evident that both of our classifiers performs better than this random classifier.

Based on all the above, one can say this is a good classifier.
