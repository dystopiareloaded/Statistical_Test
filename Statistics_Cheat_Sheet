# 📊 Statistical Test Cheat Sheet for Credit Card Spending Analysis

| 💡 Question / Business Case                                                        | 🅰️ Variable A         | 🅱️ Variable B           | 🔢 Variable Types              | ✅ Recommended Test                      |
|------------------------------------------------------------------------------------|------------------------|--------------------------|--------------------------------|------------------------------------------|
| 1. Does gender influence card type?                                                | Gender                 | Card Type                | Categorical vs Categorical     | Chi-Square Test of Independence          |
| 2. Does gender influence expense type?                                             | Gender                 | Exp Type                 | Categorical vs Categorical     | Chi-Square Test of Independence          |
| 3. Is spending different between genders?                                          | Gender                 | Amount                   | Categorical (2) vs Numerical   | Independent t-test                       |
| 4. Is spending different across card types?                                        | Card Type              | Amount                   | Categorical (>2) vs Numerical  | ANOVA / Kruskal-Wallis                   |
| 5. Is spending different across expense types?                                     | Exp Type               | Amount                   | Categorical (>2) vs Numerical  | ANOVA / Kruskal-Wallis                   |
| 6. Does spending vary significantly between cities?                                | City                   | Amount                   | Categorical (>2) vs Numerical  | ANOVA / Kruskal-Wallis                   |
| 7. Is there greater variation in spending in urban vs rural cities?               | City_Type              | Amount                   | Categorical (2) vs Variance    | Levene’s Test                            |
| 8. Is spending normally distributed overall or by category?                        | Amount                 | —                        | Numerical only                 | Shapiro-Wilk Test                        |
| 9. Does daily/weekly/monthly spending follow a trend over time?                    | Date                   | Amount                   | Time vs Numerical              | Time Series / Trend Analysis             |
| 10. Is there a relationship between Age and Spending? *(if Age exists)*            | Age                    | Amount                   | Numerical vs Numerical         | Pearson / Spearman Correlation           |
| 11. Do different card types show different usage by gender?                        | Gender                 | Card Type                | Categorical vs Categorical     | Chi-Square Test                          |
| 12. Is the average spending in Delhi above ₹X with 95% confidence?                 | City = 'Delhi'         | Amount                   | One group vs Value             | Confidence Interval / 1-sample t-test    |
| 13. Does mean spending differ across weekdays vs weekends?                         | Day Type               | Amount                   | Categorical (2) vs Numerical   | Independent t-test                       |
