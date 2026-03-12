### Project Title
Data-Driven Readmission Risk Prediction for Improved Diabetes Care Coordination

**Author**
Harini Jagannathan

#### Executive summary

Hospital readmissions among diabetic patients remain a significant clinical and financial challenge, particularly under value-based care models where avoidable readmissions can lead to penalties and increased total cost of care. This project develops and evaluates machine learning models using demographic, clinical, and utilization data available at discharge to identify patients at elevated risk of unplanned 30-day hospital readmission.

Exploratory data analysis and feature engineering highlighted that prior healthcare utilization, inpatient history, medication burden, and age are key indicators of readmission risk, reflecting overall patient complexity and care intensity. Multiple classification models were evaluated including Logistic Regression, Decision Trees, Random Forest, Gradient Boosting, and K-Nearest Neighbors with performance assessed using accuracy, recall, and ROC-AUC. Among these models, Gradient Boosting demonstrated the strongest overall performance, while Random Forest achieved the highest recall, indicating its effectiveness in identifying patients who were actually readmitted.

Model interpretability techniques such as SHAP analysis confirmed that historical healthcare utilization and treatment complexity are the most influential predictors of readmission risk. In addition, K-Means clustering was used to segment patients into risk groups, revealing distinct patient populations with different utilization patterns and readmission rates.

From a population health perspective, these findings demonstrate how machine learning can support proactive risk stratification and targeted care management. By identifying high-risk patients prior to discharge, healthcare providers can allocate resources more effectively, implement early interventions, and reduce preventable readmissions - ultimately improving patient outcomes while supporting the goals of value-based healthcare delivery.

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

To address the research question, this project applies a combination of exploratory data analysis, feature engineering, supervised machine learning, and unsupervised learning techniques. Exploratory data analysis was conducted to understand the distribution of variables and identify patterns related to hospital readmission risk. Feature engineering was then used to create clinically meaningful variables, such as measures of prior healthcare utilization and patient complexity.

Multiple supervised classification models—including Logistic Regression, Decision Trees, Random Forest, Gradient Boosting, and K-Nearest Neighbors were trained and compared to predict 30-day readmission risk. Model performance was evaluated using accuracy, recall, and ROC-AUC, with particular emphasis on recall to ensure the models effectively identify patients at high risk of readmission in a value-based care context. Hyperparameter tuning was performed to optimize model performance.

In addition, unsupervised learning using K-Means clustering was applied to segment patients into risk groups based on utilization patterns and clinical characteristics. Finally, SHAP (SHapley Additive Explanations) was used to interpret model predictions and identify the most influential factors driving readmission risk.

#### Results
What did your research find?

The analysis found that patient readmission risk is strongly associated with prior healthcare utilization and indicators of clinical complexity. Variables such as total prior visits, inpatient history, medication burden, and age were among the most influential predictors of 30-day readmission, suggesting that patients with higher healthcare utilization and more complex care needs are more likely to be readmitted.

Among the models evaluated, Gradient Boosting demonstrated the strongest overall predictive performance, achieving the highest ROC-AUC, while Random Forest achieved the highest recall, meaning it identified the largest proportion of patients who were actually readmitted. Simpler models such as Logistic Regression and Decision Trees showed moderate performance, while K-Nearest Neighbors performed less effectively for this dataset.

In addition to predictive modeling, unsupervised clustering identified distinct patient segments with different utilization patterns and readmission rates. One cluster showed significantly higher prior healthcare utilization and the highest readmission rate, highlighting a group of patients who may benefit most from targeted care management interventions. Overall, the findings demonstrate that machine learning can help identify high-risk patients and support proactive strategies to reduce avoidable hospital readmissions.

#### Next steps
What suggestions do you have for next steps?

Future work could incorporate additional data such as comorbidities, medication adherence, and social determinants of health to improve prediction accuracy. Further model development could explore advanced approaches such as deep neural networks or additional boosting algorithms, along with expanded hyperparameter tuning and validation across multiple datasets. Finally, integrating the model into clinical workflows for discharge planning and care management could help healthcare providers identify high-risk patients earlier and support targeted interventions to reduce avoidable readmissions.

#### Outline of project

- Click [here](https://github.com/hjag038/hospital_readmission_risk/blob/main/hospital_readmission_risk.ipynb) to access the Jupyter notebook


##### Contact and Further Information

Thank you for reviewing this project. I welcome feedback, collaboration opportunities, and discussions related to healthcare analytics, applied machine learning, and value-based care.

Author: Harini Jagannathan

Focus Areas: Healthcare Analytics | Applied AI/ML | Population Health | Risk Stratification
