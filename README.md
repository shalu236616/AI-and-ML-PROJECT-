
# AI & ML for Cyber Security — Intrusion Detection Projects

Machine learning experiments applying decision trees, ensemble methods, and time-series analysis to network intrusion detection.

## 📂 Contents

| Notebook | What it does |
|---|---|
| `IREP_Decision_Tree_On_Intrusion_detection.ipynb` | Applies IREP-based decision tree rule induction to classify network traffic as normal vs. malicious |
| `modification_of_decision_tree_using_AdaBoost.ipynb` | Boosts a decision tree classifier with AdaBoost to improve intrusion detection performance |
| `Analyze_Time_Series_Network_Traffic_Data.ipynb` | Explores traffic patterns by hour and source IP, used to understand the data before building the detection models below |
| `PROJECT_WORK.ipynb` |  |

## 🎯 Problem

Network intrusion detection systems (IDS) need to classify traffic as benign or malicious in real time. This repo explores how classic ML models (decision trees) and ensemble boosting (AdaBoost) perform on this task, along with time-series patterns in traffic data.

## 📊 Dataset

<!-- Fill in: -->
- **Name:** e.g. NSL-KDD / UNSW-NB15 / CICIDS2017
- **Source:** link to dataset
- **Size:** number of records, number of features
- **Classes:** e.g. Normal, DoS, Probe, R2L, U2R

## ⚙️ Approach

<!-- Fill in: -->
- Preprocessing steps (encoding, scaling, feature selection)
- Train/test split ratio
- Models used and why (IREP decision tree, AdaBoost-boosted tree)
- Evaluation metrics used (accuracy, precision, recall, F1, confusion matrix)

## 📈 Results

<!-- Fill in a results table, e.g.: -->

| Model | Accuracy | Precision | Recall | F1-score |
|---|---|---|---|---|
| Decision Tree (IREP) | — | — | — | — |
| AdaBoost + Decision Tree | — | — | — | — |

<!-- Add a short takeaway, e.g. "AdaBoost improved recall on minority attack classes by X%" -->

## 🛠️ Tech Stack

Python · scikit-learn · pandas · NumPy · Matplotlib · Jupyter Notebook

## 🚀 How to Run

```bash
git clone https://github.com/shalu236616/ai-ml-intrusion-detection.git
cd ai-ml-intrusion-detection
pip install -r requirements.txt
jupyter notebook
```

## 📝 Notes

This work explores classical ML approaches to intrusion detection and connects to ongoing research into federated learning for secure IoT threat detection.
