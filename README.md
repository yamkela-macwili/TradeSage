# TradeSage
# Predicting Forex Closing Prices Using Machine Learning: A Step Towards Building a Trading Bot

This project involves developing a machine learning model to predict the closing prices of forex currency pairs. The goal is to leverage historical market data and advanced feature engineering techniques to build a robust predictive model that can provide accurate and actionable insights for forex trading. This is the first part of a comprehensive effort to build an actual trading bot.

## Objectives

- Predict Closing Prices: Develop a machine learning model to accurately predict the closing prices of forex currency pairs.
- Feature Engineering: Utilize advanced feature engineering techniques to extract meaningful features from raw market data.
- Model Evaluation: Evaluate the performance of different models using metrics like R-squared and Mean Squared Error.
- Model Deployment: Deploy the model as an API to make real-time predictions available for trading decisions.
- Trend Identification: Emphasize the role of added features in identifying market trends, setting the foundation for the next part of the project—building a fully functional trading bot.

## Data Collection and Preprocessing

- **Data Source**: Historical market data was collected, including attributes such as open price, high price, low price, close price, volume, and others.
- **Data Cleaning**: The data was cleaned to handle missing values and ensure consistency.
- **Data Transformation**: The raw data was transformed into a structured format suitable for machine learning, including the extraction of date-time features.

## Feature Engineering

- **Date-Time Features**: Extracted features such as hour, day of the week, month, and year from the timestamp.
- **Lag Features**: Created lag features to capture the behavior of the market over time.
- **Rolling Statistics**: Calculated rolling mean and standard deviation to capture trends.
- **Technical Indicators**: Computed technical indicators like RSI, MACD, and Golden Crossover to enhance the feature set.
- **Price Change Features**: Calculated daily price changes and other relevant metrics.

## Model Development

- **Model Selection**: Explored different machine learning models, including Linear Regression and Random Forest Regressor.
- **Random Forest Model**: Selected the Random Forest Regressor for its superior performance and ability to handle complex interactions between features.
- **Feature Scaling**: Applied feature scaling to ensure all features were on a similar scale.

## Model Evaluation

- **Training and Testing**: Split the data into training and testing sets to evaluate model performance.
- **Metrics**: Evaluated the model using Mean Squared Error (MSE) and R-squared (R²) scores.
- **Results**: Achieved an R² score of 0.9996 and an MSE of 6.6676e^-06, indicating a highly accurate model.

## Model Deployment

- **API Development**: Created a Flask API to serve the model for real-time predictions.
- **Containerization**: Used Docker to package the API and model into a container for easy deployment.
- **Cloud Deployment**: Deployed the containerized API on a cloud platform to make it accessible for real-time trading decisions.

## Results and Insights

- **Feature Importance**: Identified key features that significantly impact the closing prices, such as High, Low, RSI, and Open prices.
- **Model Interpretation**: Used SHAP (SHapley Additive exPlanations) to interpret model predictions and understand the influence of different features.
- **Business Value**: The deployed model can be used by traders to make informed decisions based on real-time predictions of closing prices.

## Conclusion

This project demonstrates the successful application of machine learning to predict forex closing prices. By leveraging advanced feature engineering and robust model evaluation, the project provides valuable insights and a scalable solution for real-time trading decisions. Importantly, this is the first part of a larger initiative to build a fully functional trading bot, where the added features will play a crucial role in trend identification and market analysis.

## Installation

To view the project locally, follow these steps:

```bash
# Clone the repository
git clone https://github.com/yamkela-macwili/forex-price-prediction.git

# Navigate to the project directory
cd forex-price-prediction
