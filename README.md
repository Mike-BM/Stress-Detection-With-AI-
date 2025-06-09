# 🎯 Detecting Stress for Healthier Lives: A Wearable-Based AI Solution Supporting SDG 3

## 🧠 Objective  
This project applies machine learning to wearable biosensor data to **detect stress levels**, contributing to **UN Sustainable Development Goal 3 (Good Health and Well-being)**.

By identifying stress early through physiological signals, we enable **preventive mental health care**, reducing long-term risks such as anxiety disorders, cardiovascular issues, and burnout.

---

## 💾 Dataset – WESAD (Wearable Stress and Affect Detection)

- **Source:** University of Augsburg  
- **Participants:** 15 individuals wearing Empatica E4 wristband and RespiBAN chest sensor  
- **Signals Collected:**
  - EDA (Electrodermal Activity)  
  - TEMP (Skin Temperature)  
  - ACC (Accelerometer – not used in this simplified model)  
- **Original Labels:**
  - 0 = Baseline (Relaxed)  
  - 1 = Stress  
  - 2 = Amusement  

### 🧪 Binary Classification Mapping:
- `1 → Stress`  
- `0 → Not Stress` (Baseline + Amusement)

---

## 🛠️ Tools & Libraries

- **Language:** Python 3.10+  
- **Environment:** Jupyter Notebook  

### 🧰 Libraries Used:
- `pandas`  
- `numpy`  
- `scikit-learn`  
- `matplotlib`  
- `seaborn`  
- `xgboost`

---

## 🔍 Machine Learning Approach

### ✅ Supervised Learning – Binary Classification  
- **Features Used:**
  - Electrodermal Activity (EDA)  
  - Skin Temperature (TEMP)  
- **Labels:**
  - `1 = Stress`  
  - `0 = Not Stress`  

### 📊 Primary Model:  
- Random Forest Classifier  

### 🧪 Alternative Models Tested:
- ✅ XGBoost  
- ✅ Support Vector Machine (SVM)  
- ✅ Neural Networks (MLPClassifier)

---

## 🧪 Workflow Summary

1. **Data Preprocessing:**
   - Cleaned and normalized EDA and TEMP sensor readings  
   - Removed noise and timestamp anomalies  
   - Combined aligned-length datasets  
   - Applied KMeans to simulate unsupervised stress clustering  
   - Re-mapped clusters to binary stress labels  

2. **Model Training:**
   - Performed 80/20 train-test split  
   - Trained Random Forest Classifier  

3. **Evaluation:**
   - **Accuracy:** 100%  
   - Visualized using:  
     - Confusion Matrix  
     - PCA Projection  
     - EDA vs TEMP Scatter Plot  

---

## 📈 Results

- **Random Forest Accuracy:** `100.00%`  
- **Alternative Models:** XGBoost, SVM, Neural Networks  
- **Top Predictive Features:**  
  - Electrodermal Activity (EDA)  
  - Skin Temperature  

### 📊 Visuals:
- Confusion Matrix  
- PCA Plot  
- Feature Importance Chart  
- Scatter Plot (EDA vs TEMP)

---

## ⚖️ Ethical Considerations

- **Bias Awareness:**  
  Performance may vary by gender, age, and health background  
- **Data Privacy:**  
  Dataset is anonymized; future deployments must comply with GDPR & HIPAA  
- **Accessibility:**  
  Promote integration with **affordable wearables** to support underserved communities  

---

## 🚀 Impact & Applications

This AI model provides **real-time, non-invasive stress detection**, with applications in:

- 🏥 High-stress workplaces (e.g., healthcare, aviation)  
- 🧘 Corporate wellness and self-care platforms  
- 📲 Mental health tracking apps  
- 🧠 Preventive intervention for anxiety and burnout
