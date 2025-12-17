# 🐚 Abalone Dataset Analysis & Age Prediction

An analytical, insight-driven data science project focused on understanding **abalone growth patterns** and **predicting age** using biological and physical measurements.

This project follows a **clean, research-oriented workflow**, combining exploratory data analysis (EDA), visual storytelling, and machine learning to ensure **clarity, interpretability, and real-world relevance**.

---

## ⭐ Project Overview

This case study transforms raw biological measurement data into a structured analytical narrative to examine how **size, weight, and age (rings)** are related in abalones.

The project enables analysts and researchers to explore:

- Growth patterns across physical dimensions  
- Variability in weight-based attributes  
- Age distribution of abalones  
- Relationships between size, weight, and age  
- Feasibility of predicting age using measurable biological features  

---

## 🗂 Dataset Details

| Property | Description |
|--------|-------------|
| Dataset Name | Abalone.csv |
| Source | UCI Machine Learning Repository |
| Rows | 4,177 |
| Columns | Sex, Length, Diameter, Height, Whole Weight, Shucked Weight, Viscera Weight, Shell Weight, Rings |
| Target Variable | Rings |
| Derived Metric | Age = Rings + 1.5 years |

---

## 🎯 Objectives

- Perform Exploratory Data Analysis (EDA) to understand feature distributions  
- Identify meaningful patterns between size, weight, and age  
- Clean and preprocess real-world biological data  
- Visualize feature relationships clearly and intuitively  
- Build and evaluate machine learning models for abalone age prediction  

---

## ⚙️ Data Processing Workflow

### 📍 1. Data Cleaning
- Removed duplicate records  
- Verified and handled missing values  
- Treated outliers using the **Interquartile Range (IQR)** method  
- Encoded categorical feature **Sex** into numerical format  

### 📍 2. Feature Engineering
- Generated summary statistics and central tendency measures  
- Created a correlation matrix to identify influential predictors  
- Converted **Rings → Age** for biological interpretability  
- Normalized numerical features for stable model training  

### 📍 3. Data Visualization
- 📈 Length vs Whole Weight (Scatter Plot)  
- 📉 Age (Rings) Distribution (Histogram)  
- 📦 Weight Variability (Box Plots)  
- 🔗 Correlation Heatmap  
- 📊 Size vs Weight Pairwise Trend Analysis  

---

## 🧠 Analytical Insights

### 🧬 Size Distribution
Length, Diameter, and Height exhibit stable and centrally distributed patterns, indicating consistent biological growth across the abalone population.

### 🐚 Weight Variability
Weight-based features (Whole, Shucked, Viscera, Shell weight) show higher variability, suggesting that abalones of similar size can differ substantially in mass due to age and biological factors.

### 🔗 Age Correlation
Whole Weight demonstrates a strong positive correlation with Rings (age), making it the most influential predictor for age estimation.

### 🧓 Age Group Distribution
Most abalones fall within mid-range age groups, indicating a mature and balanced population rather than dominance of juvenile or aged specimens.

### 📊 Growth Trends
An increase in size and weight corresponds to an increase in ring count, validating expected biological growth-age relationships.

---

## 🤖 Machine Learning & Model Evaluation

Two regression models were trained and evaluated using an 80–20 train-test split.

### 🔹 Linear Regression (Baseline Model)
- **MAE:** 1.64 years  
- **RMSE:** 2.25 years  
- **R² Score:** 0.50  

Captures general linear relationships and serves as a strong baseline.

### 🔹 Random Forest Regressor (Best Model)
- **MAE:** 1.57 years  
- **RMSE:** 2.19 years  
- **R² Score:** 0.53  
- **Pseudo Accuracy:** **83.97%**

Random Forest outperforms Linear Regression by modeling **non-linear biological growth patterns**, resulting in improved accuracy and reliability.

> *Pseudo Accuracy represents the percentage of predictions within an acceptable error tolerance and is used as an intuitive complement to standard regression metrics.*

---

## 🎯 Key Takeaway

Abalone age can be effectively inferred from physical and weight-based measurements.  
**Whole Weight emerges as the strongest predictor**, and ensemble learning (Random Forest) provides superior predictive performance—forming a strong foundation for practical age estimation models.

---

## 🧰 Tools & Technologies Used

| Tool | Purpose |
|-----|--------|
| Python (Pandas, NumPy) | Data cleaning and analysis |
| Matplotlib, Seaborn | Data visualization |
| Scikit-learn | Machine learning modeling |
| Jupyter Notebook | Interactive development |

---

## 🚀 Future Enhancements

- Hyperparameter tuning for Random Forest  
- Experimentation with Gradient Boosting and XGBoost  
- Feature importance–based explainability  
- Cross-validation for stronger generalization  
- Deployment of a lightweight age prediction web application  

---
---
📎 Project Files

[📘 Abalone Analysis Notebook](PROJECT_ML_PART_A.ipynb)

[📄 Dataset](abalone.csv)

---
👤 Author

Yash Pawar
🎯 Aspiring Data Analyst | Python & Machine Learning Enthusiast | MIT-WPU

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/yash-pawar2/)  
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/yash-pawar2)  
[![Email](https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white)](mailto:Yash.r.pawar246@gmail.com)


