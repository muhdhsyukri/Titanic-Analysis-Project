# Titanic Survival Analysis

## Introduction
This project analyzes the Titanic dataset to explore factors influencing passenger survival rates during the tragic sinking of the RMS Titanic in 1912. Using Python and its powerful data analysis libraries such as Pandas, Matplotlib, and Seaborn, the analysis focuses on answering specific questions about survival rates and their relationship to factors like passenger class, gender, age, and more.

The project includes:
- Data preprocessing and cleaning.
- Exploratory data analysis with meaningful visualizations.
- Insights derived from survival trends.

---

## Dataset Information
- **Source**: [Titanic Dataset](https://github.com/pandas-dev/pandas/blob/main/doc/data/titanic.csv)
- **Features**:
  - `Survived`: Survival status (1 = Survived, 0 = Did not survive).
  - `Pclass`: Passenger class (1 = First class, 2 = Second class, 3 = Third class).
  - `Sex`: Gender of the passenger.
  - `Age`: Age of the passenger.
  - `SibSp`: Number of siblings/spouses aboard.
  - `Parch`: Number of parents/children aboard.
  - `Fare`: Ticket fare.
  - `Embarked`: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton).

---

## Questions Answered
1. What percentage of passengers survived?
2. How do survival rates differ by passenger class?
3. Were women more likely to survive than men?
4. Did age influence survival rates?
5. What was the impact of family size on survival?
6. How did embarkation points affect survival rates?

---

## Key Findings and Insights

1. Overall Survival Rate
- **38% of passengers survived** the Titanic disaster.

2. Survival Rates by Gender
- **Women** had a significantly higher survival rate (**74%**) compared to men (**19%**).
 
I added three graph visualization regarding the issue:

1. Survival rates by gender
2. Survival rates by age group
3. Survival rates by embarking points

### 3. Survival Rates by Passenger Class
- **First-class passengers** had the highest survival rate (**63%**), followed by second-class (**47%**) and third-class (**24%**).

### 4. Age and Survival
- Younger passengers had a better chance of survival. Many survivors were children.
- Age distribution shows that older passengers had a lower survival rate.

### 5. Family Size and Survival
- Passengers traveling with small families (1–3 family members) had higher survival rates.
- Traveling alone significantly reduced survival chances.

**Visualization**:  


### 6. Embarkation Point and Survival
- Passengers who embarked at **Cherbourg (C)** had the highest survival rate (**55%**).
- Survival rates for Queenstown (Q) and Southampton (S) were **39%** and **33%**, respectively.

---

## Project Structure
The project is divided into the following sections:

### 1. Data Loading
- Load the dataset using Pandas and preview its structure.

### 2. Data Preprocessing
- Handle missing values:
  - Fill missing `Age` values with the median.
  - Drop rows with missing `Embarked` values.
- Encode categorical variables (`Sex` and `Embarked`) for analysis.
- Add new features:
  - **FamilySize**: Number of family members aboard.
  - **IsAlone**: Indicator for passengers traveling alone.

### 3. Exploratory Data Analysis (EDA)
- Analyze survival trends by gender, passenger class, age, family size, and embarkation point.
- Visualize findings using Matplotlib and Seaborn.

### 4. Insights
- Derive actionable insights from the analysis and answer predefined questions.
