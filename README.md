# Learner Profiling & Job Clustering

## Overview
This project applies a structured data science workflow to segment Scaler learners based on job profiles, companies, compensation, and career features. By combining advanced clustering techniques with detailed data preprocessing and visualization, the notebook uncovers actionable career trends, skill gaps, and company insights to support curriculum design, counseling, and placement strategies.

## Key Objectives
- **Profile learners and companies** using robust unsupervised learning methods.
- **Detect patterns and trends** across job roles, salaries, and career moves.
- **Generate actionable recommendations** for learners and Scaler’s strategy team.

## Data Preparation & Preprocessing
- **Data Validation & Cleaning**
  - Checked schema and data types for consistency.
  - **Missing Value Imputation:** Handled null values using domain-aware strategies.
  - **Duplicate Removal:** Eliminated redundant records.
- **Outlier Handling**
  - Detected and clipped extreme outliers to reduce noise.
  - Applied domain thresholds and visual inspection.
- **Manual Segmentation**
  - Created early buckets and aggregated categories to explore intuitive patterns before modeling.
- **Feature Engineering & Checks**
  - Encoded categorical variables and standardized numerical features.
  - **Multicollinearity Check:** Used Variance Inflation Factor (VIF) to drop/reduce redundant features.

## Analysis & Clustering Techniques
1. **Exploratory Data Analysis (EDA)**
   - Univariate, bivariate, and multivariate analysis of learner demographics, compensation, and roles.
   - Identification of relationships between companies, experience, and pay scales.

2. **Clustering Workflow**
   - **KMeans Clustering:** Determined optimal cluster count using Elbow Method and Silhouette Score.
   - **Hierarchical Clustering:** Applied on a sample to build dendrograms and uncover hierarchical relationships.
   - **DBSCAN:** Detected and excluded noisy or niche learner profiles to refine cluster quality.

3. **Dimensionality Reduction & Visualization**
   - **PCA** to compress correlated features and stabilize models.
   - **t-SNE and UMAP** for clear 2D visualization of clusters and career patterns.

4. **Cluster Profiling & Insights**
   - Segmented learners into meaningful groups (e.g., top-tier roles, mid-career shifts, niche tech stacks).
   - Highlighted high-growth companies and roles.
   - Suggested skill-building areas and career pathways for learners.

## Tools & Libraries
- **Data Handling:** `pandas`, `numpy`
- **Visualization:** `matplotlib`, `seaborn`, `plotly`
- **Machine Learning:** `scikit-learn` (KMeans, Hierarchical, DBSCAN, PCA)
- **Advanced Visualization:** `umap-learn` for UMAP, `openTSNE` for t-SNE
- **Statistical Checks:** `statsmodels` for VIF and multicollinearity
- **Environment:** Google Colab (Python 3.x)

## Key Highlights
- End-to-end **data quality pipeline** (imputation, cleaning, feature checks).
- Integrated **manual and automated clustering** to validate findings.
- Combined **centroid-based, hierarchical, and density-based methods** for robustness.
- Used **Hopkins statistic** to confirm clusterability.
- Produced **clear visuals and business-ready insights**.

---

**Author:** Gargi Mishra  
**Tags:** Clustering, Machine Learning, Unsupervised Learning, Career Analytics, Data Science
