# Project Title
---
## Analyzing Laboratory and Demographic Data to Predict Hepatitis C Risk Factors
---
## Introduction
This project aims to explore and analyze a dataset containing demographic information and laboratory test results for blood donors and Hepatitis C patients. Hepatitis C is a significant global health issue, and understanding its risk factors through data analysis can lead to early detection, better management, and prevention strategies.

The project's objectives are to:

- Understand patterns and correlations in demographic and test values.
- Identify key differences between healthy individuals and Hepatitis C patients.
- Predict outcomes and potential trends for the next year using the data.

## Dataset Source
The dataset used in this project, titled "HCV Data", is publicly available from the UCI Machine Learning Repository, a well-known resource for datasets widely used in machine learning and data analysis.

## Tools
- Excel-Data cleaning
- Python-Mining and crapping of data
- PowerBI-Creating reports
- SQL Server-Data analysis

## Data Cleaning and Preparation
- Handle Missing Data
- Data Normalization
- Outlier Detection

## Exploratory Data Analysis (EDA) Questions
1. What is the distribution of age among the different categories?
age_distribution_by_category.png
3. How do ALT and AST levels vary across categories?
4. What is the correlation between ALT and Bilirubin levels?
5. What is the gender distribution among Hepatitis C patients and blood donors?
6. How do cholesterol levels vary with age?

## Data Analysis
```python
import pandas as pd
data_source_url = "https://archive.ics.uci.edu/dataset/571/hcv+data"

print("Dataset sourced from:", data_source_url)

file_path = "hcvdat.csv" 
data = pd.read_csv(hcvdat.csv)
print("Preview of the dataset:")
print(data.head())
```
## Analysis of Results
Based on the charts, the following insights can be derived as follows:

1. __Age Distribution by Category__
__Observations:__
  - Blood donors are predominantly in the 20–40 age range
  - Hepatitis C patients are generally older, with a significant number in the 50+ age group.

__Implication:__
  - Age is a significant factor in Hepatitis C prevalence, likely due to cumulative exposure to risk factors or age-related vulnerabilities in liver health.

2. __ALT and AST Levels by Category__
__Observations:__
  - Blood donors have ALT and AST levels within the normal range.
  - Hepatitis C patients exhibit a broader and elevated range for both enzymes, with several extreme outliers.

__Implication:__
  - Elevated ALT and AST levels are strong biomarkers of liver dysfunction, making them reliable indicators for screening and diagnosis of Hepatitis C.

3. __Correlation Between ALT and Bilirubin Levels__
__Observations:__
  - A positive correlation exists between ALT and Bilirubin levels, particularly among Hepatitis C patients.
  - Blood donors cluster in the lower range for both markers, while Hepatitis C patients show higher values.

__Implication:__
  - This correlation confirms the clinical relevance of ALT and Bilirubin as co-indicators of liver health, with elevated levels suggesting liver damage or dysfunction common in   Hepatitis C.

4. __Gender Distribution by Category__
__Observations:__
  - Blood donors show a relatively balanced gender distribution, with a slight male majority.
  - Among Hepatitis C patients, males outnumber females significantly.

__Implication:__
  - Males may have a higher risk of Hepatitis C, potentially due to behavioral factors (e.g., lifestyle, occupational exposure) or biological differences.

## Recommendations
1. __Targeted Screening Programs:__
  - Focus on individuals over 50 years of age, particularly males, as they appear more vulnerable to Hepatitis C based on the analysis.
  - Include liver enzyme tests (ALT and AST) and Bilirubin as standard biomarkers in routine health checkups for at-risk populations.

2. __Health Awareness Campaigns:__
  - Educate the public, especially older age groups and males, about the risk factors and symptoms of Hepatitis C.
  - Promote routine testing in regions or professions with higher exposure risks.

3. __Improved Diagnostics:__
  - Leverage ALT, AST, and Bilirubin levels in conjunction for early detection of liver damage, enabling earlier interventions.
  - Consider machine learning models to predict Hepatitis C risk based on demographic and laboratory data.

4. __Gender-Specific Interventions:__
  - Investigate the higher prevalence in males and design interventions targeting behavioral or occupational risks specific to them.

5. __Longitudinal Studies:__
  - Encourage follow-up studies to analyze trends over time, exploring how risk factors evolve with age and other demographic factors.

## Conclusion and Future Actions
The analysis highlights critical patterns that can guide preventive strategies and diagnostic protocols for Hepatitis C. By integrating the recommendations, healthcare providers can enhance early detection, reduce disease progression, and tailor interventions to high-risk groups. Future actions should focus on predictive modeling, public health initiatives, and addressing the limitations in dataset representativeness


