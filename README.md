# INFLAMMATORY-BOWEL-SYNDROME-SURVEY-DATA
Data Cleaning and Preprocessing Summary

This notebook documents the complete data cleaning and preprocessing workflow performed on a cross-sectional survey dataset comprising 320 participants. The primary objective was to transform the raw Google Forms data into a structured, analysis-ready dataset while maintaining data integrity and ensuring reproducibility.

The preprocessing began with an initial inspection of the dataset, including variable names, data types, missing values, and overall dataset structure. Personally identifiable information (participant names) was removed to preserve confidentiality. Demographic variables were standardized by retaining predefined age groups and categorizing the free-text occupation responses into meaningful occupational categories.

Survey responses from the Perceived Stress Scale (PSS-10) were converted into numeric format using the original 0–4 scoring system, allowing subsequent computation of stress scores. Variable names were simplified to concise, descriptive labels to improve code readability and facilitate interpretation during exploratory data analysis.

Clinical variables related to abdominal pain and abdominal distension were carefully cleaned using questionnaire skip logic. Participants reporting the absence of symptoms had follow-up fields appropriately coded (e.g., no pain, zero pain days, no distension), whereas genuine missing responses among symptomatic participants were preserved as missing values. Free-text entries describing pain duration were standardized, numeric values were extracted, and implausible responses exceeding the questionnaire's specified 10-day reference period were treated as missing.

Data consistency was verified through cross-tabulations, frequency distributions, and manual inspection of remaining missing observations. The final cleaned dataset retains all eligible participants while preserving genuine missing values, providing a transparent and statistically appropriate foundation for exploratory data analysis, visualization, and subsequent inferential statistical analyses.
