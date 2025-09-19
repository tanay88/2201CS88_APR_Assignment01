# 📩 YouTube–Twitter–SMS Spam Detection (Naive Bayes)

This project demonstrates how to build a **Spam Detection System** using **Naive Bayes** with **TF–IDF vectorization**.  
It classifies messages (from YouTube, Twitter, and SMS) as either **Ham (legitimate)** or **Spam**.  

The dataset used is: [YouTube-Twitter-SMS Spam Dataset](https://www.kaggle.com/datasets) (`Final-Dataset.csv`).

---

## 🚀 Project Workflow
1. **Load Dataset** – Read the spam dataset (`Final-Dataset.csv`).
2. **Preprocessing** – Select `FORMATTED_CONTENT` (text) and `CLASS` (label).
3. **Train-Test Split** – 80% training, 20% testing.
4. **Feature Extraction** – Convert text into numerical features using **TF-IDF**.
5. **Model Training** – Train a **Multinomial Naive Bayes** classifier.
6. **Evaluation** – Classification report, confusion matrix, accuracy metrics.
7. **Regularization Analysis** – Compare effect of different smoothing factors (`alpha`) on accuracy.

---

## 📊 Visualizations
The project generates:
- Confusion Matrix (Heatmap)  
- Train vs Test Error Comparison  
- Alpha vs Accuracy Curve (Effect of regularization)

---

## 📂 Dataset
Dataset is located at: /kaggle/input/youtube-twitter-sms-spam-dataset/Final-Dataset.csv


Columns used:
- `FORMATTED_CONTENT` → Message text  
- `CLASS` → Label (`0 = Ham`, `1 = Spam`)

---

## 🛠️ Installation & Requirements
Install dependencies:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn

Key Learnings

TF–IDF vectorization improves performance over simple Bag-of-Words.

Naive Bayes is fast, interpretable, and effective for spam filtering tasks.

Regularization (alpha) helps balance bias–variance tradeoff.

Train Accuracy: 0.7669
Test Accuracy : 0.7523


