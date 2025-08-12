📌 Task 3 – Decision Tree Classifier on Bank Marketing Dataset

This project was completed as part of my **Data Science Internship at Prodigy InfoTech**.
The goal was to **build a Decision Tree Classifier** to predict whether a customer will subscribe to a term deposit based on their demographic and behavioral data.

---

📊 Dataset

* **Source:** [UCI Machine Learning Repository – Bank Marketing Dataset](https://archive.ics.uci.edu/ml/datasets/bank+marketing)
* **File Used:** `bank-additional-full.csv`
* **Shape:** 41,188 rows × 21 columns
* **Target Variable:** `y` (Yes = customer subscribed to term deposit, No = did not subscribe)

---

🎯 Problem Statement

Predict whether a customer will subscribe to a term deposit using demographic and behavioral features such as age, job, marital status, previous campaign contact, etc.

---

🛠️ Preprocessing Steps

* **Dropped irrelevant columns** → `duration` (not useful for prediction before the call is made).
* **Processed `pdays`** → created a flag for previous contact and replaced `-1` with `0`.
* **Encoded categorical features** → One-Hot Encoding.
* **Stratified Train/Test Split** → preserved target distribution across splits.

---

🤖 Model Building

* **Algorithm:** Decision Tree Classifier
* **Hyperparameter Tuning:** `GridSearchCV` to find best depth, split, and leaf parameters.
* **Class Balancing:** `class_weight='balanced'` to handle target imbalance.

---

📈 Evaluation Metrics

* **Accuracy**
* **Precision**
* **Recall**
* **F1-Score**
* **ROC AUC Score**
* **Confusion Matrix Visualization**

---

🔍 Key Features (Top 10 by Importance)

* `emp.var.rate`
* `euribor3m`
* `nr.employed`
* `cons.price.idx`
* `age`
* `previous`
* `cons.conf.idx`
* `pdays`
* `contact_cellular`
* `month`

---

📊 Results

The tuned Decision Tree model achieved:

* **Accuracy:** 84%
* **F1-Score:** 86%
* **ROC AUC:** 78.68%

If you want, I can also make you a **visually styled README** with emojis, sections, and banners to make your GitHub repo look even more professional. That would make it stand out like a portfolio piece.
