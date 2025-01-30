# Anomaly Detection Project
Classify whether a user is anomalous or normal using supervised and unsupervised models.
This is best viewed in google colab <a href="https://drive.google.com/drive/folders/19JOW3OeHC3QpidOxh4jC5u7v5HfRcl_L?usp=sharing" target="_blank">here</a> as all the visualisations and outputs are preserved in the interactive python notebook.

## ROC AUC Curve
![roc-auc](https://github.com/user-attachments/assets/1d07a97c-190d-40b3-bd78-aadca07b7bf2)


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

# Improvements
- Feature engineering
    - IQR of user's ratings
    - no. of items rated/not rated
    - no. of items rated neutral
    - fsti: The ratio between the number of items rated by the user and the total number of items in the recommender system.
    - fsmaxrti: The ratio between the number of items rated by the user with maximum score and the total number of items in the recommender system.
    - fsminrti: The ratio between the number of items rated by the user with minimum score and the total number of items in the recommender system.
    - fspi: The ratio between the number of popular items rated by the user and the total number of popular items, K, in the recommender system.
    - fspii: The ratio between the number of popular items rated by the user and the total number of items rated by the user.
- Models
    - Catboost
    - SVM
- Dealing with data imbalance
    - mixup approach data augmentation for DNN
    - SMOTE
    - class weights
