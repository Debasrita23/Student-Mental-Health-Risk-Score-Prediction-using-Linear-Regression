
# 🧠 Student Mental Health Risk Score Prediction using Linear Regression

This project predicts a student's mental health risk score using a **Linear Regression model**. It uses a synthetic dataset with lifestyle-related features to identify how different habits impact mental well-being.

---

## 📌 Objective

To build a machine learning model that estimates the **risk score of mental health issues** in students based on the following key behavioral factors:

- Sleep Hours
- Study Hours
- Screen Time
- Social Activity

---

## 📊 Features Used

| Feature         | Description                            |
|----------------|----------------------------------------|
| `SleepHours`    | Average hours of sleep per day         |
| `StudyHours`    | Average hours spent studying daily     |
| `ScreenTime`    | Average screen time in hours per day   |
| `SocialActivity`| Average hours spent on social activity |

---

## 🗂️ Dataset

A synthetic dataset is created using NumPy to simulate data for 200 students, with randomized values in realistic ranges. The target variable `RiskScore` (ranging from 0 to 100) is generated as a linear combination of input features with added noise.

The dataset is saved as:  
`student_mental_health_data.csv`

---

## ⚙️ Technologies Used

- Python 🐍
- NumPy
- Pandas
- Scikit-learn
- Seaborn
- Matplotlib

---

## 🧮 Workflow

1. **Data Generation**
   - Random values for each feature are generated using `np.random.uniform`.
   - `RiskScore` is calculated using a custom formula combining all features.

2. **Data Preprocessing**
   - Load the CSV using pandas.
   - Split the data into features (`X`) and target (`y`).
   - Perform train/test split using `train_test_split`.

3. **Model Training**
   - Apply `LinearRegression` from `sklearn.linear_model`.
   - Train the model on the training dataset.

4. **Model Evaluation**
   - Predict on test data and compute **R² score**.
   - Visualize actual vs predicted scores.

5. **Visualization**
   - Generate **scatter plots** between each feature and `RiskScore`.
   - Add **best-fit regression lines** to each plot using `sns.regplot()`.

---

## 📈 Results

- **R² Score** indicates how well the model fits the data.
- The scatter plots help identify the influence of each factor on mental health risk.
- Example insight: More screen time or study hours may indicate higher stress/risk, while more sleep or social activity may reduce risk.

---

## 📷 Sample Plots

- Feature vs RiskScore scatter plots with regression lines:
  - Sleep Hours vs Risk Score
  - Study Hours vs Risk Score
  - Screen Time vs Risk Score
  - Social Activity vs Risk Score

*(To see the plots, run the notebook in Jupyter.)*

---

## 📁 File Structure


