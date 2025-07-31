# 🧠 Text Classification using Naive Bayes

This project demonstrates **text classification** using the **Naive Bayes algorithm** on the popular **SMS Spam Collection Dataset**. The model classifies SMS messages as **spam** or **ham (not spam)** based on the message content.

---

## 📌 What is Naive Bayes?

**Naive Bayes** is a probabilistic classifier based on **Bayes' Theorem**, assuming that features are independent given the class label.

### Bayes’ Theorem:
\[
P(C|X) = \frac{P(X|C) \cdot P(C)}{P(X)}
\]
Where:
- \( P(C|X) \) is the posterior probability of class \( C \) given feature \( X \)
- \( P(X|C) \) is the likelihood of feature \( X \) given class \( C \)
- \( P(C) \) is the prior probability of class \( C \)
- \( P(X) \) is the evidence or overall probability of feature \( X \)

---

## 📂 Dataset

**SMS Spam Collection Dataset**  
- Source: [UCI Repository](https://archive.ics.uci.edu/ml/datasets/sms+spam+collection)
- Format: Tab-separated values (`.tsv`)
- Shape: **5572 rows × 2 columns**
  - `label`: `spam` or `ham`
  - `message`: text message content

### 📊 Class Distribution:
- **Ham**: 4825 messages  
- **Spam**: 747 messages

---

## 📈 Project Workflow

### ✅ Step 1: Import Libraries

Standard Python libraries for data handling, machine learning, and visualization.

### ✅ Step 2: Load and Inspect Dataset

- Print the first few rows
- Display shape, info, and description
- Plot class distribution
- Check and handle missing values (none in this dataset)

### ✅ Step 3: Preprocessing

- Encode labels (`spam` = 1, `ham` = 0)
- Split data into train and test sets
- Convert text to numerical features using **Bag of Words** with `CountVectorizer`

### ✅ Step 4: Model Training

- Use **Multinomial Naive Bayes** (best for text data with word counts)

### ✅ Step 5: Evaluation

- Compute **accuracy**, **confusion matrix**, and **classification report**
- Visualize confusion matrix using `seaborn`

---

## 🔍 Model Performance

| Metric      | Value      |
|-------------|------------|
| Accuracy    | ~98.5%     |
| Precision   | High       |
| Recall      | High       |
| F1 Score    | Balanced   |

### 🌀 Confusion Matrix Example:

