AI for Sustainable Development: Stress Detection using Wearables
🎯 Project Title
"Detecting Stress for Healthier Lives: A Wearable-based AI Solution Supporting SDG 3"

🧠 Objective
This project applies machine learning to wearable biosensor data to detect stress levels, contributing to UN Sustainable Development Goal 3 (Good Health and Well-being). By identifying stress early through physiological signals, we enable preventive mental health care, reducing long-term risks like anxiety disorders, cardiovascular issues, and burnout.

💾 Dataset
WESAD (Wearable Stress and Affect Detection)

Source: University of Augsburg

Devices Used: Empatica E4 wristband and RespiBAN chest sensor

Participants: 15

Signals Collected:

Electrodermal Activity (EDA)

Skin Temperature

Accelerometer

Respiration, ECG, EMG

Labels:

0 = Baseline (relaxed)

1 = Stress

2 = Amusement

🛠️ Tools & Libraries

Language: Python 3.10+

IDE: Jupyter Notebook

Libraries: pandas, numpy, scikit-learn, xgboost, matplotlib, seaborn

🔍 ML Approach
✅ Supervised Learning

Problem Formulation: Binary classification

Label 1 = Stress

Label 0 = Not Stress (Baseline or Amusement)

Model Used: Random Forest Classifier

(Alternative models tested: XGBoost, SVM, Neural Networks)

🧪 Workflow Summary

Data Preprocessing:

Loaded and normalized EDA and TEMP data

Converted multi-class labels to binary (stress vs. not stress)

Model Training:

Used 80/20 train-test split

Trained Random Forest model

Evaluation:

Confusion Matrix

Classification Report

Feature Importance Plot

📈 Results

Accuracy: ~99.9%

Key Features: EDA and Skin Temperature were most predictive

Visuals: Confusion Matrix, PCA plot, Feature Importance

⚖️ Ethical Considerations

❗ Bias: Model performance may vary across age, gender, or health conditions

💬 Privacy: Dataset is anonymized. Future deployments must follow GDPR/HIPAA

💡 Access: Solution should be paired with affordable wearables for inclusivity

🚀 Impact
This AI model supports mental health monitoring in a non-invasive and real-time manner.
Potential Use Cases:

Stress detection in high-risk jobs (nurses, pilots)

Wellness tracking apps

Preventive interventions before burnout
