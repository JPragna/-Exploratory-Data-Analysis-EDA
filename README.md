# Module 2: Exploratory Data Analysis (EDA)

## 📌 Overview

This module focuses on exploring the cleaned HR dataset to identify meaningful insights, trends, anomalies, and relationships that influence employee attrition and wellness. The goal is to assist HR professionals in proactively addressing employee turnover and boosting retention and engagement through data-driven decision-making.

---

## 🎯 Key Objectives

- Understand overall data trends and variable distributions
- Visualize key patterns and detect potential outliers
- Investigate correlations between attrition and other features
- Test hypotheses to validate key assumptions (e.g., “Does overtime increase attrition?”)
- Identify any unusual patterns or biases (e.g., department or gender-based attrition)

---

## 🛠️ Tools & Technologies Used

- Python (Pandas, NumPy, Matplotlib, Seaborn, SciPy)
- Google Colab
- CSV Dataset (M2_UPDATED.csv)
- PNG/PDF exports of key graphs

---

## 📊 Key Visualizations & Insights

1. **Attrition by Overtime**  
   - Employees who worked overtime had significantly higher attrition.
   - **Pearson Correlation:** 0.246  
   - **Chi-Square Test:** Stat = 87.56, p < 0.00001 ✅ Significant

2. **Attrition by Tenure Bucket**  
   - Higher attrition observed in the early tenure (0–2 years).
   - Longer tenure (10+ years) shows lower attrition.

3. **Attrition by Age Group**  
   - Young employees (under 30) had higher attrition rates.
   - Attrition declines with age.

4. **Attrition by Department**  
   - The Sales department showed a noticeably higher attrition rate compared to R&D.

5. **Attrition by Income Level**  
   - Low-income groups showed significantly higher attrition compared to medium or high earners.

6. **Attrition by Job Satisfaction & Involvement**  
   - Employees with low job satisfaction and involvement scores were more likely to leave.
   - **T-Test (Job Satisfaction):** Stat = -3.98, p < 0.0001 ✅ Significant  
   - **Chi-Square (Job Involvement):** Stat = 28.49, p < 0.0001 ✅ Significant

7. **Attrition by Gender & Marital Status**  
   - Gender was not statistically significant.
   - Marital status showed some variations, with single employees having slightly higher attrition.

---

## 📐 Correlation & Hypothesis Testing

| Test | Feature | Result |
|------|---------|--------|
| Pearson Correlation | OverTime_Yes vs Attrition | r = 0.246 ✅ |
| Spearman Correlation | OverTime_Yes vs Attrition | ρ = 0.246 ✅ |
| Chi-Square Test | OverTime_Yes vs Attrition | p < 0.00001 ✅ Significant |
| Chi-Square Test | Job Involvement vs Attrition | p < 0.0001 ✅ Significant |
| T-Test | Job Satisfaction vs Attrition | p < 0.0001 ✅ Significant |
| Chi-Square Test | Performance Rating vs Attrition | p = 0.99 ❌ Not Significant |

---

## 🚩 Unusual Patterns & Biases

- **Overtime Bias:** Strong relationship with attrition — employees who are overworked leave more often.
- **Tenure Spike:** Resignations spike significantly in the first 1–2 years — early disengagement issue.
- **Income Disparity:** Employees in the low-income tier leave more frequently — monetary dissatisfaction.
- **Department Discrepancy:** Sales team attrition is higher — possible due to stress, targets, or travel demands.
- **No Gender Bias Found:** No statistically significant gender-based attrition differences.

---

## 📝 Summary of Insights for HR

- Focus on reducing overtime and monitoring early-tenure employees for signs of disengagement.
- Reassess compensation structure for low-income workers to improve retention.
- Implement department-specific interventions, especially in Sales.
- Promote wellness and satisfaction programs for young employees and those with low involvement scores.

---

## 📂 Deliverables

- ✅ Google Colab Notebook with full code & markdown commentary
- ✅ PNG/PDF versions of 7+ visualizations
- ✅ 2-page HR summary report of insights and actions

---

## 📌 Next Steps (Module 3)

The findings from this module will feed into the predictive modeling stage (Module 3), where we will build classification models to predict attrition and later build wellness recommendation systems based on engagement and satisfaction metrics.

