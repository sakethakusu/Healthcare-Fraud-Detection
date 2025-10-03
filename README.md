# Healthcare-Fraud-Detection
Machine learning project for healthcare provider fraud detection using Medicare claims data (~558K rows, 55 features). Includes preprocessing, feature engineering, Decision Tree model with hyperparameter tuning, evaluation (accuracy 94%, recall 88%), and visualizations for fraud risk detection.
# 🏥 Healthcare Provider Fraud Detection  

This project uses **machine learning** to detect fraudulent healthcare provider claims. By analyzing **Medicare claims data (558,000+ rows, 55 columns)**, we developed a **Decision Tree classifier** with optimized hyperparameters to flag high-risk providers for audits.  

---

## 📌 Project Overview  
- **Problem:** Fraudulent healthcare claims cost billions annually.  
- **Dataset:** 558,211 rows, 55 columns (beneficiary IDs, claim details, diagnosis/procedure codes, chronic condition indicators, fraud labels).  
- **Goal:** Build a fraud detection model to identify suspicious claims while minimizing false positives.  

---

## 🛠️ Methodology  

### Data Preprocessing  
- Dropped uninformative columns  
- Handled missing values via imputation  
- Balanced class distribution (fraud vs non-fraud)  

### Feature Engineering  
- Extracted diagnosis/procedure code features  
- Encoded categorical values  
- Aggregated claim-level statistics  

### Model Selection  
- **Decision Tree Classifier**  
- Hyperparameter tuning with **GridSearchCV**  
- Best depth = **13**, avoiding overfitting  

---

## 📊 Results  

- **Accuracy:** 94%  
- **Recall (Fraud Detection):** 88%  
- **ROC Curve:** High TPR, low FPR  
- **Feature Importance:** Diagnosis & procedure codes, claim durations were strong predictors  

📈 **Visual Outputs:**  
- Decision Tree Plot  
- Confusion Matrix  
- ROC Curve  
- Feature Importance Ranking  

---

## ⚡ Challenges  
- Missing and incomplete data  
- Imbalanced fraud vs non-fraud cases  
- Risk of overfitting with deep trees  
- Limited labeled fraud samples  

---

## 🔮 Future Work  
- Try **Random Forest & XGBoost** for better performance  
- Add **ensemble models** for balanced precision/recall  
- Incorporate **unsupervised anomaly detection**  
- Deploy fraud scoring tool for healthcare payers  

---

👩‍💻 **Developed by:**  
Group Project – Saketha Kusu & Team  
🎓 *MS Health Informatics – Michigan Technological University*  
