# 📧 Spam Email Detection using Machine Learning

A complete **Machine Learning** project that classifies emails as **Spam** or **Not Spam** using **Logistic Regression** and **TF-IDF Vectorization**. The project includes the entire ML pipeline—from data preprocessing and model training to deployment as an interactive **Flask web application**.

---

## 🚀 Features

* 📊 Exploratory Data Analysis (EDA)
* 🧹 Data Cleaning & Preprocessing
* 📝 TF-IDF Text Vectorization
* 🤖 Logistic Regression Classifier
* 📈 Model Evaluation
* 🌐 Flask Web Application
* 🎨 Responsive HTML & CSS Interface

---

## 📂 Project Structure

```text
Spam-Detection/
│
├── app.py                     # Flask application
├── train_model.py             # Model training script
├── spam_or_not_spam.csv       # Dataset
├── model.pkl                  # Trained model
├── vectorizer.pkl             # Saved TF-IDF vectorizer
├
├── README.md
│
├── templates/
│   └── index.html
│
├── static/
│   ├── style.css
│   
│
└── images/
    ├── demo.png
    └── roc_auc_curve.png
    |__confusion_matrix.png

```

---

## 📌 Dataset

**Dataset:** `spam_or_not_spam.csv`

The dataset contains labeled email messages classified into:

* Spam
* Not Spam

---

## ⚙️ Workflow

### 1️⃣ Data Loading

* Loaded dataset using Pandas
* Inspected data types
* Checked dataset dimensions

---

### 2️⃣ Data Cleaning

Performed preprocessing by:

* Removing duplicate emails
* Removing missing values
* Preparing clean training data

---

### 3️⃣ Exploratory Data Analysis

* Dataset distribution
* Class balance
* Basic visualizations
* Statistical overview

---

### 4️⃣ Text Vectorization

Email text is converted into numerical features using **TF-IDF (Term Frequency–Inverse Document Frequency)**.

Benefits:

* Captures important words
* Reduces influence of common words
* Produces sparse numerical vectors suitable for machine learning

---

### 5️⃣ Model Training

The classifier used is:

* **Logistic Regression**

Reasons for choosing Logistic Regression:

* Fast to train
* Computationally efficient
* Performs well on high-dimensional sparse text data
* Easily interpretable

---

### 6️⃣ Model Evaluation

The model is evaluated using:

* Accuracy
* Confusion Matrix
* Precision
* Recall
* F1-Score
* Classification report

---

## 🌐 Flask Web Application

The project includes a user-friendly Flask web application where users can:

* Paste an email
* Click **Predict**
* Instantly view whether the email is **Spam** or **Not Spam**

---

## 🛠️ Technologies Used

### Programming Language

* Python

### Machine Learning

* Scikit-learn

### Data Analysis

* Pandas
* NumPy

### Visualization

* Matplotlib

### Web Framework

* Flask

### Frontend

* HTML5
* CSS3

Run the Flask application:

```bash
python app.py
```

Open your browser and visit:

```
http://127.0.0.1:5000
```

---

## ▶️ How to Use

1. Launch the Flask application.
2. Paste an email into the input field.
3. Click **Predict**.
4. The model classifies the email as:

   * ✅ Not Spam
   * 🚨 Spam

---

## 📈 Results

The Logistic Regression model demonstrates strong performance for spam classification using TF-IDF features.

| Metric    |  Value |
| --------- | -----: |
| Accuracy  | 95.65% |
| Precision | 70.93% |
| F1-Score  | 82.99% |

## 💡 Future Improvements

* Compare Logistic Regression with:

  * Naive Bayes
  * Support Vector Machine (SVM)
  * Random Forest
* Hyperparameter tuning using **Optuna**
* Deep Learning models (LSTM/BERT)
