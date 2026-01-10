# Student Academic Performance & Resilience 
### Predictive Risk Management  
**Advanced Modeling & Sensitivity Analysis of Secondary Education Performance**

---

The goal of this project is to **predict the student’s final grade** using a dataset composed of **33 explanatory variables** spanning multiple dimensions, including:

- Demographic characteristics  
- Socio-economic background  
- Family environment  
- Health and lifestyle factors  
- Academic history and behavioral indicators  

By integrating these heterogeneous signals, the model aims to capture both **structural determinants** and **dynamic risk factors** influencing academic performance.

---

### Data Architecture & Feature Engineering

- **Dimensionality Management**  
  Addressed scale imbalance and extreme skewness in key variables (e.g. absences) using logarithmic transformations, improving numerical stability and model interpretability. Latent student profiles were encoded to structure high-dimensional information.

- **Feature Intelligence**  
  Engineered composite indices (e.g. *Parental Education Index*, *Alcohol Index*) to capture complex environmental interactions.

- **The “Momentum” Variable**  
  Developed a progression index between grading periods (`G1 → G2`) to isolate **academic velocity** rather than static performance.

---

### Sensitivity Analysis & Dual-Engine Modeling

- **Subject-Specific Dynamics**  
  Identified a fundamental divergence in academic logic between disciplines:

  - **Portuguese (Linear / Humanities-Oriented)**  
    Optimized using **Ridge / Lasso Regularization**  
    → `R² ≈ 0.86`

  - **Mathematics (Cumulative / STEM-Oriented)**  
    Optimized using **Random Forest & XGBoost**  
    → `R² ≈ 0.85`, capturing non-linear *snowball effects*

- **The Minimalist Nucleus**  
  Statistically demonstrated that a **5-variable core model** retains **98% of total predictive power**, maximizing operational sustainability for school staff.

  <img width="1029" height="444" alt="image" src="https://github.com/user-attachments/assets/e8a053b2-f8a9-4af3-bf3e-00c03795ea31" />

  <img width="1041" height="435" alt="image" src="https://github.com/user-attachments/assets/96bf51bb-ff18-4c75-bf9b-dc75ed73b353" />

---

### Actionable Insights & Residual Audit

- **Bias & Residual Analysis**  
  Identified *“Fragile Passers”*: students with passing grades but high-friction traits  
  (absenteeism, low ambition) who are statistically likely to collapse later in the year.

- **Dropout Profiling**  
  Isolated *“Zero-Grade”* cases to distinguish between:
  - Pure academic failure  
  - Socio-logistical disengagement (absence, detachment, external constraints)

---

## Strategic Intervention Timeline

The project provides a **decision roadmap** synchronized with the academic calendar:

| Phase              | Monitoring Focus                 | Predictive Power | Administrative Action                          |
|--------------------|----------------------------------|------------------|------------------------------------------------|
| Baseline (Sept)    | Academic Debt (Past Failures)    | R² ≈ 0.25        | Targeted preventive tutoring                   |
| Pivot (Nov)        | G1 Momentum & Friction           | R² ≈ 0.70        | “Fragile Passer” prevention interviews         |
| Emergency (March)  | G2 Terminal Trajectory           | R² ≈ 0.85        | Intensive individualized rescue plans          |

---

## Project Structure

- **Notebook 1 – EDA & Signals**  
  Correlation discovery and data cleaning.

- **Notebook 2 – Engineering & FAMD**  
  Variable architecture, feature construction, and dimensionality reduction.

- **Notebook 3 – Predictive Modeling**  
  Algorithm benchmarking, cross-validation, and sensitivity analysis.

- **Notebook 4 – Strategy & Insights**  
  Translating statistical results into operational academic interventions.

---

## Key Takeaways

**The “Silent Anchor” Effect — Attendance**
In Mathematics, absenteeism is not merely a grading penalty but a **structural constraint**. The data reveals a **non-linear content ceiling**: once a critical absence threshold is crossed, the probability of academic recovery collapses exponentially, largely independent of initial `G1` performance.

**Ambition as a Resilience Buffer**
Educational aspiration emerges as the **primary psychological stabilizer**. Students aiming for higher education exhibit significantly higher recovery rates after mid-year setbacks compared to peers with comparable grades but lower motivational outlooks.

**Model Parsimony & Operational Scalability**
A **98% efficiency ratio** was achieved, demonstrating that a **5-variable core model** (Failures, Absences, `G1/G2` Momentum, and Ambition) consistently matches or outperforms full 30+ variable models. This parsimony ensures **interpretability, robustness, and deployability** for non-technical school staff.

---

## Limitations & Ethical Considerations

- Models are trained on historical data and may inherit structural or socio-economic biases.
- Predictive outputs are designed to **support**, not replace, human educational judgment.
- No automated decisions should be taken without contextual validation by educators.

---

## Conclusion

This project demonstrates how **educational data science** can move beyond grade prediction to become a **strategic risk management tool**, enabling earlier, fairer, and more effective academic interventions.

