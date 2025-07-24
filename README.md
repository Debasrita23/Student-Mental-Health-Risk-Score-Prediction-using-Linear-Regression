# 🧠 Student Mental Health Risk Score Prediction using Linear Regression

This project aims to predict the **mental health risk score** of students using **Linear Regression** based on key behavioral factors. It explores how habits like sleep, study hours, screen time, and social interaction impact a student's mental well-being.

---

## 📌 Objective

To use a regression model to estimate mental health risk from daily lifestyle parameters, identify contributing factors, and visualize their relationships through data plots.

---

## 📂 Dataset

A **synthetic dataset** is generated using NumPy to simulate 200 students' lifestyle behavior. The dataset includes:

| Column           | Description                                 |
|------------------|---------------------------------------------|
| `SleepHours`      | Daily average sleep in hours                |
| `StudyHours`      | Daily average time spent studying           |
| `ScreenTime`      | Daily screen time usage in hours            |
| `SocialActivity`  | Daily social interaction time in hours      |
| `RiskScore`       | Calculated mental health risk score (0–100) |

The data is saved to `student_mental_health_data.csv`.

---

## 🛠️ Tools & Libraries

- Python
- NumPy, Pandas
- Scikit-learn
- Seaborn, Matplotlib
- Jupyter Notebook

---

## 📈 Workflow

### 1. **Data Generation & Loading**
- Created a dataset using random values for sleep, study, screen time, and social activity.
- RiskScore is computed using a linear formula with added noise.

### 2. **Data Visualization**
- **Scatter plots** between each feature and RiskScore.
- **Best-fit regression lines** added using `sns.regplot()`.
- A **correlation heatmap** generated using Seaborn to show inter-feature relationships.

### 3. **Model Training**
- Features: `SleepHours`, `StudyHours`, `ScreenTime`, `SocialActivity`
- Target: `RiskScore`
- Train/Test split: 80/20
- Model: `LinearRegression` from scikit-learn

### 4. **Evaluation**
- Predicted vs Actual Risk Scores plotted.
- **R² Score** calculated to evaluate performance.

---

## 📊 Visual Outputs

✅ Scatter plots with best-fit lines:
- `SleepHours` vs `RiskScore`
- `StudyHours` vs `RiskScore`
- `ScreenTime` vs `RiskScore`
- `SocialActivity` vs `RiskScore`

✅ Correlation heatmap to identify strong or weak linear relationships between features.

✅ Predicted vs Actual Risk Score comparison plot.

---

## 🧮 Result

- The model fits well for a synthetic dataset with an **R² score** indicating how well features explain the risk.
- Features like **high study hours** or **screen time** showed a positive correlation with risk.
- Features like **sleep** and **social activity** showed a negative correlation.

---

## 🗂️ File Structure

 - Student_Mental_Health_Risk_Score.ipynb # Jupyter notebook with code & plots
 - student_mental_health_data.csv # Generated synthetic dataset
 - README.md # Project description


