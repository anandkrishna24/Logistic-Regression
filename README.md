# Credit Card Fraud Detection – Logistic Regression

## 🧩 Dataset
- **Source**: Kaggle Credit Card Fraud Detection  
- **Size**: 284,807 transactions (492 frauds), binary `Class` label.

## ✅ Methodology
1. Load dataset and split (80/20 stratified).
2. Standardize features.
3. Apply logistic regression with `class_weight='balanced'`.
4. Predict probabilities → threshold = 0.5 (default).
5. Evaluate:
   - Confusion Matrix
   - Precision, Recall, F1-score
   - ROC-AUC Score
6. Visualizations:
   - Confusion matrix
   - ROC curve
   - Sigmoid function plot
7. Threshold adjustment demo.

## 📈 Results (example)
- **ROC-AUC**: ~0.93–0.95
- **Recall** (fraud): higher due to balanced weights
- Visuals located in `/plots`

## 🔧 Instructions
1. Place `creditcard.csv` in the root folder.
2. Run the notebook to train and evaluate.
3. View or include the plots from `/plots`.

---

### 💡 Explanation
- **class_weight='balanced'** helps address extreme imbalance.
- The sigmoid plot shows how raw scores map to probabilities.
- ROC curve and AUC highlight trade-off between detecting fraud vs false positives.
- Threshold tuning allows prioritizing recall or precision as needed.
