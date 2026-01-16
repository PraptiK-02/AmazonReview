# Amazon Review Sentiment Analysis  
## Fast, Scalable Machine Learning for Text Classification

---

## 📌 Project Overview
Customer reviews contain valuable insights about product quality, customer satisfaction, and brand perception. However, review data is unstructured and large in volume, making manual analysis impractical.

This project builds a **fast and scalable sentiment analysis model** to automatically classify Amazon customer reviews as **Positive** or **Negative**. The goal is to demonstrate how classic machine learning techniques can efficiently transform large-scale text data into actionable insights.

This project is designed as a **portfolio-quality, real-world AI/ML use case** that balances performance, interpretability, and execution efficiency.

---

## 🎯 Why This Project?
I chose this project for three key reasons:

1. **Real-World Relevance**  
   Nearly every consumer-facing company relies on customer feedback. Automating sentiment analysis is a common and valuable business application of AI.

2. **Scalability & Practicality**  
   Instead of using computationally expensive deep learning models, this project demonstrates how traditional machine learning (TF-IDF + Logistic Regression) can achieve strong performance while remaining fast and scalable.

3. **Industry-Style Decision Making**  
   The project emphasizes trade-offs professionals make in practice: sampling large datasets, optimizing runtime, and prioritizing interpretability over complexity.

---

## 📊 Dataset Description
- **Dataset:** Amazon Reviews Polarity Dataset
- **Source:** Public benchmark dataset (used in academic and industry research)
- **Size:** ~35 million reviews in total (subset used in this project)
- **Labels:**
  - `1` → Negative sentiment
  - `2` → Positive sentiment
- **Features:**
  - Review title
  - Review text

Due to the large size and complex formatting of the raw dataset (quoted text with embedded commas and newlines), a **representative subset** of the data was used for efficient training and evaluation.

---

## 🛠️ Tools & Technologies
- **Python**
- **Pandas** – data loading and preprocessing
- **Scikit-learn**
  - TF-IDF Vectorizer
  - Logistic Regression
  - Model evaluation metrics
- **Matplotlib & Seaborn** – visualization
- **Google Colab** – development environment
- **Git & GitHub** – version control and project publishing

---

## 🧠 Methodology

### 1. Data Loading & Preparation
- Downloaded the dataset directly within Google Colab to avoid slow browser uploads
- Used robust CSV parsing to handle complex text formatting
- Sampled a manageable subset for efficient processing
- Combined review titles and review text for improved signal

### 2. Feature Engineering
- Converted text into numerical features using **TF-IDF**
- Limited feature space to balance speed and model quality

### 3. Model Training
- Trained a **Logistic Regression classifier**
- Chosen for:
  - Fast training and inference
  - Strong baseline performance
  - Interpretability

### 4. Evaluation
- Evaluated on a held-out test sample
- Metrics used:
  - Accuracy
  - Precision
  - Recall
  - F1-score
  - Confusion Matrix

---

## 📈 Results
- **Accuracy:** ~87% on an 8,000-review test sample
- **Balanced performance** across positive and negative classes
- Slightly higher recall for positive reviews, indicating strong ability to detect satisfied customers

These results demonstrate that traditional ML models can perform competitively on large-scale text classification tasks while remaining computationally efficient.

---

## 💡 Business Value
This model can be used to:
- Automatically summarize customer sentiment at scale
- Identify trends in positive and negative feedback
- Support product improvement and customer experience strategies
- Reduce manual effort in review analysis

---

