# Diabetes Prediction

For this project, I use the CDC Diabetes Health Indicators dataset to illustrate my approach to model selection. I first do predictions with a baseline model and a couple of untuned models using the train test data. I also balance the dataset (given that there is a class imbalance), do hyperparameter tuning, apply the best thresholds, and use PCA (using different variation retention). The best model is selected depending on the performance metrics ideal for the problem at hand. For this particular project, the best-performing model is determined based on the F1 score since the aim is to ensure correct prediction of diabetic cases to target them for medication. F1 score gives a balace between precision and recall.  


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
- The main challenge presented was poor performance regarding predicting diabetic cases. The models performed well in predicting non-diabetic cases but predicted the diabetic cases poorly. This is mainly due to class imbalance. The baseline model presented the need for improving model performance with class balance, hyperparameter tuning, and threshold tuning
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
