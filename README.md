# 📊 Statistical Analysis & Business Decisions Project (A/B Testing & Data-Driven Decisions)

This project applies a **Data-Driven Decision Making** methodology to conduct statistical tests (A/B testing, parametric, and non-parametric tests), verify underlying assumptions, and translate statistical findings into actionable business decisions.

---

## 📌 Project Structure & Checkpoints

| Checkpoint | Topic | Key Content & Explanation |
| :--- | :--- | :--- |
| **Checkpoint 4** | **p-value & Confidence Intervals** | Proper interpretation of the $p$-value beyond a naive "$p < 0.05$" threshold; evaluating 95% Confidence Intervals (CI) in terms of precision and Effect Size. |
| **Checkpoint 5** | **Parametric Test Assumptions** | Verifying core assumptions prior to testing: Normality (*Shapiro-Wilk*) and Homogeneity of Variance (*Levene’s test*). |
| **Checkpoint 6** | **Business-Driven Results** | Translating statistical outputs into business metrics and delivering a strategic recommendation regarding product rollout. |

---

## 🔬 Statistical Methodology

### 1. Assumptions Checking
Before applying parametric tests (e.g., *t-test*, *ANOVA*), data are evaluated against the following criteria:
* **Normality Assumption:** Compliance with a normal distribution is evaluated using the *Shapiro-Wilk* or *Kolmogorov-Smirnov* test ($p > 0.05$) alongside *Q-Q Plots*.
* **Homogeneity of Variance (Homoscedasticity):** Equality of variance across groups is assessed using *Levene’s Test* ($p > 0.05$).
> **Note:** If assumptions are violated, non-parametric alternatives (*Mann-Whitney U*, *Kruskal-Wallis*) or data transformations are utilized.

### 2. Correct Interpretation of $p$-value & Confidence Intervals
* **$p$-value ($p$):** Represents the probability of observing the data (or more extreme results) assuming the null hypothesis ($H_0$) is true. While $p < 0.05$ provides evidence to reject $H_0$, it does not measure the magnitude of the effect.
* **Confidence Interval (CI):** A 95% CI provides an estimated range for the true population parameter and quantifies the uncertainty/precision of the estimate. An interval that excludes zero indicates a statistically significant difference.

---

## 💼 Business Interpretation & Decision

1. **Rollout Recommendation:** The A/B test confirms that Variant B performs statistically significantly better than the control. Full deployment to 100% of the user base is recommended.
2. **Risk Management:** Because the lower bound of the 95% Confidence Interval remains strictly positive, the financial and operational risk of this rollout is minimal.
3. **Financial Impact:** The implementation is projected to drive measurable uplifts in core business KPIs (e.g., Conversion Rate, ARPU).

---

## 🛠️ Requirements & Dependencies

To execute the notebook and reproduce the analysis, install the required Python packages:

```bash
pip install numpy pandas scipy statsmodels matplotlib seaborn
```

---

## 🚀 How to Run the Project

```bash
# Clone the repository
git clone https://github.com/username/repository-name.git

# Navigate to the project directory
cd repository-name

# Launch Jupyter Notebook
jupyter notebook
