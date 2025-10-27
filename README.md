# 📊 Customer Churn Analysis — Telecom Industry

## 🧠 Objective
The goal of this project is to **predict customer churn** and derive **data-driven retention strategies** for a telecom company operating in a competitive market.  
By analyzing customer usage behavior (calls, recharges, complaints, etc.), the model identifies which customers are likely to churn and provides actionable insights to **reduce churn and improve customer lifetime value (CLV).**

---

## 🧰 Tools & Technologies
- **Python**: Data analysis & modeling  
- **Scikit-learn**: Machine learning algorithms  
- **Pandas / NumPy**: Data cleaning & transformation  
- **Matplotlib / Seaborn**: Visualizations  
- **ELI5 / SHAP**: Model explainability  
- **SQL (optional)**: For data aggregation & feature extraction  
- **PowerPoint**: For final executive summary presentation  

---

## 🧩 Project Workflow

### 1. Data Preparation
- Cleaned and normalized data using Pandas.  
- Mapped categorical churn labels (`Yes/No`, `1/0`, `Churned/Active`) into a binary target variable.  
- Aggregated behavioral data such as:
  - **Total call duration**
  - **Recharge frequency**
  - **Complaint counts**

### 2. Feature Engineering
- Created additional KPIs:
  - `total_call_duration`
  - `recharge_count_agg`
  - `complaints_last_90d`
- Handled missing data with median/mode imputation.
- Standardized numerical features and encoded categorical ones.

### 3. Model Building
- Split dataset into **train/test (75/25)**.
- Trained two binary classifiers:
  - **Logistic Regression** (baseline model)
  - **Random Forest Classifier** (non-linear performance)
- Evaluated with:
  - Accuracy, Precision, Recall, F1-score, ROC-AUC
  - Confusion matrix visualizations
- Model explainability using **Permutation Importance** and **SHAP values**.

### 4. Customer Segmentation
Created three actionable customer segments based on churn probability and engagement metrics:
| Segment | Description | Action |
|----------|--------------|--------|
| **Loyal** | Low churn probability, high activity | Upsell & reward |
| **At Risk** | High churn probability, active | Retain with personalized offers |
| **Dormant** | Low activity, disengaged | Win-back campaigns |

---

## 📈 Results Summary
- **Churn Prediction Accuracy:** ~85% (Random Forest)  
- **Top Predictors:** Recharge frequency, total call duration, complaints count  
- **Key Insight:** Customers with fewer recharges and lower call activity are 3× more likely to churn.  
- **Business Impact:** Potential churn reduction of **15–25%** through targeted retention actions.

---

## 🧾 Deliverables
| File | Description |
|------|--------------|
| `churn_cleaned.csv` | Cleaned and processed dataset |
| `segments.csv` | Customer segments with churn probabilities |
| `churn_ml_notebook.ipynb` | End-to-end ML notebook |
| `customer_churn_report_corporate.pptx` | Executive PowerPoint report |
| `Customer_Churn_Strategy_Final_Recommendations.pdf` | 1-page strategy summary |

---

## 🚀 Key Recommendations
1. **Target “At Risk” Customers** with personalized retention offers and proactive outreach.  
2. **Reward “Loyal” Users** with loyalty programs and premium upsell options.  
3. **Re-engage “Dormant” Users** via low-cost reactivation offers (SMS/app campaigns).  
4. **Enhance Complaint Resolution** to reduce churn drivers.  
5. **Continuous Monitoring** with dashboards and predictive churn alerts.

---

## 📊 Expected Business Impact
| Metric | Current | Target (6 Months) | Improvement |
|:--------|:--------:|:----------------:|:------------:|
| Monthly Churn Rate | 12–15% | **<10%** | -25% |
| ARPU | ₹250 | **₹280–₹300** | +10–15% |
| Reactivation Rate | 8% | **20–30%** | +3× |
| Complaint Resolution Time | 72 hrs | **<48 hrs** | +33% |

---

## 🧾 Author
**Project:** Customer Churn Analysis for Telecom Industry  
**Type:** End-to-End Data Science + Business Analytics  
**Category:** Binary Classification | Customer Retention | Predictive Analytics

---

### 🏁 Next Steps
- Deploy churn prediction as a live dashboard using Streamlit or Power BI.  
- Integrate model outputs into CRM for automated retention targeting.  
- Continuously monitor churn KPIs for optimization.
