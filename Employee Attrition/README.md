# Employee Attrition Prediciton & Behavioral Analysis  
### Classification Modeling Project  
**Advanced Modeling & Strategic Stabilization of Workforce**

---

The goal of this project is to predict employee attrition using a comprehensive dataset of **30+ explanatory variables** spanning multiple organizational dimensions, including:

- Demographic characteristics & Marital status
- Structural organizational data** (Department, Job Role, Job Level)
- Compensation patterns & Performance–Reward alignment
- Psychometric engagement & Satisfaction indicators
- Career trajectories & Behavioral archetypes

By integrating these heterogeneous signals, the model captures both **Direct Drivers** (structural factors) and **Systemic Triggers** (complex interactions), moving beyond observation toward **actionable organizational intelligence**.

---

### Data Architecture & Feature Engineering

**Dimensionality Management & Stability**
- Addressed scale imbalance and right-skewness in key variables (e.g., *Monthly Income*, *Tenure*) using **logarithmic transformations** and **Robust Scaling**.
- Ensured numerical stability for distance-based models and improved convergence for the **LightGBM champion**.

**Feature Intelligence – Career Dynamics**
Engineered composite ratios to move beyond static time-based metrics:

  - **Manager Stability**  
    Stability of the reporting line relative to company tenure.
  - **Stagnation Index**  
    Proportional time elapsed since the last promotion.
  - **Career Stability**  
    Historical “Job Hopping” frequency relative to total working years.

**The *Archetype* Variable**
- Leveraged **unsupervised clustering** to define latent profiles (e.g., *Workhorse Elite*, *Quiet Disengaged*).
- Isolated **burnout risk** and **engagement intensity** as primary predictors of vulnerability.

<img width="1062" height="323" alt="image" src="https://github.com/user-attachments/assets/f7792113-06df-4e5f-ac1e-684c9d8d99d0" />

---

### Sensitivity Analysis & Dual-Engine Modeling

**Architecture-Specific Dynamics**
Identified a fundamental divergence in predictive logic between model types:

**Direct Drivers — Logistic Regression**
  - Optimized via **L2 Regularization** ($R^2 \approx 0.81$).
  - Identified:
    - **Foundational anchors**: Age, Manager Stability  
    - **Risk accelerators**: Single status, Business Travel

<img width="1047" height="619" alt="image" src="https://github.com/user-attachments/assets/b47d00ab-4c88-4585-8c39-ea906db24c24" />

**Systemic Triggers — LightGBM**
  - Achieved **Weighted F1 ≈ 0.96**.
  - Captured non-linear *“Circuit Breakers”* where logistical friction (commute) amplifies structural stagnation.

---

### Actionable Insights & Systemic Audit

**Performance–Reward Disconnect**
  Identified a critical **Systemic Weakness**:
  - Performance ratings show **no correlation** with Salary Hikes or Job Involvement.
  - Leads to perceived unfairness and frustration among highly engaged talent.

**SHAP Global Impact Highlights**
- **Age (Top SHAP)**: Younger employees are consistently the most at risk.
- **Career Stability**: Low career inertia acts as a foundational constraint on retention.
- **Managerial Anchor**: Weak managerial relationships catalyze departure, especially for *Balanced Contributors*.

<img width="1045" height="649" alt="image" src="https://github.com/user-attachments/assets/8ce05e38-0526-4ec6-8ee0-af5bcbb0d5f8" />

---

### Strategic Intervention Roadmap

A tiered decision framework synchronized with organizational urgency:

| Horizon        | Monitoring Focus        | Initiative                          | Target Objective |
|---------------|--------------------------|-------------------------------------|------------------|
| Immediate     | HR Dept Stabilization    | Rescue Plan & Watch Committee       | Stop the “Seniority Drain” in HR |
| Short Term    | Circuit Breakers         | Logistical Shield & Time Sanctuary  | Protect Workhorse Elites |
| Short–Medium  | Operational Dashboards   | Predictive Monitoring               | Real-time risk tracking |
| Long Term     | Root Cause Engineering   | Performance & Bonus Overhaul        | Restore trust & fairness |

---

### Project Structure

- **Notebook 1 – Ingestion & Cleaning**  
  Logical imputation and MCAR statistical validation.
- **Notebook 2 – Behavioral Clustering**  
  K-Means segmentation and Archetype definition.
- **Notebook 3 – Global EDA**  
  Discovery of the HR *“Seniority Drain”* and Performance–Reward disconnect.
- **Notebook 4 – Feature Engineering & Modeling**  
  Ratio generation and multi-model benchmarking (*LightGBM Champion*).
- **Notebook 5 – Strategy & Recommendations**  
  Translating SHAP values into a tiered *Rescue Plan* and long-term resilient framework.

---

## Key Takeaways

**The Workhorse Elite Burnout Signal**
High performance is a double-edged sword. *Workhorse Elites* leave at the highest rates (~30%), suggesting attrition driven by **workload pressure**, not disengagement.

**HR as a Single Point of Failure**
The HR department faces a unique crisis: senior and experienced staff are exiting. Without a stable HR team, turnover reduction efforts are **mathematically likely to fail**.

**Model Parsimony & Operational Scalability**
With **Weighted F1 = 0.96** and **Label Stability (ARI ≈ 0.86)**, engineered behavioral features match or outperform full 30+ variable models while remaining interpretable for leadership.

---

### Limitations & Ethical Considerations

- **Self-Fulfilling Prophecy**: High-risk profiling must enable support—not restriction.
- **“Ghost” Variables**: Missing data on management quality and team culture.
- **Static Snapshot**: Requires regular recalibration to adapt to economic cycles.

---

### Conclusion

This project demonstrates how **HR Data Science** can move beyond reporting to become a **strategic risk management tool**, enabling earlier, fairer, and more effective interventions to protect the organization’s most valuable asset: **its talent**.
