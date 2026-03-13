# Waze User Churn Prediction

This project applies machine learning techniques to predict user churn using behavioral usage data from Waze.

The goal of the project is to identify patterns associated with users who are likely to stop using the platform, enabling earlier intervention through retention strategies.

---

## Project Overview

User churn is an important challenge for digital platforms. Understanding which users are likely to leave allows companies to target retention efforts and improve long-term engagement.

This project builds and compares two ensemble machine learning models:

- Random Forest
- XGBoost

The models are trained on engineered behavioral features derived from user activity data.

---

## Machine Learning Workflow

1. Data preparation and feature engineering
2. Handling missing values and encoding variables
3. Train / validation / test split
4. Model training with Random Forest
5. Model training with XGBoost
6. Hyperparameter tuning using GridSearchCV
7. Model selection based on recall
8. Precision-recall analysis
9. Decision threshold optimization

---

## Final Model

Champion Model: **XGBoost**

The XGBoost model was selected because it achieved higher recall, making it better suited for identifying users at risk of churn.

---

## Bonus Analysis

The project also demonstrates **decision threshold optimization**, showing how adjusting the classification threshold can significantly increase recall when the business objective prioritizes identifying potential churners.

---

## Tools & Libraries

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Matplotlib

---

## Repository Structure

```
waze-user-churn-prediction
│
├── waze_user_churn_prediction.ipynb
├── Waze_User_Churn_Prediction.html
├── xgb_churn_model.pkl
├── requirements.txt
└── data/
```


---

## Key Takeaways

- Feature engineering improves predictive performance.
- Ensemble models capture nonlinear behavioral patterns.
- Recall-focused evaluation is appropriate for churn prediction.
- Decision threshold tuning can significantly improve model usefulness.

---

## Future Improvements

- Expand hyperparameter tuning
- Test additional gradient boosting models
- Incorporate additional behavioral features
- Evaluate model performance with business impact metrics
