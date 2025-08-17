Titanic Survival Prediction Overview

This project predicts whether a passenger survived the Titanic disaster using Logistic Regression implemented from scratch (NumPy only).

Dataset:

train.csv → Training data (includes survival labels).
test.csv → Test data (predict survival for these passengers).
Target column → Survived (0 = Did not survive, 1 = Survived).

Steps:

Data Cleaning:

Filled missing values in Age, Fare, and Embarked.
Dropped unnecessary columns (Name, Ticket, Cabin).
Converted categorical features (Sex, Embarked) into numbers.

Feature Scaling:

Normalized features using mean and standard deviation.
Added a bias column for Logistic Regression.

Model (Logistic Regression from Scratch):

Implemented the sigmoid function.
Used gradient descent to optimize parameters.
Trained the model on Titanic training data.

Prediction & Output:

Printed training accuracy.
Predicted survival on test.csv.
Saved results to submission.csv.

Tools Used:

Python
NumPy
Pandas

How to Run :

Place train.csv and test.csv in the project folder.

Run the script:

python titanic_prediction.py
Check the generated file: submission.csv

Output:

Training Accuracy: ~75–80% (may vary).
Final file → submission.csv with:
PassengerId
Survived

DATA SET LINK : https://www.kaggle.com/datasets/yasserh/titanic-dataset
