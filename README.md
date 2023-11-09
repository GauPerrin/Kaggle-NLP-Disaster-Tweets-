# Kaggle-NLP-Disaster-Tweets-
Submissions to the NLP Kaggle Competition : "Natural Language Processing with Disaster Tweets"

**Approach**

1.	No Particular Preprocessing:
•	Initially, I started without any significant data preprocessing, except for dropping imprecise location and keyword information.
•	Achieved around 78% accuracy with a Ridge Classifier and a basic Count Vectorizer.
2.	Switch to TF-IDF:
•	Switched from a Count Vectorizer to a TF-IDF Vectorizer.
•	Achieved an improvement to approximately 80.5% accuracy. This is expected as TF-IDF often performs better for NLP tasks compared to simple counts.
3.	Model Exploration:
•	Tried different models like Logistic Regression and XGBoost (XGBClassifier) with grid search.
•	Observed that these models gave poorer results than the Ridge Classifier. This could be due to the specific parameters or features used in those models or overfitting.
4.	Text Preprocessing with Stop Words and Lemmatization:
•	Introduced text preprocessing techniques like removing stop words and lemmatization to clean the text data.
•	Initially, the combination of stop words and lemmatization resulted in a decrease in cross-validation score, indicating that this preprocessing may have removed useful information or introduced issues in the text data.
5.	Experimentation with Preprocessing:
•	Tried different combinations of text preprocessing:
•	First, stop words alone.
•	Then, lemmatization alone.
•	Only lemmatization resulted in a better cross-validation score, but the test score remained at 78.5%, which is similar to the initial score without preprocessing.


At that point I knew I would have hard times improving my model without going through a deep learning model.

**Improvement points**
-actively integrate the keywords and locations
-Try using a deeplearning model 
