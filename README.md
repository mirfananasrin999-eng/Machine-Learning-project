### Dataset Overview & Data Understanding

The dataset contains patient health and clinical measurements with 918 rows and 12 columns. There are no missing values in the 
numerical columns.  

### Target Variable (HeartDisease): Approximately 55.34% of the records belong to class 1 (presence of heart disease), while 44.66% belong to class 0. 

Key Statistics:Age: Ranges from 28 to 77 years (Average: 53.51 years). 

RestingBP: Ranges from 0 to 200 mm Hg (Average: 132.40). 

Cholesterol: Ranges from 0 to 603 mm/dl (Average: 198.80).   

MaxHR: Ranges from 60 to 202 (Average: 136.81). 
### Data CleaningDuplicates & Missing Values: 
Checked using hr.duplicated().sum() and hr.isnull().sum(). The dataset contains no duplicate rows and no missing values.    

### Exploratory Data Analysis (EDA) & Visualizations

① Heart Disease DistributionVisualization: A count plot showing the target class frequency.   Insight: Out of all the patients, around 490 have heart disease, and around 410 do not, indicating that patients with heart disease are slightly higher in number.

② Age vs. Heart DiseaseVisualization: A histogram with KDE (sns.histplot) mapping age distribution split by heart disease status.   Insight: Most patients diagnosed with heart disease are concentrated between 55 and 65 years old, whereas patients without heart disease are more commonly seen between 40 and 55 years old. This shows that heart disease frequency increases with age in this dataset.   

③ Chest Pain Type vs. Heart DiseaseVisualization: A count plot breaking down chest pain types (ATA, NAP, ASY, TA) against the target variable.   Insight: Patients with heart disease are mostly found in the ASY (Asymptomatic) category, while patients without heart disease are predominantly in the ATA (Atypical Angina) and NAP (Non-Anginal Pain) categories.

④ Cholesterol Distribution by Heart DiseaseVisualization: A box plot comparing cholesterol levels across heart disease classes.   Insight: The median cholesterol level is roughly 225 for patients without heart disease and 220 for patients with heart disease.   Project SummaryGoal: Predict the presence of heart disease using clinical attributes and Logistic Regression.   Status: Objectives, exploratory analysis, and feature visualization steps have been successfully mapped out and executed in your notebook structure.
