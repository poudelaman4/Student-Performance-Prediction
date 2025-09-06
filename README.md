# 🎓 Student Performance Prediction

## 📌 Project Overview
This project predicts students' **average exam scores** based on various factors such as gender, race/ethnicity, parental education level, lunch type, and test preparation course.  

Dataset used: **StudentsPerformance.csv**

---

## 🛠️ Steps Performed
1. **Data Cleaning**
   - Added `avg_score` column = mean of math, reading, writing scores.
   - Checked for missing values (none found).

2. **Exploratory Data Analysis (EDA)**
   - Visualized distributions of categorical features.
   - Compared average scores by gender, parental education, test prep.
   - Correlation heatmap of features with `avg_score`.

3. **Model Training**
   - Models compared: 
     - Linear Regression  
     - Decision Tree Regressor  
     - Random Forest Regressor  
     - Gradient Boosting Regressor  
     - Support Vector Regressor (SVR)  

   - Evaluation Metrics:
     - Mean Squared Error (MSE)  
     - Root Mean Squared Error (RMSE)  
     - R² Score  

---

## 📊 Results

| Model | RMSE | R² Score |
|-------|------|----------|
| Linear Regression | ~0 | **1.0** |
| Gradient Boosting | ~0.68 | 0.998 |
| Decision Tree | ~0.69 | 0.998 |
| Random Forest | ~0.93 | 0.996 |
| SVR | ~5.74 | 0.846 |

---

## 🔎 Inference
- **Linear Regression achieved R²=1.0**, which is unusual in real-world scenarios.  
- All tree-based models performed very well (>0.99 R²).  
- **SVR performed worse (R²=0.84)**, but still good.  
- This dataset is relatively **simple**, which explains the near-perfect results.  

---

## 🚀 Future Work
- Try **hyperparameter tuning** (`GridSearchCV`, `RandomizedSearchCV`) to see if performance can improve.  
- Use **cross-validation** for more reliable performance estimation.  
- Experiment with predicting **individual subject scores** instead of average score.
