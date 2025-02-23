# uav-cyber-intrusion-detection
Machine learning models for cyber-physical intrusion detection in Unmanned Aerial Vehicles (UAVs) based on the UAVs Dataset Under Normal and Cyberattacks, achieving up to 95.7% accuracy with Bagging Classifier.

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

| Model                  | Accuracy  | Precision (avg) | Recall (avg) | F1-Score (avg) |
|------------------------|:----------:|:---------------:|:------------:|:--------------:|
| 🔹 **Logistic Regression**   | 41.17%    | 0.37            | 0.33         | 0.29           |
| 🌲 **Random Forest**         | 93.56%    | 0.95            | 0.95         | 0.95           |
| ⚡ **XGBoost**               | 89.40%    | 0.92            | 0.92         | 0.92           |
| 🐈 **CatBoost**              | 84.80%    | 0.89            | 0.88         | 0.88           |
| 🎛 **Bagging Classifier**    | ⭐ **95.73%** | 0.97            | 0.97         | 0.97           |

---

## 🔍 **Key Insights**
- 🎯 **Bagging Classifier** emerged as the top performer (**95.73% accuracy**), demonstrating robustness in detecting intrusions.  
- 🌲 **Random Forest** also performed excellently (**93.56% accuracy**), confirming tree-based models' effectiveness.  
- ⚡ **XGBoost** showed strong performance (**89.40% accuracy**) with faster computations.  
- 🐈 **CatBoost** had decent results (**84.80% accuracy**) but could benefit from further tuning.  
- ⚠️ **Logistic Regression** underperformed, indicating that more complex models are needed for this dataset.

---

## 📜 **Detailed Classification Reports**

<details>
<summary>🔍 Click to expand</summary>

### 📈 **Logistic Regression (41.17% Accuracy)**  
- Struggled with class imbalance and complex patterns.

### 🌲 **Random Forest (93.56% Accuracy)**  
- Achieved near-perfect classification across all classes.  
- High precision and recall.

### ⚡ **XGBoost (89.40% Accuracy)**  
- Balanced precision-recall trade-off with efficient computation.

### 🐈 **CatBoost (84.80% Accuracy)**  
- Performed well but less robust compared to ensemble models.

### 🎛 **Bagging Classifier (95.73% Accuracy)**  
- Best overall performance with the highest accuracy and balanced class predictions.


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
