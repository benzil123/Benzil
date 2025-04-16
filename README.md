
---

###  Traffic Incident Detection from Tweets

This project detects whether a tweet describes a **traffic incident** or not using natural language processing (NLP) and machine learning.

---

###  Files

- `traffic_tweet_classifier.py`: Main script for training and testing the model.
- `fixed_tweets.csv`: Cleaned CSV dataset containing tweet text.
- `README.md`: This file.

---

###  Requirements

Install the required Python packages using:

```bash
pip install pandas numpy scikit-learn nltk
```

---

###  What It Does

1. Cleans tweet text (removes URLs, punctuation, etc.)
2. Labels each tweet as:
   - `1` = Traffic Incident
   - `0` = Not a Traffic Incident  
3. Converts text to features using TF-IDF.
4. Trains a **Logistic Regression** classifier.
5. Prints accuracy and classification report.

---

###  How to Run

```bash
python traffic_tweet_classifier.py
```

---

###  Example Output

```
Accuracy: 0.86

Classification Report:
              precision    recall  f1-score   support

           0       0.87      0.90      0.88       30
           1       0.85      0.81      0.83       20

    accuracy                           0.86       50
```

---

###  Notes

- Tweets are labeled using a simple keyword match (e.g. "accident", "jam").
- You can improve it by training on manually labeled data or using deep learning.

---
