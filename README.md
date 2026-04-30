# 🌲 Forest Cover Type Classification System

## 📌 Project Overview

This project presents a **complete end-to-end data science pipeline** for predicting forest cover types using environmental and geographical features.

It integrates:

* Data cleaning & preprocessing
* Exploratory Data Analysis (EDA)
* Statistical analysis & hypothesis testing
* Machine learning model comparison
* Hyperparameter tuning
* Model evaluation (Confusion Matrix & ROC Curve)
* Model explainability (Feature Importance & SHAP)
* Deployment using Streamlit

👉 The final output is an **interactive web application** that predicts forest cover type based on user inputs.

---

## 🎯 Objectives

* Build a robust classification system for forest cover prediction
* Understand relationships between environmental variables
* Compare multiple machine learning models
* Optimize model performance
* Explain model decisions
* Deploy the solution for real-world usage

---

## 📂 Dataset

* Cleaned dataset with **56 features**
* Target variable: `Cover_Type` (7 classes)
* Features include:

  * Elevation, Aspect, Slope
  * Hydrology distances
  * Hillshade measurements
  * Wilderness areas
  * Soil types

---

## 🧹 Data Cleaning

Performed using `forest_cleaning.ipynb`

* Handled missing values
* Removed duplicates
* Validated ranges (e.g., slope, aspect)
* Treated outliers using IQR
* Ensured consistent data types

---

## 📊 Exploratory Data Analysis (EDA)

Conducted in `forest_eda.ipynb`

### Key Insights:

* Elevation plays a **major role** in forest classification
* Certain cover types dominate specific elevation ranges
* Some variables show weak correlation with target
* Dataset shows **class imbalance**

---

## 📈 Statistical Analysis

Performed in `forest_statistical_analysis.ipynb`

### Methods:

* Skewness & kurtosis analysis
* Normality testing (Shapiro-Wilk)
* ANOVA test
* Chi-square test
* Correlation significance testing
* Regression analysis

### Insights:

* Elevation is **not normally distributed**
* Significant differences exist between cover types
* Soil type is statistically dependent on forest type
* Environmental variables strongly influence classification

---

## 🤖 Machine Learning Models

Implemented in `forest_models.ipynb`

Models used:

* Logistic Regression
* Decision Tree
* Random Forest
* K-Nearest Neighbors (KNN)

### Key Finding:

👉 **Random Forest outperformed all other models**

---

## ⚙️ Hyperparameter Tuning

Performed using `forest_tuning.ipynb`

* Used GridSearchCV
* Optimized model parameters
* Improved generalization and accuracy

---

## 🔲 Model Evaluation

### 📌 Confusion Matrix (`forest_confusion_matrix.ipynb`)

* High accuracy across most classes
* Some misclassification between similar cover types

### 📌 ROC Curve (`forest_roc_curve.ipynb`)

* Strong multi-class performance
* High AUC values across most classes
* Model shows excellent separability

---

## 🌟 Model Explainability

### 📌 Feature Importance (`forest_feature_importance.ipynb`)

* Elevation is the most influential feature
* Soil and terrain variables also important

### 📌 SHAP Explainability (`forest_shap_explainability.ipynb`)

* Provides local and global interpretability
* Explains how each feature contributes to predictions

---

## 🧠 Final Model

Saved using `forest_model.ipynb`

* Exported trained model (`model.pkl`)
* Ready for deployment

---

## 🚀 Deployment (Streamlit App)

Implemented in:
👉 

### Features:

* User-friendly interface
* Real-time prediction
* Input environmental parameters
* Outputs forest cover type

### Supported Classes:

* Spruce/Fir
* Lodgepole Pine
* Ponderosa Pine
* Cottonwood/Willow
* Aspen
* Douglas-fir
* Krummholz

---

## 🛠️ Technologies Used

* Python
* Pandas, NumPy
* Matplotlib, Seaborn
* Scikit-learn
* SHAP
* Streamlit

---

## 📁 Project Structure

```
forest-cover-classification/
│
├── notebooks/
│   ├── forest_cleaning.ipynb
│   ├── forest_eda.ipynb
│   ├── forest_statistical_analysis.ipynb
│   ├── forest_models.ipynb
│   ├── forest_tuning.ipynb
│   ├── forest_confusion_matrix.ipynb
│   ├── forest_roc_curve.ipynb
│   ├── forest_feature_importance.ipynb
│   ├── forest_shap_explainability.ipynb
│   ├── forest_model.ipynb
│   └── forest_streamlit_app.ipynb
│
├── data/
│   └── forest_cleaned_dataset.csv
│
├── model.pkl
└── README.md
```

---

## 💡 Key Learnings

* Importance of data cleaning before modeling
* Role of statistical validation in analysis
* Model selection and evaluation techniques
* Explainability is critical in ML projects
* End-to-end pipeline development

---

## 🔮 Future Improvements

* Add advanced models (XGBoost, LightGBM)
* Improve class imbalance handling
* Deploy app to cloud (Hugging Face / AWS)
* Add real-time data integration

---

## 👨‍💻 Author

**Mohammad Saiful Alam**
M.Sc. in Data Science & Machine Learning
Research Officer at BFRI

---

## ⭐ Support

If you found this project useful, please ⭐ the repository!
