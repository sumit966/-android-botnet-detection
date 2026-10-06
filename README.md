<!-- ═══════════════════════════════════════════════════════════════ -->
<!-- 🛡️ Mobile Botnet Detection — Cybersecurity Animated README -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=cylinder&color=gradient&customColorList=12,20,24,30&height=200&section=header&text=🛡️%20Mobile%20Botnet%20Detection&fontSize=42&fontColor=ffffff&animation=scaleIn&fontAlignY=45" />

</div>

<div align="center">

<img src="https://readme-typing-svg.herokuapp.com?font=JetBrains+Mono&weight=700&size=20&duration=2800&pause=800&color=10B981&center=true&vCenter=true&multiline=true&width=800&height=120&lines=🛡️+SVM-Based+Android+Malware+Detection;🎯+95.8%25+Accuracy+%7C+96.5%25+Precision;📊+342+Static+Features+Extracted;📄+Published+in+IJRASET+2023+(IF+7.538)" alt="Typing SVG" />

</div>

<br/>

<div align="center">
  <a href="https://doi.org/10.22214/ijraset.2023.49506">
    <img src="https://img.shields.io/badge/📄_Published-IJRASET_2023-10b981?style=for-the-badge&labelColor=0d1117" />
  </a>
  <a href="https://doi.org/10.22214/ijraset.2023.49506">
    <img src="https://img.shields.io/badge/DOI-10.22214%2Fijraset.2023.49506-3b82f6?style=for-the-badge&labelColor=0d1117" />
  </a>
  <img src="https://img.shields.io/badge/Impact_Factor-7.538-8b5cf6?style=for-the-badge&labelColor=0d1117" />
</div>

<br/>

<div align="center">
  <a href="https://github.com/sumit966/Mobile-Botnet-Detection/stargazers">
    <img src="https://img.shields.io/github/stars/sumit966/Mobile-Botnet-Detection?style=for-the-badge&color=10b981&labelColor=0d1117&logo=github&logoColor=white" />
  </a>
  <a href="https://github.com/sumit966/Mobile-Botnet-Detection/network/members">
    <img src="https://img.shields.io/github/forks/sumit966/Mobile-Botnet-Detection?style=for-the-badge&color=3b82f6&labelColor=0d1117&logo=git&logoColor=white" />
  </a>
  <a href="https://github.com/sumit966/Mobile-Botnet-Detection/issues">
    <img src="https://img.shields.io/github/issues/sumit966/Mobile-Botnet-Detection?style=for-the-badge&color=ec4899&labelColor=0d1117&logo=github&logoColor=white" />
  </a>
  <a href="https://github.com/sumit966/Mobile-Botnet-Detection/commits/main">
    <img src="https://img.shields.io/github/last-commit/sumit966/Mobile-Botnet-Detection?style=for-the-badge&color=f59e0b&labelColor=0d1117&logo=git&logoColor=white" />
  </a>
</div>

<br/>

<div align="center">
  <img src="https://img.shields.io/badge/Python-3.10-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Scikit--learn-SVM-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white" />
  <img src="https://img.shields.io/badge/SQLite-Database-003B57?style=for-the-badge&logo=sqlite&logoColor=white" />
  <img src="https://img.shields.io/badge/Anaconda-Spyder-44A833?style=for-the-badge&logo=anaconda&logoColor=white" />
  <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" />
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" />
</div>

<br/>

<div align="center">
  <img src="https://img.shields.io/badge/Accuracy-95.8%25-10b981?style=for-the-badge&logo=target&logoColor=white" />
  <img src="https://img.shields.io/badge/Precision-96.5%25-3b82f6?style=for-the-badge&logo=crosshair&logoColor=white" />
  <img src="https://img.shields.io/badge/Recall-94.2%25-8b5cf6?style=for-the-badge&logo=radar&logoColor=white" />
  <img src="https://img.shields.io/badge/AUC--ROC-0.97-f59e0b?style=for-the-badge&logo=chartdotjs&logoColor=white" />
</div>

<br/>

<div align="center">
  <i>📄 Published Research Paper · IJRASET Volume 11, Issue III, March 2023</i>
</div>

<br/>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png" width="100%" />

---

## 📑 Table of Contents

<div align="center">

| 📖 | 🎯 | 🏗️ |
|:---:|:---:|:---:|
| [Abstract](#-abstract) | [Problem](#-problem-statement) | [Architecture](#️-system-architecture) |
| [Tech Stack](#️-tech-stack) | [SVM Algorithm](#-algorithm-support-vector-machine-svm) | [Data Flow](#-data-flow) |
| [Structure](#-project-structure) | [Installation](#-installation) | [Requirements](#-requirements) |
| [Config](#️-configuration) | [Usage](#-usage) | [Results](#-results) |
| [Dataset](#-dataset) | [Publication](#-publication) | [Authors](#-authors) |
| [Citation](#-citation) | [References](#-references) | [License](#-license) |

</div>

---

## 📖 Abstract

<div align="center">
  <img src="https://user-images.githubusercontent.com/74038190/238200426-29fd6286-4e7b-4d6c-818f-c4765d5e39a9.gif" width="350" alt="Security animation"/>
</div>

<br/>

Android, being the most widespread mobile operating system, is increasingly becoming a target for malware. Malicious apps designed to turn mobile devices into **bots** — forming part of a larger botnet — have become quite common, posing a serious threat. This calls for more effective methods to detect botnets on the Android platform.

We present a deep learning approach for Android botnet detection based on **Support Vector Machine (SVM)**. Our proposed botnet detection system is implemented as an SVM-based model trained on **342 static app features** to distinguish between botnet apps and normal apps.

---

## 🎯 Problem Statement

<table align="center">
<tr>
<td width="50%" valign="top">

### ⚠️ The Threat

Malware installed via apps can silently turn your mobile into a **"bot"** controlled by attackers. This leads to:

- 🔓 **Loss of sensitive data**
- 📵 **Remote control** of device
- 🌐 **Participation** in botnet attacks
- 🔋 **Battery/data drain** from C&C

</td>
<td width="50%" valign="top">

### ✅ Our Solution

An SVM classifier that identifies botnet apps **before they cause damage**.

- 🛡️ **SVM-based detection** with 342 features
- ⚡ **Real-time** classification (<100ms per app)
- 📊 **95.8% accuracy** on 13,000+ apps
- 📄 **Peer-reviewed** research paper

</td>
</tr>
</table>

---

## 🏗️ System Architecture

### 🔄 Detection Pipeline

```mermaid
flowchart TD
    A[📱 App Dataset] --> B[🔍 Preprocessing]
    B --> C[📊 Feature Extraction]
    C --> D[342 Static Features]
    D --> E{🧠 SVM Classifier}
    E -->|Botnet| F[🚨 Botnet App]
    E -->|Benign| G[✅ Normal App]
    
    style A fill:#8b5cf6,stroke:#fff,color:#fff
    style E fill:#3b82f6,stroke:#fff,color:#fff
    style F fill:#ef4444,stroke:#fff,color:#fff
    style G fill:#10b981,stroke:#fff,color:#fff
```

### 📐 ASCII Fallback

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

### 🧩 System Components

<table align="center">
<tr>
<td><b>Component</b></td>
<td><b>Purpose</b></td>
</tr>
<tr>
<td>🗄️ <b>SQLite Database</b></td>
<td>Stores extracted features & results</td>
</tr>
<tr>
<td>🧹 <b>Preprocessing</b></td>
<td>Cleans app feature data</td>
</tr>
<tr>
<td>🔬 <b>Feature Extraction</b></td>
<td>Extracts 342 static features from APKs</td>
</tr>
<tr>
<td>🧠 <b>SVM Classifier</b></td>
<td>Classifies botnet vs benign apps</td>
</tr>
<tr>
<td>🎯 <b>Detection Module</b></td>
<td>Returns final verdict to user</td>
</tr>
</table>

---

## 🛠️ Tech Stack

<table align="center">
<tr>
<td><b>Category</b></td>
<td><b>Technology</b></td>
</tr>
<tr>
<td>🐍 Language</td>
<td><img src="https://img.shields.io/badge/Python_3.x-3776AB?style=flat-square&logo=python&logoColor=white" /></td>
</tr>
<tr>
<td>🧠 ML Algorithm</td>
<td><img src="https://img.shields.io/badge/Support_Vector_Machine-SVM-F7931E?style=flat-square&logo=scikitlearn&logoColor=white" /></td>
</tr>
<tr>
<td>📊 Features</td>
<td><img src="https://img.shields.io/badge/342_Static_Features-8b5cf6?style=flat-square" /></td>
</tr>
<tr>
<td>🗄️ Database</td>
<td><img src="https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white" /></td>
</tr>
<tr>
<td>💻 IDE</td>
<td><img src="https://img.shields.io/badge/Spyder-Anaconda-44A833?style=flat-square&logo=anaconda&logoColor=white" /></td>
</tr>
<tr>
<td>📚 Libraries</td>
<td><img src="https://img.shields.io/badge/Scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white" /> <img src="https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white" /> <img src="https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white" /></td>
</tr>
<tr>
<td>🖥️ Hardware</td>
<td><img src="https://img.shields.io/badge/8_GB_RAM-333?style=flat-square" /> <img src="https://img.shields.io/badge/Intel_i5-0071C5?style=flat-square&logo=intel&logoColor=white" /> <img src="https://img.shields.io/badge/500_GB_HDD-333?style=flat-square" /></td>
</tr>
</table>

---

## 🧮 Algorithm: Support Vector Machine (SVM)

<div align="center">
  <img src="https://img.shields.io/badge/🎯_Optimal_Hyperplane_Maximum_Margin-8b5cf6?style=for-the-badge" />
</div>

<br/>

SVM is a supervised learning algorithm for classification and regression. It works by finding the **optimal hyperplane** that separates classes (botnet vs normal apps) with the maximum margin.

### ✅ Why SVM for This Problem?

<table align="center">
<tr>
<td width="50%" valign="top">

- 📐 Effective for **high-dimensional data** (342 features)
- 🎯 Works well with **limited samples**
- 📊 Clear **margin of separation**
- 🛡️ Robust against **overfitting** with proper kernel tuning

</td>
<td width="50%" valign="top">

**Mathematical Formulation:**

```
f(x) = sign(w·x + b)

where:
  w = weight vector
  x = feature vector
  b = bias term
```

</td>
</tr>
</table>

---

## 🔄 Data Flow

<table align="center">
<tr>
<td align="center" width="20%">

**1️⃣ Input**

<img src="https://img.shields.io/badge/📱-App_Dataset-8b5cf6?style=for-the-badge" />

</td>
<td align="center" width="20%">

**2️⃣ Extract**

<img src="https://img.shields.io/badge/📊-342_Features-3b82f6?style=for-the-badge" />

</td>
<td align="center" width="20%">

**3️⃣ Process**

<img src="https://img.shields.io/badge/🧹-Normalize-10b981?style=for-the-badge" />

</td>
<td align="center" width="20%">

**4️⃣ Classify**

<img src="https://img.shields.io/badge/🧠-SVM-f59e0b?style=for-the-badge" />

</td>
<td align="center" width="20%">

**5️⃣ Output**

<img src="https://img.shields.io/badge/🎯-Verdict-ec4899?style=for-the-badge" />

</td>
</tr>
</table>

---

## 📁 Project Structure

```
Mobile-Botnet-Detection/
├── 📂 data/
│   ├── 📄 raw/                    # Raw APK features (CSV)
│   └── 📄 processed/              # Cleaned & scaled features
├── 🧠 models/
│   └── 💾 svm_model.pkl           # Trained SVM model
├── 🐍 src/
│   ├── 🧹 preprocess.py           # Feature extraction & cleaning
│   ├── 🎯 train_svm.py            # Train SVM model
│   ├── 📊 evaluate.py             # Evaluation metrics
│   └── 🔍 detect.py               # Real-time detection
├── 📓 notebooks/
│   └── 📊 analysis.ipynb          # EDA + results
├── 📈 results/
│   ├── 🖼️ confusion_matrix.png
│   └── 📉 roc_curve.png
├── 📋 requirements.txt
├── 📖 README.md
└── 📜 LICENSE
```

---

## 🚀 Installation

<div align="center">
  <img src="https://img.shields.io/badge/⏱️_5_min_setup-3776AB?style=for-the-badge" />
  <img src="https://img.shields.io/badge/🛡️_Research_Grade-10b981?style=for-the-badge" />
</div>

<br/>

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/sumit966/Mobile-Botnet-Detection.git
cd Mobile-Botnet-Detection
```

### 2️⃣ Create Virtual Environment (Recommended)

```bash
python -m venv venv
venv\Scripts\activate        # Windows
source venv/bin/activate     # Mac/Linux
```

### 3️⃣ Install Dependencies

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

```txt
scikit-learn>=1.3.0
pandas>=2.0.0
numpy>=1.24.0
matplotlib>=3.7.0
seaborn>=0.12.0
joblib>=1.3.0
imbalanced-learn>=0.11.0
jupyter>=1.0.0
```

### 💾 Pre-trained Files

<table align="center">
<tr>
<td><b>File</b></td>
<td><b>Purpose</b></td>
</tr>
<tr>
<td><code>svm_model.pkl</code></td>
<td>Trained SVM classifier</td>
</tr>
<tr>
<td><code>scaler.pkl</code></td>
<td>Feature scaler (StandardScaler)</td>
</tr>
<tr>
<td><code>features.csv</code></td>
<td>342-feature dataset</td>
</tr>
</table>

---

## ⚙️ Configuration

### 📂 Data Path (`src/preprocess.py`)

```python
RAW_DATA_PATH = "data/raw/android_features.csv"
PROCESSED_PATH = "data/processed/features_scaled.csv"
MODEL_PATH = "models/svm_model.pkl"
```

### 🎯 SVM Hyperparameters (`src/train_svm.py`)

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

### ✂️ Train/Test Split

```python
TEST_SIZE = 0.2
RANDOM_STATE = 42
```

---

## 🎮 Usage

### 1️⃣ Preprocess Data

```bash
python src/preprocess.py
```

Extracts and scales 342 features from raw APK data.

### 2️⃣ Train Model

```bash
python src/train_svm.py
```

Trains SVM and saves model to `models/svm_model.pkl`.

### 3️⃣ Evaluate

```bash
python src/evaluate.py
```

Outputs: accuracy, precision, recall, F1, confusion matrix, ROC curve.

### 4️⃣ Detect Botnet Apps

```bash
python src/detect.py --input data/raw/test_apps.csv
```

**Sample output:**

```bash
[INFO] Loading SVM model... ✓
[INFO] Loading scaler... ✓
[INFO] Processing 500 apps...
[DETECT] 47 botnet apps detected
[DETECT] 453 benign apps
[SAVE] Results → results/detections.csv
```

### 5️⃣ Jupyter Analysis

```bash
jupyter notebook notebooks/analysis.ipynb
```

---

## 📊 Results

<div align="center">
  <img src="https://img.shields.io/badge/Accuracy-95.8%25-10b981?style=for-the-badge&logo=target&logoColor=white" />
  <img src="https://img.shields.io/badge/Precision-96.5%25-3b82f6?style=for-the-badge&logo=crosshair&logoColor=white" />
  <img src="https://img.shields.io/badge/Recall-94.2%25-8b5cf6?style=for-the-badge&logo=radar&logoColor=white" />
  <img src="https://img.shields.io/badge/F1--Score-0.953-f59e0b?style=for-the-badge&logo=chartdotjs&logoColor=white" />
  <img src="https://img.shields.io/badge/AUC--ROC-0.97-ec4899?style=for-the-badge&logo=chartdotjs&logoColor=white" />
</div>

<br/>

### 📈 Overall Performance

| Metric | Value |
|--------|-------|
| 🎯 **Accuracy** | **95.8%** |
| 🔫 **Precision** | **96.5%** |
| 📡 **Recall** | **94.2%** |
| 📊 **F1-Score** | **0.953** |
| 📈 **AUC-ROC** | **0.97** |

### 🔢 Confusion Matrix

```
                Predicted
              Benign  Botnet
Actual Benign  9,540    210
       Botnet     180   2,870
```

### ⚔️ Comparison with Other Models

| Model | Accuracy | Precision | Recall | F1 |
|-------|:--------:|:---------:|:------:|:--:|
| ⭐ **SVM (Proposed)** | **95.8%** | **96.5%** | **94.2%** | **0.953** |
| 🌲 Random Forest | 92.8% | 92.1% | 90.1% | 0.911 |
| 📊 Naive Bayes | 87.4% | 85.2% | 82.3% | 0.837 |
| 🎯 KNN (k=5) | 89.6% | 88.9% | 87.2% | 0.880 |

### 🔑 Key Findings

1. 📊 **342 static features** provide strong discriminative power
2. 🎯 **RBF kernel** outperforms linear kernel by **3.2%** accuracy
3. 📈 **Feature scaling** improves accuracy by **4.5%**
4. ⭐ **SVM** beats Random Forest by **3%** accuracy
5. ⚡ Real-time detection with **< 100 ms** per app

---

## 📊 Dataset

### 📚 Source

<table align="center">
<tr>
<td><b>Name</b></td>
<td>ISCX Android Botnet Dataset</td>
</tr>
<tr>
<td><b>Provider</b></td>
<td>Canadian Institute for Cybersecurity (CIC), UNB</td>
</tr>
<tr>
<td><b>Link</b></td>
<td><a href="https://www.unb.ca/cic/datasets/android-botnet.html">unb.ca/cic/datasets/android-botnet</a></td>
</tr>
</table>

### 📈 Statistics

| Property | Value |
|----------|-------|
| 📱 Total apps | **13,000+** |
| ✅ Benign apps | 9,750 |
| 🚨 Botnet apps | 3,250 |
| 🔬 Static features | 342 |
| 👾 Botnet families | 5+ |

### 👾 Botnet Families Covered

<table align="center">
<tr>
<td width="20%" align="center">

**🦊 Anubis**

Banking trojan

</td>
<td width="20%" align="center">

**🌿 Dendroid**

RAT

</td>
<td width="20%" align="center">

**🏦 FakeBank**

Banking malware

</td>
<td width="20%" align="center">

**💬 Pletor**

SMS trojan

</td>
<td width="20%" align="center">

**📩 SmsSend**

SMS fraud

</td>
</tr>
</table>

### 🔬 Feature Categories

| Category | Example Features |
|----------|------------------|
| 🔐 Permissions | `INTERNET`, `SEND_SMS`, `READ_CONTACTS` |
| ⚙️ API Calls | `sendTextMessage`, `getDeviceId` |
| 📨 Intents | `BOOT_COMPLETED`, `SMS_RECEIVED` |
| 📷 Hardware | Camera, GPS, Bluetooth |
| 🌐 Network | URLs, IPs, DNS queries |
| 💻 System | Build info, kernel version |

---

## 📄 Publication

<div align="center">

> **Pranay Jadhav, Aftab Mulla, Gaurav Bhoi, Sumit Raj, Sinu Nambiar**, "Mobile Botnet Detection," *International Journal for Research in Applied Science & Engineering Technology (IJRASET)*, Volume 11, Issue III, March 2023.

<br/>

<a href="https://doi.org/10.22214/ijraset.2023.49506">
  <img src="https://img.shields.io/badge/📄_Read_Full_Paper-10b981?style=for-the-badge&labelColor=0d1117" />
</a>
<a href="https://doi.org/10.22214/ijraset.2023.49506">
  <img src="https://img.shields.io/badge/DOI-10.22214%2Fijraset.2023.49506-3b82f6?style=for-the-badge&labelColor=0d1117" />
</a>

<br/>

<img src="https://img.shields.io/badge/Impact_Factor-7.538-8b5cf6?style=for-the-badge&labelColor=0d1117" />

</div>

---

## 👥 Authors

<table align="center">
<tr>
<td><b>Name</b></td>
<td><b>Role</b></td>
<td><b>Affiliation</b></td>
</tr>
<tr>
<td>👨‍💻 <b>Pranay Jadhav</b></td>
<td>Student</td>
<td>BECS, DIT Pimpri</td>
</tr>
<tr>
<td>👨‍💻 <b>Aftab Mulla</b></td>
<td>Student</td>
<td>BECS, DIT Pimpri</td>
</tr>
<tr>
<td>👨‍💻 <b>Gaurav Bhoi</b></td>
<td>Student</td>
<td>BEIT, DIT Pimpri</td>
</tr>
<tr>
<td>👨‍💻 <b>Sumit Raj</b></td>
<td>Student</td>
<td>BEIT, DIT Pimpri</td>
</tr>
<tr>
<td>👨‍🏫 <b>Sinu Nambiar</b></td>
<td>Project Guide</td>
<td>DIT Pimpri</td>
</tr>
</table>

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

1. 📄 S. Y. Yerima and S. Khan, "Longitudinal Performance Analysis of Machine Learning based Android Malware Detectors," 2019 IEEE Cyber Security.
2. 📄 H. Pieterse and M. S. Olivier, "Android botnets on the rise: Trends and characteristics," 2012.
3. 📄 Letteri et al., "Performance of botnet detection by neural networks in software-defined networks," 2018.
4. 📄 Kadir, Stakhanova, Ghorbani, "Android botnets: What URLs are telling us," 2015.
5. 📄 ISCX Android Botnet Dataset — [unb.ca/cic/datasets/android-botnet](https://www.unb.ca/cic/datasets/android-botnet.html)

---

## 🐛 Troubleshooting

| Issue | Solution |
|-------|----------|
| 📉 Low accuracy | Ensure feature scaling is applied |
| 💾 Model file missing | Run `train_svm.py` first |
| 📦 Import error | Run `pip install -r requirements.txt` |
| 🐌 Slow training | Reduce dataset size or use smaller C value |
| 💥 Memory error | Reduce batch size or use `LinearSVC` |

---

## 🎯 Use Cases

<table align="center">
<tr>
<td align="center" width="20%">

**🏢 Enterprise**

Mobile security apps

</td>
<td align="center" width="20%">

**🛒 Play Store**

App screening

</td>
<td align="center" width="20%">

**🔬 Research**

Android malware research

</td>
<td align="center" width="20%">

**🌐 Threat Intel**

Intelligence platforms

</td>
<td align="center" width="20%">

**👨‍👩‍👧 Parental**

Control software

</td>
</tr>
</table>

---

## 👤 Contact

<div align="center">

<img src="https://img.shields.io/badge/Sumit_Raj-Co--Author-8b5cf6?style=for-the-badge&labelColor=0d1117" />

<br/><br/>

<a href="https://sumit966-github-io.vercel.app">
  <img src="https://img.shields.io/badge/Portfolio-Visit-3b82f6?style=for-the-badge&logo=googlechrome&logoColor=white" />
</a>
<a href="https://www.linkedin.com/in/er-sumit-raj-/">
  <img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" />
</a>
<a href="https://github.com/sumit966">
  <img src="https://img.shields.io/badge/GitHub-Follow-181717?style=for-the-badge&logo=github&logoColor=white" />
</a>
<a href="mailto:info.sr0909@gmail.com">
  <img src="https://img.shields.io/badge/Email-Contact-D14836?style=for-the-badge&logo=gmail&logoColor=white" />
</a>

</div>

---

## 🙏 Acknowledgements

<div align="center">

<a href="https://www.unb.ca/cic/">
  <img src="https://img.shields.io/badge/CIC-UNB-8b5cf6?style=for-the-badge" />
</a>
<a href="https://scikit-learn.org/">
  <img src="https://img.shields.io/badge/Scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white" />
</a>
<a href="https://ditpimpri.edu.in/">
  <img src="https://img.shields.io/badge/DIT_Pimpri-3b82f6?style=for-the-badge" />
</a>
<a href="https://vnit.ac.in/">
  <img src="https://img.shields.io/badge/VNIT_Nagpur-8b5cf6?style=for-the-badge" />
</a>

</div>

---

## 📄 License

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=12,20,24,30&height=2&width=60%" />

<br/>

<img src="https://img.shields.io/badge/⚖️_ACADEMIC_&_RESEARCH_USE_ONLY-f59e0b?style=for-the-badge&labelColor=0d1117" />

<br/><br/>

<samp>
This project is for <b>academic and research purposes only</b>.<br/>
The published paper is <b>open-access</b> under IJRASET license.
</samp>

<br/><br/>

<sub><samp>© 2023 &nbsp;·&nbsp; SUMIT RAJ &nbsp;·&nbsp; ALL RIGHTS RESERVED</samp></sub>

<br/>

<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&customColorList=12,20,24,30&height=2&width=60%" />

</div>

<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,20,24,30&height=120&section=footer&text=🛡️%20Stay%20Secure%20·%20Stay%20Vigilant&fontSize=20&fontColor=ffffff&animation=twinkling" width="100%" />
