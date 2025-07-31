# Anti-Money Laundering (AML) Analytics: Customer Segmentation & Risk Scoring

This repository contains a Jupyter Notebook (`[Cluster_ +_Risk_Scoring]_Anti_Money_Laundering_Analytics.ipynb`) that demonstrates an approach to **Anti-Money Laundering (AML) analytics** focusing on customer segmentation and risk scoring.

The notebook showcases a data-driven methodology to identify potentially suspicious financial activities by:

-   **Data Wrangling and Feature Engineering:** Cleaning raw financial transaction data, handling missing values, and creating new, insightful features such as `total_inflows`, `total_outflows`, `pass_through_ratio`, `transaction_velocity`, and `income_discrepancy_ratio`. It also incorporates account and customer age.
-   **Exploratory Data Analysis (EDA):** Visualizing the distributions of various financial and engineered metrics, and identifying potential outliers through boxplots and histograms.
-   **Correlation Analysis:** Examining relationships between different financial and behavioral indicators using a heatmap to understand their interdependencies.
-   **Customer Segmentation (Clustering):**
    * **K-Means Clustering:** Applying K-Means to segment customers into distinct groups based on their financial behavior patterns. The Elbow method is used to explore the optimal number of clusters.
    * **DBSCAN (Density-Based Spatial Clustering of Applications with Noise):** An attempt to identify dense clusters and outliers (noise points) in the dataset, which can be indicative of unusual behavior.
-   **Risk Scoring:** Developing a custom `risk_score` based on key financial behaviors like high pass-through ratios, income discrepancies, and salary portability, aiming to flag high-risk accounts.

## Key Features

-   **Comprehensive Data Preprocessing:** Includes date conversions, handling of missing values, and data type corrections.
-   **Domain-Specific Feature Engineering:** Creates features directly relevant to AML analysis.
-   **Comparative Clustering:** Explores both K-Means and DBSCAN for customer segmentation.
-   **Customizable Risk Scoring Logic:** Provides a clear example of how to build a simple risk scoring mechanism.
