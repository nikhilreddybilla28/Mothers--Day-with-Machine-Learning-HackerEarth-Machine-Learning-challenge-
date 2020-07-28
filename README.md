# Mothers--Day-with-Machine-Learning

![Dataset](https://img.shields.io/badge/Dataset-HackerEarth-blue.svg) ![Python 3.6](https://img.shields.io/badge/Python-3.6-brightgreen.svg) ![NLTK](https://img.shields.io/badge/Library-LightGBM_Xgboost-orange.svg)

## build a sophisticated sentiment analysis-based NLP model that can classify sentiments of tweets into positive, negative, and neutral.

## Dataset:
The dataset consists of various parameters such as text and language of a tweet, the number of times it was retweeted, and the Twitter handle of the author.

## DEPENDENCIES:	

jupyter notebook : 6.0.3

numpy - 1.15.4   

pandas - 1.0.3   

matplotlib - 3.1.3  	

seaborn- 0.10.1  

sci-kit learn(sklearn) - 0.20.1    	

keras(keras.preprocessing) 2.3.1         

re            

nltk    	

pickle	

*Classifier :  
			
			LightGBM  v-2.3.1
			
			XgBoost v-1.1.1

# APPROACH:

## 1)EDA(EDA):
Origial data is analysed, column wise and missing values and noise are corrected , then the data is analysed again.
The text is cleaned by removing mentions , instagram tags and twitter tags .
The tidy test is then made into corpus using nltk , then its made into embedding vectors.
Original_author is then made into dummies(onehot encoded)and along with number of retweets its is concatenated with embedding data.
This is made into dataframe and downloaded as csv
the same process is done for test data and downloaded as csv
the label data is also downloaded as csv 


## 2)Modelling,Training, Evaluation &Prediction(LGBM2):
The downloaded csv files from eda are loaded using pandas
train data is split into train and validation  
and using lightgbm classifier , model is trained (cv is internally used on train data)
model is validated with validation data and confusion matrix is observed,
then the model is used to predict labels on test data.
the predicted test labels is made as a dataframe and analysed and downloaded as csv file

2)Modelling,Training, Evaluation &Prediction(LGBM2):
The downloaded csv files from eda are loaded using pandas								
train data is split into train and validation  and using lightgbm classifier , model is trained (cv is internally used on train data)						
model is validated with validation data and confusion matrix is observed,then the model is used to predict labels on test data.
predicted test labels is  then made as a dataframe and analysed and downloaded as csv file.


PS:There are some packages imported but not used please ignore them.
