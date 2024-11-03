# House Price Prediction in King County, Washington State, USA

This project aims to predict house sales prices in King County, Washington, using Multiple Linear Regression (MLR) and other machine learning techniques. The dataset comprises historical data of houses sold between May 2014 and May 2015, with a focus on understanding the factors contributing to higher property values, specifically those priced at $650,000 and above.

## Dataset

The dataset contains house prices from King County, including the Seattle area. It was obtained from Kaggle and is published under the **CC0: Public Domain** license. Unfortunately, the original source of the data was not indicated by the user who provided it on Kaggle. 

- **Number of Variables:** 21
- **Number of Observations:** 21,613

### Variables

The dataset includes the following key variables (not exhaustive):

- `price`: Sale price of the house
- `bedrooms`: Number of bedrooms
- `bathrooms`: Number of bathrooms
- `sqft_living`: Square footage of the living area
- `sqft_lot`: Square footage of the lot
- `floors`: Number of floors
- `condition`: Condition of the house
- `grade`: Grade of the house (construction and design quality)

## Objectives

1. **Prediction Accuracy:** Achieve an accuracy of at least 75-80% in predicting house sales prices.
2. **Feature Analysis:** Identify which factors contribute to higher property values, particularly for houses priced at $650,000 and above.

## Models Evaluated

Several models were evaluated for predicting house prices, with the following results:

| Model                    | R² Score | Root Mean Squared Error (RMSE) | Mean Absolute Error (MAE) |
|--------------------------|----------|---------------------------------|----------------------------|
| XGBoost Regressor        | 0.836    | 86,178.84                       | 60,414.41                  |
| Linear Regression        | 0.834    | 86,651.35                       | 62,420.97                  |
| Lasso                    | 0.834    | 86,820.25                       | 62,550.66                  |
| Ridge                    | 0.833    | 87,068.63                       | 62,768.25                  |
| Gradient Boosting        | 0.750    | 106,431.56                      | 80,450.01                  |
| Extra Tree Regressor     | 0.618    | 131,562.28                      | 88,463.50                  |
| Decision Tree Regressor  | 0.578    | 138,434.86                      | 94,959.53                  |
| ElasticNet               | 0.558    | 141,686.96                      | 109,102.14                 |
| K-Neighbors Regressor    | 0.421    | 162,069.00                      | 121,644.83                 |

The **XGBoost Regressor** showed the best performance with an R² Score of **0.836** and a Root Mean Squared Error (RMSE) of **86,178.84**, indicating the highest predictive accuracy among the models tested.
