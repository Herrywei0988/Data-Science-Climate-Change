# Renewable Energy Trends in India: LSTM and Machine Learning Analysis

## Project Overview
This project focuses on analyzing and forecasting renewable energy trends in India, specifically wind and hydroelectric power generation. Using historical data from 2013–2023, we applied advanced machine learning techniques such as LSTM models to predict daily energy generation and uncover seasonal and regional patterns. The study aims to provide insights for energy planning and sustainability.

## Features
Exploratory Data Analysis (EDA): Uncovered seasonal trends and regional patterns using visualizations like heatmaps and line plots.
Time-Series Prediction: Developed LSTM models to forecast daily wind and hydro power generation over a 60-day horizon.
Performance Evaluation: Evaluated models using metrics like MSE, MAE, and R-squared for accuracy assessment.
Proposed Enhancements: Suggested hybrid modeling and advanced architectures (e.g., Transformer) for better prediction performance.
Automated Data Preprocessing: Streamlined data cleaning, normalization, and feature engineering workflows.

## Dataset
The dataset was sourced from Kaggle and contains daily power generation records for various energy sources across Indian regions. Note: Due to size limitations, the dataset is not included in the repository. You can download it from Kaggle and place it in the data/ folder.

## Results

###  Model Performance
The LSTM models were evaluated using the following metrics:
- **Mean Squared Error (MSE)**: Quantifies the average squared difference between predicted and actual values.
- **Mean Absolute Error (MAE)**: Represents the average magnitude of prediction errors.
- **R-squared (R²)**: Measures how well the predictions align with actual values.

| Model          | MSE    | MAE   | R²    |
|-----------------|--------|-------|-------|
| Wind Model     | 430.02 | 17.09 | 0.01  |
| Hydro Model    | 1348.02| 29.63 | -1.21 |

### Key Findings
####  Wind Generation
- The LSTM model effectively captured general trends in wind energy production, such as long-term patterns and periodic fluctuations.
- However, the model struggled with short-term variations, particularly during sudden peaks and drops caused by the unpredictable nature of wind speeds and directions.

####  Hydro Generation
- Seasonal patterns in hydroelectric power production were partially captured, with higher energy generation during monsoon months (July–September).
- The model exhibited poor accuracy due to high variability in the data, caused by factors such as rainfall irregularities, reservoir management, and regional climatic differences.

### Visualization of Predictions
#### Wind Power
- Predicted values closely followed actual trends in smoother sections but deviated significantly during abrupt changes.

#### Hydro Power
- Predicted values failed to match extreme peaks and troughs in actual hydroelectric generation due to the dataset's inherent variability.


###  Challenges
- **Wind Model**: The low R² value (0.01) indicates limited precision in explaining variations in wind data.
- **Hydro Model**: The negative R² value (-1.21) highlights significant discrepancies between predictions and actual hydro generation, reflecting limitations in modeling high variability and external factors.

### Insights
- **Wind Energy**: The wind energy model performed better than the hydro energy model, as wind data exhibited less seasonal variability.
- **Hydro Energy**: Hydro energy predictions would benefit from incorporating additional features, such as rainfall data, water reservoir levels, and meteorological information, to better capture underlying patterns.
