# ✅ Statistical Test Decision Guide


| Variable A                  | Variable B         | Test / Method                           | Purpose                                                                        |
| --------------------------- | ------------------ | --------------------------------------- | ------------------------------------------------------------------------------ |
| **Categorical**             | **Categorical**    | ✅ **Chi-Square Test of Independence**   | Test association between two categories (e.g., Gender vs Card Type)            |
| **Categorical**             | **Numerical**      | ✅ **t-test / ANOVA**                    | Compare means across categories (e.g., Amount by Gender or Card Type)          |
| **Numerical**               | **Numerical**      | ✅ **Correlation (Pearson/Spearman)**    | Assess strength/direction of relationship (e.g., Age vs Spending)              |
| **Numerical**               | Time (Date)        | ✅ **Trend Analysis / Time Series**      | See if a metric changes over time (e.g., Monthly Spend)                        |
| **Categorical (2 groups)**  | Numerical          | ✅ **Independent t-test**                | Compare means between 2 groups (e.g., Male vs Female spending)                 |
| **Categorical (>2 groups)** | Numerical          | ✅ **One-Way ANOVA**                     | Compare means across 3+ groups (e.g., Spending by Card Type)                   |
| **Categorical**             | Proportion         | ✅ **Z-test for Proportions**            | Compare category proportions (e.g., % of users preferring Gold Card by Gender) |
| **Numerical**               | Distribution check | ✅ **Shapiro-Wilk / Kolmogorov-Smirnov** | Test for normality of data distribution                                        |
| **2 Variances**             |                    | ✅ **Levene’s Test / Bartlett’s Test**   | Compare variances (e.g., Urban vs Rural Spending Variability)                  |
| **Groups (non-normal)**     | Numerical          | ✅ **Kruskal-Wallis / Mann-Whitney U**   | Non-parametric tests to compare groups                                         |


--- 
# 🧪 Test Selection Quick Summary

| Test                       | When to Use                                              |
| -------------------------- | -------------------------------------------------------- |
| **Chi-Square Test**        | Categorical vs Categorical                               |
| **t-test**                 | Compare 2 group means (numerical by 2-category variable) |
| **ANOVA**                  | Compare 3+ group means                                   |
| **Kruskal-Wallis**         | Non-parametric ANOVA (for 3+ groups, non-normal)         |
| **Mann-Whitney U**         | Non-parametric t-test (for 2 groups, non-normal)         |
| **Levene’s Test**          | Compare variances between groups                         |
| **Shapiro-Wilk**           | Test for normality of a distribution                     |
| **Pearson Correlation**    | Linear relationship between 2 numeric variables          |
| **Spearman Correlation**   | Monotonic relationship (non-parametric)                  |
| **Z-test for proportions** | Compare proportions between groups                       |


---  
# 🛠️ Bonus: Mapping from Your Credit Card Project   

| Question Example                                       | Variable Types                      | Recommended Test                  |
| ------------------------------------------------------ | ----------------------------------- | --------------------------------- |
| Does gender influence card type or expense type?       | Categorical vs Categorical          | ✅ Chi-Square                      |
| Do urban and rural cities differ in spending variance? | Categorical vs Numerical (variance) | ✅ Levene's Test                   |
| Is spending different between genders?                 | Categorical (2) vs Numerical        | ✅ t-test                          |
| Does spending vary by expense type?                    | Categorical (>2) vs Numerical       | ✅ ANOVA                           |
| Does spending vary by card type (data not normal)?     | Categorical vs Numerical            | ✅ Kruskal-Wallis (non-parametric) |
| Is the spending distribution normal?                   | Numerical only                      | ✅ Shapiro-Wilk                    |
| Does gender affect average monthly spending trend?     | Categorical vs Time Series          | ✅ Grouped Trend Analysis          |
| Is there correlation between Age and Spending?         | Numerical vs Numerical              | ✅ Pearson or Spearman             |


--- 

# 📊 Statistical Test Cheat Sheet for Credit Card Spending Project 

| **Question / Business Case**                                                  | **Variable A**         | **Variable B** | **Variable Types**            | **Test / Method**                       |
| ----------------------------------------------------------------------------- | ---------------------- | -------------- | ----------------------------- | --------------------------------------- |
| 1. Does **gender influence card type**?                                       | Gender                 | Card Type      | Categorical vs Categorical    | ✅ **Chi-Square Test of Independence**   |
| 2. Does **gender influence expense type**?                                    | Gender                 | Exp Type       | Categorical vs Categorical    | ✅ **Chi-Square Test of Independence**   |
| 3. Is **spending different between genders**?                                 | Gender                 | Amount         | Categorical (2) vs Numerical  | ✅ **Independent t-test**                |
| 4. Is **spending different across card types**?                               | Card Type              | Amount         | Categorical (>2) vs Numerical | ✅ **ANOVA** (or Kruskal-Wallis)         |
| 5. Is **spending different across expense types**?                            | Exp Type               | Amount         | Categorical (>2) vs Numerical | ✅ **ANOVA** (or Kruskal-Wallis)         |
| 6. Does **spending vary significantly between cities**?                       | City                   | Amount         | Categorical (>2) vs Numerical | ✅ **ANOVA** or **Kruskal-Wallis**       |
| 7. Is there a **greater variation in spending in urban vs rural cities**?     | City\_Type             | Amount         | Categorical (2) vs Variance   | ✅ **Levene’s Test**                     |
| 8. Is **spending normally distributed** overall or by category?               | Amount                 | –              | Numerical only                | ✅ **Shapiro-Wilk Test**                 |
| 9. Does **daily/weekly/monthly spending** follow a **trend over time**?       | Date                   | Amount         | Time vs Numerical             | ✅ **Time Series Plot / Trend Analysis** |
| 10. Is there a **relationship between Age and Spending**? *(if you have Age)* | Age                    | Amount         | Numerical vs Numerical        | ✅ **Pearson / Spearman Correlation**    |
| 11. Do **different card types show different usage by gender**?               | Gender                 | Card Type      | Categorical vs Categorical    | ✅ **Chi-Square Test**                   |
| 12. Is the **average spending in Delhi** above ₹X with 95% confidence?        | City = 'Delhi'         | Amount         | One group vs value            | ✅ **t-test / Confidence Interval**      |
| 13. Does **mean spending differ across weekdays vs weekends**?                | Day Type (Weekday/End) | Amount         | Categorical (2) vs Numerical  | ✅ **t-test**                            |

---
 
