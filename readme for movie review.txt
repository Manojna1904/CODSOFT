Movie Rating Prediction with Python

This project builds a **Machine Learning model** to predict the IMDb rating of Indian movies based on their **features such as genre, director, actors, year, duration, and votes**.

It applies **data preprocessing, feature engineering, and ML modeling** using regression techniques.

Project Overview

The IMDb movie dataset contains details like:

Movie Name
Yearof release
Duration(in minutes)
Rating(target variable)
Genre
Director
Main Actors
Votes(number of votes on IMDb)

Steps Followed

1. Data Preprocessing

* Removed missing ratings.
* Extracted year from release date.
* Cleaned **duration** and **votes** into numeric format.
* Dropped missing values.

2. Feature Engineering

* **Genres** → One-hot encoded using `MultiLabelBinarizer`.
* **Director & Actors** → Encoded with `LabelEncoder` (top 50 retained, others set as *Other*).
* **Numerical features** → Scaled using `StandardScaler`.

3. Train-Test Split

* **X (features):** All except *Name, Genre, Rating*.
* **y (target):** Rating.
* Split into **80% training / 20% testing**.

4. Models Used

* **Linear Regression**
* **Random Forest Regressor**

5. Evaluation Metrics

* **MAE (Mean Absolute Error)**
* **RMSE (Root Mean Squared Error)**
* **R² Score (Coefficient of Determination)**

---

Model Performance

Example results (your results may vary):

| Model             | MAE  | RMSE | R²   |
| ----------------- | ---- | ---- | ---- |
| Linear Regression | 0.55 | 0.72 | 0.63 |
| Random Forest     | 0.34 | 0.49 | 0.82 |

Random Forest performs better** for this dataset.

---

How to Run

1. Clone the repository


2. Install dependencies

3. Run the script

Future Improvements

* Add **deep learning models** (Neural Networks).
* Include **textual features** like movie description/plot.
* Perform **hyperparameter tuning** for Random Forest.
* Deploy as a **Flask/Django web app** for user input.

## 📜 License

This project is open-source and available under the **MIT License**.

