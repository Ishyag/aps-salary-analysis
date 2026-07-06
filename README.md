# aps-salary-analysis
# APS Salary Analysis by Job Category and Inferred Gender

## Project Overview
This project analyzes publicly available Albuquerque Public Schools salary data to explore salary patterns by job category and inferred gender.
Because APS salary data does not report employee gender, this project infers likely gender from first names. The results should be interpreted as exploratory, not definitive.

## Research Question
How do APS salaries differ by inferred gender, and how much do those differences vary across job categories?

## Tools Used
- Python
- pandas
- matplotlib
- Google Colab
- Google Sheets
- GitHub

## Data Source
The data comes from the Albuquerque Public Schools employee salary information page. The original dataset includes employee name, position description, and annual salary.

## Methods
The data was copied into Google Sheets, downloaded as a CSV, and cleaned in Python using pandas. Salary values were converted into numeric format, employee first names were extracted, and job titles were grouped into broader job categories using keyword-based rules.
Likely gender was inferred from first names. Names that were ambiguous, gender-neutral, or not found were labeled as unknown and excluded from the main likely male/likely female salary comparisons.

## Key Findings
- Likely female employees had a slightly higher average salary than likely male employees.
- Likely female employees also had a higher median salary.
- Salary differences varied across job categories.
- The largest male-higher average salary gaps appeared in Administrator, Office, and Secretary/Clerk roles.
- The largest female-higher average salary gaps appeared in Student Support, Transportation, and Teacher roles.
- Likely female and likely male employees were concentrated in different types of jobs.

## Limitations
This project has several limitations. Gender was inferred from first names and may misclassify individuals. The dataset does not include years of experience, education level, full-time or part-time status, contract length, school assignment, overtime, or extra-duty pay. Job categories were also created using keyword-based rules, so some roles may have been grouped imperfectly.
Because of these limitations, the findings should be interpreted as exploratory rather than proof of unequal pay.

## Files
- `APS_salary_Code.ipynb`: Full Google Colab notebook
- `aps_salary_final_dataset.csv`: Cleaned dataset
- `overall_gender_salary_summary.csv`: Overall salary summary
- `salary_gap_by_job_category.csv`: Salary gap by job category
- `figures/`: Project graphs

## Conclusion
Overall, this project found that APS salary patterns by inferred gender are more complex than a single average salary comparison. Likely female employees had a slightly higher average and median salary overall, but salary differences varied across job categories. The results suggest that occupational sorting, or differences in which roles inferred gender groups are concentrated in, may help explain overall salary patterns.
