![alt text](https://raw.githubusercontent.com/denisgaribovic/phishing-email-detection/main/Banner.png)

# 🛡️ Phishing Email Detection

A production-ready machine learning pipeline that detects phishing emails using both natural language processing (NLP) and metadata-based features. This project simulates how security teams can **automate email threat detection**, minimize human error, and strengthen cybersecurity defenses — powered by interpretable, scalable models.

---

## ✨ Highlights

- 📬 Analyzed thousands of labeled emails from the [CEAS 2008 Phishing Dataset](https://www.kaggle.com/datasets/naserabdullahalam/phishing-email-dataset)
- 🧠 Combined TF-IDF text vectors with custom-engineered metadata features
- ⚖️ Trained and optimized a Logistic Regression classifier using GridSearchCV
- 📊 Evaluated with Precision, Recall, F1 Score, and ROC AUC to handle imbalanced classes
- 🔍 Visualized top phishing keywords, URL domains, and sender patterns
- 🧩 Modular and extensible — adaptable for modern SOC and email filtering systems

---

## 🎯 Business Context

Phishing remains one of the **top cybersecurity threats**, used to trick users into exposing credentials or downloading malware. Detecting these attacks early helps organizations:

- 🛡️ Prevent data breaches, identity theft, and financial fraud  
- 📉 Reduce incident response time and SOC workload  
- 🔐 Enhance email security with ML-powered automation  
- 💡 Train users and improve awareness with real-world examples

This project provides a practical, lightweight solution that can be integrated into existing **email gateways**, **alerting pipelines**, or **user awareness platforms** like KnowBe4.

---

## 🔐 Real-World Applications

This model can be adapted or extended to power:

- ✅ Email security filters (pre-screening for SOC teams)
- 🧠 Threat triage dashboards (e.g. custom internal tools)
- 🧪 Research into phishing tactics and social engineering
- 🎓 Awareness training with realistic phishing examples

---

## 📚 Dataset Overview

We used the **CEAS 2008 Email Dataset**, a benchmark dataset for phishing research. It contains a mix of phishing and legitimate emails, with real headers, body text, and links.

Key features engineered from each email:

| Feature | Description |
|--------|-------------|
| `email_text` | Raw subject + body content of the email |
| `sender_domain` | Extracted from the `From` field |
| `url_domains` | Domains of all URLs found in the message |
| `url_count` | Number of URLs in the email |
| `keyword_count` | Frequency of suspicious terms (e.g. "urgent", "verify") |

---

## 🛠️ Project Workflow

### 1. 📥 Data Preparation

- Loaded and cleaned raw email text
- Extracted metadata (sender domain, URL domains, keyword frequency)
- Removed HTML, stopwords, and special characters from body text

### 2. 🧱 Feature Engineering

- Created TF-IDF vectors (uni/bi-grams) for email text
- Combined with structured metadata (URL count, keyword flags)
- Used `scipy.hstack()` to merge into a single sparse feature matrix

### 3. 🤖 Model Training & Tuning

- Split data using stratified train-test split to preserve class balance
- Trained Logistic Regression (baseline) with `liblinear` solver
- Performed hyperparameter tuning over regularization strength (`C`)

### 4. 📈 Model Evaluation

- Assessed using:
  - ✅ F1 Score (preferred for imbalanced binary classification)
  - 🔍 ROC AUC Curve
  - 📉 Confusion Matrix
- Visualized:
  - Top phishing indicators by coefficient weight
  - Most common phishing sender domains and URLs
  - Word clouds for phishing vs legitimate emails

---

## 💡 Key Takeaways

- 🧠 Text + metadata fusion dramatically improves classification accuracy
- 🔍 Visuals help explain model behavior to non-technical stakeholders
- 🔐 Even simple models like Logistic Regression can be powerful with the right features
- 🚀 This pipeline is lightweight, interpretable, and production-ready
