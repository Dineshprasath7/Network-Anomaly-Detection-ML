# **Network Anomaly Detection using NSL-KDD Dataset**

This project aims to detect network anomalies using the **NSL-KDD** dataset. Multiple machine learning models were implemented for anomaly detection, and a comparison of their performance was made using accuracy and classification metrics. Additionally, an ensemble model was created for improved prediction accuracy.

---

##  **Project Overview**

- **Dataset:** NSL-KDD (KDDTrain+.txt and KDDTest+.txt)  
- **Goal:** Classify network traffic as **Normal** or **Anomaly** using various machine learning models.  
- **Techniques Used:**  
  - Data Preprocessing  
  - Feature Encoding  
  - Feature Scaling  
  - Model Training and Evaluation  
  - Ensemble Learning  

---

---

##  **Approaches Followed**

### 1. **Data Preprocessing**
- Loaded the NSL-KDD dataset using Pandas.
- Defined appropriate column names for clarity.
- Dropped the `difficulty_level` column as it was not relevant for classification.
- Encoded categorical features (`protocol_type`, `service`, `flag`) using **Label Encoding**.
- Converted the target variable (`label`) into a binary format:
  - `normal` → **0**  
  - `anomaly` → **1**  
- Scaled the features using **StandardScaler** for effective model training.

---

### 2. **Models Implemented**

| Algorithm                      |
|--------------------------------|
| Naive Bayes                    | 
| Logistic Regression            |
| K-Nearest Neighbors (KNN)      |
| Decision Tree                  |
| Random Forest                  | 
| Support Vector Machine (SVM)   |
| Artificial Neural Network (ANN)|
- **Naive Bayes:** Efficient for high-dimensional data but may perform poorly on complex datasets.  
- **Logistic Regression:** Effective for binary classification tasks.  
- **KNN:** Non-parametric model suitable for smaller datasets.  
- **Decision Tree:** Quick and interpretable but prone to overfitting.  
- **Random Forest:** Ensemble model that reduces overfitting by using multiple trees.  
- **SVM:** Powerful for high-dimensional data and finds the optimal hyperplane.  
- **ANN:** Capable of learning complex patterns in data using multiple hidden layers.

---

### 3. **Ensemble Model**

A **Voting Classifier** was created using:  
- Naive Bayes  
- Logistic Regression  
- K-Nearest Neighbors  
- Decision Tree  
- Random Forest  
- Support Vector Machine  

---

## 📈 **Evaluation Metrics**
- **Accuracy**  
- **Precision**  
- **Recall**  
- **F1-Score**  


