# Supervised Machine Learning Projects

Two comprehensive machine learning projects covering classification and regression tasks with detailed analysis and model development.

## 📊 Project Comparison

| Aspect | Classification Project (Black Box) | Regression Project (White Box) |
|--------|-----------------------------------|--------------------------------|
| **Problem Type** | Classification | Regression |
| **Business Goal** | Predict categorical outcomes | Predict global video game sales |
| **Main Algorithm** | Classification algorithms | KNN Regression |
| **Key Metrics** | Accuracy, Precision, Recall, F1-Score | RMSE, R-squared, Model Accuracy |
| **Dataset Size** | Classification dataset | 16,598 games, 11 features |

## 🔍 Project 1: Classification Model
**Black Box Approach** - Focused on predicting categorical outcomes

### Objectives:
- What features influence the target variable?
- Can feature engineering improve model performance?
- How do different model versions compare?

### Key Features:
- Data preprocessing and feature engineering
- Multiple classification algorithms tested
- Hyperparameter tuning for optimal performance
- Model evaluation using comprehensive metrics

## 🎮 Project 2: Video Game Sales Prediction  
**White Box Approach** - Predicting global sales using game features

### Problem Statement:
Develop machine learning models to predict global video game sales based on platform, genre, publisher, and regional sales data.

### Key Findings:
- **Top Platforms:** GB (2.62M avg), NES (2.56M), GEN (1.05M)
- **Top Genres:** Platform (0.95M), Shooter (0.80M), Role-Playing (0.63M)
- **Sales Trends:** Peak in 2012-2014, gradual decline thereafter
- **Data Quality:** Minimal missing data (<2%), 11,493 unique game titles

### Dataset Features:
- Platform (31 types), Genre (12 categories), Publisher (578 companies)
- Regional sales data (NA, EU, JP, Other)
- Global_Sales as target variable (0.01M - 82.74M range)

## 🛠 Technical Implementation

### Common Technologies:
- **Python** with pandas, numpy, matplotlib, seaborn
- **scikit-learn** for machine learning algorithms
- **Jupyter Notebook** for analysis and visualization
- Model evaluation and hyperparameter tuning

### Classification Specific:
- Multiple classification algorithms compared
- Focus on model interpretability and feature importance

### Regression Specific:
- KNN Regression with optimal k-value selection
- Extensive EDA on gaming industry trends
- Regional sales pattern analysis

## 📈 Key Insights

### From Classification:
- [Feature importance analysis and model performance insights]

### From Regression:
- Nintendo dominates top-selling games across multiple platforms
- Platform and genre significantly impact global sales performance
- Action (3,316 games) and Sports genres are most common
- Successful model predicting sales with identified optimal parameters

