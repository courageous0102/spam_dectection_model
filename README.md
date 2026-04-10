# 📧 Spam Detection Model using Logistic Regression

## 🚀 Project Overview

This project is a **Spam Mail Detection System** built using **Machine Learning (Logistic Regression)**.
It classifies messages/emails as **Spam (1)** or **Ham (0)** based on their content.

The model uses **TF-IDF (Term Frequency - Inverse Document Frequency)** to convert text data into numerical features.

---

## 🧠 Key Concepts Used

* Natural Language Processing (NLP)
* TF-IDF Vectorization
* Logistic Regression
* Text Classification

---

## 📂 Project Structure

```
spam-detection/
│
├── spam_model.py        # Main ML model code
├── dataset.csv          # Dataset (spam/ham messages)
├── requirements.txt     # Dependencies
└── README.md            # Project documentation
```

---

## ⚙️ Technologies Used

* Python 🐍
* Scikit-learn
* Pandas
* NumPy

---

## 📊 Dataset

The dataset contains labeled messages:

* **Spam (1)** → Unwanted / promotional / scam messages
* **Ham (0)** → Normal / safe messages

Example:

| Message               | Label |
| --------------------- | ----- |
| "Win money now!"      | Spam  |
| "Let's meet tomorrow" | Ham   |

---

## 🔧 Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/spam-detection.git
cd spam-detection
```

### 2️⃣ Create Virtual Environment (Optional but Recommended)

```bash
python -m venv venv
venv\Scripts\activate   # Windows
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ How to Run

```bash
python spam_model.py
```

---

## 🧪 Example Usage

```python
input_mail = ["Congratulations! You won a free ticket"]

input_features = feature_extraction.transform(input_mail)

prediction = model.predict(input_features)

if prediction[0] == 1:
    print("Spam Mail")
else:
    print("Ham Mail")
```

---

## 🔍 How It Works

1. **Text Preprocessing**

   * Convert to lowercase
   * Remove stopwords

2. **Feature Extraction**

   * TF-IDF converts text into numerical vectors

3. **Model Training**

   * Logistic Regression learns patterns from data

4. **Prediction**

   * Classifies new messages as Spam or Ham

---

## 🎯 Features

* Simple and efficient model
* High accuracy for basic spam detection
* Easy to extend with advanced models

---

## ⚠️ Limitations

* May fail on very complex or new spam patterns
* Depends heavily on dataset quality

---

## 🚀 Future Improvements

* Use advanced models (Naive Bayes, SVM, Deep Learning)
* Add GUI/Web interface
* Improve preprocessing (stemming, lemmatization)

---

## 🤝 Contributing

Feel free to fork this repository and contribute improvements.

---

## 📜 License

This project is open-source and free to use.

---

## 💡 Author

Developed as a beginner-friendly Machine Learning project for learning NLP and classification.
