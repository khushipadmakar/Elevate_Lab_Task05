# Elevate_Lab_Task05
#  Titanic Dataset Exploratory Data Analysis (EDA)

This project focuses on performing exploratory data analysis (EDA) on the **Kaggle Titanic dataset** to understand key factors influencing survival, using Python and popular data visualization libraries.

---

## Objective

To explore the Titanic dataset and identify patterns, trends, and relationships among features that contributed to passenger survival.

---

## 🗂Dataset Overview

The dataset includes details such as:

- **Survived**: Survival (0 = No, 1 = Yes)
- **Pclass**: Passenger class (1 = 1st, 2 = 2nd, 3 = 3rd)
- **Name**, **Sex**, **Age**
- **SibSp**: Siblings/Spouses aboard
- **Parch**: Parents/Children aboard
- **Ticket**, **Fare**, **Cabin**, **Embarked**

---

## 🔧 Tools & Libraries Used

- Python 3.x
- pandas
- numpy
- seaborn
- matplotlib

---

##  Steps Performed

### 1.  Data Overview
- Used `.info()`, `.describe()`, `.head()` to understand data structure and missing values.

### 2.  Data Cleaning
- Handled missing values (`Age`, `Cabin`, `Embarked`).
- Converted categorical columns (`Sex`, `Embarked`) using encoding or dummy variables.

### 3.  Visualizations

#### a. `sns.heatmap()`  
- **Used for**: Finding correlations between numerical features.  
- **Observation**: Strong positive correlation between `Fare` and `Survived`.

#### b. `sns.pairplot()`  
- **Used for**: Pairwise relationships between features.  
- **Observation**: Survivors are clustered in higher fare and lower age range.

#### c. `sns.histplot()` – Age & Fare  
- **Observation**: Most passengers were 20–40 years old; few paid high fares.

#### d. `sns.boxplot()` – Age vs Pclass  
- **Observation**: 1st class passengers were generally older than 3rd class.

#### e. `sns.countplot()` – Sex, Pclass, Embarked vs Survival  
- **Observation**: Females and 1st class passengers had higher survival rates.

#### f. `sns.violinplot()` – Fare by Class & Survival  
- **Observation**: Higher fares linked to higher survival, especially in 1st class.

#### g. `sns.scatterplot()` – Age vs Fare by Survived  
- **Observation**: Survivors are concentrated among young passengers with higher fares.

---

##  Summary of Findings

- **Gender**: Females had significantly higher survival rates.
- **Class**: 1st class passengers were more likely to survive.
- **Age**: Children and younger people had better survival chances.
- **Fare**: Higher fare indicates a better chance of survival.
- **Embarked**: Passengers from Cherbourg (C) had a higher survival rate.

---

##  How to Run

1. Clone or download this repository.
2. Install the required packages:
   ```bash
   pip install pandas matplotlib seaborn
