# Decision Trees
This project implements a machine learning pipeline using regression and classification decision trees to predict passenger survival in the Titanic - Machine Learning from Disaster Competition.
## Dataset
You can download the dataset and participate in the competition using the following link: [Titanic - Machine Learning from Disaster](https://www.kaggle.com/competitions/titanic/overview). Two datasets `train.csv` and `test.csv` are used for training and testing the model.
## Preprocessing
The same preprocessing steps are applied to both train and test data:
- Extract titles from the `Name` column and group rare titles into the category `Rare`
- Apply one-hot encoding to categorical features.
- Remove unhelpful columns like `Ticket` and `PassengerId`
- Train a **Regression Decision Tree** to fill out the missing values in the column `Age`
## Model
Two models are used in this project: 
- A **Regression Decision Tree** to predict and fill out the missing `Age` values.
- A **Classification Decision Tree** as the final and core model to predict passenger survival.
## How to run
Download the Kaggle Titanic Dataset [Titanic - Machine Learning from Disaster](https://www.kaggle.com/competitions/titanic/overview) and place `train.csv` and `test.csv` in the same folder as the `decision_tree.ipynb`. Run all the cells inside the notebook in order.
## Results
By running the last cell in the notebook a `submission.csv` file is produced with **PassengerId** and **Survived** values. After submitting the prediction file to Kaggle a result of 0.77033 is achieved. 