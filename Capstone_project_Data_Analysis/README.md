# AI Capstone Project: Titanic Survival Analysis

This project focuses on data cleaning, analysis, and feature engineering for the Titanic dataset to gain insights into survival rates. Below are the steps and detailed instructions for the project.

## 1. Dataset Loading and Basic Inspection
**Task**: Load the dataset using Pandas and inspect the basic structure.
- Load the CSV file using `pd.read_csv()`.
- Inspect the dataset using `df.head()`, `df.info()`, and `df.describe()`.
- Understand the types of features available (categorical vs. numerical).

## 2. Data Cleaning
**Task**: Handle missing values and deal with incorrect or inconsistent data.
- Identify missing values using `isnull().sum()`.
- For "Age" and "Fare", use imputation strategies (fill missing values using the median).
- Handle missing data in "Cabin" and "Embarked" columns (drop or fill with appropriate values).
- Convert categorical columns (e.g., "Sex", "Embarked") into numerical form using `pd.get_dummies()`.

## 3. Exploratory Data Analysis (EDA)
**Task**: Perform EDA using visualizations and statistical analysis.
- Use `Seaborn` and `Matplotlib` for visualizations.
  - Bar plots: Visualize survival rates across different classes and gender.
  - Histograms: Plot distributions for "Age" and "Fare".
  - Box plots: Show spread and outliers in "Age" and "Fare".
  - Heatmaps: Display a correlation matrix with `sns.heatmap()`.
  - Pair plots: Explore pairwise relationships using `sns.pairplot()`.

## 4. Feature Engineering
**Task**: Create new features to enrich the dataset.
- Combine "SibSp" and "Parch" to create a new feature `FamilySize = SibSp + Parch + 1`.
- Create a feature `IsAlone` (1 if `FamilySize == 1`, 0 otherwise).
- Group passengers into age buckets using `pd.cut()`.
- Create bins for fare prices using `pd.qcut()`.

## 5. Data Analysis and Insights
**Task**: Analyze relationships between features and the target variable.
- Compare survival rates by gender, passenger class, age, and fare.

## 6. Statistical Insights
**Task**: Provide statistical insights and hypothesis testing.
- Use NumPy to calculate statistical metrics (mean, median, etc.).
- Perform hypothesis testing on passenger class and survival rates.

## 7. Conclusion and Reporting
**Task**: Summarize findings and present key insights.
- Highlight key takeaways from the analysis.
- Include visualizations and analysis results in the summary report.

## Expected Outcomes
- Hands-on experience with real-world datasets.
- Skills in data cleaning, preprocessing, and analysis using Pandas, NumPy, Seaborn, and Matplotlib.
- Creation of new features through feature engineering.

