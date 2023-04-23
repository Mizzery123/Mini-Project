# SC1015 Mini Project A124 Team 9 - Detecting Fake News
![image](https://user-images.githubusercontent.com/41039452/233805482-b8e6ebb2-7c03-4af3-900e-36abadd03517.png)

## About 
This is a mini-project for SC1015 which focuses on prediction of fake news. Please view the source code in order from : 
1. [Data Cleaning and Preparation](https://github.com/Mizzery123/Mini-Project/blob/main/Notebooks/Data%20Cleaning.ipynb)
2. [Exploratory Data Analysis & Visualization](https://github.com/Mizzery123/Mini-Project/blob/main/Notebooks/Exploratory%20Data%20Analysis%20%26%20Visualization.ipynb)
3. [Machine Learning](https://github.com/Mizzery123/Mini-Project/blob/main/Notebooks/Machine%20Learning.ipynb)

[Slides](https://github.com/Mizzery123/Mini-Project/blob/main/Slides/dsai%20slides%20team%209%20pdf%20updated.pdf) can be accessed here.
   
  
## Dataset Used
 [Original Dataset](https://www.kaggle.com/datasets/saurabhshahane/fake-news-classification) can be retrieved here from Kaggle.
 [Cleaned Dataset](https://github.com/Mizzery123/Mini-Project/tree/main/Dataset) after our Data Preparation stage can be obtained here.


## Team Members 
- @weihsuen Ling Wei Hsuen - Data Preparation 
- @pushparajanroshini Pushparajan Roshini - Exploratory Data Analysis [EDA]
- @Mizzery123 Lim Shao Jie - Machine Learning 

## Practical Motivation
Dire consequences of false and dis-information today, especially due to the increase in recent anti-asian hate crimes from Covid-19 due to spread of fake news

## Problem Formulation & Aim
How can we effectively differentiate between real and fake news using features of the article?
Which indicator and model is the best for prediction of fake news?

## Data Preparation
#### 1. Data Cleaning 
- Junk Values in Excel 
- Dropping NaN values, relabelling of columns 
- Changing improper data types 
#### 2. Removal of irrelevant values 
- Symbols, Stopwords from title and text 
#### 3. Created new columns 
- Title,text and stopword count
- Lemmatisation and Tokenisation 
- Sentiment Generation using polarity scores 
- Emotion Generation 
#### 4. Final clean-up and saving of cleaned dataset

## Exploratory Data Analysis with title and text data
#### 1. Initial Assumptions and data-driven insights from dataset and research 
- Fake news have longer titles, shorter text, carry heavier emotions, have fewer stopwords 
#### 2. Word Count Analysis 
- Number of fake news >> real news 
- Higher mean of fake news titles but lower mean of fake news text
#### 3. Corpus Analysis 
- Unigram and Bigram analysis 
#### 4. Stopword Count Analysis
- Fake and Real news contain similar distribution of stopwords
#### 5. Sentiment Analysis
- Fake news have more negative polarity
#### 6. Emotion Analysis
- Fake news text display heavier emotions
#### 7. Correlation
- All indicators do not have any strong linear relationship

## 8 Indicators Used 
- Title and Text word count 
- Title and Text stopword count
- Title and Text emotions
- Title and Text sentiment polarity

##  Models used in Machine Learning
1. Logistic Regression
2. Decision Tree
3. Random Forest
4. Support Vector Machine Classifier [SVM]
5. Ensemble : combination of all the 4 models

##  Results
| Outcome    | Model            | Accuracy  |
| ---------- | --------------------- | --------- |
| Best       | Logistic Regression   | 96.1  93.3|
| Inaccurate | SVM                   | 97.4  50.0|
| Worst      | Ensemble              | 70.1      |


## Conclusion and what we learnt 
- Our problem requires high accuracy on new unseen data hence insufficient/skewed data could have caused overfitting in SVM train and test data 
- It is possible to do correlation with categorical data once it has been converted to numerical data through Label Encoding
- New Machine Learning Models we implemented
- Other relevant predictors like source of news, sampling techniques and a variety of socio-cultural context datasets could have  improved prediction.

## References 
- [Research Findings](https://arxiv.org/pdf/1703.09398.pdf)
- [Research Findings 2](https://towardsdatascience.com/fake-news-detector-with-deep-learning-approach-part-i-eda-757f5c052)
- [Research Paper](https://dr.ntu.edu.sg/bitstream/10356/147544/2/FYP%20-%20Elbert%20Widjaja%20-%20Fake%20News%20Detection%20using%20Social%20Media%20Data.pdf) 
- [Cleaning and Preparation](https://www.dataquest.io/blog/how-to-clean-and-prepare-your-data-for-analysis/)
- [Sentiment Analysis](https://www.kirenz.com/post/2021-12-11-text-mining-and-sentiment-analysis-with-nltk-and-pandas-in-python/text-mining-and-sentiment-analysis-with-nltk-and-pandas-in-python/)

