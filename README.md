# Boston Crime Data Analysis and Prediction

### Overview

This project focuses on analyzing crime data in Boston through data visualization and predictive modeling. The goal is to uncover patterns, visualize crime trends, and predict various aspects of criminal activities, such as crime types, crime severity, and district-level crime rates.

### Dataset

The dataset contains detailed information on crimes in Boston, including:

- Latitude and Longitude for crime locations
- OFFENSE_CODE_GROUP: Crime categories
- DISTRICT: Police district where the crime occurred
- OCCURRED_ON_DATE: Date and time of the crime
- UCR_PART: Crime severity classification (Part One, Part Two, Part Three)

The dataset was extracted from a ZIP file, Crimes in Boston.zip, and preprocessed to handle missing values and format time-based features.

### Features

##### 1. Exploratory Data Analysis

- Crimes Over the Years: Visualizing the number of crimes per year.
- Crimes by Hour of the Day: Identifying peak hours of criminal activities.
- Crimes by District: Highlighting the most and least crime-affected districts.
- Top Crime Categories: Displaying the most frequent crime types.

##### 2. Heatmap Visualization

A heatmap created with Folium to represent crime hotspots based on latitude and longitude. The heatmap is saved as crime_heatmap.html for easy access.

##### 3. Predictive Analysis

- Crime Type Prediction: Predicting crime categories using a Random Forest Classifier.
- District-Level Crime Prediction: Estimating the number of crimes in each district using Random Forest Regression.
- Crime Severity Prediction: Classifying crimes into severity categories (Part One, Part Two, Part Three).

### Visualizations

- Bar Chart: Crimes over the years and crimes by district.
- Count Plot: Distribution of crimes by hour.
- Heatmap: Geographic representation of crime hotspots.
- Top Crime Categories: Bar chart showing the most common crime types.

### Key Results

- Classification Report for Crime Type Prediction: Precision, recall, and F1-scores indicate model performance for predicting specific crime categories. Weighted averages suggest room for improvement in underrepresented classes.
- Mean Squared Error for District Crime Prediction: MSE for predicting district-level crime counts indicates the model's regression performance.
- Crime Severity Prediction: A Random Forest Classifier achieved high accuracy for predicting severity levels, with weighted averages above 0.90.

### Challenges and Future Work

Class Imbalance: Many crime categories have low representation, impacting classification performance. Future work could include:
- Oversampling underrepresented classes.
- Using advanced models like Gradient Boosting or XGBoost.

Feature Engineering: Incorporating weather, socioeconomic, or traffic data might improve prediction accuracy.

### Source

Dataset: [Boston Crime Dataset on Kaggle](https://www.kaggle.com/datasets/ankkur13/boston-crime-data)
