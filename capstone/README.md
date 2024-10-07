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
  
  Total of 8 models evaluated by GridSearch
      Linear Regression, Decision Tree, MultiNomialNB, SVM -> Count Vectorizer, TDIDF processing

  
Evaulation:
   
  Best test accuracy and minimal false positives (mis-classification rate)   
 
  
Conclusion:

   - Linear Regression with Count Vectorizer text processing technique produced the best model with accuracy of 92%
   - Looking at confusion matrix LR classified 100 fake messages as facts, while MultinomialNB classifed 59 fake messages as true.
   - Though MultiNomialNB had relatively lower accuracy, it has less false negatives, making it the chosen model.
   -  DecisionTree model had the least accuracy and longest execution time.
    

Business (Non Technical) Report

    The society has witnessed the evidence of Covid-19 misinformation, from readily accessible and available outlets: internet, social media and news outlets.
    The misinformation spread has resulted in vaccine avoidance, mask refusal and FDA unapproved self medications by individuals and society as a whole.
    The massive scale of misinformation spread cannot be controlled or monitored proactively by scarce manual resources (fact checking).
    So we propose Artificial Intelligence (AI) infused systems to classify misinformation as the first level of defense.
    The figure below illustrates such deployment scenario, in real world to control misinformation, increase awareness and reduce burden to individual and public health.













    Citizen's ability to fact check medical news can be provided by low barriers of entry: mobile applications, web browser plugins, fact checking sites and automated social media content moderation.  Users have multiple options to proactively check news on a individual basis (input to an app) or collectively ( viral new checking). Social media and news outlets can deploy and use the AI model as first line of defense augumenting their content moderation team, to weed out fake news at scale and then have human in the loop to confirm or label its findings.

    By leveraging Artifical Intelligence, scare human resources can be freed and redirected to assist medical emergencies during disease outbreak.
    Dissemenating real news to citizens will not only control the spread of the disease but also reduce the burden on Governments by improving trust with the public.
    Having clear, transparent, scientifically backed medical information can also improve development of public health policies and play a role in preventing health emergencies. 
    
    We sincerely hope, that AI infused systems will play a proactive role in the future, not only as readiness for moderating and dissemenating science backed medical news, but also influence public health policies.
