# 🧠 Supervised Machine Learning Projects

## 📋 Overview
This repository contains two machine learning projects demonstrating both **regression** and **classification** techniques for real-world business problems.

---

## 🎮 Project 1: Video Game Sales Prediction

### 🎯 Business Problem
Predict global video game sales to help publishers and retailers optimize production and distribution strategies.

### 📊 Dataset Overview
- **Records:** 16,598 games  
- **Features:** 11 columns including platform, genre, publisher, regional sales  
- **Target:** Global_Sales (in millions)

### 🔍 Key Insights

| Category | Top Performers | Average Sales |
|-----------|----------------|---------------|
| **Platforms** | GB, NES, GEN | 2.62M, 2.56M, 1.05M |
| **Genres** | Platform, Shooter, Role-Playing | 0.95M, 0.80M, 0.63M |
| **Top Games** | Wii Sports, Super Mario Bros. | 82.74M, 40.24M |

### 📈 Model Performance

#### Linear Regression
| Model | R² Score | RMSE | Status |
|-------|-----------|------|---------|
| Multiple Features | -3.92e+24 | 2.53 trillion | ❌ Poor |
| Platform Only | -3.92e+24 | 2.53 trillion | ❌ Poor |

#### KNN Regression
| Model | R² Score | RMSE | Status |
|-------|-----------|------|---------|
| Baseline (k=5) | -0.024 | 1.294 | ⚠️ Weak |
| **Tuned (k=31)** | **0.049** | **1.248** | ⚠️ Weak |

### 🏆 Final Model
```python
KNeighborsRegressor(n_neighbors=31)
```

**R² Score:** 0.049  
**RMSE:** 1.248 million  

---

## 💳 Project 2: Credit Score Classification

### 🎯 Business Problem
Automate credit score classification (**Good / Standard / Poor**) to reduce manual assessment efforts in financial services.

### 📊 Dataset Overview
- **Records:** 100,000 → 68,405 (after cleaning)  
- **Features:** 28 columns including financial and behavioral data  
- **Target:** Credit_Score (Multi-class)

### 📊 Model Performance Comparison

#### Logistic Regression
| Model | Accuracy | Precision | Recall | F1-Score |
|--------|-----------|-----------|--------|-----------|
| Basic Features | 58.8% | 0.578 | 0.588 | 0.516 |
| Extended Features | 59.4% | 0.576 | 0.594 | 0.527 |

#### KNN Classification
| Model | Train Accuracy | Test Accuracy | Precision | Recall | F1-Score |
|--------|----------------|----------------|------------|--------|-----------|
| KNN V1 (k=5) | 84.3% | 77.5% | 0.776 | 0.775 | 0.775 |
| KNN V2 (k=7) | 71.6% | 62.1% | 0.612 | 0.621 | 0.614 |

### 🏆 Final Model
```python
KNeighborsClassifier(n_neighbors=5)
```

**Test Accuracy:** 77.5%  
**Precision:** 0.776 
**Recall:** 0.775  
**F1-Score:** 0.775 

---


## 🛠 Technical Implementation

### 🧩 Technologies Used
- Python (pandas, numpy, matplotlib, seaborn)  
- scikit-learn for machine learning algorithms  
- Jupyter Notebook for analysis and visualization  

### 📁 Project Structure
```
├── White Box(Regression).ipynb      # Video game sales prediction
├── Black Box(Classification).ipynb  # Credit score classification
├── vgsales.csv                      # Regression dataset
├── train.csv                        # Classification dataset
└── README.md                        # Project documentation
```


---

## 👨‍💻 Author
**Ali Hasan**  
_Data Science Bootcamp - Supervised Machine Learning Projects_
