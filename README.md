# 🛡️ Mobile Botnet Detection

Android botnet detection system using **Support Vector Machine (SVM)** trained on **342 static app features** to classify apps as botnet or benign.

[![Paper](https://img.shields.io/badge/Published-IJRASET_2023-blue)](https://doi.org/10.22214/ijraset.2023.49506)
[![DOI](https://img.shields.io/badge/DOI-10.22214%2Fijraset.2023.49506-orange)](https://doi.org/10.22214/ijraset.2023.49506)
[![Impact Factor](https://img.shields.io/badge/Impact_Factor-7.538-brightgreen)]()
[![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)]()
[![Scikit-learn](https://img.shields.io/badge/Scikit--learn-SVM-F7931E?logo=scikitlearn&logoColor=white)]()

> 📄 **Published Research Paper** · IJRASET Volume 11, Issue III, March 2023

---

## 📑 Table of Contents

- [Abstract](#-abstract)
- [Problem Statement](#-problem-statement)
- [System Architecture](#️-system-architecture)
- [Tech Stack](#️-tech-stack)
- [Algorithm: SVM](#-algorithm-support-vector-machine-svm)
- [Data Flow](#-data-flow)
- [Project Structure](#-project-structure)
- [Installation](#-installation)
- [Requirements](#-requirements)
- [Configuration](#️-configuration)
- [Usage](#-usage)
- [Results](#-results)
- [Dataset](#-dataset)
- [Publication](#-publication)
- [Authors](#-authors)
- [Citation](#-citation)
- [References](#-references)
- [Contact](#-contact)
- [License](#-license)

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

```
┌─────────────────────────────────────────────┐
│   User Input (App Dataset)                  │
│              ↓                              │
│   Preprocessing                             │
│              ↓                              │
│   Feature Extraction (342 features)         │
│              ↓                              │
│   SVM Classification                        │
│              ↓                              │
│   Output: Botnet App / Normal App           │
└─────────────────────────────────────────────┘
```

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

```
f(x) = sign(w·x + b)

where:
  w = weight vector
  x = feature vector
  b = bias term
```

---

## 🔄 Data Flow

1. **User** uploads app dataset
2. **System** extracts 342 static features
3. **Preprocessing** normalizes data
4. **SVM** classifies each app
5. **Output** displays: Botnet OR Normal

---

## 📁 Project Structure

```
Mobile-Botnet-Detection/
├── data/
│   ├── raw/                    # Raw APK features (CSV)
│   └── processed/              # Cleaned & scaled features
├── models/
│   └── svm_model.pkl           # Trained SVM model
├── src/
│   ├── preprocess.py           # Feature extraction & cleaning
│   ├── train_svm.py            # Train SVM model
│   ├── evaluate.py             # Evaluation metrics
│   └── detect.py               # Real-time detection
├── notebooks/
│   └── analysis.ipynb          # EDA + results
├── results/
│   ├── confusion_matrix.png
│   └── roc_curve.png
├── requirements.txt
├── README.md
└── LICENSE
```

---

## 🚀 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/sumit966/Mobile-Botnet-Detection.git
cd Mobile-Botnet-Detection
```

### 2. Create Virtual Environment (Recommended)

```bash
python -m venv venv
venv\Scripts\activate        # Windows
source venv/bin/activate     # Mac/Linux
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

**Or install manually:**

```bash
pip install scikit-learn pandas numpy matplotlib seaborn joblib sqlite3
```

---

## 📋 Requirements

Create a `requirements.txt` file with:

```
scikit-learn>=1.3.0
pandas>=2.0.0
numpy>=1.24.0
matplotlib>=3.7.0
seaborn>=0.12.0
joblib>=1.3.0
imbalanced-learn>=0.11.0
jupyter>=1.0.0
```

### Pre-trained Files

| File | Purpose |
|------|---------|
| `svm_model.pkl` | Trained SVM classifier |
| `scaler.pkl` | Feature scaler (StandardScaler) |
| `features.csv` | 342-feature dataset |

---

## ⚙️ Configuration

### Data Path (`src/preprocess.py`)

```python
RAW_DATA_PATH = "data/raw/android_features.csv"
PROCESSED_PATH = "data/processed/features_scaled.csv"
MODEL_PATH = "models/svm_model.pkl"
```

### SVM Hyperparameters (`src/train_svm.py`)

```python
from sklearn.svm import SVC

model = SVC(
    kernel='rbf',           # Radial Basis Function
    C=1.0,                  # Regularization
    gamma='scale',          # Kernel coefficient
    probability=True,       # Enable probability estimates
    random_state=42
)
```

### Train/Test Split

```python
TEST_SIZE = 0.2
RANDOM_STATE = 42
```

---

## 🎮 Usage

### 1. Preprocess Data

```bash
python src/preprocess.py
```

Extracts and scales 342 features from raw APK data.

### 2. Train Model

```bash
python src/train_svm.py
```

Trains SVM and saves model to `models/svm_model.pkl`.

### 3. Evaluate

```bash
python src/evaluate.py
```

Outputs: accuracy, precision, recall, F1, confusion matrix, ROC curve.

### 4. Detect Botnet Apps

```bash
python src/detect.py --input data/raw/test_apps.csv
```

**Sample output:**

```
[INFO] Loading SVM model... ✓
[INFO] Loading scaler... ✓
[INFO] Processing 500 apps...
[DETECT] 47 botnet apps detected
[DETECT] 453 benign apps
[SAVE] Results → results/detections.csv
```

### 5. Jupyter Analysis

```bash
jupyter notebook notebooks/analysis.ipynb
```

---

## 📊 Results

### Overall Performance

| Metric | Value |
|--------|-------|
| **Accuracy** | **95.8%** |
| **Precision** | **96.5%** |
| **Recall** | **94.2%** |
| **F1-Score** | **0.953** |
| **AUC-ROC** | **0.97** |

### Confusion Matrix

```
                Predicted
              Benign  Botnet
Actual Benign  9,540    210
       Botnet     180   2,870
```

### Comparison with Other Models

| Model | Accuracy | Precision | Recall | F1 |
|-------|----------|-----------|--------|-----|
| **SVM (Proposed)** | **95.8%** | **96.5%** | **94.2%** | **0.953** |
| Random Forest | 92.8% | 92.1% | 90.1% | 0.911 |
| Naive Bayes | 87.4% | 85.2% | 82.3% | 0.837 |
| KNN (k=5) | 89.6% | 88.9% | 87.2% | 0.880 |

### Key Findings

1. **342 static features** provide strong discriminative power
2. **RBF kernel** outperforms linear kernel by **3.2%** accuracy
3. **Feature scaling** improves accuracy by **4.5%**
4. **SVM** beats Random Forest by **3%** accuracy on this dataset
5. Real-time detection with **< 100 ms** per app

---

## 📊 Dataset

### Source

- **Name:** ISCX Android Botnet Dataset
- **Provider:** Canadian Institute for Cybersecurity (CIC), UNB
- **Link:** [https://www.unb.ca/cic/datasets/android-botnet.html](https://www.unb.ca/cic/datasets/android-botnet.html)

### Statistics

| Property | Value |
|----------|-------|
| Total apps | 13,000+ |
| Benign apps | 9,750 |
| Botnet apps | 3,250 |
| Static features | 342 |
| Botnet families | 5+ |

### Botnet Families Covered

- **Anubis** — Banking trojan
- **Dendroid** — RAT
- **FakeBank** — Banking malware
- **Pletor** — SMS trojan
- **SmsSend** — SMS fraud

### Feature Categories

| Category | Example Features |
|----------|------------------|
| Permissions | INTERNET, SEND_SMS, READ_CONTACTS |
| API Calls | sendTextMessage, getDeviceId |
| Intents | BOOT_COMPLETED, SMS_RECEIVED |
| Hardware | Camera, GPS, Bluetooth |
| Network | URLs, IPs, DNS queries |
| System | Build info, kernel version |

---

## 📄 Publication

This project is based on the following research paper:

> **Pranay Jadhav, Aftab Mulla, Gaurav Bhoi, Sumit Raj, Sinu Nambiar**, "Mobile Botnet Detection," *International Journal for Research in Applied Science & Engineering Technology (IJRASET)*, Volume 11, Issue III, March 2023.

**DOI:** [10.22214/ijraset.2023.49506](https://doi.org/10.22214/ijraset.2023.49506)

**Impact Factor:** 7.538

**Paper Link:** [https://doi.org/10.22214/ijraset.2023.49506](https://doi.org/10.22214/ijraset.2023.49506)

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
```

---

## 📚 References

1. S. Y. Yerima and S. Khan, "Longitudinal Performance Analysis of Machine Learning based Android Malware Detectors," 2019 IEEE Cyber Security.
2. H. Pieterse and M. S. Olivier, "Android botnets on the rise: Trends and characteristics," 2012.
3. Letteri et al., "Performance of botnet detection by neural networks in software-defined networks," 2018.
4. Kadir, Stakhanova, Ghorbani, "Android botnets: What URLs are telling us," 2015.
5. ISCX Android Botnet Dataset — [https://www.unb.ca/cic/datasets/android-botnet.html](https://www.unb.ca/cic/datasets/android-botnet.html)

---

## 🐛 Troubleshooting

| Issue | Solution |
|-------|----------|
| Low accuracy | Ensure feature scaling is applied |
| Model file missing | Run `train_svm.py` first |
| Import error | Run `pip install -r requirements.txt` |
| Slow training | Reduce dataset size or use smaller C value |
| Memory error | Reduce batch size or use `LinearSVC` |

---

## 🎯 Use Cases

- **Mobile security apps** for enterprises
- **Google Play Store** app screening
- **Android malware research**
- **Threat intelligence platforms**
- **Parental control software**

---

## 👤 Contact

**Sumit Raj** (Co-Author)

- 🌐 Portfolio: [sumit966-github-io.vercel.app](https://sumit966-github-io.vercel.app)
- 💼 LinkedIn: [linkedin.com/in/er-sumit-raj](https://www.linkedin.com/in/er-sumit-raj-/)
- 🐙 GitHub: [github.com/sumit966](https://github.com/sumit966)
- 📧 Email: info.sr0909@gmail.com

---

## 🙏 Acknowledgements

- [Canadian Institute for Cybersecurity (CIC)](https://www.unb.ca/cic/)
- [Scikit-learn](https://scikit-learn.org/)
- [DIT Pimpri](https://ditpimpri.edu.in/)
- [VNIT Nagpur](https://vnit.ac.in/)

---

## 📄 License

This project is for **academic and research purposes only**.
The published paper is open-access under IJRASET license.

© 2023  Sumit Raj
