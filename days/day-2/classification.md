START
  │
  ▼
1. Problem samjho
   ├─ Binary classification?
   └─ Multi-class classification?
  │
  ▼
2. Basic data checks
   ├─ Missing values?
   ├─ Categorical features?
   └─ ID columns?
  │
  ├─ Drop ID columns
  ├─ Handle missing values
  └─ Encode categorical features
  │
  ▼
3. Train–test split
  │
  ▼
4. Baseline model train karo
   ├─ Logistic Regression
   └─ Ya Random Forest
  │
  ▼
5. Metrics check karo
   ├─ Accuracy
   ├─ Precision
   ├─ Recall
   └─ F1-score
  │
  ▼
6. Class imbalance check karo
   ├─ Kya ek class bahut zyada hai?
   │
   ├─ YES → class_weight="balanced"
   │        ya resampling
   │
   └─ NO → normal training
  │
  ▼
7. Target metric decide karo
   ├─ Fraud/Churn/Medical?
   │      → Recall important
   │
   ├─ Spam detection?
   │      → Precision important
   │
   └─ Balanced case?
          → F1-score use karo
  │
  ▼
8. Feature importance nikaalo
   ├─ Mutual Information
   ├─ Random Forest importance
   └─ Permutation importance
  │
  ▼
9. Top features select karo
   ├─ Common features (2+ methods me)
   └─ Usually 8–12 features
  │
  ▼
10. Final model train karo
    ├─ Logistic Regression
    ├─ Random Forest
    └─ Ya XGBoost
  │
  ▼
11. Threshold tuning (optional)
    ├─ Precision–recall balance
    └─ Best F1 ya business metric
  │
  ▼
12. Final evaluation
    ├─ Classification report
    ├─ Confusion matrix
    └─ Final conclusion
  │
  ▼
END → Final model ready
