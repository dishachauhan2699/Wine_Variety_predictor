 Wine_Variety_predictor

## TASKS
 - Building a predictive model for predicting the wine “variety” (MODELS_WINE.IPYNB)
 - 5 actionable Insights from the Data (EDA_NON_TEXTUAL.IPYNB)
 - Leverage the “reviews” data and draw actionable insights from it. (TEXTUAL_DATA_ANALYSIS.ipynb)

## FOLDERS
 - Notebooks(contains 2 Analysis notebooks with graphs and 1 Model based Notebook used for Creating classifiers)
 - Models (pkl files of model[RFC was around 2.9Gbs wasn't uploaded])
 - OUPUT (contains 3 csv files)
    - train and valid( contains all features and actual and predcited columns)
    - test ( contains all features and predcited column)
 ## SUMMARY

 - DATA CLEANING(Removing duplicates, Imputing missing values, Removing columns with high Nans)
 - CONTINUOUS AND CATEGORY WISE COLUMNS SUMMARIZATION(Provide data Insight)
 - ONE HOT ENCODING(Countries)
 - TEXT CLEANING(Case change, Removing stop words, Stemming, Lemmatization)
 - TEXT VECTORIZATION
 - CREATING SPARSE MATRIX OF REVIEW VECTORS, COUNTRIES, PRICE, POINT
 - HYPER PARAMETER TUNING OF COLUMNS

 ## SPLITTING DATA
 - The training data has been split into two parts, train(90%) and validataion(10%), as the Classifiers used are tree based they show exemplary accuracy on trained data, so validation helps us in knowing how the model is performing on unforseen data
 
 ## FEATURES 
 - country (ENCODED)
 - review_description (PROCESSED AND VECTORIZED)
 - points (NOT SCALED AS TREE BASED MODELS DON'T NEED SCALING)
 - price (NOT SCALED AS TREE BASED MODELS DON'T NEED SCALING)

 ## PREDICTED
 - variety (Label encoded)
 ## MODELS
 - XGBClassifier
 - LGBMC Classifier(Works well with dataset with more than 10k Tuples)
 - Random Forest Classifier

 ## ACCURACY

|Accuracy| Trainset | Validset |
|---------|----------| --------|
| XGB     | 98.7 %   |   73 %  |
| LGBMC   | 99.1%    |   75 %  |
| RFC     | 98%      |   68.9 %|


 

