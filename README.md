# Waste Management Clustering in Indonesian Cities using K-Means

## 📁 Dataset
📎 Source: [SIPSN – Indonesian Waste Management Information System](https://sipsn.menlhk.go.id)

## Project Summary

This project explores and clusters waste management performance across Indonesian cities using Exploratory Data Analysis (EDA) and K-Means Clustering. It aims to identify regional patterns and segmentation based on handling, reduction, and recycling of waste. **The project was developed as part of Big Data course final exam**, utilizing real-world data from the Indonesian Ministry of Environment.

### ⭐ Situation

Indonesia is facing a growing waste management crisis. The national waste volume reached **38.8 million tons in 2023**, and although both handling and recycling efforts are increasing, they still fall short of mitigating the rise in waste production. Additionally, disparities in performance across regions suggest structural inefficiencies and unequal access to waste infrastructure.

### ⭐ Task

This project aims to:
- Analyze multi-year waste management performance data at the city/regency level.
- Understand core indicators like total waste, reduction rate, recycling rate, and overall management effectiveness.
- Apply clustering techniques to group regions based on performance similarities.
- Provide insights to support region-specific policy interventions.

### ⭐ Action

- Collected a national dataset from the **SIPSN (Sistem Informasi Pengelolaan Sampah Nasional)** covering 2018–2023, totaling 1,394 records across 13 indicators.
- Cleaned the dataset: fixed data types, handled missing values (using group-based mean/median imputation), and removed irrelevant fields.
- Performed EDA:
  - Descriptive statistics
  - Histograms for distribution patterns
  - Correlation matrix (highlighted strong linear dependencies)
  - Boxplots for outlier detection
- Applied K-Means Clustering:
  - Used Elbow Method to determine optimal **k = 3**
  - Evaluated cluster quality with **Silhouette Score (0.482)** and **Davies-Bouldin Index (0.744)**
- Explored clusters via:
  - Pairplots
  - Heatmaps
  - Statistical summaries per cluster

### ⭐ Result

- **Cluster 0**: Cities with minimal waste management (only 32.9% of waste handled), lower waste volume (avg. 101K tons/year), likely low infrastructure.
- **Cluster 1**: Moderate performance (81.3% managed), but still room to improve in reduction and recycling. Reflects cities with improving but incomplete systems.
- **Cluster 2**: Cities with excellent waste processing (89.1% managed, 17.4% recycling rate), highest waste volume (avg. 501K tons/year), mostly metropolitan areas like Jakarta.

These results offer actionable segmentation that can inform public policy, helping prioritize funding, infrastructure, and intervention based on regional performance.

## 📊 Key Visual Insights

- **Histograms** revealed right-skewed distribution in total waste produced and handled.
- **Correlation matrix** showed very strong relationships between `handled waste`, `total managed`, and `reduction`.
- **Boxplots** confirmed presence of extreme outliers—mostly in metropolitan regions.
- **Pairplots** allowed visual inspection of cluster spread and feature distributions.
- **Heatmaps** illustrated inter-cluster differences in recycling and reduction efficiency.

