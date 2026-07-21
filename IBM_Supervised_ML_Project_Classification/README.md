# Mental Health in Tech: Predicting Treatment-Seeking Behavior
### Understanding Workplace Factors Influencing Mental Health Support Decisions
**Exploratory Analysis, Statistical Assessment, Machine Learning Classification & Qualitative Insight Extraction**

---

## Project Overview

This project analyzes mental health treatment-seeking behavior among technology professionals using the Mental Health in Tech Survey dataset.

The objective is to understand which workplace, organizational, and personal factors are associated with employees' decisions to seek mental health treatment. The analysis combines exploratory data analysis, predictive modeling, and qualitative analysis of open-ended survey responses to identify key drivers, barriers, and organizational conditions influencing mental health support access.

The central question addressed is:

**Which factors most strongly influence whether technology professionals seek mental health treatment, and what workplace practices can encourage healthier support environments?**

---

## Data Preparation & Analysis Framework

The dataset contains 1,259 survey responses covering demographic characteristics, employment conditions, workplace culture, mental health resources, and treatment history.

Data preparation focused on creating a reliable analytical foundation through:

- Validation of survey structure, target distribution, and variable quality
- Handling of missing values while preserving meaningful information
- Standardization of inconsistent categorical responses, including gender categories
- Removal of implausible age values and creation of meaningful career-stage groups
- Consolidation of rare categories to reduce sparsity
- Transformation of categorical and ordinal variables into modeling-ready features
- Creation of separate datasets for predictive modeling and qualitative comment analysis

The final modeling dataset contained 1,233 observations and 98 numeric features after preprocessing.

---

## Analytical Approach / Modeling Framework

The project combines multiple analytical approaches to capture both predictive performance and interpretability.

### Exploratory & Statistical Analysis

Initial analysis examined:

- Distribution of treatment-seeking behavior
- Relationships between workplace factors and treatment decisions
- Missing data patterns and response behaviors
- Potential multicollinearity among predictors using Variance Inflation Factor (VIF)

Feature redundancy was reduced to improve model stability and interpretability.

### Predictive Modeling

Three supervised classification models were developed and evaluated:

- Regularized Logistic Regression for interpretable relationships between predictors and treatment-seeking probability

<img width="720" height="593" alt="image" src="https://github.com/user-attachments/assets/a234ed91-c54b-40f7-95a7-5157b1be5c58" />

- Decision Tree classification to capture non-linear relationships and identify decision patterns
- Random Forest classification to improve predictive robustness and evaluate feature importance

Models were optimized using cross-validation and evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC

### Qualitative Analysis

Open-ended comments were analyzed to complement quantitative findings through:

- Text cleaning and preprocessing
- Word frequency analysis
- Topic modeling using Latent Dirichlet Allocation (LDA)
- Sentiment analysis
- Generative AI-assisted thematic interpretation

<img width="1212" height="612" alt="image" src="https://github.com/user-attachments/assets/7a56ebf2-3567-44a8-a91f-a9d7bded3e94" />

This approach provided additional context around workplace culture, stigma, benefits, and support experiences.

---

## Key Findings / Results

### Predictive Modeling Performance

| Model | Accuracy | F1-score | ROC-AUC |
|---|---:|---:|---:|
| Logistic Regression | 0.688 | 0.705 | 0.753 |
| Decision Tree | 0.794 | 0.813 | 0.848 |
| Random Forest | 0.777 | 0.789 | 0.867 |

<img width="1057" height="590" alt="image" src="https://github.com/user-attachments/assets/7d2ee8d8-614b-4270-bcfd-2696dfa435e6" />

The Random Forest achieved the strongest discrimination capability, while the Decision Tree provided the highest balance between predictive accuracy and interpretability.

### Main Predictive Factors

Across models, the most influential factors associated with treatment-seeking behavior were:

- Level of work interference caused by mental health conditions
- Family history of mental health challenges
- Availability of mental health benefits
- Access to care options
- Workplace anonymity and psychological safety
- Support from colleagues and supervisors
- Flexible work arrangements

### Qualitative Insights

Analysis of employee comments revealed recurring themes:

- Fear of stigma and professional consequences remains a major barrier
- Supportive workplace cultures encourage openness and treatment access
- Benefits alone are insufficient without trust and confidentiality
- Flexible work arrangements can help employees manage mental health challenges
- Manager awareness and leadership engagement strongly influence employee experiences

---

## Strategic Insights

The analysis demonstrates that treatment-seeking behavior is not driven by a single factor but by the interaction between individual circumstances and workplace environments.

Key insights include:

- Organizations with accessible resources and supportive cultures create conditions where employees are more likely to seek help
- Psychological safety and confidentiality are essential for effective mental health programs
- Workplace policies must go beyond offering benefits by ensuring employees trust and understand available support
- Manager behavior represents a critical factor in reducing stigma and improving access to care

The combination of predictive modeling and qualitative analysis provides a more complete understanding of employee mental health experiences.

---

## Actionable Recommendations

Based on the findings, organizations can improve mental health support by:

- Developing clear and accessible mental health policies
- Improving communication around available resources and confidentiality procedures
- Training managers to recognize concerns and provide appropriate support
- Expanding flexible work options when operationally feasible
- Creating peer-support initiatives and inclusive workplace practices
- Measuring program effectiveness through employee feedback and engagement indicators

A data-driven monitoring approach can help organizations evaluate whether interventions improve access, trust, and employee well-being over time.

---

## Limitations & Future Improvements

Several limitations should be considered:

- The dataset is based on self-reported survey responses and may contain reporting bias
- The sample represents a specific period and population within the technology sector
- Some demographic categories contain limited observations
- Open-ended comments provide valuable context but represent a small subset of respondents

Future improvements could include:

- Incorporating larger and more recent workforce datasets
- Applying advanced natural language processing approaches
- Developing longitudinal analysis to measure changes over time
- Building predictive dashboards for organizational monitoring

---

## Project Structure

- **Notebook 1:** Exploratory data analysis, dataset overview, and initial behavioral insights
- **Notebook 2:** Data cleaning, feature engineering, and preparation of modeling datasets
- **Notebook 3:** Classification modeling, model comparison, and feature importance analysis
- **Notebook 4:** Text analysis of employee comments, topic modeling, sentiment analysis, and qualitative insights
- **Notebook 5:** Integrated synthesis, strategic interpretation, and recommendations

---

## Key Takeaways

- Workplace conditions strongly influence mental health treatment-seeking behavior
- Organizational support, benefits, and psychological safety are key drivers of help-seeking
- Machine learning models identified important predictive factors while maintaining interpretability
- Qualitative analysis revealed persistent barriers related to stigma and disclosure concerns
- Combining quantitative and qualitative methods provides deeper insight into employee experiences

---

## Conclusion

This project demonstrates how data analytics and machine learning can be used to better understand workplace mental health dynamics.

By combining predictive modeling with qualitative interpretation, the analysis provides evidence-based insights into the factors influencing treatment-seeking behavior and highlights how organizations can create more supportive, inclusive, and effective mental health environments.
