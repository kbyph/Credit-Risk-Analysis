# Credit Risk Analysis - Machine Learning

## Overview of Project
- Utilize Machine Learning statistical algorithms to make predictions based on the provided data patterns
- Resample the data using the `RandomOverSampler`, `SMOTE`, `ClusterCentroids`, `SMOTEENN`, `BalancedRandomForestClassifier`, and `EasyEnsembleClassifier` algorithms.

## Resources
- Software
  - Python
  - Anaconda Prompt(mlenv)
  - Jupyter Notebook
- Data Source
  - LoanStats_2019Q1.csv
  
## Results

### RandomOverSampler

The balanced accuracy score is 64%.
- ![image](https://user-images.githubusercontent.com/102638461/184522556-65d304ad-08f9-42a5-94a7-74584874eedf.png)

The "High Risk" precision rate was only 1% with the recall at 66% giving this model an F1 score of 2%.
"Low Risk" had a precision rate of 100% and recall at 62%.
- ![image](https://user-images.githubusercontent.com/102638461/184522567-2b0d88a2-bd13-40ed-b408-8d231b1e3c2f.png)
- ![image](https://user-images.githubusercontent.com/102638461/184522570-bd38dc8c-fd55-408a-8117-396078e658d3.png)


### SMOTE
The balanced accuracy score is 65%.
- ![image](https://user-images.githubusercontent.com/102638461/184522588-72b9238f-da8a-404a-83c4-ca758d0d40af.png)

The "High Risk" precision rate was only 1% with the recall at 61% giving this model an F1 score of 2%.
"Low Risk" had a precision rate of 100% and recall at 69%.
- ![image](https://user-images.githubusercontent.com/102638461/184522607-1a465538-4222-4896-b96d-7d64731e7f1c.png)
- ![image](https://user-images.githubusercontent.com/102638461/184522620-f7a1b858-957d-4f85-8a22-7b2e40dc48ba.png)


### ClusterCentroids
The balanced accuracy score is 54%.
- ![image](https://user-images.githubusercontent.com/102638461/184522628-dd81ca24-5bcf-4687-bed9-ec6fbabc695b.png)

The "High Risk" precision rate was only 1% with the recall at 69% giving this model an F1 score of 1%.
"Low Risk" had a precision rate of 100% and recall at 40%.
- ![image](https://user-images.githubusercontent.com/102638461/184522673-303497d6-ca8b-49f9-afac-173ec43ae2cd.png)
- ![image](https://user-images.githubusercontent.com/102638461/184522689-5439edb2-6604-4adb-bd1e-d4dacbe9609b.png)


### SMOTEENN
The balanced accuracy score is 64%.
- ![image](https://user-images.githubusercontent.com/102638461/184522698-316572c0-259f-469e-83aa-f2ae60daa2a8.png)

The "High Risk" precision rate was only 1% with the recall at 72% giving this model an F1 score of 2%.
"Low Risk" had a precision rate of 100% and recall at 57%.
- ![image](https://user-images.githubusercontent.com/102638461/184522711-c89e5199-3bb5-4521-9574-3a315c2c0087.png)
- ![image](https://user-images.githubusercontent.com/102638461/184522726-c5fe898b-e3f8-453b-bad9-00f48cbe949d.png)


### BalancedRandomForestClassifier
The balanced accuracy score is about 79%.
- ![image](https://user-images.githubusercontent.com/102638461/184522778-b365cf91-706f-47ef-b129-0639327cb28f.png)

The "High Risk" precision rate was only 3% with the recall at 70% giving this model an F1 score of 6%.
"Low Risk" had a precision rate of 100% and recall at 87%.
- ![image](https://user-images.githubusercontent.com/102638461/184522784-c6b7f133-f673-4caf-b469-a6bc13d47a61.png)
- ![image](https://user-images.githubusercontent.com/102638461/184522788-f611a034-028f-45a7-9609-00cefa59d54f.png)


### EasyEnsembleClassifier
The balanced accuracy score is 93%.
- ![image](https://user-images.githubusercontent.com/102638461/184522804-477ab628-46aa-4d4e-b344-44c950e68688.png)

The "High Risk" precision rate was only 9% with the recall at 92% giving this model an F1 score of 16%.
"Low Risk" had a precision rate of 100% and recall at 94%.
- ![image](https://user-images.githubusercontent.com/102638461/184522808-f24a63d9-582f-4c66-a750-978d7bdab022.png)
- ![image](https://user-images.githubusercontent.com/102638461/184522816-a278a4ce-3769-4457-8c05-04607efa9d91.png)


## Summary
According to the dataset, the Easy Ensemble AdaBoost Classifier yielded the best results with the highest scores and rates amongst all other models.

**Ranking all models based on "High Risk" results:**
- `EasyEnsembleClassifer`: 93% accuracy, 9% precision, 92% recall, and 16% F1 Score
- `BalancedRandomForestClassifer`: 79% accuracy, 3% precision, 70% recall and 6% F1 Score
- `SMOTE`: 65% accuracy, 1% precision, 61% recall and 2% F1 Score
- `SMOTEENN`: 64% accuracy, 1% precision, 72% recall and 2% F1 Score
- `RandomOverSampler`: 64% accuracy, 1% precision, 66% recall and 2% F1 Score
- `ClusterCentroids`: 54% accuracy, 1% precision, 69% recall and 1% F1 Score
