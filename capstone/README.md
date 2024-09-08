The notebook 

   https://

  has the NLP classifier model evaluation for 'Covid-19 Fake or Fact news' analysis
  Markdowns with 'Findings:" in the notebook summarizes key points.


Business Definition:

  Covid-19 misinformation from social media has caused undue burden on humanity. 
The project will evaluate NLP classifier models and identify the best candidate to use in emergencies, that can help classify messages as facts or fake.

Data Analysis:

  : Dataset balanced or not
  : Histogram of sentence length, word length
  : 3 ngram plot to identify influential words
  : identify stop words influence
  : plot wordcloud

Data Preprocessing:

  Remove duplicates, drop null attribute samples
  Remove punctuations, numbers, hashtags, http urls, stopwords


Modeling:
  
  Total of 6 models evaluated by GridSearch
      Linear Regression, Decision Tree, MultiNomialNB -> Count Vectorizer, TDIDF processing

  
Evaulation:
   
  Best test accuracy and minimal false positives    
 
  
Conclusion:

   - Linear Regression with Count Vectorizer text processing technique produced the best model with accuracy of 92%
   - Looking at confusion matrix LR classified 100 fake messages as facts, while MultinomialNB classifed 59 fake messages as true.
   - Though MultiNomialNB had relatively lower accuracy, it has less false negatives,making it the chosen model.
   -  DecisionTree model had the least accuracy.
    
Next steps
 - Look into cleaning the messages further to remove irrelevant or inconsequential words
 - Looking into other word processing techniques (stemming, word2vec) 
 - Fine tune the model hyperparameters for Linear Regression and MultinomialNB, perform GridSearch to improve model accuracy and reduce false negatives.
 - Add additional NLP classifier models 
