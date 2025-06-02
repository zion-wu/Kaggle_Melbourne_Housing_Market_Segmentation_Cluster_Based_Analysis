# Melbourne Housing Market Clusters Analysis

This project analyzes the Melbourne housing market by applying clustering techniques to identify meaningful groups of properties based on price, size, and location. The insights gained from this analysis can guide real estate marketing strategies, property valuations, and investment decisions.

## 📊 Project Overview

Understanding different types of properties in the housing market is essential for real estate firms, investors, and policymakers. By using unsupervised learning methods—specifically K-Means and Hierarchical Clustering—this project reveals hidden patterns within the Melbourne housing market data from January 2016.

### Objectives

- Segment properties based on key features like price, size, and location.
- Visualize clusters using t-SNE and geographic mapping.
- Provide actionable insights for real estate marketing, property valuation, and investment.

## 🔍 Dataset

The dataset is sourced from Kaggle: [Melbourne Housing Market](https://www.kaggle.com/datasets/anthonypino/melbourne-housing-market), originally scraped from publicly available records on Domain.com.au. It contains details such as:

- **Price** (in AUD)
- **Rooms** (number of rooms)
- **Distance** (from CBD)
- **Bedroom2** (number of bedrooms)
- **Bathroom** (number of bathrooms)
- **Car** (number of parking spots)
- **Landsize** (in square meters)
- **BuildingArea** (in square meters)
- **YearBuilt**
- **Latitude/Longitude** (for mapping)

*Note: The full dataset (`Melbourne_housing_FULL.csv`) is included in the repository for reference.*

## 🧰 Methods

1. **Data Preparation**
   - Removed rows with missing values in key features.
   - Handled outliers based on logical thresholds.
   - Applied log transformations to skewed variables (Price, Landsize, BuildingArea, Distance).
   - Standardized all features using Z-score normalization.

2. **Clustering Techniques**
   - **K-Means Clustering**: Determined optimal clusters via Elbow Method; selected 4 clusters.
   - **Hierarchical Clustering**: Chosen as the final method due to better Silhouette Score.
   - **t-SNE Visualization**: Confirmed distinct cluster separations in high-dimensional space.
   - **Geospatial Mapping**: Plotted clusters on a map using latitude and longitude.

3. **Evaluation**
   - Compared clustering results with predefined housing types (e.g., house, unit, townhouse).
   - Analyzed cluster distributions across suburbs and regions.

## 📈 Key Findings

- **Cluster 0**: Balanced suburban homes with moderate prices and size, located farther from the CBD.
- **Cluster 1**: Affordable, compact homes in suburban areas.
- **Cluster 2**: High-priced properties in central, high-demand areas.
- **Cluster 3**: Luxury estates or unique outlier properties with large areas and high prices.

These insights can assist:
- **Real estate agencies**: Develop targeted marketing strategies.
- **Investors**: Identify undervalued or high-potential properties.
- **Urban planners**: Understand housing patterns for policy and development.
