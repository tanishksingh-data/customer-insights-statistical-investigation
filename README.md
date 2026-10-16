# 📊 Customer Insights: A Statistical Investigation

An end-to-end statistics and Exploratory Data Analysis (EDA) project analyzing consumer behavior, spending patterns, and demographic distributions across retail customer segments[cite: 1, 2].

---

## 📌 Project Overview
A retail company wanted to understand what story their customer data tells[cite: 1]. Using a synthetic dataset of 10,675 transaction records across approximately 1,000 unique customers[cite: 2], this project validates key business assumptions and uncovers spending drivers using descriptive and inferential statistics[cite: 1].

---

## 🛠️ Tools & Technologies
* **Language:** Python[cite: 4]
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, SciPy
* **Environment:** Jupyter Notebook

---

## 📁 Dataset Summary
* **Records:** 10,675 rows, 12 columns, 0 missing values[cite: 2, 8]
* **Key Features:** `Age`, `Gender`, `State`, `Education`, `Married`, `NumPets`, `MonthlySpend`, `DaysSinceLastInteraction`, `JoinDate`, `TransactionDate`[cite: 3, 4, 8]

---

## ⚙️ Steps Completed

1. **Data Cleaning & Auditing**
   * Standardized date formats (`JoinDate`, `TransactionDate`) into datetime objects.
   * Verified data types and confirmed zero missing or duplicate values[cite: 8].

2. **Descriptive Statistics**
   * Calculated central tendency and dispersion metrics for continuous variables (Mean Spend: **$331.61**, Median: **$282.11**).
   * Summarized demographic distributions across education levels, gender identity, and states[cite: 3, 8].

3. **Data Visualization (EDA)**
   * Plotted distributions (histograms and KDE) for `Age` and `MonthlySpend`.
   * Analyzed spending across education levels and geographic states with boxplots and bar charts.
   * Evaluated feature correlations with a heatmap.

4. **Hypothesis Testing ($\alpha = 0.05$)**
   * **One-Way ANOVA (`MonthlySpend` vs. `Education`):**
     * Result: $F = 0.2288$, $p = 0.9224$
     * Conclusion: **Fail to Reject $H_0$**. Customer education level does not have a statistically significant effect on monthly spending.
   * **Chi-Square Test (`State` vs. `Education`):**
     * Result: $\chi^2 = 433.05$, $p = 1.42 \times 10^{-69}$
     * Conclusion: **Reject $H_0$**. There is a statistically significant relationship between geographic location and educational demographics.

---

## 💡 Key Business Takeaways
* **Universal Premium Offerings:** Spending power is consistent across education tiers—high-value products should not be limited to advanced degree holders.
* **Geographically Targeted Messaging:** Because education demographics vary significantly by state, marketing campaigns should be customized to regional profiles.
* **Customer Win-Back:** The median time since last interaction is **445 days**, highlighting an opportunity for an automated re-engagement campaign for users inactive for over 12 months.

---
