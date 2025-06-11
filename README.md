# 🧠 Kaiburr Task 5 – Text Classification on Consumer Complaint Dataset

## 📌 Project Overview
This project performs text classification on the [Consumer Complaint Dataset](https://catalog.data.gov/dataset/consumer-complaint-database) using Deep Learning (PyTorch). The goal is to classify complaints into the following categories:

| Label | Category                                        |
|-------|-------------------------------------------------|
| 0     | Credit reporting, repair, or other              |
| 1     | Debt collection                                 |
| 2     | Consumer Loan                                   |
| 3     | Mortgage                                        |

---

## 🧰 Technologies Used
- Python 3.x
- PyTorch
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn

---

## 🧪 Tasks Covered (Per Instructions)

| Task Step | Description |
|-----------|-------------|
| 1️⃣ EDA & Feature Engineering | Data cleaned, filtered, and mapped to labels |
| 2️⃣ Text Pre-processing | Lowercasing, tokenization, vocabulary building |
| 3️⃣ Model Selection | Custom BiLSTM model with embeddings (PyTorch) |
| 4️⃣ Model Comparison | (optional) Can be extended with classical models |
| 5️⃣ Model Evaluation | Accuracy and F1-score computed |
| 6️⃣ Prediction | Final prediction logic (to be demoed on sample text) |

---

## 📊 Dataset
- File: `complaints.csv`
- Source: [data.gov consumer complaint database](https://catalog.data.gov/dataset/consumer-complaint-database)
- Columns used: `product`, `complaint_what_happened`

---

## 🧠 Model Summary

- Custom PyTorch Dataset & Dataloader
- Vocabulary built using top occurring tokens
- Sequence padded and batch-loaded
- BiLSTM classification model trained
- Softmax output with cross-entropy loss

---

## 📈 Evaluation Metrics

- Accuracy
- F1-score (macro & per-class)
- Confusion matrix (optional)

---

## ▶️ How to Run

1. ### Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```
   
2. ### Launch the notebook:
   ```
   jupyter notebook code.ipynb
   
   ```
3. ### Run all cells in order, starting from data loading.

## 📸 Screenshots


### 🔹 Data Preprocessing
![Data Preprocessing](https://github.com/seenivasaperumal46/Kaiburr-Task-5/blob/400f8c63eb3386b7c35ff077cc569e368c865fdd/image-2.png)

### 🔹 Class Distribution Visualization
![Class Distribution Visualization](https://github.com/seenivasaperumal46/Kaiburr-Task-5/blob/400f8c63eb3386b7c35ff077cc569e368c865fdd/image-4.png)

### 🔹  Text Cleaning
![Text Cleaning](https://github.com/seenivasaperumal46/Kaiburr-Task-5/blob/400f8c63eb3386b7c35ff077cc569e368c865fdd/image-5.png)

### 🔹 Model Training
![Model Training](https://github.com/seenivasaperumal46/Kaiburr-Task-5/blob/400f8c63eb3386b7c35ff077cc569e368c865fdd/image-6.png)

### 🔹 Model Evaluation
![Model Evaluation](https://github.com/seenivasaperumal46/Kaiburr-Task-5/blob/400f8c63eb3386b7c35ff077cc569e368c865fdd/image-8.png)

### 🔹 Final Result & Output
We predict a sample complaint:

"There is a hard inquiry I didn’t authorize."

![Final Result & Output](https://github.com/seenivasaperumal46/Kaiburr-Task-5/blob/400f8c63eb3386b7c35ff077cc569e368c865fdd/image-1.png)
