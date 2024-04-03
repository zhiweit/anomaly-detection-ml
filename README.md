# Anomaly Detection Project
This is a machine learning project done to classify whether a user is anomalous or normal. 
This is best viewed in google colab <a href="https://drive.google.com/drive/folders/19JOW3OeHC3QpidOxh4jC5u7v5HfRcl_L?usp=sharing" target="_blank">here</a> as all the visualisations and outputs are preserved in the ipython notebook.

# Problem and Task
Given users' ratings (0-5) of items, identify whether a user is anomalous or not. The data given consists of 3 columns (user, item, rating) e.g. user 3 gives rating 5 for item 1.
The dataset is imbalanced as there are few anomalous users compared to normal ones. There are three phases of the project across three weeks where data with labels for previous phase are released as well along with new test set. We are recommended to try at least two supervised methods and one unsupervised method, and be ranked the best team in terms of performance (ROC AUC) to score well for this project.

# Approach
## Supervised Methods
- Logistic Regression
- KNN Classifier
- Random Forest
- XGBoost Classifier
- Neural Networks

## Unsupervised Methods
- Autoencoder
- Isolation Forest
- Local Outlier Factor (LOF)

# Final Approach - Ensemble Approach to Classify Evaluation/Batch Test Data
Classify a user as normal or anomalous according to majority classification from chosen models, with equal vote weightage for each model.
Eventually used all of my supervised models (Logistic Regression, KNN Classifier, Random Forest, XGBoost Classifier, Neural Networks) and none of the unsupervised methods as the F1 score and AUC performance for the unsupervised methods were very sub-optimal, probably because the features from feature engineering with were not very good in distinguishing anomalous users from normal ones.
