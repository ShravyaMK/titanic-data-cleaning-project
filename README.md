# Titanic Data Cleaning & Visualization Project

This project analyzes the Titanic passenger dataset to explore patterns in survival based on gender, class, age, and fare.

## What was done
- Loaded the raw Titanic dataset (891 passengers, 12 columns)
- Handled missing values:
  - Dropped the `Cabin` column (77% missing)
  - Filled missing `Age` values with the median
  - Filled missing `Embarked` values with the mode
- Checked for and confirmed no duplicate rows
- Analyzed outliers in `Fare` and connected them to passenger class
- Created visualizations using Matplotlib and Seaborn

## Key Insights
- Overall survival rate was around 38% (most passengers died)
- **Gender**: Women survived at a much higher rate than men, reflecting the "women and children first" policy
- **Class**: 1st class passengers had significantly higher survival rates than 3rd class passengers
- **Fare**: Passengers who survived generally paid higher fares, consistent with the class-survival link
- **Age**: Most passengers were young adults (20-40). Note: an artificial spike appears at the median age due to the missing-value fill method used

## Tools Used
- Python, Pandas, Matplotlib, Seaborn (via Google Colab)
