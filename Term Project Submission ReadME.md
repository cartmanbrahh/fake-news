##############################################################
# BIG DATA | TERM PROJECT | 
# Authors : Ankita BHATTACHARYA, Abdourahmane DIALLO, 
#           Sungyun HWANG, Amaratou MAHAMADOU
# Date created : 19.04.2021
##############################################################


This is a ReadME file containing an exhaustive list of contents,
notebooks and instructions to execute the code provided. 

1. Dataset and data description
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

2. Instructions to run the notebooks
The data train.csv and test.csv must be saved in the same directory as the 
notebooks. For notebooks on databricks, you will have to upload the two files 
train.csv and test.csv onto Databricks. 
For the last notebook on Google Colab, you will have to upload
the file train.csv (and test.csv if you please) onto "session storage" as 
mounting to drive was not working. 

3. Notebooks
Notebook 03 : Exploratory Analysis

I.Loading the pre-requisites
II. Loading the data
III. Exploratory analysis
	III.A. NA values
	III.B. Distribution of the target counts
IV.Relationship between features extracted and the target
V.Preprocessing data
VI. Word clouds


Notebook 04 : Aggregations using Spark Dataframes

I. Loading the data and prerequisites
II. Exploratory analysis
	II.A. Univariate Analysis
	II.B. Bivariate Analysis

Notebook 05 : MLlib, training ML models for fake news prediction

I. Loading the data and prerequisites
II. Some preliminary cleaning !
III. Text Preprocessing
IV. Training the classification models
	IV.A. Logistic Regression
		IV.A.1. Obtaining errors and other evaluation metrics on our model
		IV.A.2. Tuning hyper parameters
	IV.B. Random Forest Classifier


Notebook 06 : Pipelines 

I. Loading the data and prerequisites
II. Some preliminary cleaning !
III. Defining the pipeline
	A. Feature extraction
	B. ML model
		1. Logistic Regression
			1.a. Hyper parameter tuning
		2. Naive Bayes Regression
		
		
Notebook 07 : Deep Learning Model : RNN (using LSTM)
Fake News Detection | Tensorflow | Google Colab
I. Loading the prerequisites & data
II. Some preliminary cleaning !
	II.A. Dealing with NAs
III. Text Mining : Preprocessing
	III.A. Obtaining the vocabulary
	III.B. Word Embeddings
	III.C. Padding
IV. Creating the RNN model
	IV.A. Running the Model
V. Checking for overfitting !
	V.A. Correcting for overfitting
	V.B. Better results !
	
	
For bugs or issues contact  ankita.bhattacharya@ut-capitole.fr


VI. Hyper-parameter tuning : Using Keras tuner
Learning rate
Units of the dense layer
