# 🧮 Calories Burn Analysis  
**An end-to-end data science project — EDA, Classification & Regression Modelling**

---

## 📘 Project Overview  
This project explores **fitness data** to analyze how workout types, gender, body metrics, and heart rate influence calories burned.  
It uses **data visualization** and **machine learning** to uncover key patterns affecting calorie expenditure.  
Includes both **regression (predicting calories)** and **classification (categorizing burn levels)** models.  

🔗 **Repository:** [github.com/siya-lalwani/calorie-burn-analysis](https://github.com/siya-lalwani/calorie-burn-analysis)

---

## 🎯 Objectives  
- Understand relationships between **workout parameters** and **calorie burn**.  
- Visualize **calorie distribution**, **workout comparisons**, and **gender-based trends**.  
- Generate **correlation heatmaps** to identify numeric dependencies.  
- Build:
  - 🧠 **Random Forest Regressor** for calorie prediction  
  - 🔥 **Random Forest Classifier** for calorie burn categorization  
- Identify key predictors using **feature importance analysis**.

---

## 🛠️ Technologies Used  
- **Python**  
- **Pandas**, **NumPy** — Data cleaning & manipulation  
- **Matplotlib**, **Seaborn** — Data visualization  
- **Scikit-learn** — Machine learning & evaluation  

---

## 📊 Key Visualizations  

### 🔹 Distribution of Calories Burned  
**Interpretation:**  
- Most workouts fall in a **moderate calorie-burn range** — balanced intensity.  
- Slight right skew shows a few **high-burn sessions (HIIT/Cardio)**.  
- Calorie burn varies significantly with **session type and intensity**.  

---

### 🔹 Calories Burned by Workout Type  
**Interpretation:**  
- **Cardio** and **HIIT** show the highest medians → most efficient for calorie burn.  
- **Yoga** and **Stretching** display smaller ranges → low-intensity workouts.  
- Variation within categories shows **effort and duration** impact results.  

---

### 🔹 Calories Burned vs Average BPM  
**Interpretation:**  
- Strong **positive correlation**: higher heart rate → higher calories burned.  
- **Longer sessions** (larger points) confirm both duration & intensity matter.  
- **HIIT & Cardio** dominate high-BPM zones — validating physiological patterns.  

---

### 🔹 Feature Importance Plot  
**Interpretation:**  
- **Average BPM** and **Session Duration** are top predictors.  
- **Weight** and **Workout Type** add meaningful impact.  
- Confirms both **physiological** and **workout-related** features drive predictions.  

---

## 📈 Model Metrics & Interpretation  

### ⚙️ Random Forest Regressor  
**Workflow:** 80/20 train-test split (`random_state=42`), evaluated using **R²** and **MAE**.

| Metric | Description | Value |
|:--------|:-------------|:------|
| **R² Score** | Measures how much variance is explained (1.0 = perfect) | ≈ 0.85–0.9 |
| **MAE** | Mean Absolute Error — avg. absolute difference between predicted & actual calories | ≈ 20–30 |

**Interpretation:**  
✅ High R² → model explains most calorie-burn variance.  
✅ Low MAE → predictions are close to real-world values.  

---

### ⚙️ Random Forest Classifier  
**Workflow:** Classified sessions into *High*, *Medium*, *Low*, and *Very High* calorie burns.  
Evaluated using **precision**, **recall**, and **F1-score**.

| Class | Precision | Recall | F1-score | Support |
|:-------|:-----------:|:--------:|:----------:|:----------:|
| High | 1.00 | 1.00 | 1.00 | 998 |
| Low | 1.00 | 1.00 | 1.00 | 994 |
| Medium | 1.00 | 1.00 | 1.00 | 970 |
| Very High | 1.00 | 1.00 | 1.00 | 1038 |
| **Accuracy** |  | **1.00** |  | 4000 |
| **Macro Avg** | 1.00 | 1.00 | 1.00 | 4000 |
| **Weighted Avg** | 1.00 | 1.00 | 1.00 | 4000 |

**Interpretation:**  
✅ Balanced precision & recall → consistent model performance.  
✅ Confirms classifier learned **meaningful calorie-related distinctions**.  

---

## 💡 Insights  
- Both **heart rate** and **duration** are dominant predictors of calorie burn.  
- **HIIT & Cardio** are the most efficient workout types.  
- The model demonstrates strong generalization and interpretability.  

---

## ❤️ Built With  
**Pandas • NumPy • Matplotlib • Seaborn • Scikit-learn**

---

*Built with ❤️ by [Siya Lalwani](https://github.com/siya-lalwani)*
