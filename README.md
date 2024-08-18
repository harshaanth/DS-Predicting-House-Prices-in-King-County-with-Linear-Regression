# Predicting House Prices King County

# Description
A linear regression project to predict house prices in King County, Washington, using features such as square footage, number of bedrooms, and location. This project involves data preprocessing, feature selection, and building a predictive model to estimate housing prices.

### Data Information

The dataset contains the following attributes:

- `id`: Unique identifier for each home
- `date`: Date when the home was sold
- `price`: Sale price of the home
- `bedrooms`: Number of bedrooms
- `bathrooms`: Number of bathrooms
- `sqft_living`: Square footage of the home
- `sqft_lot`: Square footage of the lot
- `floors`: Number of floors
- `waterfront`: Whether the home has a waterfront view (1 if yes, 0 if no)
- `view`: Quality of the view (0 to 4 scale)
- `condition`: Condition of the home (1 to 5 scale)
- `grade`: Overall grade given to the home (1 to 13 scale)
- `sqft_above`: Square footage of the home excluding the basement
- `sqft_basement`: Square footage of the basement
- `yr_built`: Year the home was built
- `yr_renovated`: Year the home was renovated
- `zipcode`: ZIP code of the home
- `lat`: Latitude coordinate
- `long`: Longitude coordinate
- `sqft_living15`: Square footage of living space in the 15 most recent homes
- `sqft_lot15`: Square footage of the lot in the 15 most recent homes

### Libraries and Dependencies

The following libraries are used in this project:

- Data Manipulation: `pandas`, `numpy`
- Data Visualization: `matplotlib`, `seaborn`, `statsmodels.graphics.gofplots.ProbPlot`
- Model Building: `statsmodels`, `sklearn`
- Model Evaluation: `sklearn.metrics`, `sklearn.model_selection`
- Data Preprocessing: `sklearn.preprocessing`

## Data Loading and Preprocessing

The dataset is read from a Google Drive link and preprocessed. The `price` column is converted from a string to a numeric value, and the `date` column is dropped as it is not used in numerical computations.

## Exploratory Data Analysis (EDA)

We perform the following analyses:

- **Univariate Analysis**: Checking distributions and log-transforming the target variable.
- **Bivariate Analysis**: Examining correlations and visualizing relationships between features.
- **Multicollinearity Check**: Using Variance Inflation Factor (VIF) to identify and address multicollinearity.

## Interpretations

- **Bathrooms**: Each additional bathroom increases the predicted price by 14.166%.
- **Waterfront**: Homes with a waterfront view have a predicted price that is 51.182% higher than non-waterfront homes.

## Conclusion

This project demonstrates how linear regression can be used to predict home prices based on various features. Key steps included data preprocessing, feature selection, and model evaluation. For further details, refer to the Jupyter notebook in this repository.

## Files in the Repository

- `Predicting_house_prices_in_King_County_with_Linear_Regression.ipynb`: The Jupyter notebook containing the full analysis and code.
- `README.md`: Project overview and instructions.
