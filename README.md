# Obesity Level Classification using Machine Learning in R

This repository contains the full R-based machine learning workflow to classify obesity levels using demographic and lifestyle variables. It supports the MSc Dissertation project titled:

**"Estimation of Obesity Levels Based On Eating Habits and Physical Condition: A Classification Approach"**

## 📊 Project Overview

The study uses a dataset sourced from the UCI Machine Learning Repository with 17 attributes and a multi-class target (`NObeyesdad`) indicating seven obesity levels:

- Insufficient Weight
- Normal Weight
- Overweight Level I
- Overweight Level II
- Obesity Type I
- Obesity Type II
- Obesity Type III

## 🧠 Machine Learning Models Applied

- Multinomial Logistic Regression
- Decision Tree
- Random Forest
- Support Vector Machine (SVM)

## ⚙️ Pipeline Overview

1. **Data Preprocessing**
   - Handling missing values
   - Outlier detection using IQR
   - Type conversion and standardization

2. **Exploratory Data Analysis (EDA)**
   - Histograms, Boxplots, Correlation heatmaps
   - Class imbalance visualizations

3. **Model Training and Evaluation**
   - Accuracy, Kappa, Precision, Recall, F1-score
   - Confusion matrix for each model
   - AUC and ROC for multi-class (One-vs-Rest)

4. **Feature Importance**
   - Extracted using `randomForest`
   - Top features visualized

5. **Hyperparameter Tuning**
   - Grid search for Random Forest's `mtry`

## 📁 File Descriptions

| File | Description |
|------|-------------|
| `data/OD.csv` | Raw dataset |
| `src/Obesity.R` | Complete R script with preprocessing, training, and evaluation |
| `report/Final_Dissertation.doc` | MSc Dissertation report  |
| `README.md` | This documentation |

## 🧰 Libraries Used

- `tidyverse`, `caret`, `randomForest`, `rpart`, `e1071`, `MLmetrics`
- `ggplot2`, `GGally`, `corrplot`, `pROC`

## 📈 Results

- Random Forest provided the best overall performance with high AUC values, especially for severe obesity classes.
- Data preprocessing and class balancing were critical to model performance.

## 📝 How to Run

1. Clone this repository.
2. Open `Obesity.R` in RStudio.
3. Install required libraries (first block of the script).
4. Run the script step-by-step or as a whole.

## 📚 Dataset Source

[UCI Machine Learning Repository – Obesity Dataset](https://archive.ics.uci.edu/dataset/544/estimation+of+obesity+levels+based+on+eating+habits+and+physical+condition)

## 📄 License

This project is licensed under the MIT License.

## 🙋‍♀️ Author

Dissertation by Nitesh Bhalerao 
LinkedIn: https://www.linkedin.com/in/niteshbhalerao2704/
Supervised by Dr. Yang Li | MSc Data Science, University of East London

---
