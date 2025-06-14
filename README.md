# 🧠 Parkinson's Disease Detection using SVM and XGBoost

## 🩺 Problem Statement

Parkinson’s Disease is a progressive neurological disorder that affects movement and speech. Early and accurate detection is crucial for timely treatment and better patient outcomes. This project aims to develop a machine learning model that can classify whether a person has Parkinson’s Disease using voice-based biomedical features.

---

## 📂 Dataset

* **Source**: [Click here to view the dataset](#) *(add actual link)*
* **Features**: Biomedical voice measurements like:

  * MDVP\:Fo(Hz), MDVP\:Fhi(Hz), MDVP\:Flo(Hz)
  * Jitter (% and Abs), Shimmer
  * Harmonic-to-Noise Ratio (HNR), Spread1, PPE, etc.
* **Target**: `status`

  * `1` = Parkinson's Disease
  * `0` = Healthy

---

## 🧰 Tech Stack

* **Language**: Python
* **Libraries**:

  * `Pandas`, `NumPy` – Data handling
  * `Matplotlib`, `Seaborn` – Data visualization
  * `scikit-learn` – Preprocessing & SVM
  * `XGBoost` – Boosting-based classification
* **Platform**: Jupyter Notebook

---

## ⚙️ Workflow

### 1. 📥 Data Loading and Exploration

* Loaded dataset using Pandas
* Checked for null values, duplicates, class balance

### 2. 📊 Exploratory Data Analysis (EDA)

* Visualized correlation matrix
* Plotted feature distributions
* Compared key features across classes

### 3. 🧠 Feature Selection

* Removed weakly correlated features
* Retained influential predictors like `MDVP:Fo(Hz)`, `Spread1`, and `PPE`

### 4. 🧼 Data Preprocessing

* Applied `StandardScaler` for feature scaling
* Performed train-test split

### 5. 🏗️ Model Building

* **Support Vector Machine (SVM)**: Effective for small, high-dimensional datasets
* **XGBoost**: Gradient boosting classifier ideal for capturing complex patterns

### 6. 📈 Model Evaluation

* Evaluated using Accuracy Score & Confusion Matrix
* (Optional) Explored ensemble performance

---

## 📊 Results

| Model   | Accuracy |
| ------- | -------- |
| SVM     | \~92%    |
| XGBoost | \~94%    |

> Both models achieved high accuracy, with XGBoost showing superior performance. Its robustness makes it suitable for real-world healthcare applications for early Parkinson’s detection.

---

## 💡 Future Improvements

* Incorporate additional clinical data beyond voice features
* Implement Deep Learning models (e.g., LSTM/CNN) for time-series voice signal analysis
* Experiment with ensemble methods (stacking, voting) for improved performance
* Develop a user-friendly front-end UI for real-time disease prediction

---

## 👨‍💻 Project Owner

This project is developed and maintained by **Sanchit Singh** as part of a practical journey into applying machine learning in healthcare diagnostics.

---

## 🚀 Final Note

This project showcases the potential of machine learning in supporting early medical diagnosis. With interpretable models and high accuracy, algorithms like **SVM** and **XGBoost** offer promising steps toward accessible, AI-powered healthcare solutions.
