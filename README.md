# uav-cyber-intrusion-detection
Machine learning models for cyber-physical intrusion detection in Unmanned Aerial Vehicles (UAVs) based on the UAVs Dataset Under Normal and Cyberattacks, achieving up to 96.28% accuracy with Bagging Classifier.

# 🛡️ UAV Cyber-Physical Intrusion Detection System

![License](https://img.shields.io/badge/license-MIT-green)
![Python](https://img.shields.io/badge/python-3.10-blue)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Completed-success)
![Status](https://img.shields.io/badge/status-Finished-brightgreen)

## 🌟 **Overview**
This project implements machine learning models to detect cyber-physical intrusions in **Unmanned Aerial Vehicles (UAVs)** by analyzing network traffic.  
It is based on the study:  
> **Cyber-Physical Intrusion Detection System for Unmanned Aerial Vehicles**  
> *Samuel Chase Hassler, Umair Ahmad Mughal (Student Member, IEEE), and Muhammad Ismail (Senior Member, IEEE)*  

📄 **Dataset Used:** [UAVs Dataset Under Normal and Cyberattacks](https://github.com/uamughal/UAVs-Dataset-Under-Normal-and-Cyberattacks/blob/main/Dataset_T-ITS.csv)  

---

## 🎯 **Project Objectives**
- ✅ Preprocess and merge 8 subsets of the UAV dataset (~54,783 records).  
- ✅ Handle missing values and perform class distribution checks.  
- ✅ Train and evaluate multiple machine learning models.  
- ✅ Identify the most accurate model for UAV intrusion detection.

---

## 🏗️ **Data Preprocessing Steps**  
- 🧹 **Merging:** Combined 8 data subsets into a single dataset.  
- 🔍 **Missing Values:** Filled null entries using appropriate imputation techniques.  
- 📊 **Class Distribution:** Analyzed and addressed class imbalance issues.

---


## 🧪 **Machine Learning Models & Results**

| Model                      |   Accuracy   | Precision (avg) | Recall (avg) | F1-Score (avg) |
| -------------------------- | :----------: | :-------------: | :----------: | :------------: |
| 🔹 **Logistic Regression** |    40.96%    |       0.43      |     0.36     |      0.36      |
| 🌲 **Random Forest**       |    94.28%    |       0.95      |     0.95     |      0.95      |
| ⚡ **XGBoost**              |    90.24%    |       0.92      |     0.92     |      0.92      |
| 🐈 **CatBoost**            |    85.51%    |       0.89      |     0.88     |      0.87      |
| 💡 **LightGBM**            |    92.48%    |       0.94      |     0.94     |      0.94      |
| 🎛 **Bagging Classifier**  | ⭐ **96.28%** |       0.97      |     0.97     |      0.97      |

---

## 🔍 **Key Insights**

* ⭐ **Bagging Classifier** remains the top performer (**96.28% accuracy**) with excellent consistency across all metrics.
* 🌲 **Random Forest** achieved strong results (**94.28% accuracy**) and high performance in every class.
* 💡 **LightGBM** slightly outperformed XGBoost, delivering a solid **92.48% accuracy**.
* ⚡ **XGBoost** still showed reliable and efficient performance (**90.24% accuracy**).
* 🐈 **CatBoost** achieved moderate performance (**85.51% accuracy**) and could benefit from additional tuning.
* ⚠️ **Logistic Regression** performed the worst (**40.96% accuracy**), showing its limitations for complex, multi-class intrusion detection tasks.

---

## 📜 **Detailed Classification Reports**

<details>
<summary>🔍 Click to expand</summary>

### 🔹 **Logistic Regression (40.96% Accuracy)**

* **Precision (avg):** 0.43
* **Recall (avg):** 0.36
* **F1-score (avg):** 0.36
* Heavily struggled with class imbalance and complex decision boundaries.

### 🌲 **Random Forest (94.28% Accuracy)**

* **Precision (avg):** 0.95
* **Recall (avg):** 0.95
* **F1-score (avg):** 0.95
* Strong generalization across all classes with minimal misclassification.

### ⚡ **XGBoost (90.24% Accuracy)**

* **Precision (avg):** 0.92
* **Recall (avg):** 0.92
* **F1-score (avg):** 0.92
* Efficient and well-balanced performance, especially effective on classes 1 and 4.

### 🐈 **CatBoost (85.51% Accuracy)**

* **Precision (avg):** 0.89
* **Recall (avg):** 0.88
* **F1-score (avg):** 0.87
* Struggled slightly with class 2 but performed well overall.

### 💡 **LightGBM (92.48% Accuracy)**

* **Precision (avg):** 0.94
* **Recall (avg):** 0.94
* **F1-score (avg):** 0.94
* Excellent performance and close to Random Forest with faster inference.

### 🎛 **Bagging Classifier (96.28% Accuracy)**

* **Precision (avg):** 0.97
* **Recall (avg):** 0.97
* **F1-score (avg):** 0.97
* Outperformed all models with the most consistent and reliable predictions across classes.

</details>

---


## 💡 **Technologies Used**
- 📚 **Python 3.10**  
- 🔍 **scikit-learn**  
- ⚡ **XGBoost**  
- 🐈 **CatBoost**  
- 🎛 **Bagging Classifier**  
- 🛠 **Pandas, NumPy, Matplotlib, Seaborn**  

---

## 📝 **Conclusion**
The project demonstrates that **ensemble learning techniques** like **Bagging** and **Random Forest** provide exceptional performance for detecting cyber-physical intrusions in UAV networks. Future work could explore deep learning models or real-time detection systems.

---

## 📜 **Citation**
If you use this work, please cite the original paper:

> **Samuel Chase Hassler, Umair Ahmad Mughal, and Muhammad Ismail.** 2024.  
> *Cyber-Physical Intrusion Detection System for Unmanned Aerial Vehicles.*  
> **Trans. Intell. Transport. Sys. 25, 6 (June 2024), 6106–6117.**  
> [https://doi.org/10.1109/TITS.2023.3339728](https://doi.org/10.1109/TITS.2023.3339728)


---

## ✨ **Acknowledgments**  
- 📄 Thanks to [Umair Ahmad Mughal](https://github.com/uamughal) for providing the **[UAVs Dataset Under Normal and Cyberattacks](https://github.com/uamughal/UAVs-Dataset-Under-Normal-and-Cyberattacks/blob/main/Dataset_T-ITS.csv)**.

---

## 🙌 **Author's Note**
> 📝 *Although I'm not an expert in this field, I gave my best effort in implementing and analyzing this project based on the referenced research paper. Feedback and contributions are always welcome!*  

---

⭐ **If you found this project helpful, give it a star!** ⭐
