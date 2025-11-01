Supervised Machine Learning Projects
📋 Overview
Two machine learning projects demonstrating regression and classification techniques for real-world business problems.

🎮 Project 1: Video Game Sales Prediction (Regression)
Business Problem
Predict global video game sales to help publishers and retailers optimize production and distribution strategies.

Dataset
16,598 games with platform, genre, publisher, and regional sales data

Target: Global_Sales (in millions)

Key Features: Platform, Genre, Publisher, Regional Sales (NA, EU, JP, Other)

Key Insights
Top Platforms: GB (2.62M avg), NES (2.56M), GEN (1.05M)

Top Genres: Platform (0.95M), Shooter (0.80M), Role-Playing (0.63M)

Sales Trends: Peak in 2008-2009, Nintendo dominates top-selling titles

Top Games: Wii Sports (82.74M), Super Mario Bros. (40.24M)

Model Performance
Model	R² Score	RMSE	Key Findings
Linear Regression	-3.92e+24	2.53 trillion	Poor performance with categorical features
**K			
readme.md file so it will be beautify
We are going to create a README.md file that summarizes both projects (Regression and Classification) and highlights the models' performance.

Steps:

Start with a project overview.

For each project, provide:

Problem statement

Dataset description

Key insights from EDA

Models built and their performance

Final model chosen and its performance metrics

Compare the two projects and models.

Include technical details and how to run the code.

Note: We have two separate projects: one regression and one classification.

Let's structure the README as follows:

Supervised Machine Learning Projects
Overview
Brief description of the two projects.

Project 1: Video Game Sales Prediction (Regression)
Problem Statement
Dataset
Exploratory Data Analysis (EDA)
Models and Performance
Final Model and Insights
Project 2: Credit Score Classification (Classification)
Problem Statement
Dataset
Exploratory Data Analysis (EDA)
Models and Performance
Final Model and Insights
Conclusion
How to Run
We'll use the details provided in the two notebooks.

Supervised Machine Learning Projects
📋 Overview
This repository contains two comprehensive machine learning projects demonstrating both regression and classification techniques for real-world business problems.

🎮 Project 1: Video Game Sales Prediction
🎯 Business Problem
Predict global video game sales to help publishers and retailers optimize production and distribution strategies.

📊 Dataset Overview
Records: 16,598 games

Features: 11 columns including platform, genre, publisher, regional sales

Target: Global_Sales (in millions)

🔍 Key Insights
Category	Top Performers	Average Sales
Platforms	GB, NES, GEN	2.62M, 2.56M, 1.05M
Genres	Platform, Shooter, Role-Playing	0.95M, 0.80M, 0.63M
Top Games	Wii Sports, Super Mario Bros.	82.74M, 40.24M
📈 Model Performance
Linear Regression
Model	R² Score	RMSE	Status
Multiple Features	-3.92e+24	2.53 trillion	❌ Poor
Platform Only	-3.92e+24	2.53 trillion	❌ Poor
KNN Regression
Model	R² Score	RMSE	Status
Baseline (k=5)	-0.024	1.294	⚠️ Weak
Tuned (k=31)	0.049	1.248	✅ Best
🏆 Final Model
python
KNeighborsRegressor(n_neighbors=31, weights='distance')
R² Score: 0.049

RMSE: 1.248 million units

Interpretation: Modest predictive power, indicates need for better feature engineering

💳 Project 2: Credit Score Classification
🎯 Business Problem
Automate credit score classification (Good/Standard/Poor) to reduce manual assessment efforts in financial services.

📊 Dataset Overview
Records: 100,000 → 68,405 (after cleaning)

Features: 28 columns including financial and behavioral data

Target: Credit_Score (Multi-class)

🧹 Data Cleaning Highlights
Handled missing values and inconsistent entries

Converted Credit_History_Age to months

Applied temporal filling for customer data

Removed outliers using IQR method

📊 Model Performance Comparison
Logistic Regression
Model	Accuracy	Precision	Recall	F1-Score
Basic Features	58.8%	0.578	0.588	0.516
Extended Features	59.4%	0.576	0.594	0.527
KNN Classification
Model	Train Accuracy	Test Accuracy	Precision	Recall	F1-Score
KNN V1 (k=5)	84.3%	77.5%	0.776	0.775	0.775
KNN V2 (k=7)	71.6%	62.1%	0.612	0.621	0.614
🏆 Final Model
python
KNeighborsClassifier(n_neighbors=5)
Test Accuracy: 77.5%

Precision: 0.776 (weighted)

Recall: 0.775 (weighted)

F1-Score: 0.775 (weighted)

Business Impact: Can automate 77.5% of credit assessments accurately with minimal overfitting.

🛠 Technical Implementation
🏗️ Architecture
python
# Common Technologies
Python + pandas + numpy + matplotlib + seaborn + scikit-learn

# Model Evaluation
- Regression: R², RMSE, Residual Analysis
- Classification: Accuracy, Precision, Recall, F1-Score, Confusion Matrix
📁 Project Structure
text
├── White Box(Regression).ipynb      # Video game sales prediction
├── Black Box(Classification).ipynb  # Credit score classification
├── vgsales.csv                      # Regression dataset
├── train.csv                        # Classification dataset
└── README.md                       # Project documentation
🚀 Quick Start
Prerequisites
bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
Running the Projects
bash
# Launch Jupyter Notebook
jupyter notebook

# Open either:
# - White Box(Regression).ipynb
# - Black Box(Classification).ipynb
📈 Performance Summary
Project	Best Model	Key Metric	Performance	Business Impact
Sales Prediction	KNN Regression (k=31)	R² Score	0.049	Modest sales forecasting capability
Credit Scoring	KNN Classification (k=5)	Accuracy	77.5%	High automation potential for credit assessment
🔮 Key Learnings
Video Game Sales
Simple categorical features limit regression performance

Nintendo's dominance in the gaming industry is evident

Future improvements: Incorporate temporal trends and market factors

Credit Scoring
KNN outperforms logistic regression for non-linear patterns

Basic financial features provide strong predictive power

Model shows excellent generalization with minimal overfitting

👨‍💻 Author
Ali Hasan
Data Science Bootcamp Participant
📧 [Your Email]
🔗 [Your LinkedIn]

<div align="center">
🌟 If you find this project useful, please give it a star! 🌟

</div>
