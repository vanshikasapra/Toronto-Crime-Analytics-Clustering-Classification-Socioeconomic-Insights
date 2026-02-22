# Toronto-Crime-Analytics-Clustering-Classification-Socioeconomic-Insights
**Project Overview**

This project analyzes crime patterns across Toronto neighborhoods to identify how different types of crime align with underlying socioeconomic and demographic characteristics. Rather than focusing on total crime counts, the analysis emphasizes crime composition, neighborhood segmentation, and structural drivers of risk, with the goal of supporting more targeted and proactive decision-making. The project was completed as part of a graduate-level data mining and visualization course and demonstrates end-to-end analytics skills including data preprocessing, feature engineering, unsupervised learning, classification modeling, and interpretation.

**Problem Statement**

Crime prevention strategies are often reactive and rely on aggregate metrics that hide meaningful heterogeneity across neighborhoods. This project aims to answer: How do neighborhoods differ in types of crime, not just volume? Do distinct socioeconomic profiles align with specific crime patterns? Can clustering and classification uncover actionable insights for resource allocation and prevention?

**Data Sources**

Toronto Major Crime Indicators (MCI): Event-level data covering Assault, Auto Theft, Break and Enter, Robbery, and Theft Over.
Toronto Neighborhood Census (2021): Demographic and socioeconomic variables including population, age, income inequality (Gini), unemployment, low-income prevalence (LIM-AT), education levels, and housing indicators.

**Feature Engineering**

Key transformations included:
Converting raw crime counts into crime mix proportions by neighborhood
Normalizing socioeconomic variables using z-score standardization
Merging crime and census data at the neighborhood level
Creating risk indicators and temporal groupings (day vs night, violent vs non-violent)

**Modeling Approach**

The analysis combines multiple analytical techniques:
Clustering
K-Means clustering used to segment neighborhoods by:
  Crime composition (4 crime clusters)
  Socioeconomic characteristics (4 socioeconomic clusters)
Cluster validation performed using elbow method and silhouette scores
PCA (2D and 3D) used for dimensionality reduction and visual validation
Cluster centroids summarized using z-score heatmaps

Classification
Logistic Regression, Random Forest, and Gradient Boosting models applied to:
  Predict day vs night crime occurrence
  Predict violent vs non-violent crime
Models evaluated using accuracy and AUC
Feature importance used to identify consistent risk drivers

**Key Insights**

Violent crime clusters align strongly with neighborhoods showing higher inequality, higher unemployment, and lower education
Property crimes exhibit multiple mechanisms, appearing both in economically vulnerable areas and affluent, asset-dense neighborhoods
Education and inequality emerge as stronger predictors than population alone
Crime patterns vary significantly by time of day and season, supporting targeted patrol optimization

**Tools & Technologies**

Python (pandas, numpy, scikit-learn, seaborn, matplotlib)
Unsupervised learning (K-Means, PCA)
Supervised learning (Logistic Regression, Random Forest, GBM)
Data visualization & exploratory analysis

**Potential Application**

Data driven patrol planning 
Targeted community intervention programs 
Urban planning and public safety analytics
Segmentation frameworks applicable to product, risk, or user analytics 
