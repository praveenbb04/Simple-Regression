# Salary Prediction using Simple Linear Regression

A machine learning project demonstrating end-to-end implementation of Simple Linear Regression to predict salary based on years of professional experience[cite: 1]. The workflow covers data inspection, exploratory data analysis (EDA), preprocessing, model fitting using Scikit-Learn, and performance evaluation[cite: 1].

---

## 📌 Project Overview
- **Objective:** Model the relationship between years of experience ($X$) and expected salary ($y$) using an Ordinary Least Squares (OLS) regression algorithm[cite: 1].
- **Algorithm:** Simple Linear Regression (`sklearn.linear_model.LinearRegression`)[cite: 1].
- **Model Score:** Achieved an $R^2$ score of **~98.82%** on test data[cite: 1].

---

## 🛠️ Tech Stack & Dependencies
- **Python 3.x**[cite: 1]
- **Pandas** – Data wrangling and DataFrame manipulation[cite: 1]
- **NumPy** – Vectorized operations and array reshaping[cite: 1]
- **Matplotlib** – Data visualization and scatter plotting[cite: 1]
- **Scikit-Learn** – Model training, data splitting, and evaluation metrics[cite: 1]

---

## ⚙️ Machine Learning Pipeline

1. **Data Ingestion:** Load `Salary_dataset.csv` into a Pandas DataFrame[cite: 1].
2. **Data Cleaning & Preprocessing:**
   - Verify missing values (`isnull().sum()`) and duplicated entries (`duplicated().sum()`)[cite: 1].
   - Drop irrelevant index artifact columns (`Unnamed: 0`)[cite: 1].
3. **Exploratory Data Analysis (EDA):**
   - Generate scatter plots depicting `YearsExperience` vs. `Salary` to confirm linear correlation[cite: 1].
4. **Data Splitting:**
   - Split dataset into training (80%) and testing (20%) sets with `random_state=0`[cite: 1].
5. **Model Training:**
   - Reshape features into 2D arrays (`reshape(-1, 1)`) and train `LinearRegression()`[cite: 1].
6. **Model Evaluation:**
   - Measure performance using Mean Absolute Error (MAE) and $R^2$ Score[cite: 1].

---

## 📊 Dataset Summary

- **Total Samples:** 30 records[cite: 1]
- **Features:**
  - `YearsExperience` (Continuous Float) – Independent variable ($X$)[cite: 1]
- **Target:**
  - `Salary` (Continuous Float) – Dependent variable ($y$)[cite: 1]
- **Missing Values:** 0[cite: 1]
- **Duplicate Records:** 0[cite: 1]

---

## 📈 Model Performance & Learned Parameters

- **Intercept ($\beta_0$):** `≈ 25,850.00`[cite: 1]
- **Coefficient / Slope ($\beta_1$):** `≈ 9,312.58`[cite: 1]
- **Evaluation Metric:**
  - **$R^2$ Score:** `0.9882` (98.82% variance explained)[cite: 1]

$$\text{Salary} \approx 25850 + 9312.58 \times (\text{YearsExperience})$$
[cite: 1]

---

## 🚀 Getting Started

### 1. Clone the Repository
```bash
git clone [https://github.com/your-username/salary-prediction-linear-regression.git](https://github.com/your-username/salary-prediction-linear-regression.git)
cd salary-prediction-linear-regression
