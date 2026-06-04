# EDA — Global Mental Health Dataset

## Overview
This project explores a global mental health dataset using Python to investigate
treatment-seeking behaviour across demographic and occupational groups. The analysis
combines rigorous data cleaning with multivariate EDA and interactive visualisations
to map the patient journey from family history and stress to treatment outcomes.

**Author**: Ruth Gezahegn, Medical Student
**Date**: March 2026
**Dataset**: Global Mental Health Survey Dataset

## Tools & Libraries
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Plotly

## Skills
- Data Cleaning & Clinical Validation
- Multivariate EDA
- Interactive Visualisation
- Data Storytelling

## Data Cleaning
- Identified and filled 5,202 missing values in `self_employed` with `'Unknown'` to preserve dataset size and avoid bias
- Detected and removed 363 duplicate rows from 292,364 total entries
- Converted `Timestamp` from string (object) to `datetime64[ns]` for temporal consistency
- Flagged clinical anomalies including "Male Housewife" entries as data quality concerns

## Exploratory Data Analysis
- Univariate distributions across `family_history`, `Growing_Stress`, `Occupation`, `Mood_Swings`, `treatment`, and more
- Derived `Clinical_Profile` feature stratifying respondents into **Chronic Seekers**, **New Seekers**, and **Non-Seekers**
- Interactive Plotly Parallel Categories Diagram mapping the full clinical pathway:
  `Family History → Growing Stress → Coping Struggles → Treatment Seeking`

## Key Findings
- Identified a **"Resilience Gap"** — a high-risk population experiencing growing stress and coping struggles who are not accessing professional care
- The **"New Seeker"** phenomenon: a significant group with no family history entering treatment, driven by situational stressors rather than chronic or hereditary factors
- Family history alone is insufficient as a screening criterion for mental health needs
- Coping struggles emerge as a key gateway variable between stress and treatment-seeking

## Conclusion
This EDA transforms raw survey data into a cohesive clinical narrative. By moving
beyond isolated statistics into pattern recognition and multivariate flow analysis,
the project identifies actionable intervention points for improving mental health
accessibility and patient care.
