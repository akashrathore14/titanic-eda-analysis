# 🚢 Titanic Dataset Analysis (EDA)

An exploratory data analysis of **891 Titanic passengers** to find the factors that affected survival, built with Python (Pandas, NumPy, Matplotlib, Seaborn).

> 💼 **Internship Project:** This project was completed as **Task 2 (Exploratory Data Analysis)** during my **Data Analytics & Data Science with Python internship at Softnexis Technologies**.
(Data Analysis & Science with Python Task)
---

## 🏢 Internship Context

This project was completed as part of my internship at **Softnexis Technologies**. The assigned task was to perform a complete Exploratory Data Analysis (EDA) on a real-world dataset, covering:

- Data inspection, summary statistics and missing value handling
- Distribution analysis of numerical and categorical features
- Correlation and relationship analysis
- Outlier detection using the z-score method
- Advanced visualizations (faceted plots and pairplot)
- Insight extraction and a final written conclusion

The Titanic dataset was used because it contains mixed data types, which makes it well suited to demonstrating these EDA skills.

---

## 📌 Project Overview

This analysis studies passenger age, fare, gender, class and family size to understand **who survived the Titanic disaster and why**. It covers distribution analysis, correlation analysis, outlier detection and advanced visualizations, with a written conclusion for each chart and an overall conclusion at the end of the notebook.

**Key question:** *Which passenger characteristics were most strongly linked to survival?*

---

## 📂 Repository Structure

```
├── Titanic-Dataset.csv                                   # Dataset (891 rows × 12 columns)
├── Tiatanic_dataset_analysis.ipynb                       # Jupyter notebook with full analysis
├── Titanic_Dataset_Analysis_-_Overall_Conclusion.pdf     # Summary report of findings
├── DA & DS with python task - 2.pdf                      # Task guide (Softnexis Technologies)
├── Data Source.txt                                       # Dataset source link
└── README.md
```

---

## 🗃️ Dataset Description

**Source:** [Kaggle – Titanic Dataset](https://www.kaggle.com/datasets/yasserh/titanic-dataset)

The dataset (`Titanic-Dataset.csv`) has **891 passenger records and 12 columns**.

| Column | Description |
|---|---|
| `PassengerId` | Unique passenger ID |
| `Survived` | Survival (0 = No, 1 = Yes), the target column |
| `Pclass` | Passenger class (1, 2 or 3) |
| `Name` | Passenger name |
| `Sex` | Male / Female |
| `Age` | Age in years |
| `SibSp` | Number of siblings/spouses aboard |
| `Parch` | Number of parents/children aboard |
| `Ticket` | Ticket number |
| `Fare` | Ticket fare |
| `Cabin` | Cabin number |
| `Embarked` | Port of embarkation |

---

## 🧹 Data Preparation

- `Age`: 177 missing values filled with the **median**
- `Embarked`: 2 missing values filled with the **mode**
- `Cabin`: 687 missing values marked as **"Unknown"**
- No missing values remain after cleaning

---

## 🔎 Analysis Covered

1. **Distribution analysis:** age distribution, fare by class, survival by gender
2. **Correlation and relationships:** correlation heatmap and class vs survival cross-tabulation
3. **Outlier detection:** fare distribution and z-score method
4. **Advanced visualizations:** faceted analysis (age by class and survival) and pairplot

---

## 🔍 Key Findings

| Dimension | Result |
|---|---|
| **Overall survival** | About 38.4% of passengers survived |
| **Gender** | Male: 109 survived, 468 did not. Female: 233 survived, 81 did not |
| **Passenger class** | Class 1: 63.0% survived, Class 2: 47.3%, Class 3: 24.2% |
| **Correlation** | Pclass vs Survived: -0.34, Fare vs Survived: 0.26, Pclass vs Fare: -0.55 |
| **Fare** | Mean fare 32.20, heavily right-skewed; 20 outliers by z-score (above about 180) |
| **Age** | Most passengers aged 20 to 35; very weak link to survival (-0.065) |
| **Family size** | SibSp (-0.035) and Parch (0.082) have very weak links to survival |

---

## ✅ Conclusion

Being female and travelling in a higher class gave the best chance of survival, while male and Class 3 passengers had the lowest. Fare mainly reflects class, and age and family size had little effect on their own.

**Limitations:** missing ages were filled with the median, which creates an artificial peak at about 28 years, and correlation shows a relationship, not a cause.

---

## 🛠️ Tools & Libraries

- **Python 3**
- **Pandas** and **NumPy** for data manipulation
- **Matplotlib** and **Seaborn** for visualization
- **Jupyter Notebook**

---

## ▶️ How to Run

1. Clone the repository
   ```bash
   git clone https://github.com/akashrathore14/titanic-eda-analysis.git
   cd titanic-eda-analysis
   ```
2. Install the required libraries
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```
3. Launch the notebook
   ```bash
   jupyter notebook Tiatanic_dataset_analysis.ipynb
   ```
   Keep `Titanic-Dataset.csv` in the same folder as the notebook.

---

## 👤 Author

**Akash Rathore**

---

⭐ If you found this project useful, consider giving it a star!
