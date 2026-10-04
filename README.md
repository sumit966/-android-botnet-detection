# 🛡️ Mobile Botnet Detection

Android botnet detection system using **Support Vector Machine (SVM)** trained on **342 static app features** to classify apps as botnet or benign.

[![Paper](https://img.shields.io/badge/Published-IJRASET_2023-blue)](https://doi.org/10.22214/ijraset.2023.49506)
[![DOI](https://img.shields.io/badge/DOI-10.22214%2Fijraset.2023.49506-orange)](https://doi.org/10.22214/ijraset.2023.49506)
[![Impact Factor](https://img.shields.io/badge/Impact_Factor-7.538-brightgreen)]()
[![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)]()
[![Scikit-learn](https://img.shields.io/badge/Scikit--learn-SVM-F7931E?logo=scikitlearn&logoColor=white)]()

> 📄 **Published Research Paper** · IJRASET Volume 11, Issue III, March 2023

---

## 📖 Abstract

Android, being the most widespread mobile operating system, is increasingly becoming a target for malware. Malicious apps designed to turn mobile devices into bots — forming part of a larger botnet — have become quite common, posing a serious threat. This calls for more effective methods to detect botnets on the Android platform.

We present a deep learning approach for Android botnet detection based on **Support Vector Machine (SVM)**. Our proposed botnet detection system is implemented as an SVM-based model trained on **342 static app features** to distinguish between botnet apps and normal apps.

---

## 🎯 Problem Statement

Malware installed via apps can silently turn your mobile into a "bot" controlled by attackers. This leads to:

- 📵 Loss of sensitive data
- 🔓 Remote control of the device
- 🌐 Participation in large-scale botnet attacks
- 🔋 Battery/data drain from C&C communication

**Our solution:** An SVM classifier that identifies botnet apps before they cause damage.

---

## 🏗️ System Architecture
User Input (App Dataset)
↓
Preprocessing
↓
Feature Extraction (342 features)
↓
SVM Classification
↓
Output: Botnet App / Normal App


### System Components

| Component | Purpose |
|-----------|---------|
| **SQLite Database** | Stores extracted features & results |
| **Preprocessing** | Cleans app feature data |
| **Feature Extraction** | Extracts 342 static features from APKs |
| **SVM Classifier** | Classifies botnet vs benign apps |
| **Detection Module** | Returns final verdict to user |

---

## 🛠️ Tech Stack

| Category | Technology |
|----------|-----------|
| **Language** | Python 3.x |
| **ML Algorithm** | Support Vector Machine (SVM) |
| **Features** | 342 static Android app features |
| **Database** | SQLite |
| **IDE** | Spyder / Anaconda Navigator |
| **Libraries** | Scikit-learn, NumPy, Pandas |
| **Hardware** | 8 GB RAM, Intel i5, 500 GB HDD |

---

## 🧮 Algorithm: Support Vector Machine (SVM)

SVM is a supervised learning algorithm for classification and regression. It works by finding the **optimal hyperplane** that separates classes (botnet vs normal apps) with the maximum margin.

**Why SVM for this problem?**

- ✅ Effective for high-dimensional data (342 features)
- ✅ Works well with limited samples
- ✅ Clear margin of separation
- ✅ Robust against overfitting with proper kernel tuning

**Mathematical formulation:**
f(x) = sign(w·x + b)

where:
w = weight vector
x = feature vector
b = bias term


---

## 🔄 Data Flow

1. **User** uploads app dataset
2. **System** extracts 342 static features
3. **Preprocessing** normalizes data
4. **SVM** classifies each app
5. **Output** displays: Botnet OR Normal

---

## 📊 Dataset

- **Source:** ISCX Android Botnet Dataset (UNB CIC)
- **Link:** https://www.unb.ca/cic/datasets/android-botnet.html
- **Features:** 342 static features per app
- **Classes:** Botnet / Benign

---

## 👥 Authors

| Name | Role | Affiliation |
|------|------|-------------|
| **Pranay Jadhav** | Student | BECS, DIT Pimpri |
| **Aftab Mulla** | Student | BECS, DIT Pimpri |
| **Gaurav Bhoi** | Student | BEIT, DIT Pimpri |
| **Sumit Raj** | Student | BEIT, DIT Pimpri |
| **Sinu Nambiar** | Project Guide | DIT Pimpri |

---

## 📄 Citation

If you use this work, please cite:

```bibtex
@article{jadhav2023mobile,
  title={Mobile Botnet Detection},
  author={Jadhav, Pranay and Mulla, Aftab and Bhoi, Gaurav and Raj, Sumit and Nambiar, Sinu},
  journal={International Journal for Research in Applied Science \& Engineering Technology (IJRASET)},
  volume={11},
  number={III},
  year={2023},
  doi={10.22214/ijraset.2023.49506}
}

📚 References
S. Y. Yerima and S. Khan, "Longitudinal Performance Analysis of Machine Learning based Android Malware Detectors," 2019 IEEE Cyber Security.

H. Pieterse and M. S. Olivier, "Android botnets on the rise: Trends and characteristics," 2012.

Letteri et al., "Performance of botnet detection by neural networks in software-defined networks," 2018.

Kadir, Stakhanova, Ghorbani, "Android botnets: What URLs are telling us," 2015.

ISCX Android Botnet Dataset — https://www.unb.ca/cic/datasets/android-botnet.html

👤 Contact
Sumit Raj (Co-Author)

🌐 Portfolio

💼 LinkedIn

🐙 GitHub

📧 info.sr0909@gmail.com

