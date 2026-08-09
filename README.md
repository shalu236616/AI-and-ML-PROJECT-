# AI & ML for Cyber Security — Projects

Machine learning and deep learning experiments applying classical ML, ensemble methods, and neural networks to network intrusion detection, network security , IoT security and threat detection. and phishing website detection. 

---
## 📂 Contents
| Notebook | What it does |
## Featured Research Project

### 🔐 Federated IoT Intrusion Detection using q-Sigmoid

My M.Tech research project investigates the use of
Tsallis-statistics-based q-Sigmoid loss in Federated Learning
for IoT intrusion detection under imbalanced and non-IID data.

**Key topics:**

- Federated Learning
- IoT Cybersecurity
- Intrusion Detection
- q-Sigmoid Loss
- Tsallis Statistics
- Non-IID Learning
- Adaptive PerClient-q
- Machine Learning

**Datasets:**

- UNSW-NB15
- WUSTL-IIoT-2021
- CSE-CIC-IDS2018

👉 [View the complete thesis project](Federated-IoT-Intrusion-Detection-qSigmoid/)
| `IREP_Decision_Tree_On_Intrusion_detection.ipynb` | Trains a decision tree on network intrusion data, then extracts and prunes classification rules from the tree using a simplified IREP-style (Incremental Reduced Error Pruning) approach |
| `modification_of_decision_tree_using_AdaBoost.ipynb` | Benchmarks Decision Tree, AdaBoost (boosted decision stumps), and Logistic Regression on the same intrusion detection dataset |
| `PROJECT_WORK.ipynb` | Phishing website detection using a Keras neural network, benchmarked against Random Forest, XGBoost, Logistic Regression, and SVM |
| `Analyze_Time_Series_Network_Traffic_Data.ipynb` | Exploratory time-series analysis of network traffic — request patterns by source IP and traffic volume by hour |

## 📊 Datasets

- **Intrusion detection** — `cybersecurity_intrusion_data.csv`: 9,537 sessions, 11 features (network packet size, protocol type, login attempts, session duration, encryption used, IP reputation score, failed logins, browser type, unusual time access). Binary target `attack_detected` (5,273 normal / 4,264 attack).
- **Phishing detection** — `phishing website dataset.csv`: 11,055 URLs, 30 features (SSL state, URL length, domain age, web traffic rank, use of shortening services, etc.). Binary target `Result`.
- **Network traffic** — `time_series_network_traffic.csv`: 1,000 records of timestamp, source/destination IP, and data transferred (MB).

## 📈 Results

### Intrusion Detection

| Model | Accuracy |
|---|---|
| Decision Tree (gini, max_depth=6) | 89.67% |
| AdaBoost (1000 decision stumps) | 86.79% |
| Decision Tree (baseline, AdaBoost notebook) | 82.39% |
| Logistic Regression | 74.69% |
| Pruned rule set (IREP-style extraction) | 55.29% |

> The rule-extraction approach trades accuracy for interpretability — it's included to show that trade-off explicitly, not as the top-performing model. AdaBoost's 5-fold cross-validation accuracy stayed consistent (~86–88%), confirming it wasn't overfitting.

### Phishing Website Detection

| Model | Accuracy |
|---|---|
| XGBoost | 97.15% |
| Neural Network (Keras, 64-32-16-1) | 97.01% |
| Random Forest | 96.61% |
| Logistic Regression | 92.94% |
| SVM (RBF kernel) | 66.21% |

## 🛠️ Tech Stack

Python · scikit-learn · TensorFlow/Keras · XGBoost · pandas · NumPy · Matplotlib · Seaborn

## 🚀 How to Run

```bash
git clone https://github.com/shalu236616/ai-ml-cybersecurity-projects.git
cd ai-ml-cybersecurity-projects
pip install -r requirements.txt
jupyter notebook
```

## 👤 Author

Shalu Tiwari — M.Tech (CS), South Asian University

## 📝 Notes

Coursework and self-directed exploration in applied ML for cybersecurity, spanning classical ML, ensemble methods, and deep learning. The intrusion detection work connects to ongoing thesis research in federated learning for secure IoT threat detection.
