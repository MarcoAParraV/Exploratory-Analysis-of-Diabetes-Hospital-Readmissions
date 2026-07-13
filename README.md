# Exploratory-Analysis-of-Diabetes-Hospital-Readmissions
Exploratory analysis of diabetes hospital readmissions, focused on identifying factors associated with 30-day readmission through data cleaning, visualization, and subgroup analysis.

# Exploratory Analysis of Diabetes Hospital Readmissions

This project presents an exploratory data analysis of hospital readmissions among patients with diabetes. The main goal is to identify patterns associated with 30-day readmission after discharge and generate practical insights for clinical and operational decision-making.

## Project Description

The analysis uses the **Hospital Readmissions** dataset from the UCI Machine Learning Repository. The dataset contains more than 100,000 diabetes-related hospital encounters from 130 U.S. hospitals between 1999 and 2008.

This project explores questions such as:

- Which patient groups should receive higher priority for post-discharge follow-up?
- Is prior healthcare utilization associated with a higher risk of readmission?
- Are medication changes during hospitalization related to readmission rates?
- Which variables can serve as practical signals for transitional-care planning?

## Analysis Overview

The notebook includes a complete exploratory workflow:

- Loading and cleaning the dataset.
- Handling missing values represented as `?`.
- Creating derived variables, such as 30-day readmission and total prior visits.
- Summarizing numeric and categorical variables.
- Visualizing readmission timing, age distribution, length of stay, and prior healthcare utilization.
- Examining relationships between readmission and clinical or operational variables.
- Analyzing subgroups by age, medication status, A1C result, and discharge destination.
- Investigating heterogeneity, confounding, and possible Simpson’s paradox patterns.
- Exploring the relationship between length of stay and number of medications.

## Key Findings

Approximately 11% of hospital encounters resulted in a readmission within 30 days. Prior healthcare utilization appears to be one of the clearest risk signals: patients with more previous outpatient, emergency, or inpatient visits tend to have higher readmission rates.

Medication changes during hospitalization are associated with a higher readmission rate, but this should not be interpreted as direct causation. A more plausible explanation is that medication changes reflect greater clinical complexity or patients who were harder to stabilize.

Discharge destination also changes how readmission rates should be interpreted. Patients discharged to home health care, skilled nursing facilities, or transfer settings may show higher readmission rates because they already represent more fragile or clinically complex cases.

## Conclusion

This project is not intended to build a final predictive model. Instead, it provides an exploratory risk map to support hospital decision-making. The findings suggest that diabetic patients with high prior healthcare utilization should receive special attention before and after discharge, such as follow-up calls, medication review, and scheduled appointments.

The analysis also emphasizes the importance of distinguishing association from causation. Variables such as medication changes, discharge destination, and length of stay may be associated with readmission because they reflect higher clinical severity, not necessarily because they cause readmission.

## Project Files

- `diabetes_readmissions_eda1.ipynb`: main notebook containing the exploratory analysis and visualizations.
- `Análisis_Avanzado_de_Datos.pdf`: written report with interpretation, findings, hypotheses, and methodological reflection.

## Technologies Used

- Python
- Pandas
- NumPy
- Seaborn
- Matplotlib
- Jupyter Notebook
