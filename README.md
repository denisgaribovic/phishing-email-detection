![alt text](https://raw.githubusercontent.com/denisgaribovic/phishing-email-detection/main/Banner.png)

# 🛡️ Phishing Email Detection

A **machine learning project** designed to automatically **detect phishing emails** using text analysis and engineered features. This model helps organizations identify suspicious emails early, protecting users from cyber attacks and financial fraud through intelligent email screening.

---

## ✨ Highlights

- 📧 Built on the CEAS 2008 phishing email dataset with thousands of labeled emails  
- 🔍 Extracted and engineered features like suspicious words, URL counts, and sender domains  
- ⚙️ Used TF-IDF vectorization with uni- and bi-grams for rich text representation  
- 🤖 Trained and tuned a Logistic Regression model optimized for phishing detection  
- 📊 Visualized key phishing indicators using word clouds, bar charts, and confusion matrix  
- 🔥 Demonstrated strong model performance with F1-score and ROC AUC metrics  
- 🔄 Modular pipeline for preprocessing, training, evaluation, and insightful analysis  

---

## 🎯 Business Context

Phishing remains one of the biggest cybersecurity threats worldwide, causing billions in losses and data breaches annually. Organizations need robust tools to:  
- Detect phishing emails before they reach users’ inboxes  
- Reduce fraud, identity theft, and reputational damage  
- Automate email threat detection to improve efficiency and response times  

This project exemplifies how machine learning can be applied to:  
- Analyze email content and metadata to flag suspicious patterns  
- Build interpretable models that highlight what triggers phishing alerts  
- Support security teams and awareness platforms with actionable intelligence  

---

## 🛠️ Project Workflow

### 1. 📁 Data Loading & Cleaning

- Loaded and cleaned the CEAS 2008 email dataset  
- Removed HTML, URLs, digits, and stopwords from email texts  
- Extracted sender domains and destination URL domains  

### 2. 🔍 Feature Engineering

- Counted suspicious phishing-related words per email  
- Created numeric features like number of URLs and suspicious word counts  
- Vectorized text using TF-IDF with n-grams (unigrams + bigrams)  

### 3. 🤖 Model Training & Tuning

- Combined text vectors and numeric features into a single feature matrix  
- Trained Logistic Regression model with hyperparameter tuning via Grid Search  
- Maintained class balance using stratified train-test split  

### 4. 📈 Evaluation & Visualization

- Evaluated model performance with F1-score and ROC AUC  
- Visualized top phishing-indicative words and sender domains with word clouds and bar charts  
- Generated confusion matrix heatmap for prediction analysis  

---

## 🚀 How To Use

1. Clone the repo  
2. Install dependencies (`scikit-learn`, `pandas`, `numpy`, `matplotlib`, `seaborn`, `wordcloud`)  
3. Run preprocessing scripts to clean and extract features from emails  
4. Train and tune the model using the provided pipeline  
5. Explore visualizations to understand phishing patterns  
6. Integrate or extend the model for real-world email filtering applications  

---

## 📚 Resources & Dataset

- Dataset: [CEAS 2008 Email Dataset](https://www.kaggle.com/datasets/naserabdullahalam/phishing-email-dataset)  
- Python libraries used: scikit-learn, pandas, numpy, matplotlib, seaborn, wordcloud  
