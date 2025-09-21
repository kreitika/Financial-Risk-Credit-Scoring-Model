# 📊 Financial Risk & Credit Scoring Model

## Overview  
This project demonstrates how data science can support data-driven lending by building a credit scoring model that predicts default risk and visualizes results through an interactive Tableau dashboard.  

## Objective  
- Identify high-risk loan applicants.  
- Simulate policies to reduce non-performing loans (NPLs).  
- Provide interpretable results for business stakeholders.  

## Dataset  
- Source: Kaggle – *Home Credit Default Risk*.  
- Records: ~40,000 loan applications.  
- Target: Default (1) vs Non-default (0).  

## Methodology  
1. **Data Preprocessing**  
   - Imputation of missing values.  
   - Feature engineering (ratios, log transforms).  

2. **Modeling**  
   - Logistic Regression (baseline).  
   - LightGBM (boosted trees).  
   - Probability calibration with isotonic regression.  

3. **Evaluation Metrics**  
   - ROC-AUC, PR-AUC, KS statistic.  
   - Decile lift analysis.  

4. **Explainability**  
   - SHAP feature importance to interpret drivers of default.  

5. **Visualization**  
   - Tableau dashboard with risk segmentation, score distribution, default rate by segment, and calibration check.  

## Results  
- **Logistic Regression**:  
  - ROC-AUC = 0.75  
  - PR-AUC = 0.23  
  - KS = 0.37  
- **Decile Analysis**:  
  - Top 2 deciles (~20% of applicants) captured ~51% of all defaults.  
  - Decile 10 default rate ~26% vs Decile 1 ~1%.  
- **Business Impact**:  
  - Policy simulation shows potential to cut **non-performing loans by ~12%** while retaining healthy approval rates.  

## Deliverables  
- Python notebook (model training & evaluation).  
- Tableau-ready dataset (`for_tableau.csv`).  
- Visuals: ROC/PR curves, SHAP importance, decile lift table.  
- Interactive Tableau dashboard for stakeholder insights.  

---

🔗 **Dashboard Preview**: [Tableau Public link – (https://public.tableau.com/authoring/FinancialRiskCreditScoringModel/Dashboard1#1)]  
### 📌 Author
Project by *Kreitika Yadav*  
