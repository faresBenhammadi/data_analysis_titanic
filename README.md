# 🚢 Titanic Survival Data Analysis

A complete exploratory data analysis (EDA) of the Titanic dataset using **Python**, **Pandas**, **NumPy**, and **Matplotlib**.

The objective of this project is not to build a machine learning model, but to understand the dataset through data cleaning, visualization, and statistical analysis in order to identify the factors that influenced passenger survival.

---

## 📌 Project Objectives

This project investigates the following questions:

- Does age influence the probability of survival?
- Did women survive more often than men?
- Did passenger class affect survival?
- Does family size influence survival?
- Does the embarkation port have an impact on survival?
- Is there a relationship between ticket fare and survival?

---

## 📂 Dataset

**Dataset:** Titanic - Machine Learning from Disaster

The dataset contains information about **891 passengers**, including:

- Passenger class
- Age
- Sex
- Family relationships
- Ticket fare
- Embarkation port
- Survival status

---

## 🧹 Data Cleaning

Before performing the analysis, the dataset was inspected for potential issues.

### Missing values

| Column | Missing Values | Strategy |
|---------|---------------:|---------|
| Age | 177 | Removed only for age-related analysis |
| Cabin | 687 | Excluded from the analysis due to excessive missing values |
| Embarked | 2 | Kept as-is since it had no impact on the analyses performed |

### Categorical cleaning

The **Title** feature was extracted from the passenger names.

Equivalent titles were standardized to avoid duplicate categories:

- `Mlle` → `Miss`
- `Mme` → `Mrs`
- `Ms` → `Miss`

Different cleaning strategies were discussed depending on the objective:

- For **Machine Learning**, imputing missing values (e.g., using the median) would generally be preferred.
- For **Exploratory Data Analysis**, removing missing observations for a specific study provides more accurate descriptive results.

---

## 📊 Analyses Performed

The notebook includes the following analyses:

- Age vs Survival
- Sex vs Survival
- Passenger Class vs Survival
- Family Size vs Survival
- Embarkation Port vs Survival
- Ticket Fare vs Survival
- Passenger Title vs Survival

During the analysis, new features such as **Age Group**, **Family Size**, and **Fare Group** were created to improve interpretability.

---

## 📈 Main Findings

The analysis revealed several interesting patterns:

- Women had a significantly higher survival rate than men.
- First-class passengers were much more likely to survive.
- Age showed only a **very weak linear correlation** with survival.
- Passengers traveling in small families generally had better survival rates than those traveling alone or in very large families.
- Higher ticket fares were generally associated with higher survival rates.
- Passengers embarking from Cherbourg showed the highest survival rate among the three embarkation ports.
- Passenger titles showed strong differences in survival rates. Women-related titles (Mrs, Miss) had the highest survival rates, while Mr had the lowest among the common titles.

---

## ⚠️ Limitations

This project is an **exploratory analysis**, therefore the results should be interpreted carefully.

Some limitations include:

- Missing age values were removed during the age analysis.
- The Cabin column was not analyzed because most values were missing.
- Correlation does **not** imply causation.
- Several variables may be related (for example, passenger class and ticket fare), meaning one factor alone cannot fully explain survival.
- No predictive machine learning models were used.

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook
- KaggleHub

---

## 📚 Skills Practiced

This project helped reinforce several fundamental data analysis skills:

- Data inspection
- Data cleaning
- Feature engineering
- GroupBy operations
- Data visualization
- Correlation analysis
- Statistical interpretation
- Drawing conclusions from real-world datasets
- Regular expressions (feature extraction)
- Categorical data cleaning
- Feature engineering

---

## 🚀 Future Improvements

Possible extensions of this project include:

- Analyze the Cabin feature after extracting deck information.
- Perform multivariable analysis combining several features.
- Build predictive machine learning models (Logistic Regression, Random Forest, etc.).
- Create an interactive dashboard using Plotly or Streamlit.

---

## 👤 Author

**Benhammadi Fares Mohammed**


