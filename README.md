# 📊 Telecom Customer Churn Analysis & Prediction

## 🧭 1. Project Overview
Customer retention is a critical challenge for telecom companies.  
This project analyzes customer behavior to identify churn risks and optimize retention strategies using data.

The dataset contains **2,666 customers** with behavioral, transactional, and demographic features.

---

## 📦 2. Dataset Summary

| Metric | Value |
|------|------|
| Number of Observations | 2,666 |
| Number of Variables | 20 |
| Missing Values | 0 |
| Duplicate Rows | 0 |
| Dataset Size | 797.8 KiB |

### Variable Types:
- Numerical: 15  
- Categorical: 1  
- Text: 1  
- Boolean: 3  

⚠️ *State and Area code are descriptive and require encoding for modeling.*

---

## 🎯 3. Target Variable (Churn)

| Class | Description | Count | Percentage |
|------|------------|------|-----------|
| ❌ False | Non-Churn | 2,278 | 85.4% |
| ✅ True | Churn | 388 | 14.6% |

⚠️ Imbalanced dataset → techniques like **SMOTE / oversampling** recommended.

---

## 📊 4. Key Feature Insights

### ☎️ Customer Service Calls
- Mean: 1.56  
- Max: 9  
- Correlation: **0.32**  

💡 Frequent support calls = strong churn signal

---

### 🌍 International Plan
- True: 10.1%  
- Correlation: **0.275**  

💡 Slightly increases churn risk

---

### 📩 Voice Mail Plan
- Correlation: **0.108**  

💡 Limited direct impact

---

### 📈 Usage Metrics
- Day usage: **Strong correlation (~0.34)**  
- Night / Intl: weak correlation  

💡 High usage = higher churn probability

---

### 📥 Voicemail Messages
- 72.5% = zero usage  

💡 Highly skewed distribution

---

## 🔗 5. Main Drivers of Churn

- 📞 Customer service calls  
- ⏰ Total day usage  
- 🌍 International plan  
- 📊 Behavioral usage patterns  

---

## 🧠 6. Business Insights

- Customers contacting support frequently are at high risk  
- High-usage customers are more sensitive to service quality  
- Not all customers have the same value  

---

## 🚀 7. Retention Strategy

| Segment | Condition | Action |
|--------|----------|--------|
| 🔴 High Risk | Calls > 3 & Intl Plan | 🎁 Targeted offers |
| 🟡 Medium Risk | High usage | 📞 Proactive contact |
| 🟢 Low Risk | Low churn probability | ✅ Standard engagement |

---

## ⏳ 8. Churn Over Time

- 0–30 days → Low churn (2–5%)  
- 50–150 days → Increasing churn  
- 100+ days → Peak risk (~25%)  

💡 Key insight:
> Churn increases over time but becomes unreliable for small segments.

---

## 📈 9. Model Performance

- ROC-AUC: **0.9154**  
- PR-AUC: **0.8376**  
- Brier Score: **0.0485**  

### Top Features:
- Total day minutes  
- Customer service calls  
- Total eve minutes  
- International plan  

---

## 💰 10. Business Impact (ROI Analysis)

### ✅ Targeted Strategy
- ROI (Validation): **1.79**  
- ROI (Test): **2.06**  

💡 Investment is focused on high-risk customers → strong profitability

---

### ❌ Non-targeted Strategy (All Customers)
- ROI: **negative (-0.5)**  

💡 Sending offers to everyone destroys value

---

## 📊 Key Takeaways

✔️ Not all customers are equal  
✔️ Churn is predictable  
✔️ Smart targeting increases ROI  
✔️ Data-driven decisions outperform intuition  

---

## 🏁 Conclusion

The dataset is clean and reliable, allowing robust analysis.

**Main churn drivers:**
- Customer support interactions  
- Usage behavior  
- Subscription features  

💡 The real value comes from:
> Combining predictive modeling + business strategy

---

## 🎥 (Optional) Demo

Add your Canva / video explanation here: