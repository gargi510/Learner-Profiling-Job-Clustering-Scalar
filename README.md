# Learner Profiling & Job Clustering

## Overview
This project segments Scaler learners based on job profiles, companies, compensation, and career features. Using advanced clustering techniques combined with detailed preprocessing and visualization, it uncovers career patterns, skill gaps, and actionable insights to support curriculum design, counseling, and placement strategies.

## Key Objectives
- Profile learners and companies using unsupervised learning.
- Detect patterns in job roles, salaries, and career progression.
- Generate actionable recommendations for learners and organizational strategy.

## Data Preparation & Preprocessing
- **Validation & Cleaning:** Checked schema, data types, and duplicates; imputed missing values.
- **Outlier Handling:** Detected and clipped extreme values to reduce noise.
- **Manual Segmentation:** Early buckets for intuitive exploration.
- **Feature Engineering:** Encoded categorical variables, standardized numerical features, and reduced multicollinearity using VIF.

## Analysis & Clustering Techniques
1. **Exploratory Data Analysis (EDA):** Univariate, bivariate, and multivariate analysis of learner demographics, compensation, and roles.
2. **Clustering Workflow:**
   - KMeans (Elbow Method, Silhouette Score)
   - Hierarchical Clustering (dendrogram analysis)
   - DBSCAN (noise detection)
   - Manual flag-based segmentation for domain validation
3. **Dimensionality Reduction & Visualization:** PCA, t-SNE, and UMAP for cluster visualization.
4. **Cluster Profiling:** Identification of top-tier, mid-tier, and niche learner groups to inform skill-building and career pathways.

## Key Insights (Summary)
- Distinct clusters observed based on **experience, compensation, and role tiers**.
- High-value learners (senior roles, higher CTC) can be targeted for **mentorship and retention programs**.
- Mid- and lower-tier learners benefit from **structured learning and growth programs**.
- Insights can guide **talent management, strategic hiring, and personalized career interventions**.

## Tools & Libraries
- **Data Handling:** `pandas`, `numpy`
- **Visualization:** `matplotlib`, `seaborn`, `plotly`
- **Machine Learning:** `scikit-learn` (KMeans, Hierarchical, DBSCAN, PCA)
- **Advanced Visualization:** `umap-learn`, `openTSNE`
- **Statistical Checks:** `statsmodels` (VIF, multicollinearity)
- **Environment:** Google Colab (Python 3.x)

---

**Author:** Gargi Mishra  
**Tags:** Clustering, Machine Learning, Unsupervised Learning, Career Analytics, Data Science
