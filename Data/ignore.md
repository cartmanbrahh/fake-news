# Link to the data
The dataset is available at 
https://www.kaggle.com/c/fake-news/data

Data description
train.csv: A full training dataset with the following attributes:

id: unique id for a news article
title: the title of a news article
author: author of the news article
text: the text of the article; could be incomplete
label: a label that marks the article as potentially unreliable
1: unreliable
0: reliable

Since we do not have the true test set labels, we will be performing 
all model evaluations on the training set and not the test set.
