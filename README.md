# SC1015 Mini Project A124 Team 9 - Detecting Fake News
![image](https://user-images.githubusercontent.com/41039452/233805482-b8e6ebb2-7c03-4af3-900e-36abadd03517.png)



## Team Members 


## Practical Motivation
Ill effects of false and dis-information today, especially the recent anti-asian hate crimes from covid-19. 

## Problem Formulation
Differentiating between real and fake news using feature's of the article

## Data Preparation
#### 1. Cleaning of junk values in excel:
Examples of junk values are text in index columns
#### 2. Importing dataset:
Requires “encoding='ISO-8859-1'” to read csv
#### 3. Data Cleaning
Replacing column labels for better visualisation

Dropping rows with NaN values according to the 5% missing data rule

Changing dtypes
#### 4. Creating new columns 
#### 5. Removal of symbols from title and text by creating function
#### 6. Removal and counting of stopwords from title and text by creating function
Using nltk.corpus
#### 7. Lemmatisation and Tokenisation by creating function
Lemmatisation is the process of converting words to their root form
#### 8. Sentiment Generation - polarity by creating function
Using SentimentIntensityAnalyzer from nltk.sentiment.vader

Limited words to 30 for time considerations
#### 9. Emotion Generation by creating function
using python package text2emotion
#### 10. Final clean-up and saving of dataset



##  Models used
1. Logistic Regression
2. Decision Tree
3. Random Forest
4. Support Vector Machine Classifier
5. Ensemble

## Outcome
#### - 



## Dataset Used
#### https://www.kaggle.com/datasets/saurabhshahane/fake-news-classification

## References 


