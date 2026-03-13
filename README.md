# Medical_Insurance_Cost_Prediction_System
This is a ML-Based algorithm Model trained on more than 1300 rows of dataset
# 🏥 Medical Insurance Cost Prediction

A Machine Learning project that predicts **medical insurance charges** based on personal and lifestyle attributes such as age, BMI, smoking habits, and region.
The project explores data analysis, preprocessing, and multiple regression algorithms to identify the most accurate predictive model.

---

## 📌 Project Overview

Healthcare costs vary widely depending on several factors. This project uses **machine learning regression models** to estimate medical insurance charges for individuals based on demographic and health-related features.

The workflow includes:

* Data exploration
* Data visualization
* Feature encoding
* Model training
* Model comparison
* Prediction system

Dataset size: **1338 records**

---

## 📊 Dataset Features

The dataset contains the following attributes:

| Feature      | Description                                         |
| ------------ | --------------------------------------------------- |
| **age**      | Age of the primary beneficiary                      |
| **sex**      | Gender of the individual                            |
| **bmi**      | Body Mass Index                                     |
| **children** | Number of dependents covered                        |
| **smoker**   | Smoking status                                      |
| **region**   | Residential region in the US                        |
| **charges**  | Individual medical insurance cost (target variable) |

---

## 🔍 Exploratory Data Analysis

Several visualizations are used to understand the dataset:

* Age distribution
* BMI distribution
* Smoking status distribution
* Regional distribution
* Correlation heatmap
* Insurance charges distribution

Libraries used for visualization:

* **Matplotlib**
* **Seaborn**

---

## ⚙️ Data Preprocessing

Steps performed before training the models:

1. **Categorical Encoding**

   * One-hot encoding applied using `pd.get_dummies()`
   * Columns encoded:

     * sex
     * smoker
     * region

2. **Feature Selection**

```
X = dataset features
y = insurance charges
```

3. **Train-Test Split**

```
train_test_split(test_size = 0.23, random_state = 42)
```

---

## 🤖 Machine Learning Models Used

The project compares multiple regression algorithms:

| Model                           | Description                   |
| ------------------------------- | ----------------------------- |
| Linear Regression               | Basic regression model        |
| Ridge Regression                | Regularized linear regression |
| Support Vector Regression (SVR) | Kernel-based regression       |
| Decision Tree Regressor         | Tree-based learning           |
| Random Forest Regressor         | Ensemble of decision trees    |
| XGBoost Regressor               | Gradient boosting model       |

Each model is trained and evaluated using **RMSE (Root Mean Squared Error)**.

---

## 📈 Model Comparison

All models are evaluated on:

* Training RMSE
* Testing RMSE

A comparison graph is generated to visualize model performance.

This helps identify the **most accurate algorithm** for predicting insurance costs.

---

## 🔮 Prediction System

Two prediction approaches are implemented:

### 1️⃣ Dataset-based prediction

Users select a row from the test dataset:

```
Enter a number between 0 and 308
```

The model predicts the insurance charge for that record.

---

### 2️⃣ User Input Prediction

Users can manually enter values for:

* age
* bmi
* children
* smoking status
* region

The system converts inputs into the correct encoded format and produces a predicted insurance cost.

---

## 🛠️ Technologies Used

* **Python**
* **NumPy**
* **Pandas**
* **Matplotlib**
* **Seaborn**
* **Scikit-learn**
* **XGBoost**
* **Jupyter Notebook**

---

## 📂 Project Structure

```
Medical-Insurance-Prediction/
│
├── medical_insurance_prediction.ipynb
├── archive.zip (dataset)
├── README.md
```

---

## ▶️ How to Run

1. Clone the repository

```bash
git clone https://github.com/yourusername/medical-insurance-prediction.git
```

2. Navigate into the project

```bash
cd medical-insurance-prediction
```

3. Install required libraries

```bash
pip install numpy pandas matplotlib seaborn scikit-learn xgboost
```

4. Open the notebook

```bash
jupyter notebook
```

5. Run all cells to train models and make predictions.

---

## 🎯 Project Goals

* Understand how **health and lifestyle factors affect insurance costs**
* Compare multiple **machine learning regression models**
* Build a simple **predictive system**

---

## 📜 License

This project is open-source and available under the **MIT License**.

---
