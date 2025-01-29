# Heart Disease Risk Analysis Using R

## Overview
This project analyzes heart disease risk factors using R programming, focusing on gender and age. The dataset is sourced from the Cleveland database of the UCI Heart Disease dataset. Various statistical methods and visualizations were implemented to examine the relationship between gender, age, and heart attack likelihood.

## Dataset
- The dataset consists of **14 variables and 303 observations**.
- Key features include age, gender, chest pain type, blood pressure, cholesterol levels, and heart disease likelihood.
- Gender variable is renamed, and categorical variables are factored for analysis.

## Methodology
1. **Data Preprocessing**
   - Imported the dataset using `read_csv()`.
   - Converted categorical variables using `factor()`.
   - Generated summary statistics for age, grouped by gender.
   
2. **Descriptive Statistics & Visualization**
   - Computed mean, median, standard deviation, and quartiles.
   - Created histograms, boxplots, and bar plots to compare age distributions across genders.
   - Identified that females have a higher standard deviation in age and a slightly higher mean age than males.

3. **Hypothesis Testing**
   - **Chi-Square Test of Association**
     - Null Hypothesis (H₀): Gender is related to heart attack likelihood.
     - Alternative Hypothesis (H₁): Gender is not related to heart attack likelihood.
     - Result: p-value = 1.877e-06 (statistically significant), rejecting H₀.
     - Conclusion: Gender influences heart attack likelihood.

   - **Two-Sample t-Test**
     - Examined the difference in mean age between high-risk males and females.
     - Null Hypothesis (H₀): No difference in mean age between genders.
     - Result: p-value = 0.014 (< 0.05), indicating a significant difference.
     - Conclusion: Mean age of heart disease differs between genders.
     - At a stricter 0.01 confidence level, the null hypothesis is not rejected.

## Conclusion
- Gender does not directly influence heart disease likelihood, contrary to initial visualization insights.
- Age differences between high-risk males and females are statistically significant at a 0.05 confidence level but not at a 0.01 level.
- This analysis provides valuable insights into heart disease risk factors and can be further extended with additional features and machine learning techniques.

- ![Screenshot 2025-01-29 at 14 42 27](https://github.com/user-attachments/assets/382266d6-148c-4832-a9ac-f1305c988912)
- ![Screenshot 2025-01-29 at 14 44 51](https://github.com/user-attachments/assets/1ee57c3a-e60f-416f-ba8d-50c41937a342)
- ![Screenshot 2025-01-29 at 14 44 03](https://github.com/user-attachments/assets/a9a48647-1473-47f1-8c62-d2997866bd8d)
- ![Screenshot 2025-01-29 at 14 43 52](https://github.com/user-attachments/assets/42bb0e65-5fd5-45ed-9d9c-92d5adfa1bd1)
- ![Screenshot 2025-01-29 at 14 42 46](https://github.com/user-attachments/assets/f3d49474-4bac-4db7-afd7-8ece1cc9f7cc)

## Repository Structure
- `data/` - Contains the heart disease dataset.
- `scripts/` - Includes R scripts for data analysis and visualization.
- `results/` - Contains output plots and statistical summaries.

## Technologies Used
- R Programming
- `ggplot2`, `dplyr`, `tidyverse` for data analysis and visualization
- Hypothesis testing using statistical functions in R

- Install R and RStudio: Ensure R is installed from CRAN and optionally use RStudio for a better experience.

- Clone the repository:
git clone <repository-url>
cd heart-disease-analysis

- Install required packages:install.packages(c("dplyr", "ggplot2", "readr"))

- Run the analysis: Open scripts/analysis.R in RStudio and execute the script step by step.

- View results: Check the results/ directory for visualizations and statistical summaries.

## Author
Developed as part of **Semester 2 MFE 2 Project** to analyze heart disease risk factors using R programming.

