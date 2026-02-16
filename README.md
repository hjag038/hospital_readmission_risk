### Project Title
Data-Driven Readmission Risk Prediction for Improved Diabetes Care Coordination

**Author**
Harini Jagannathan

#### Executive summary

Hospital readmissions among diabetic patients represent a significant clinical and financial challenge, particularly under value-based care models where avoidable readmissions may result in penalties and increased total cost of care. This project aimed to develop a predictive model using demographic, clinical, and utilization data available at discharge to identify patients at elevated risk of 30-day readmission.

Exploratory data analysis revealed that readmission risk is strongly associated with advanced age, prior inpatient utilization, length of stay, and medication burden—factors indicative of clinical complexity and care intensity. The dataset demonstrated a relatively balanced readmission outcome, enabling effective supervised modeling without aggressive resampling.

A baseline logistic regression model was developed using engineered utilization features and standardized preprocessing to prevent data leakage. The model achieved moderate discrimination (ROC-AUC ≈ 0.64), demonstrating meaningful separation between higher- and lower-risk patients. While the model showed strong performance in identifying low-risk patients, recall for readmissions indicates opportunity for improvement in capturing high-risk individuals.

From a population health perspective, the findings confirm that utilization history and treatment complexity are key drivers of readmission risk. With further optimization and refinement, this modeling approach can support proactive discharge planning, targeted care management interventions, and more efficient allocation of care coordination resources. Ultimately, predictive risk stratification can contribute to improved patient outcomes, reduced avoidable utilization, and enhanced performance under value-based reimbursement frameworks.

#### Rationale
Why should anyone care about this question?

Avoidable 30-day readmissions for diabetic patients increase healthcare costs,
strain hospital resources, and lower quality scores. Being able to identify
high-risk patients at discharge allows care teams to focus follow-up efforts where
they can have the greatest impact, improving outcomes and supporting
value-based care goals.

#### Research Question
What are you trying to answer?

Can patient demographic, clinical, and treatment data available at discharge be
used to predict the likelihood of unplanned 30-day hospital readmission among
diabetic patients?

#### Data Sources
What data will you use to answer your question?

● https://archive.ics.uci.edu/dataset/296/diabetes+130-us+hospitals+for+years+1999-2008
● https://www.kaggle.com/datasets/dubradave/hospital-readmissions/data

#### Methodology
What methods are you using to answer the question?

The methods used to answer the question involved exploratory data analysis, feature engineering, and supervised machine learning, specifically logistic regression with regularization to model 30-day readmission risk. The model was evaluated using ROC-AUC, precision, and recall, with emphasis on identifying high-risk patients in a value-based care context.

#### Results
What did your research find?

The research found that demographic, clinical, and utilization data available at discharge can meaningfully predict 30-day hospital readmission among diabetic patients, although predictive performance is moderate at baseline.

Several factors emerged as strong indicators of readmission risk:

- Prior inpatient and emergency utilization

- Longer length of stay

- Higher medication burden (polypharmacy)

- Advanced age

- Indicators of greater treatment intensity

These findings suggest that readmission risk is closely associated with patient complexity and historical healthcare utilization patterns.

The baseline logistic regression model demonstrated moderate discrimination (ROC-AUC ≈ 0.64), indicating the model performs better than random classification and can differentiate between higher- and lower-risk patients. However, recall for readmitted patients was limited, meaning the model missed a meaningful proportion of high-risk individuals. This highlights opportunities for further optimization and model refinement.

#### Next steps
What suggestions do you have for next steps?

After establishing a logistic regression baseline, I would compare non-linear models like Decision Trees and KNN, apply PCA to manage dimensionality and correlated predictors, and use K-Means clustering to uncover patient segments that support targeted care management strategies.

#### Outline of project

- Click [here](https://github.com/hjag038/hospital_readmission_risk/blob/main/hospital_readmission_risk.ipynb) to access the Jupyter notebook


##### Contact and Further Information

Thank you for reviewing this project. I welcome feedback, collaboration opportunities, and discussions related to healthcare analytics, applied machine learning, and value-based care.

Author: Harini Jagannathan
Focus Areas: Healthcare Analytics | Applied AI/ML | Population Health | Risk Stratification