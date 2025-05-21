#  Credit Card Fraud Detection

A machine learning project to detect fraudulent credit card transactions using supervised classification models. The dataset used is highly imbalanced, reflecting real-world fraud detection challenges.

---

##  Dataset

- Source: [Kaggle Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- Contains transactions made by European cardholders in September 2013.
- Features: 28 anonymized PCA components + `Time`, `Amount`
- Target variable: `Class` (0 = non-fraud, 1 = fraud)

---

##  Objective

Detect fraudulent transactions with high **recall** and **precision**, while addressing class imbalance and ensuring robust evaluation.

---

##  Workflow

1. **Data Preprocessing**
   - Standard scaling for `Amount`
   - Stratified train-test split (80/20)

2. **Modeling**
   - Logistic Regression
   - Random Forest
   - XGBoost

3. **Evaluation Metrics**
   - Accuracy
   - Precision
   - Recall
   - F1-Score
   - ROC AUC Score
   - ROC Curve Visualization

---

##  Model Performance

| Model               | Accuracy | Precision | Recall   | F1-Score | ROC AUC |
|--------------------|----------|-----------|----------|----------|---------|
| Logistic Regression| 0.9745   | 0.0587    | 0.9184   | 0.1104   | 0.9714  |
| Random Forest       | 0.9996   | 0.9740    | 0.7653   | 0.8571   | 0.9525  |
| XGBoost             | 0.9973   | 0.3750    | 0.8878   | 0.5273   | 0.9759  |

---

##  Visualizations

- ROC Curves plotted separately for each model
---

##  Tools & Libraries

- Python
- Pandas, NumPy
- scikit-learn
- XGBoost
- Matplotlib, Seaborn

---

##  Future Improvements

- Use of SMOTE or other oversampling methods
- Hyperparameter tuning with GridSearchCV
- Real-time fraud detection simulation with Streamlit or Flask
- Feature explainability with SHAP

---

##  Conclusion

The Random Forest model delivered the best **overall precision and F1-score**, while **Logistic Regression and XGBoost** achieved higher recall, crucial for fraud detection where minimizing false negatives is key.

---

##  Author

**Harsh Nagar**  
A machine learning enthusiast exploring real-world applications of AI and data science.

---

## 📎 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
