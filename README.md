

# **Mobile App Usage Analysis and Prediction**

## **Project Overview**
This project analyzes detailed insights into mobile app usage patterns, including screen time, notifications received, and app openings. The dataset covers multiple days in August and includes popular apps, providing a granular view of digital behavior. The goal is to build predictive models to forecast app usage and identify key patterns that influence digital engagement.

---

## **Dataset Features**
The dataset contains the following columns:

| **Feature Name** | **Description** |
|------------------|------------------|
| `Date`           | The date of the recorded data. |
| `App`            | Name of the mobile application. |
| `Usage (minutes)`| Total minutes spent using the app on a given day. |
| `Notifications`  | Number of notifications received from the app. |
| `Times Opened`   | How many times the app was launched. |

---

## **Objective**
The main objective of this project is to build predictive models using machine learning techniques to estimate mobile app usage based on features like notifications received and app opening patterns.

---

## **Modeling Approach**
I applied several machine learning models and ensemble techniques to achieve robust predictions.

### **Machine Learning Models**
- **Decision Tree:** Captures non-linear patterns and provides interpretable rules.
- **Random Forest:** An ensemble of decision trees to reduce overfitting and improve accuracy.
- **Support Vector Machine (SVM):** Effective in high-dimensional feature spaces and robust to outliers.

### **Ensemble Techniques**
- **Stacking Regressor:** Combines multiple base models (Decision Tree, Random Forest, SVM) to improve prediction accuracy by using a meta-model for final predictions.

---

## **Key Steps**
1. **Data Preprocessing:** 
   - Cleaned and standardized the dataset.
   - Handled missing values and outliers.
   
2. **Exploratory Data Analysis (EDA):** 
   - Visualized trends in app usage and notification patterns over time.
   - Analyzed the relationship between app openings and total usage.

3. **Feature Engineering:** 
   - Created additional features like day-of-week and total interactions (notifications + times opened).

4. **Model Training and Evaluation:** 
   - Used cross-validation to evaluate model performance.
   - Optimized hyperparameters for individual models.
   - Applied ensembling with stacking for robust predictions.

---

## **Performance Metrics**
The models were evaluated using the following metrics:
- **Mean Absolute Error (MAE)**
- **Root Mean Squared Error (RMSE)**
- **R² Score**

---

## **Results**
| Model                | MAE   | RMSE  | R² Score |
|-----------------------|-------|-------|---------|
| Decision Tree         | 398.8042240509354 | 19.970083225939128| 0.41876076377796345   |
| Random Forest         | 375.6077065887078 | 19.38060129585013 | 0.4525686456399025   |
| **Support Vector Machine**| 324.6965507362651| 18.01933824357224 | 0.526769367593829  |
| Stacking Regressor| 336.794037343559 | 18.35194914289921| 0.5091378244662121 |

from our work we can clearly see that the support vector regressor happens to have the best result among all the technique we employed.
