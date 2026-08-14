# Titanic Data Cleaning, Visualization & Predictive Modeling Project

This project analyzes the Titanic passenger dataset — first cleaning and visualizing it, then building a machine learning model to predict passenger survival.

## Part 1: Data Cleaning & Visualization
- Loaded the raw Titanic dataset (891 passengers, 12 columns)
- Handled missing values:
  - Dropped the `Cabin` column (77% missing)
  - Filled missing `Age` values with the median
  - Filled missing `Embarked` values with the mode
- Checked for and confirmed no duplicate rows
- Analyzed outliers in `Fare` and connected them to passenger class
- Created visualizations using Matplotlib and Seaborn

### Key Insights
- Overall survival rate was around 38% (most passengers died)
- **Gender**: Women survived at a much higher rate than men, reflecting the "women and children first" policy
- **Class**: 1st class passengers had significantly higher survival rates than 3rd class passengers
- **Fare**: Passengers who survived generally paid higher fares, consistent with the class-survival link
- **Age**: Most passengers were young adults (20-40). Note: an artificial spike appears at the median age due to the missing-value fill method used

## Part 2: Predictive Modeling Using Machine Learning
- Encoded categorical columns (`Sex`, `Embarked`) into numeric values
- Split the data into 80% training and 20% testing sets
- Trained a Logistic Regression model to predict survival
- Achieved an accuracy of approximately 80% on the test set
- Evaluated performance using a confusion matrix

### Key Insights
- The model correctly predicted deaths more often (~85%) than survivals (~73%), suggesting it is slightly more cautious about predicting survival
- A limitation of the model is that it misclassifies roughly 1 in 5 passengers; trying other algorithms (e.g., Decision Trees, Random Forest) could improve accuracy further

## Tools Used
- Python, Pandas, Matplotlib, Seaborn, Scikit-learn (via Google Colab)
