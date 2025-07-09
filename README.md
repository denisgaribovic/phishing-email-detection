![alt text](https://raw.githubusercontent.com/denisgaribovic/phishing-email-detection/main/Banner.png)

# 🛡️ Phishing Email Detection

A production-ready machine learning pipeline that detects phishing emails using both natural language processing (NLP) and metadata-based features. This project simulates how security teams can **automate email threat detection**, minimize human error, and strengthen cybersecurity defenses — powered by interpretable, scalable models.

---

## 🎯 Business Context

Phishing remains one of the **top cybersecurity threats**, used to trick users into exposing credentials or downloading malware. Detecting these attacks early helps organizations:

- Prevent data breaches, identity theft, and financial fraud  
- Reduce incident response time and SOC workload  
- Enhance email security with ML-powered automation  
- Train users and improve awareness with real-world examples

This project provides a practical, lightweight solution that can be integrated into existing **email gateways**, **alerting pipelines**, or **user awareness platforms**.

---

## ✨ Project Highlights

- 📬 Analyzed thousands of labeled emails from the [CEAS 2008 Phishing Dataset](https://www.kaggle.com/datasets/naserabdullahalam/phishing-email-dataset)
- 🧠 Combined TF-IDF text vectors with custom-engineered metadata features
- ⚖️ Trained and optimized a Logistic Regression classifier using GridSearchCV
- 📊 Evaluated with Precision, Recall, F1 Score, and ROC AUC to handle imbalanced classes
- 🔍 Visualized top phishing keywords, URL domains, and sender patterns
- 🧩 Modular and extensible — adaptable for modern SOC and email filtering systems

---

## ✅ Real-World Applications

This model can be adapted or extended to power:

- Email security filters (pre-screening for SOC teams)
- Threat triage dashboards (e.g. custom internal tools)
- Research into phishing tactics and social engineering
- Awareness training with realistic phishing examples

---

## 💡 Key Takeaways

- Text + metadata fusion dramatically improves classification accuracy
- Visuals help explain model behavior to non-technical stakeholders
- Even simple models like Logistic Regression can be powerful with the right features
- This pipeline is lightweight, interpretable, and production-ready
