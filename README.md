# Titanic-Preprocessing-Workshop
# Titanic Dataset - Data Preprocessing Workshop

## 📋 Overview
This repository contains a comprehensive data preprocessing pipeline for the famous Titanic dataset. The project demonstrates essential data cleaning, handling missing values, and feature engineering techniques using Python and pandas.

## 🎯 Objectives
- Clean and preprocess the Titanic dataset for machine learning
- Handle missing values effectively
- Perform exploratory data analysis
- Engineer new features to improve model performance
- Prepare data for survival prediction models

## 📊 Dataset
The Titanic dataset contains information about passengers aboard the RMS Titanic, including:
- **PassengerId**: Unique identifier
- **Survived**: Survival status (0 = No, 1 = Yes)
- **Pclass**: Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd)
- **Name**: Passenger name
- **Sex**: Gender
- **Age**: Age in years
- **SibSp**: Number of siblings/spouses aboard
- **Parch**: Number of parents/children aboard
- **Ticket**: Ticket number
- **Fare**: Passenger fare
- **Cabin**: Cabin number
- **Embarked**: Port of embarkation

## 🔧 Preprocessing Steps

### 1. Handle Missing Values
- **Age**: Fill with median or group median (by Pclass & Sex)
- **Cabin**: Create binary indicator feature (Has_Cabin) due to high missing values
- **Embarked**: Fill with mode (most frequent value)

### 2. Data Quality Checks
- Check for duplicate records using PassengerId and Name
- Validate data types and consistency

### 3. Feature Engineering
- **Title**: Extracted from Name (Mr, Mrs, Miss, Master, etc.)
- **FamilySize**: Calculated as SibSp + Parch + 1
- **IsAlone**: Binary feature (1 if FamilySize == 1 else 0)
- **AgeGroup**: Categorized into Child, Teen, Adult, Senior


## 🚀 Getting Started

### Prerequisites
- Python 3.7+
- Jupyter Notebook/JupyterLab

### Installation
1. Clone the repository
2. Install required packages:
```bash
pip install pandas numpy matplotlib numpy jupyter
