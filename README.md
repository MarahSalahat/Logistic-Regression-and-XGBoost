# 📧 SMS Spam Detection using XGBoost

This project focuses on classifying SMS messages as **ham** (legitimate) or **spam** using machine learning techniques. It demonstrates a full pipeline including data cleaning, text preprocessing, feature extraction, and model training with **XGBoost**, a powerful gradient boosting algorithm.

## 📁 Dataset

The dataset used is the classic **SMS Spam Collection**, containing labeled messages:
- `ham`: Non-spam messages
- `spam`: Unwanted promotional or fraudulent messages

📍 File used: `spam.csv`  
📍 Encoding: `ISO-8859-1`

## 🧹 Preprocessing Steps

- Converted all text to lowercase
- Removed non-alphanumeric characters using regular expressions
- Vectorized messages using **TF-IDF (Term Frequency-Inverse Document Frequency)**

## 🛠️ Technologies Used

- Python
- pandas, numpy
- scikit-learn
- XGBoost
- TF-IDF Vectorizer

## 🧠 Model

### ✅ **XGBoost Classifier**
- `n_estimators=100`
- `learning_rate=0.1`
- `random_state=42`

### ✨ Performance

| Metric      | Ham (0) | Spam (1) |
|-------------|---------|----------|
| Precision   | 0.97    | 0.99     |
| Recall      | 1.00    | 0.83     |
| F1-Score    | 0.99    | 0.91     |

**Overall Accuracy**: `97.7%` on the test set



