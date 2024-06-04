# Disaster Tweets Classification
This project aims to classify tweets as related to real disasters or not. The dataset used is from a Kaggle competition, where the goal is to predict which tweets are about real disasters and which ones are not.
## Introduction
Classifying tweets as real disasters or not can help in crisis management and information dissemination during emergencies. This project utilizes Natural Language Processing (NLP) techniques and machine learning algorithms to perform this classification.
## Dataset
The dataset used in this project is from the Kaggle competition. It contains the following files:

* train.csv: The training set
* test.csv: The test set

The dataset includes the following columns:

* `id`: Unique identifier for the tweet
* `text`: The tweet text
* `location`: (Optional) Location where the tweet was sent from
* `keyword`: (Optional) A keyword from the tweet
* `target`: The target variable, 1 if the tweet is about a real disaster, 0 otherwise
## Model Training
The following models were trained and evaluated:

* Logistic Regression
* Random Forest
* Gradient Boosting
* AdaBoost
* Support Vector Machine (SVM)
Hyperparameter tuning was performed using GridSearchCV.
## Evaluation
The models were evaluated using the following metrics:

* Accuracy
* Precision
* Recall
* F1 Score
* ROC AUC

## Results
The Support Vector Machine (SVM) classifier achieved the best performance:

* Accuracy: 0.80
* Confusion Matrix:
  ```
  [[775  99]
  [205 444]]
  ```
* Classification Report:
```
              precision    recall  f1-score   support

           0       0.79      0.89      0.84       874
           1       0.82      0.68      0.74       649
    accuracy                           0.80      1523 
   macro avg       0.80      0.79      0.79      1523  
weighted avg       0.80      0.80      0.80      1523
```


## Conclusion
This project demonstrates the use of various machine learning models for classifying tweets as real disasters or not. The SVM model showed the best performance in terms of accuracy and other evaluation metrics.
## Contributing
Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.
