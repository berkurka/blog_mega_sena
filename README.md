# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 3: 

### Overview

Creating a classification model to predict which subreddit a post belongs to.
Used Honda and Toyota subbreddit.

Work is devided in 3 noteboos:

1. DataScraping.ipynb
     Scraping data from sub reddit Api convert into a pandas data frame and creates csv files.
2. EDA.ipynb
     Describing data, generating histogram, scatter and correlation heatmap plots.
3. Feature_eng_and_Model.ipynb
     Creating dummies, engineering new features, scale data, spliting data in train and test data frames.
     Fitting data in model, scoring model, and ploting predictions and errors.
### Methods
 - Statistic data description using Pandas,Numpy,wordcloud, librarys in Python.
 - Text columns were transformed using PorterStemmer, LancasterStemmer and WordNetLemmatize from nltk library.
 - Words were tokenized using CountVectorize from sklearn library 
 - Data was slpit in 25% test and 75% train subsets. 
 - Multinomial Naive Bayes, Random Trees, Extra Trees and Bagging with Decision Tree models where used.
### Results
 - The Random Forest Cassifier had a 92% accuracy in train set and 77% accuracy in test and 76% cross validation after hyperparameter tuning.
 - Car names were the words with most impact in this model´s classification process.
### Softwares Used
- Jupyter notebook
- Python 3.6
- Powerpoint
### Datasets

#### Data source:

[Toyota subreddit](https://www.reddit.com/r/Toyota/)

[Honda subreddit](https://www.reddit.com/r/Honda/)

#### Features dictionary before tokenizing

|Feature|Type|Description|
|---|---|---|
|title|object|Subreddit title text.|
|selftext|object|Subreddit body text.|
|ups|int64|Number of ups in subreddit post.|
|num_comments|int64|Number of comments in subreddit post.|
|author|object|Subreddit post Author name.|
|label|int64|Predicted column, 1 if Honda.|
|clean_title|object|Title after removing english stop words, double space and special characters.|
|clean_selftext|object|Body after removing english stop words, double space and special characters.|
|clean_title_lemmat|object|Clean title column after using WordNetLemmatizer.|
|clean_title_lancast|object|Clean title column after using LancasterStemmer.|
|clean_title_port|object|Clean title column after using PorterStemmer.|
|clean_selftext_lemmat|object|Clean body column after using WordNetLemmatizer.|
|clean_selftext_lancast|object|Clean body column after using LancasterStemmer.|
|clean_selftext_port|object|Clean body column after using PorterStemmer.|