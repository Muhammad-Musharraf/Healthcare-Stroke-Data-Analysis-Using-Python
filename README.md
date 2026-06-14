# 🧠 Healthcare Stroke Data Analysis Using Python

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=flat-square&logo=python)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=flat-square&logo=jupyter)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=flat-square)

A data analytics project focused on examining patient health records to uncover factors contributing to stroke risk. Through systematic data cleaning, statistical analysis, and rich visualizations, this project surfaces actionable insights across key clinical indicators including age, hypertension, heart disease, BMI, glucose levels, and smoking status.

---

## 📋 Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Key Analysis Areas](#key-analysis-areas)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
- [Results & Insights](#results--insights)
- [License](#license)

---

## Overview

Stroke is one of the leading causes of death and disability worldwide. Early identification of at-risk patients can significantly improve outcomes. This project applies exploratory data analysis (EDA) techniques to a healthcare stroke dataset to:

- Understand the distribution of patient demographics and health indicators
- Identify key risk factors associated with stroke occurrence
- Visualize relationships between clinical features and stroke probability
- Provide data-driven insights that could assist clinical decision-making

---

## Dataset

The project uses the **Healthcare Stroke Prediction Dataset**, a widely referenced medical dataset containing patient health records with the following features:

| Feature | Description |
|---|---|
| `id` | Unique patient identifier |
| `gender` | Patient gender (Male / Female / Other) |
| `age` | Age of the patient |
| `hypertension` | Whether the patient has hypertension (0 = No, 1 = Yes) |
| `heart_disease` | Whether the patient has heart disease (0 = No, 1 = Yes) |
| `ever_married` | Marital status (Yes / No) |
| `work_type` | Type of employment |
| `Residence_type` | Urban or Rural residence |
| `avg_glucose_level` | Average blood glucose level |
| `bmi` | Body Mass Index |
| `smoking_status` | Smoking history (never smoked / formerly smoked / smokes / unknown) |
| `stroke` | Target variable — stroke occurred (1) or not (0) |

**Dataset size:** 5,110 patient records × 12 columns

---

## Project Structure

```
Healthcare-Stroke-Data-Analysis-Using-Python/
│
├── Dataset/
│   └── healthcare-dataset-stroke-data.csv   # Raw dataset
│
├── Project/
│   └── stroke_analysis.ipynb                # Main Jupyter Notebook
│
├── LICENSE
└── README.md
```

---

## Key Analysis Areas

**1. Data Cleaning & Preprocessing**
- Identification and handling of missing values (notably in the `bmi` column)
- Imputation of missing BMI values with the column mean to preserve stroke-positive records
- Removal of irrelevant features (e.g., patient ID)
- Data type verification and categorical encoding

**2. Exploratory Data Analysis (EDA)**
- Univariate analysis of individual features (age distribution, BMI spread, glucose levels)
- Bivariate analysis of feature relationships with stroke outcome
- Detection of class imbalance (stroke-positive vs. stroke-negative patients)

**3. Statistical Analysis**
- Descriptive statistics (mean, median, standard deviation, quartiles)
- Correlation analysis between numerical features and stroke occurrence
- Frequency distributions for categorical variables

**4. Visualizations**
- Age distribution by stroke status
- Stroke rate by hypertension and heart disease
- BMI distribution across stroke outcomes
- Average glucose level patterns
- Smoking status impact on stroke risk
- Residence type and work type breakdowns

---

## Technologies Used

| Library | Purpose |
|---|---|
| `Python 3.8+` | Core programming language |
| `Pandas` | Data loading, cleaning, and manipulation |
| `NumPy` | Numerical computations |
| `Matplotlib` | Static plots and charts |
| `Seaborn` | Statistical visualizations |
| `Jupyter Notebook` | Interactive analysis environment |

---

## Getting Started

### Prerequisites

Make sure you have Python 3.8+ and pip installed.

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Muhammad-Musharraf/Healthcare-Stroke-Data-Analysis-Using-Python.git
   cd Healthcare-Stroke-Data-Analysis-Using-Python
   ```

2. **Install required libraries**
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```

3. **Launch Jupyter Notebook**
   ```bash
   jupyter notebook
   ```

4. **Open the notebook**
   Navigate to `Project/` and open `stroke_analysis.ipynb` in your browser.

---

## Results & Insights

Key findings from the analysis include:

- **Age** is one of the strongest predictors — stroke risk increases significantly in patients over 60
- **Hypertension and heart disease** are highly correlated with stroke occurrence
- **Elevated average glucose levels** are more common among stroke patients
- **BMI** shows moderate association with stroke risk, with higher values trending toward greater risk
- **Smoking status** (formerly smoked or currently smokes) correlates with elevated stroke risk
- The dataset is **heavily imbalanced** — only ~4.9% of patients experienced a stroke, which is an important consideration for any predictive modeling

---

## License

This project is licensed under the [MIT License](LICENSE). You are free to use, modify, and distribute this project with appropriate attribution.

---

## Author

**Muhammad Musharraf**
- GitHub: [@Muhammad-Musharraf](https://github.com/Muhammad-Musharraf)

---

> *This project is intended for educational and analytical purposes only. It does not constitute medical advice.*
