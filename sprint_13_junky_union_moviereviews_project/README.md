## SentimentAnalysis


The Film Junky Union, a new edgy community for classic movie enthusiasts, is developing a system for filtering and categorizing movie reviews. The goal is to train a model to automatically detect negative reviews. I'll be using a dataset of IMBD movie reviews with polarity labelling to build a model for classifying positive and negative reviews. The required F1 score for this project is at least 0.85.


## **Project Insight**

Following the completion of a further experiment involving three distinct models, the summarized F1 scores are as follows:

1. Model 2 - Comprising NLTK, TF-IDF, and Logistic Regression, this model yielded an F1 score of 0.92 (train) and 0.88 (test).
2. Model 3 - Integrating spaCy, TF-IDF, and Logistic Regression, this model achieved an F1 score of 0.92 (train) and 0.88 (test).
3. Model 4 - A blend of spaCy, TF-IDF, and LightGBM, this model recorded an F1 score of 0.88 (train) and 0.84 (test).

After analyzing our dataset we observed an overall increase in number of movies watched per year, which peaked at 2006. After 2006, there was a sharp decline. Generally, fewer movies had more reviews. Also, there were more negative reviews per year than positive reviews. We trained models to predict whether a review would be positive or negative. The model with the best F1 score was the Logistic Regression model which used NLTK processing and the TF-IDF Vectorizer (F1 score of 0.88).

When each of the models were tested on the reviews, the LGBM model performed best. It got only one probability wrong, and it is not as extreme as the other models.

We did not train a BERT model because we didn't have enough processing power.
