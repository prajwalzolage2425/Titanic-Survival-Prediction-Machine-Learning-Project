<div align="center">

# 🚢 Titanic-Survival-Prediction-Machine-Learning-Project

[![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=Kaggle&logoColor=white)](https://www.kaggle.com/prajwalzolage05)
[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![scikit--learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)

**End-to-end Machine Learning project to predict survival on the Titanic dataset using Random Forest**

</div>

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Features](#-features)
- [Installation](#-installation)
- [Usage](#-usage)
- [Methodology](#-methodology)
- [Results](#-results)
- [Contact](#-contact)

---

## 🎯 Overview

This repository contains a complete machine learning solution for the classic  
**Titanic Survival Prediction** problem from Kaggle.

The goal of the project is to predict whether a passenger survived the Titanic disaster
based on features such as age, gender, ticket class, fare, and family relationships.

The project focuses on:
- Clean data preprocessing
- Meaningful feature engineering
- A tuned Random Forest model
- Clear evaluation and reproducible results

---

## ✨ Features

- End-to-end ML pipeline
- Missing value handling
- Categorical feature encoding
- Feature engineering (FamilySize, IsAlone)
- Tuned Random Forest classifier
- Model evaluation with accuracy and confusion matrix
- Ready-to-submit `submission.csv` for Kaggle

---

## 🚀 Installation

### Prerequisites

- Python 3.8+
- pip
- Jupyter Notebook (optional)

### Clone Repository

```bash
git clone https://github.com/prajwalzolage2425/Titanic-Survival-Prediction.git
cd Titanic-Survival-Prediction
```

### Install Dependencies

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

---

## 💻 Usage

### Run the notebook or script

- Open the notebook in **Jupyter Notebook**, OR  
- Run the project in the **Kaggle Notebook environment**

### Generate submission file

After execution, the model generates:

```text
submission.csv
```

Upload this file directly to Kaggle.

---

## 🧠 Methodology

### Data Preprocessing

- Missing values handled using statistical techniques (median / mode)
- Categorical variables encoded using `LabelEncoder`
- Irrelevant columns removed
- Training and test datasets aligned properly

### Feature Engineering

```text
FamilySize = SibSp + Parch + 1
IsAlone    = 1 if FamilySize == 1 else 0
```

These features help capture survival patterns related to family presence.

### Model Used

```python
RandomForestClassifier(
    n_estimators=300,
    max_depth=8,
    min_samples_split=5,
    random_state=42
)
```

### Why Random Forest?

- Handles non-linear relationships
- Robust against overfitting
- Works well with mixed feature types
- Provides feature importance
- Stable and reliable for tabular data

---

## 📊 Results

| Metric | Value |
|------|------|
| Validation Accuracy | **0.8268156424581006** |
| Algorithm | Random Forest |
| Number of Trees | 300 |
| Max Depth | 8 |

### Observations

- Gender and passenger class strongly affect survival
- FamilySize improves prediction accuracy
- Random Forest provides stable and interpretable results

---

## 📧 Contact

**Prajwal Zolage**

- GitHub: https://github.com/prajwalzolage2425  
- Kaggle: https://www.kaggle.com/prajwalzolage05  

---

<div align="center">

⭐ If you found this project useful, please give it a star ⭐  
Built for learning, experimentation, and Kaggle competitions 🚀

</div>
