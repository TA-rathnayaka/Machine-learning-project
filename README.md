# FuelPredictor

## 1. Introduction

The **Auto-MPG dataset** is a collection of technical specifications for a variety of cars. It provides insights into fuel consumption (measured in miles per gallon, or MPG) alongside several technical attributes.

The goal of this project is to analyze the dataset to identify patterns and relationships among car specifications that influence fuel consumption. Furthermore, the project aims to build a predictive model that accurately estimates a car's fuel consumption using its technical specifications.

---

## 2. Dataset Description

### Dataset Source  
The dataset is available on Kaggle and originates from the **UCI Machine Learning Repository**:  
[Auto-MPG Dataset on Kaggle](https://www.kaggle.com/datasets/uciml/autompg-dataset?resource=download)

### Dataset Context  
The Auto-MPG dataset is widely used in machine learning and statistical analysis for regression problems. It captures essential information about cars manufactured between 1970 and 1982.

### Key Details  
- **Number of Instances**: 398  
- **Number of Attributes**: 9  

### Attributes
1. **mpg**: Miles per gallon (target variable, continuous).  
2. **cylinders**: Number of cylinders in the car engine (discrete).  
3. **displacement**: Engine displacement in cubic inches (continuous).  
4. **horsepower**: Engine horsepower (continuous; contains missing values).  
5. **weight**: Car weight in pounds (continuous).  
6. **acceleration**: Time to accelerate from 0 to 60 mph (continuous).  
7. **model year**: Year the car model was released (discrete).  
8. **origin**: Country of origin (categorical: 1 = USA, 2 = Europe, 3 = Japan).  
9. **car name**: String identifier for the car model (categorical, not used in modeling).

---

## 3. Objectives
- **Exploratory Data Analysis (EDA)**: Understand the dataset, visualize relationships, and clean missing values.  
- **Feature Engineering**: Transform raw attributes into meaningful features.  
- **Model Development**: Build and evaluate regression models to predict MPG based on car specifications.  
- **Insights**: Identify the most impactful features influencing fuel consumption.

---

## 4. Project Workflow
1. **Data Loading and Preprocessing**:
    - Handle missing values in the `horsepower` attribute.  
    - Normalize continuous features like `displacement`, `weight`, and `acceleration`.  
    - Encode categorical features such as `origin` and `model year`.

2. **Exploratory Data Analysis (EDA)**:
    - Visualize relationships between `mpg` and other attributes.  
    - Study feature correlations and their influence on `mpg`.  

3. **Modeling**:
    - Use machine learning models such as:
        - Linear Regression  
        - Random Forest Regressor  
    - Perform hyperparameter tuning using **RandomizedSearchCV** or **GridSearchCV**.  

4. **Model Evaluation**:
    - Evaluate models using metrics like:
        - Mean Squared Error (MSE)  
        - R-squared (R²) Score  
    - Use **Cross-Validation** to ensure robust performance.

---

## 5. Installation & Setup

### Prerequisites  
Ensure the following dependencies are installed:  
- Python 3.8 or later  
- Libraries:  
    - pandas  
    - numpy  
    - matplotlib  
    - seaborn  
    - scikit-learn  

### Clone the Repository
```bash
git clone git@github.com:TA-rathnayaka/Machine-learning-project.git


