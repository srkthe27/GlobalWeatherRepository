# Global Weather Repository

## Overview
The **Global Weather Repository** is a data-driven project aimed at analyzing weather patterns and air quality across different geographical locations. Using machine learning techniques, the project explores key weather indicators and their impact on environmental conditions, providing insights through visualization and forecasting models.

## Features
- **Climate Analysis**: Studies long-term climate patterns using time-series analysis.
- **Environmental Impact**: Examines the correlation between weather parameters and air quality.
- **Feature Importance**: Identifies the most influential weather factors affecting air quality using ML techniques.
- **Spatial Analysis**: Visualizes global weather patterns using geographical mapping.
- **Forecasting Model**: Predicts future air quality based on historical weather data.

## Dataset
The dataset includes the following key features:
- **Location Data**: Country, latitude, longitude, timezone.
- **Weather Data**: Temperature (Celsius/Fahrenheit), wind speed, pressure, precipitation, humidity, visibility, UV index, and cloud cover.
- **Air Quality Data**: Levels of Carbon Monoxide, Ozone, Nitrogen Dioxide, Sulphur Dioxide, PM2.5, and PM10.
- **Astronomical Data**: Sunrise, sunset, moon phase, moon illumination.

## Implementation Details
### 1. Data Preprocessing
- Handling missing values and outliers.
- Converting timestamps for time-series analysis.
- Normalization of weather parameters.

### 2. Exploratory Data Analysis (EDA)
- Statistical summary of key features.
- Correlation analysis to understand relationships between weather conditions and air quality.
- Visualization of geographical patterns using `folium` for heatmaps.

### 3. Feature Importance Analysis
- **Random Forest Feature Importance**: Determines key features influencing air quality.
- **Permutation Importance**: Measures the effect of each feature by shuffling data.

### 4. Forecasting Model
- **Machine Learning Algorithm**: Uses Random Forest Regressor to predict PM2.5 levels.
- **Time-Series Forecasting**: Employs past weather data to predict future air quality trends.
- **Model Evaluation**: Mean Squared Error (MSE) and Mean Absolute Error (MAE) for performance assessment.

### 5. Geographical Analysis
- **Spatial Visualization**: Uses `folium` to generate global temperature heatmaps.
- **Country-Specific Analysis**: Filters data to study regional climate variations.

## Installation
To run the project, install the required dependencies:
```sh
pip install pandas numpy scikit-learn matplotlib seaborn folium
```

## Usage
1. Load the dataset into a Pandas DataFrame.
2. Perform EDA and feature engineering.
3. Train and evaluate the Random Forest model for air quality prediction.
4. Generate feature importance plots and geographical heatmaps.
5. Analyze long-term climate trends and environmental impact.

## Results
- Identified key weather parameters affecting air quality.
- Developed a predictive model with high accuracy.
- Visualized temperature and air quality trends globally.
- Provided actionable insights into climate variations and pollution levels.

## License
This project is open-source and available under the MIT License.

