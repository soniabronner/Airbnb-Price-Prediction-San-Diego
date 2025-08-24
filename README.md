# Airbnb Price Prediction San Diego

👉 [View the Project Notebook](Airbnb_GroupProject.ipynb)

## Project Overview

This university project focuses on predicting Airbnb accommodation prices in San Diego using a combination of exploratory data analysis (EDA), feature engineering with geospatial data, and machine learning models.
The main goal was to understand which factors influence Airbnb prices and to build and compare predictive models that incorporate both property characteristics and nearby Points of Interest (POIs).

 ## Data
 The study is based on a dataset Airbnb listings in San Diego

 ## Methodology
 ### Data Preprocessing
- Handling missing values
- Encoding categorical variables
- Outlier removal

### Exploratory Data Analysis (EDA)
- Summary statistics, histograms, and correlation analysis.
- Visualization of Airbnb listings on a basemap of San Diego.

### Spatial Feature Engineering
- Integration of Points Of Interest (POIs) from OpenStreetMap (restaurants, cafés, bars, fast food, marketplaces).
- Kernel Density Estimation (KDE) for POI density around listings.
- Geospatial visualizations of listings and amenities.

### Machine Learning Models
- Baseline model: Predicting mean price.
- Decision Tree Regressor (with/without POI features).
- Linear Regression (with/without POI features).
- Random Forest Regressor with hyperparameter tuning.

### Model Evaluation
- Root Mean Squared Error (RMSE) and R² metrics.
- Feature importance analysis.
- Predicted vs. actual price comparisons and spatial error mapping.


## Key Results
- The Random Forest Regressor achieved the best performance, with an R² ≈ 0.53 and an RMSE ≈ 224 USD.
- Including POIs slightly improved prediction accuracy, suggesting that location and nearby amenities have measurable impact on prices.
- Key predictors:
  - Bathrooms and bedrooms were the most influential features.
  - Accommodation capacity and proximity to restaurants and cafés also contributed significantly.
 
## Tools & Libraries
- Python (pandas, numpy, geopandas, matplotlib, seaborn)
- Geospatial libraries: folium, contextily, osmnx
- Machine Learning: scikit-learn
- Data: Airbnb listings (GeoJSON) + OpenStreetMap POIs

## Conclusion
This project demonstrates how urban data and machine learning can be combined to predict Airbnb accommodation prices. 
The analysis shows that both property features and urban amenities influence price formation, with Random Forest providing the most robust predictions.
