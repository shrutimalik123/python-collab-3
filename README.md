
Data-Science-Readiness-Portfolio: CVS Health Data Scientist Roadmap

This repository documents my daily, practical exercises designed to master the core technical skills required for a mid-to-senior level Data Scientist role, with a specific focus on the requirements outlined by the CVS Health Data Scientist job description (Python, SQL, ML/DL, MLOps, and Healthcare Data).

Day,                   Project File,                              Skill Focus                                 ,Description
Day 1,               data_profiler.py,            "Python, Pandas, Data Cleaning, Feature Engineering",      "Simulated raw patient data, handled missing values (mean       imputation for Age, categorical fill for Diagnosis), and engineered the Mean Arterial Pressure (MAP) feature."

Day 2,            advanced_sql_sim.py,           "Python, Pandas Window Functions (SQL Simulation), Complex Data Aggregation",Simulated a complex SQL query using Pandas' .groupby().rank() method to partition and rank high-risk patients (using MAP) for targeted clinical intervention.

Day 3,           predictive_model.py,             "Machine Learning (scikit-learn), Logistic Regression, Feature Scaling, Model Evaluation, Interpretation","Trained a simple Logistic Regression model to predict patient risk (High_Risk). Focused on data splitting, standardization, evaluation, and critically, model interpretation (Feature Coefficients)."

Day 3 Results Snapshot
The Logistic Regression model was trained on the engineered features (Age, MAP, Medication_Count). This step confirms the features created in Day 1 and 2 are useful for predictive modeling.

Metric / Result	                        Insight
Model Type	               Logistic Regression (Chosen for high interpretability in clinical settings)
Data Split	               70% Train, 30% Test
Key Coefficient	           MAP had the highest positive coefficient, indicating it is the strongest predictor of high risk.
Interpretability	         Successfully isolated features driving the risk prediction, vital for compliance and explainability.

🛠️ Requirements & Setup
All scripts are written in Python and primarily use standard data science libraries:

pandas

numpy

scikit-learn

To run any script:

Bash

python <filename>.py
