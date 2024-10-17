# Obesity Classification Analysis

This project explores the classification of obesity levels using a dataset containing various lifestyle and health-related features. The goal is to build and evaluate machine learning models to predict the weight category of individuals based on demographic, dietary, and physical activity data.


## Dataset Overview
The dataset consists of 1,610 samples and 15 features, which include demographic factors (e.g., `Age`, `Sex`), lifestyle habits (e.g., `Physical_Exercise`, `Consumption_of_Fast_Food`), and the target variable `Class`, representing different levels of obesity.

## Exploratory Data Analysis (EDA)
- **Data Inspection:** No missing values were found, and all features were numeric.
- **Statistical Summary:** Identified key statistics for features like `Age` and `Height`.
- **Correlation Analysis:** Found that features such as `Physical_Exercise` and `Consumption_of_Fast_Food` had significant correlations with obesity levels.
- **Visualizations:** Plotted various features against the target variable to gain insights into their distributions and relationships.

## Feature Engineering
- **Age Binning:** Grouped `Age` into categories to simplify model interpretation.
- **Feature Selection:** Removed less informative features based on correlation analysis to improve model performance.

## Machine Learning Models
Several models were trained and evaluated, including:
- **Logistic Regression**
- **Decision Tree Classifier**
- **Random Forest Classifier**
- **Gradient Boosting (AdaBoost, GradientBoostingClassifier, XGBoost, LGBM)**
- **Stacking Classifier**

Hyperparameter tuning was performed for selected models to improve their accuracy.

## Model Performance
The following table summarizes the performance of the models:

| Model                                   | Accuracy | Precision | Recall  | F1      |
|-----------------------------------------|----------|-----------|---------|---------|
| Logistic Regression                     | 0.69     | 0.56      | 0.55    | 0.55    |
| Decision Tree Classifier                | 0.83     | 0.80      | 0.86    | 0.82    |
| Random Forest Classifier                | 0.88     | 0.89      | 0.90    | 0.90    |
| ExtraTreesClassifier                    | 0.87     | 0.89      | 0.90    | 0.89    |
| GradientBoostingClassifier              | 0.77     | 0.75      | 0.76    | 0.76    |
| AdaBoostClassifier                      | 0.68     | 0.60      | 0.58    | 0.59    |
| XGBClassifier                           | 0.88     | 0.87      | 0.89    | 0.88    |
| LGBMClassifier                          | 0.84     | 0.82      | 0.87    | 0.84    |
| HistGradientBoostingClassifier          | 0.86     | 0.85      | 0.87    | 0.86    |
| Stacking Classifier                     | 0.88     | 0.87      | 0.90    | 0.89    |
| **Tuned RandomForestClassifier**        | 0.88     | 0.89      | 0.90    | 0.90    |
| **Tuned XGBClassifier**                 | 0.84     | 0.84      | 0.81    | 0.82    |

## Conclusion and Recommendations
- **Best Model:** The Random Forest Classifier showed the highest accuracy, precision, recall, and F1-score.
- **Future Improvements:** Consider addressing class imbalance, collecting more data, or using deep learning techniques for better performance.


