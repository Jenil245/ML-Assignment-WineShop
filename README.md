# ML-Assignment-Winery

# About DATA
The dataset which is provided represents WineShop online purchase history.

Dataset contains 82657 entries and 12 columns. Two columns contains numerical values. Two columns contains text data. Rest 8 columns are categorical. We have to predict variety of grapes that has been used in making wine.

<b>Target variable has 17 different categories.</b>

# Data Preprocessing
Dataset has too many null values. Categorical columns contains some category which has really low frequency.
I kept only top ten frequency for each column. I removed null values and low frequency values with others.

# Feature Selection & Engineering
I performed chi2 test to check whether target variable and feature column are dependent or independent. I didn't get any strong evidence that they are independent so I kept most of the features. Then I encoded categorical columns with one hot encoding. I performed count vectorizer on text data.

# Model Development
I explored two models:

1) Bernoulli Naive Bayes :
I decided this model because of all the features were binary either 0 or 1. 

And I got <b>63.5% accuracy</b> which is really great because target variable has <b>17 different categories.</b> Model was trained in about two minutes.

2) CatBoost :
These is a very powerful model which follows ensemble boosting approach and highly optimized for categorical data. 

I got <b>66.7% accuracy</b>. Model took about one hour to train.
