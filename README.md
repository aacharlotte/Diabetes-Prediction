# Diabetes Prediction

The CDC Diabetes Health Indicators dataset is used for this project to illustrate how I go about model selection. I first do predictions with a couple of untuned models, using the train test data. I then balance the dataset, do parameter tuning, apply the best thresholds, and use PCA (using different variation retantion)


### Tools and Libraries Used
- **Pandas**: Data manipulation
- **NumPy**: Numerical computations  
- **Seaborn**: Data visualization  
- **Matplotlib**: Plotting and customization
- **time**: Track model training time with PCA 

---

## Problem Statement
 Predict whether an individual is diabetic based on health indicators such as BMI, smoking, physical activity, etc.

---

## Aim of the Project
Build a classification model that ensures that both classes (diabetic and non-diabetic) are detected well, with priority given to detecting all diabetic cases to target these for proper diagnosis.

---

## Skills and Concepts Demonstrated
- EDA  
- Preprocessing
- Train-test split
- Building a baseline model  
- Building 6 classification models and improving their performance with class balance, hyperparameter tuning, and threshold tuning
- Interpreting model performance metrics 

---

## Visualizations and Interpretation

### Correlation Heatmap
<img src="https://github.com/aacharlotte/Diabetes-Prediction/blob/main/correlation%20heatmap.png" width="120%" />

**Key Observations:**
- No very high correlations between features were identified. 

---

### Baseline model performance
<img src="https://github.com/aacharlotte/Diabetes-Prediction/blob/main/Baseline%20%20Logistic%20Regression%20ConfusionMatrix.png" width="60%" />

**Key Observations:**
- The baseline model provided performance reference and presented data challenges to be handled with advanced models.
- The main challenge presented was poor performance regarding predicting diabetic cases. This is mainly due to class imbalance.
---

### Best model: Random Forest
<img src="https://github.com/aacharlotte/Diabetes-Prediction/blob/main/Best%20model%20-%20Random%20Forest%20ConfusionMatrix.png" width="60%" />

**Key Observations:**
- Of the six models built, Random Forest emerged as the best-performing model with the highest recall and F1-score (as also seen in the table below). The better recall indicates that this model misses fewer real diabetic cases compared to other models. 

---

### Baseline model performance
<img src="https://github.com/aacharlotte/Diabetes-Prediction/blob/main/Model%20performance.png" width="100%" />


---

## Author & License
**Author**: [Charlotte Arinaitwe]  
**Date**: 2025  
**License**: MIT

---
