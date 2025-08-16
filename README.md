# 🫀 Predicting Cardiovascular Diseases Using Deep Learning

## 📌 Overview
This project applies **deep learning** and **machine learning** techniques to predict the risk of **Cardiovascular Diseases (CVDs)** using integrated patient datasets from Kaggle.  
The models analyze demographic, clinical, lifestyle, and medical history data to detect early risk factors and improve healthcare decision-making.

By leveraging **DNN**, **CNN**, and a **Complex DNN** alongside traditional models like **Logistic Regression**, **Random Forest**, and **Gradient Boosting**, the study aims to maximize **accuracy**, **recall**, and **interpretability**.

---

## 🎯 Objectives
1. **Develop Deep Learning Models** – Train models capable of accurately predicting CVD risk.
2. **Identify Key Predictive Factors** – Use SHAP and LIME for interpretability.
3. **Evaluate Model Performance** – Assess accuracy, precision, recall, F1-score, and ROC-AUC.
4. **Compare with Traditional ML Models** – Benchmark deep learning models against interpretable classical algorithms.

---

## 🧪 Methodology

### Data Source & Preprocessing
- **Dataset**: Kaggle cardiovascular health dataset.
- **Cleaning**: Removed duplicates, handled missing values.
- **Feature Engineering**: Derived `BMI`, categorical encodings, and normalized continuous features.

### Deep Learning Models
1. **Original DNN** – Fully connected layers with dropout for regularization.
2. **CNN (1D)** – Captures local patterns in structured patient data.
3. **Complex DNN** – More layers and units for fine-grained pattern recognition.

**Common Hyperparameters**:
- Activation: `ReLU` (hidden layers), `Sigmoid` (output)
- Optimizer: `Adam`
- Loss: Binary Crossentropy
- Regularization: 50% dropout layers

### Traditional ML Models
- **Logistic Regression** – Interpretable baseline.
- **Random Forest** – Robust ensemble method.
- **Gradient Boosting** – Sequential learning for improved accuracy.

---

## 📊 Model Evaluation
Metrics used:
- **Accuracy**
- **Precision**
- **Recall (Sensitivity)**
- **F1-score**
- **ROC-AUC**

**Cross-validation**:
- Stratified 10-fold CV to handle class balance.

---

## 🔍 Key Results
| Model                  | Accuracy | Precision | Recall | ROC-AUC |
|------------------------|----------|-----------|--------|---------|
| Complex DNN            | 0.88     | 0.86      | 0.90   | 0.92    |
| CNN                    | 0.86     | 0.84      | 0.88   | 0.89    |
| Logistic Regression    | 0.72     | 0.75      | 0.68   | 0.79    |
| Random Forest          | 0.74     | 0.76      | 0.69   | 0.80    |
| Gradient Boosting      | 0.85     | 0.84      | 0.86   | 0.87    |

---

## 💡 Insights & Business Value
- **Clinical Application** – High-recall models can minimize missed diagnoses.
- **Interpretability** – SHAP/LIME highlights the most influential features.
- **Policy Support** – Data-driven patient risk assessment supports healthcare resource planning.
- **Scalability** – Models can be retrained for different populations or integrated with EHR systems.

---

## 🛠 Tech Stack
- **Python** – pandas, numpy, scikit-learn, TensorFlow/Keras
- **Visualization** – matplotlib, seaborn, SHAP, LIME
- **Modeling** – DNN, CNN, Complex DNN, Logistic Regression, Random Forest, Gradient Boosting

---

## 📷 Visuals

<img width="580" height="487" alt="GBM- Confusion matrix" src="https://github.com/user-attachments/assets/63a179cb-7b66-4433-bc59-4c9b89bfda5f" />

<img width="622" height="502" alt="GBM ROC curve" src="https://github.com/user-attachments/assets/675fe7fd-74a2-4fde-86b9-ac177e06afe2" />

<img width="567" height="487" alt="logistic- confusion matrix" src="https://github.com/user-attachments/assets/f7d59a09-c19b-450c-bf74-9bbf991ee0fe" />

<img width="607" height="496" alt="logistic ROC curve" src="https://github.com/user-attachments/assets/6c78fa78-0722-453d-a8d4-bb1782db3a17" />

<img width="998" height="697" alt="PRC for all model" src="https://github.com/user-attachments/assets/ea5a2fff-6268-4fb1-84b6-dc3ea41f96dd" />

<img width="610" height="497" alt="RF ROC curve" src="https://github.com/user-attachments/assets/4819b745-4d94-4d5c-a950-79ae44285a16" />

<img width="1013" height="697" alt="ROC for all model" src="https://github.com/user-attachments/assets/f849bd9c-2a08-47a4-a918-27d49da52835" />

---

## 👥 Contributors
- **Dineshkumar Lingapandiyan** – Deep learning architecture, evaluation
- **Jayashree Rajkumar** – Data preprocessing, interpretability analysis
- **Nagalakshmi Ramakrishna** – Model comparison, reporting
