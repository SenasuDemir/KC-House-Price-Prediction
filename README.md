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

| Model                     | R² Score | Mean Squared Error (MSE) |
|---------------------------|----------|----------------------------|
| Linear Regression         | 0.69     | 148,622                    |
| Ridge                     | 0.69     | 148,630                    |
| Lasso                     | 0.69     | 148,622                    |
| ElasticNet                | 0.57     | 174,008                    |
| Decision Tree Regressor   | 0.68     | 150,958                    |
| Extra Tree Regressor      | 0.68     | 107,249                    |
| XGBoost                   | 0.86     | 99,350                     |
| Random Forest Regressor   | 0.98     | 39,980                     |

The **Random Forest Regressor** showed the best performance with an R² Score of **0.98** and a Mean Squared Error (MSE) of **39,980**.
