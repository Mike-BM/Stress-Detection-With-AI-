🎯 Detecting Stress for Healthier Lives: A Wearable-based AI Solution Supporting SDG 3
🧠 Objective
This project applies machine learning to wearable biosensor data to detect stress levels, contributing to UN Sustainable Development Goal 3 (Good Health and Well-being).
By identifying stress early through physiological signals, we enable preventive mental health care, reducing long-term risks such as anxiety disorders, cardiovascular issues, and burnout.
________________________________________
💾 Dataset
WESAD (Wearable Stress and Affect Detection)
•	Source: University of Augsburg
•	Participants: 15 individuals wearing Empatica E4 wristband and RespiBAN chest sensor
•	Signals Collected:
o	EDA (Electrodermal Activity)
o	TEMP (Skin Temperature)
o	ACC (Accelerometer – not used in this simplified model)
•	Labels:
o	0: Baseline (Relaxed)
o	1: Stress
o	2: Amusement
For binary classification, we mapped labels as:
•	1 → Stress
•	0 → Not Stress (Baseline + Amusement)
________________________________________
🛠️ Tools & Libraries
•	Python 3.10+
•	Jupyter Notebook
•	Libraries:
o	pandas
o	numpy
o	scikit-learn
o	matplotlib
o	seaborn
o	xgboost
________________________________________
🔍 ML Approach
✅ Supervised Learning – Binary Classification
•	Features Used:
o	Electrodermal Activity (EDA)
o	Temperature (TEMP)
•	Label Mapping:
o	1 = Stress
o	0 = Not Stress
•	Primary Model Used:
o	Random Forest Classifier
•	Alternative Models Tested:
o	✅ XGBoost
o	✅ Support Vector Machine (SVM)
o	✅ Neural Networks (MLPClassifier)
________________________________________
🧪 Workflow Summary
1. Data Preprocessing:
•	Cleaned and normalized EDA and TEMP sensor readings
•	Dropped initial timestamp/noise rows
•	Combined datasets with aligned length
•	Applied KMeans clustering to simulate unsupervised labeling
•	Remapped cluster output to stress and non-stress
2. Model Training:
•	Performed 80/20 train-test split
•	Trained Random Forest Classifier
3. Evaluation:
•	Achieved 100% Accuracy
•	Visualized results using:
o	Confusion Matrix
o	PCA projection
o	EDA vs TEMP cluster scatter plot
________________________________________
📈 Results
•	Accuracy (Random Forest): 100.00%
•	Alternative Models Tested:
o	XGBoost
o	Support Vector Machine (SVM)
o	Neural Networks
•	Key Features: EDA and Temperature
•	Visuals:
________________________________________
⚖️ Ethical Considerations
•	Bias Awareness: Model may behave differently across genders, ages, and health statuses
•	Data Privacy: Dataset is anonymized; deployment must follow GDPR/HIPAA regulations
•	Accessibility: This model should be used with affordable wearable sensors to reach underserved communities
________________________________________
🚀 Impact
This AI model enables real-time, non-invasive stress monitoring and can be deployed in:
•	High-stress workplaces (e.g., nurses, pilots)
•	Corporate wellness programs
•	Personal mental health tracking
•	Preventive interventions
