Overview
This project analyzes a synthetic dataset of 500 patient records to explore whether demographic and clinical variables can predict Long COVID outcomes. The dataset “includes 500 synthetically generated patient records designed to simulate post‑COVID health outcomes,” containing variables such as age, gender, COVID‑19 severity, hospitalization, physical activity, and long‑term symptoms like fatigue, breathing issues, mental health impact, and brain fog (excerpt from report).
The goal was to evaluate multiple machine learning models, compare their performance, and understand the limitations of predicting Long COVID risk using limited and imbalanced data.

Dataset
Source: Post‑COVID Health Effects Dataset (Kaggle, 2025)
Records: 500 synthetic patient profiles
Variables include:
• 	Demographics: Age, Gender
• 	COVID Experience: Severity, Hospitalization, Loss of Taste/Smell, Physical Activity
• 	Long‑Term Outcomes: Days to Recovery, Fatigue Level, Breathing Issues, Mental Health Impact, Brain Fog
• 	Target: Long COVID Risk (Low / Medium / High)
The dataset is synthetic and intended for demonstrating analytical techniques—not clinical prediction.

Methods
Supervised Models
• 	Logistic Regression
• 	Random Forest Classifier
• 	Naive Bayes
• 	Extra Trees Classifier
Unsupervised Model
• 	K‑Means Clustering with PCA visualization
Core Tasks
• 	Data cleaning & encoding
• 	Exploratory data analysis
• 	Model training & evaluation
• 	Confusion matrix interpretation
• 	Feature importance analysis

Key Findings
• 	Logistic Regression struggled to detect true positive cases for brain fog and breathing issues; ROC‑AUC values (~0.58) indicated weak predictive power.
• 	Random Forest achieved the highest accuracy (56%) but “correctly identified only one instance of high‑risk for long COVID,” heavily under‑predicting severe cases (excerpt from report).
• 	K‑Means Clustering showed significant overlap between clusters, indicating weak natural separation in the dataset.
• 	Naive Bayes & Extra Trees both achieved ~50% accuracy and showed strong bias toward the majority class.
• 	Most influential features: Days to Recovery and Age consistently ranked highest across models.
Overall, models achieved 30–56% accuracy, reflecting limited predictive signal and significant class imbalance.

Recommendations
To improve predictive performance, future datasets should include:
• 	COVID variant exposure
• 	Vaccination status
• 	Pre‑existing conditions
• 	More detailed acute‑phase symptom data
• 	Class balancing techniques (SMOTE, ADASYN, stratified sampling)

Skills Demonstrated
• 	Machine learning model development
• 	Data preprocessing & encoding
• 	Model evaluation (accuracy, precision, recall, F1, ROC‑AUC)
• 	Clustering & PCA
• 	Feature importance interpretation
• 	Technical writing & analytical communication
