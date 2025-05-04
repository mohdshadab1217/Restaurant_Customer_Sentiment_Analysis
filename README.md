# 🧠 Restaurant Review Sentiment Analysis

This project uses **scikit-learn** to train a binary sentiment classification model based on restaurant review summaries.

## 📝 Project Objective

To classify customer sentiment as positive (rating 4 or 5) or negative (rating 1 or 2) using the `Summary` of a review.

## 📊 Dataset

- Source: `Reviews.csv`
- Features used:
  - `Summary`: Text of the review summary
  - `Score`: Numerical rating (1 to 5)
- Labels:
  - 1 → Positive (Score 4 or 5)
  - 0 → Negative (Score 1 or 2)

## 🔧 Preprocessing

- Removed missing values.
- Filtered neutral scores (e.g., Score = 3).
- Applied text preprocessing (e.g., lowercasing, punctuation removal).
- Vectorized text using TFIDF.

## 🤖 Model

- Trained with MultinomialNB (can be changed to other classifiers).
- Used `train_test_split` for validation.
- Evaluation metrics: Accuracy, Confusion Matrix.

## 🚀 How to Run

1. **Install dependencies**:
 pip install pandas scikit-learn

2. Run the notebook:
 Launch main.ipynb in Jupyter and execute all cells.

## 📌 Notes
1. The model uses only review summaries, not full review text.

2. Neutral ratings (score = 3) are ignored during training.

### 📜 License
For educational use. Dataset credit: Kaggle Amazon Fine Food Reviews Dataset