# school-absence-case-study

## Authors: author: Cameron Kerkemeyer and RJ Burjek

## Investigating Cultural and Personal Factors Behind Student Absences

This case study explores the relationship between school attendance and personal, cultural, and educational traits of students. While external circumstances are often cited as the main cause of school absences, this research investigates whether internal and demographic characteristics—such as **race, gender, learning ability, and school level**—also contribute significantly to school absenteeism.

The study uses data originally collected by **Susan Quine (1973)** on Australian Aboriginal and white students. For each student, the dataset includes their **cultural background**, **gender**, **school level**, **learning classification**, and **number of absences** during a school year.

---

## Objectives

- Determine if **race**, **gender**, **school level**, and **learner type** are statistically significant predictors of school absenteeism.
- Explore interaction effects among variables.
- Build and evaluate statistical models using various techniques.
- Validate models through diagnostic testing and transformation.

---

## Methods Used

- Linear Regression Modeling
- Type-III ANOVA
- Interaction Effect Analysis
- Model Diagnostics:
  - Q-Q Plots
  - Residual vs. Fitted Plots
  - Shapiro-Wilk Test
  - Bonferroni Outlier Detection
  - Cook’s Distance
- Box-Cox Transformations
- Tukey’s Honest Significant Difference (HSD) Test
- Stepwise Shrinkage for Model Selection

---

## Tools & Technologies

- **R / RStudio** for statistical analysis
- **ggplot2** for visualization
- Base R packages for modeling and diagnostics

---

## Key Findings

- **Race** had a statistically significant effect on absence rates, with non-Aboriginal students typically having fewer absences.
- **Interaction effects** (e.g., between race and gender or school level) were explored, but many were not statistically significant.
- **Final model** used a transformed response variable:  
  \[(\text{Absence} + 1)^{-1}\]  
  With predictors: **race + gender + learner type + school level**
- The model met assumptions after transformation and provided reasonable predictive accuracy.
- Additional data could improve generalizability and model robustness.

---

## Project Structure

- **Data:**  Raw and cleaned data files
- **Plots:** Generated visualizations
- **Summary:** Final write-up or R Markdown reports


---

## Takeaways

- Cultural background can significantly affect a student’s ability to consistently attend school.
- Race was the most impactful predictor in this dataset.
- Other variables (like gender and learner type) contributed to a lesser extent.
- Model refinement and testing with more diverse datasets is recommended for future work.

---

## Acknowledgments

- Data Source: *Susan Quine, 1973*
- Study conducted as part of a college-level case study in statistical modeling and inference.

