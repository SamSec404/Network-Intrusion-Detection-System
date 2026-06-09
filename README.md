# Network Intrusion Detection System (NIDS)

## Overview

This project implements a **Network Intrusion Detection System (NIDS)** using Machine Learning and Artificial Intelligence techniques to identify malicious network traffic and distinguish it from normal network activity.

The system was developed as part of an Artificial Intelligence laboratory project and demonstrates the application of supervised learning, unsupervised learning, search optimization, and intelligent agent concepts in cybersecurity.

The project utilizes a network traffic dataset containing 6,000 records and evaluates multiple AI approaches including:

* K-Nearest Neighbors (KNN)
* Reflex-Based Agent
* K-Means Clustering
* Genetic Algorithm for Feature Selection

The objective is to accurately classify network traffic while reducing computational complexity through feature optimization.

---

## Objectives

* Detect malicious network traffic patterns.
* Compare multiple AI techniques for intrusion detection.
* Evaluate classification performance using standard metrics.
* Reduce feature dimensionality using Genetic Algorithms.
* Improve detection efficiency while maintaining accuracy.

---

## Dataset

The project uses a network traffic dataset containing network activity records.

### Dataset Characteristics

* Total Records: 6,000
* Features: Network traffic attributes
* Target Classes:

  * Normal Traffic
  * Malicious/Intrusive Traffic

The dataset is included in the repository:

```text
network_traffic.csv
```

---

## Technologies Used

### Programming Language

* Python

### Development Environment

* Jupyter Notebook

### Libraries

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn

---

## AI Techniques Implemented

### 1. Reflex Agent

A rule-based intelligent agent was implemented as a baseline intrusion detection mechanism.

#### Result

* Accuracy: 82.17%

The reflex agent makes decisions using predefined conditions and serves as a benchmark for comparing machine learning approaches.

---

### 2. K-Nearest Neighbors (KNN)

KNN was used as the primary supervised learning classifier.

#### Configuration

```text
K = 1
```

#### Result

```text
Accuracy = 95.75%
```

KNN achieved the highest classification accuracy among the implemented techniques and proved highly effective for intrusion detection.

---

### 3. K-Means Clustering

An unsupervised learning approach was used to explore natural groupings within network traffic data.

#### Purpose

* Discover hidden traffic patterns.
* Analyze separation between normal and malicious traffic.
* Visualize clustering behavior.

The clustering results demonstrated meaningful separation between traffic categories.

---

### 4. Genetic Algorithm Feature Selection

A Genetic Algorithm was applied to identify the most relevant network traffic features.

#### Results

* Original Features: Full Feature Set
* Selected Features: 11

The optimized feature subset maintained classification performance while reducing computational requirements.

#### Benefits

* Faster training
* Reduced complexity
* Lower storage requirements
* Improved deployment efficiency

---

## Project Workflow

```text
Dataset Collection
        │
        ▼
Data Preprocessing
        │
        ▼
Exploratory Data Analysis
        │
        ▼
Feature Selection (Genetic Algorithm)
        │
        ▼
Model Training
 ├── Reflex Agent
 ├── KNN
 └── K-Means
        │
        ▼
Performance Evaluation
        │
        ▼
Intrusion Detection Results
```

---

## Evaluation Metrics

The project evaluates model performance using:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

These metrics help assess the effectiveness of intrusion detection techniques.

---

## Results Summary

| Method            | Accuracy          |
| ----------------- | ----------------- |
| Reflex Agent      | 82.17%            |
| KNN (K=1)         | 95.75%            |
| K-Means           | Pattern Discovery |
| Genetic Algorithm | 11 Feature Subset |

### Best Performing Technique

🏆 **K-Nearest Neighbors (K=1)**

Accuracy achieved:

```text
95.75%
```

---

## Repository Structure

```text
Network-Intrusion-Detection-System/
│
├── Network_Intrusion_Detection_System.ipynb
├── network_traffic.csv
├── NIDS_Report.docx
├── README.md
│
└── Output Visualizations
```

---

## Installation

### Clone Repository

```bash
git clone https://github.com/Malik-Sanaullah/Network-Intrusion-Detection-Sysytem.git

cd Network-Intrusion-Detection-Sysytem
```

### Create Virtual Environment

```bash
python -m venv nids_env
```

### Activate Environment

#### Windows

```bash
nids_env\Scripts\activate
```

#### Linux/macOS

```bash
source nids_env/bin/activate
```

### Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn notebook jupyter ipykernel
```

---

## Running the Project

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```text
Network_Intrusion_Detection_System.ipynb
```

Run all notebook cells:

```text
Shift + Enter
```

or

```text
Run → Run All Cells
```

---

## Future Improvements

* Deep Learning-Based IDS
* Real-Time Traffic Monitoring
* Explainable AI (XAI)
* Hybrid Detection Models
* Cloud Deployment
* Live Dashboard Integration

---

## Academic Purpose

This project was developed for educational and research purposes to demonstrate the practical application of Artificial Intelligence techniques in cybersecurity and network intrusion detection.

---

## Author

**Malik Muhammad Sanaullah**

Computer Science Student

FAST National University of Computer and Emerging Sciences

Pakistan

---

## License

This project is intended for educational and academic use.
