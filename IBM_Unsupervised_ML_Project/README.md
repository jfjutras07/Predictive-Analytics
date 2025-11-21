# IBM ML Course – Unsupervised Learning Project: Country Development Clustering

This file contains my final project for the Unsupervised Machine Learning module of the **IBM Machine Learning Professional Certificate (Coursera)**. The project analyzes country-level socio-economic and health indicators from Kaggle to identify patterns among nations, cluster them according to development profiles, and provide actionable insights for international aid planning. The goal is to help organizations like HELP International prioritize interventions and allocate resources effectively.

## Contents

1. **Unsupervised_ML_Project_EDA.ipynb** – Introduction and Exploratory Data Analysis (EDA)
    - Overview of country-level development, trade, and health indicators  
    - Initial exploration of dataset features
    - Identification of patterns, missing values, and potential variables for clustering
    - Analysis of GDP-relative ratios vs. absolute per-capita values

2.  **Unsupervised_ML_Project_Prep_PCA_Clustering.ipynb** – Data Preparation, PCA, and Clustering
    - Cleaning and normalizing inconsistent or missing values
    - Handling outliers in economic and health indicators
    - Standardizing features for clustering
    - Performing Principal Component Analysis (PCA) for dimensionality reduction
    - Applying multiple clustering algorithms: K-Means, Hierarchical Clustering, and DBSCAN
    - Evaluating cluster quality and interpretability
    - Comparing ratios vs. absolute values for clustering performance

3.  **Unsupervised_ML_Project_Actionable_Insights.ipynb** – Cluster Interpretation and Recommendations
    - Analyzing the composition of each cluster to understand development profiles (e.g., low vs. high development, trade patterns, health indicators)
    - Identifying potential priority nations for intervention based on cluster membership and key socio-economic challenges
    - Visualizing clusters and key indicators using radar and bar charts for stakeholder communication
    - Linking cluster insights to actionable recommendations: prioritizing clusters and countries for aid programs, determining key drivers of outcomes, translating insights into project-level interventions, and strategically allocating resources while monitoring impact
