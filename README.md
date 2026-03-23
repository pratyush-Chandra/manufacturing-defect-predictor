# manufacturing-defect-predictor
**90% production runs non-optimal → Urgent optimization opportunity identified**

## 🎯 Business Problem
Analyzed 10K shop-floor sensor records to predict manufacturing defects, optimize OEE, and reduce waste—directly aligning with industrial process improvement mission.

## 🔍 Key Findings
Vibration >0.06mm/s = 40% higher defects (SQL: 0.067 vs 0.047mm/s good runs)

Energy consumption strongest corr with defects (0.28)

ML Model: 91% accuracy, 100% defect recall (vibration coeff 1.13 dominates)

OEE calculated at ~8% → 15-20% improvement potential


## 🛠️ Technical Execution
 Data Ingestion → Pandas (10K rows: temp, RPM, vib, energy, quality)
 EDA → Correlation heatmap, z-score anomalies, scatter plots
 SQL Analytics → GROUP BY defect/vibration thresholds
 ML Pipeline → Logistic Regression, feature scaling, confusion matrix
 Executive Dashboards → Plotly interactive viz + OEE KPIs

 
## 💡 Business Recommendations (Client Deliverable)
1. **Immediate**: Auto-alerts when vibration >0.06mm/s
2. **Short-term**: Energy audit for high-consumption machines  
3. **Long-term**: Deploy ML model to shop-floor for real-time defect prediction

## 📊 Results Visualized
![Heatmap: Energy/Defect Corr 0.28](heatmap.png)
![Feature Importance: Vibration Rules](coeff_importance.html)
![100% Defect Detection](confusion_matrix.png)

## Tech Stack
**Python** | **Pandas** | **SQLite** | **Scikit-learn** | **Plotly** | **Seaborn**

---

