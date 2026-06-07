# Classification Models

A collection of machine learning classification projects developed using Python and Scikit-Learn. This repository explores real-world healthcare and business datasets, demonstrating the complete machine learning workflow from data preprocessing and feature engineering to model training, evaluation, and performance comparison.

The projects focus on binary classification problems in healthcare diagnostics and customer behavior prediction.

---

## Projects Included

### 1. Cardiovascular Disease Prediction

Predicts the likelihood of heart disease based on lifestyle, demographic, and health-related factors.

#### Features Used

* General Health
* Checkup Frequency
* Exercise Habits
* Skin Cancer History
* Other Cancer History
* Depression
* Diabetes
* Arthritis
* Sex
* Age Category
* Height
* Weight
* BMI
* Smoking History
* Alcohol Consumption
* Fruit Consumption
* Green Vegetable Consumption
* Fried Potato Consumption

#### Target Variable

* Heart Disease (Yes/No)

#### Objective

Develop a machine learning model capable of identifying individuals at risk of cardiovascular disease using health and lifestyle indicators.

---

### 2. Bank Marketing Response Prediction

Predicts whether a customer will subscribe to a bank's term deposit based on demographic information and previous marketing campaign interactions.

#### Features Used

* Age
* Job
* Marital Status
* Education
* Credit Default Status
* Account Balance
* Housing Loan Status
* Personal Loan Status
* Contact Type
* Contact Day
* Contact Month
* Call Duration
* Campaign Contacts
* Previous Contact Days
* Previous Contacts
* Previous Campaign Outcome

#### Target Variable

* Term Deposit Subscription (Yes/No)

#### Models Evaluated

* Logistic Regression
* Support Vector Machine (RBF Kernel)
* Random Forest Classifier
* XGBoost Classifier

#### Evaluation

Models were evaluated using:

* Confusion Matrix
* K-Fold Cross Validation
* Mean Accuracy
* Standard Deviation

#### Results

| Model                  | Cross Validation Accuracy |
| ---------------------- | ------------------------- |
| Logistic Regression    | 89.79%                    |
| Support Vector Machine | 89.82%                    |
| XGBoost                | 89.38%                    |
| Random Forest          | 90.04%                    |

Random Forest achieved the highest average cross-validation accuracy on the dataset.

---

### 3. Cervical Cancer Prediction

A machine learning model developed to predict cervical cancer risk using patient health records and screening test results.

#### Data Preprocessing

The dataset contained missing values which were handled through:

* Removal of highly incomplete records
* Mean-value imputation for numerical variables
* Random binary imputation for categorical indicators
* Feature cleaning and preparation

#### Target Construction

The original dataset contained multiple diagnostic outcomes:

* Dx
* Hinselmann
* Schiller
* Citology
* Biopsy

A new target variable was created using the statistical mode of the diagnostic test outcomes to provide a unified classification target.

#### Objective

Predict cervical cancer diagnosis from patient screening data and clinical history.

---

## Machine Learning Workflow

The projects follow a standard machine learning pipeline:

1. Data Collection
2. Data Cleaning
3. Missing Value Handling
4. Feature Engineering
5. Feature Encoding
6. Feature Scaling
7. Train-Test Split
8. Model Training
9. Cross Validation
10. Performance Evaluation

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-Learn
* XGBoost
* Jupyter Notebook

---

## Repository Structure

```text
classification-models/
│
├── CVD.ipynb
├── CVD_cleaned.csv
│
├── bank_dataset.ipynb
├── bank.csv
│
├── cervical_canc.ipynb
├── cervical-cancer_csv.csv
│
└── README.md
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/classification-models.git
cd classification-models
```

Install dependencies:

```bash
pip install pandas numpy matplotlib scikit-learn xgboost jupyter
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

---

## Key Concepts Demonstrated

* Binary Classification
* Data Preprocessing
* Missing Value Imputation
* Feature Engineering
* Ordinal Encoding
* Label Encoding
* Feature Scaling
* Logistic Regression
* Support Vector Machines
* Random Forest
* XGBoost
* Cross Validation
* Model Evaluation

---

## Future Improvements

* Hyperparameter Optimization
* Ensemble Learning Techniques
* Deep Learning Models
* Model Explainability with SHAP
* Deployment using Flask or FastAPI
* Interactive Prediction Dashboard

---

## Author

**Damilola Ayinde (Gon-Frecces)**

Python Developer | Machine Learning Engineer 

Passionate about applying machine learning and data-driven solutions to healthcare, finance, and real-world engineering challenges.


